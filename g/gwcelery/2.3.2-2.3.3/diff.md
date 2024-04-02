# Comparing `tmp/gwcelery-2.3.2.tar.gz` & `tmp/gwcelery-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwcelery-2.3.2.tar", max compression
+gzip compressed data, was "gwcelery-2.3.3.tar", max compression
```

## Comparing `gwcelery-2.3.2.tar` & `gwcelery-2.3.3.tar`

### file list

```diff
@@ -1,247 +1,247 @@
--rw-r--r--   0        0        0   108001 2024-03-23 00:10:57.577431 gwcelery-2.3.2/CHANGES.rst
--rw-r--r--   0        0        0       64 2024-03-23 00:10:57.577431 gwcelery-2.3.2/CONTRIBUTING.rst
--rw-r--r--   0        0        0    19716 2024-03-23 00:10:57.578431 gwcelery-2.3.2/LICENSE.rst
--rw-r--r--   0        0        0     1351 2024-03-23 00:10:57.578431 gwcelery-2.3.2/README.rst
--rw-r--r--   0        0        0      634 2024-03-23 00:10:57.578431 gwcelery-2.3.2/doc/Makefile
--rw-r--r--   0        0        0   191486 2024-03-23 00:10:57.580431 gwcelery-2.3.2/doc/_static/acceptance-tests-checklist.png
--rw-r--r--   0        0        0   241593 2024-03-23 00:10:57.581431 gwcelery-2.3.2/doc/_static/celeryevent-screenshot.png
--rw-r--r--   0        0        0   206465 2024-03-23 00:10:57.583431 gwcelery-2.3.2/doc/_static/deployment-screenshot.png
--rw-r--r--   0        0        0   161306 2024-03-23 00:10:57.584431 gwcelery-2.3.2/doc/_static/flask-screenshot.png
--rw-r--r--   0        0        0   328056 2024-03-23 00:10:57.586431 gwcelery-2.3.2/doc/_static/flower-screenshot.png
--rw-r--r--   0        0        0   114719 2024-03-23 00:10:57.587431 gwcelery-2.3.2/doc/_static/logo-0.5x.png
--rw-r--r--   0        0        0   351955 2024-03-23 00:10:57.590431 gwcelery-2.3.2/doc/_static/logo.png
--rw-r--r--   0        0        0   230777 2024-03-23 00:10:57.592431 gwcelery-2.3.2/doc/_static/sentry-screenshot.png
--rwxr-xr-x   0        0        0     7356 2024-03-23 00:10:57.592431 gwcelery-2.3.2/doc/conf.py
--rw-r--r--   0        0        0     4346 2024-03-23 00:10:57.593431 gwcelery-2.3.2/doc/configuration.rst
--rw-r--r--   0        0        0     5698 2024-03-23 00:10:57.593431 gwcelery-2.3.2/doc/contributing.rst
--rw-r--r--   0        0        0    10846 2024-03-23 00:10:57.593431 gwcelery-2.3.2/doc/deployment.rst
--rw-r--r--   0        0        0    10308 2024-03-23 00:10:57.593431 gwcelery-2.3.2/doc/design.rst
--rw-r--r--   0        0        0      563 2024-03-23 00:10:57.593431 gwcelery-2.3.2/doc/gwcelery.conf.rst
--rw-r--r--   0        0        0      284 2024-03-23 00:10:57.593431 gwcelery-2.3.2/doc/gwcelery.email.rst
--rw-r--r--   0        0        0      329 2024-03-23 00:10:57.593431 gwcelery-2.3.2/doc/gwcelery.igwn_alert.rst
--rw-r--r--   0        0        0      227 2024-03-23 00:10:57.594431 gwcelery-2.3.2/doc/gwcelery.rst
--rw-r--r--   0        0        0       79 2024-03-23 00:10:57.594431 gwcelery-2.3.2/doc/gwcelery.sentry.rst
--rw-r--r--   0        0        0       97 2024-03-23 00:10:57.594431 gwcelery-2.3.2/doc/gwcelery.tasks.alerts.rst
--rw-r--r--   0        0        0      103 2024-03-23 00:10:57.594431 gwcelery-2.3.2/doc/gwcelery.tasks.bayestar.rst
--rw-r--r--   0        0        0      107 2024-03-23 00:10:57.594431 gwcelery-2.3.2/doc/gwcelery.tasks.circulars.rst
--rw-r--r--   0        0        0       98 2024-03-23 00:10:57.594431 gwcelery-2.3.2/doc/gwcelery.tasks.condor.rst
--rw-r--r--   0        0        0       91 2024-03-23 00:10:57.594431 gwcelery-2.3.2/doc/gwcelery.tasks.core.rst
--rw-r--r--   0        0        0     2404 2024-03-23 00:10:57.594431 gwcelery-2.3.2/doc/gwcelery.tasks.detchar.rst
--rw-r--r--   0        0        0     1110 2024-03-23 00:10:57.594431 gwcelery-2.3.2/doc/gwcelery.tasks.em_bright.rst
--rw-r--r--   0        0        0      129 2024-03-23 00:10:57.594431 gwcelery-2.3.2/doc/gwcelery.tasks.external_skymaps.rst
--rw-r--r--   0        0        0     9887 2024-03-23 00:10:57.594431 gwcelery-2.3.2/doc/gwcelery.tasks.external_triggers.rst
--rw-r--r--   0        0        0      112 2024-03-23 00:10:57.594431 gwcelery-2.3.2/doc/gwcelery.tasks.first2years.rst
--rw-r--r--   0        0        0      139 2024-03-23 00:10:57.595431 gwcelery-2.3.2/doc/gwcelery.tasks.first2years_external.rst
--rw-r--r--   0        0        0       88 2024-03-23 00:10:57.595431 gwcelery-2.3.2/doc/gwcelery.tasks.gcn.rst
--rw-r--r--   0        0        0      100 2024-03-23 00:10:57.595431 gwcelery-2.3.2/doc/gwcelery.tasks.gracedb.rst
--rw-r--r--   0        0        0      103 2024-03-23 00:10:57.595431 gwcelery-2.3.2/doc/gwcelery.tasks.gwskynet.rst
--rw-r--r--   0        0        0      109 2024-03-23 00:10:57.595431 gwcelery-2.3.2/doc/gwcelery.tasks.igwn_alert.rst
--rw-r--r--   0        0        0      109 2024-03-23 00:10:57.595431 gwcelery-2.3.2/doc/gwcelery.tasks.inference.rst
--rw-r--r--   0        0        0      121 2024-03-23 00:10:57.595431 gwcelery-2.3.2/doc/gwcelery.tasks.legacy_gracedb.rst
--rw-r--r--   0        0        0      112 2024-03-23 00:10:57.595431 gwcelery-2.3.2/doc/gwcelery.tasks.notice_text.rst
--rw-r--r--   0        0        0     8111 2024-03-23 00:10:57.595431 gwcelery-2.3.2/doc/gwcelery.tasks.orchestrator.rst
--rw-r--r--   0        0        0      100 2024-03-23 00:10:57.595431 gwcelery-2.3.2/doc/gwcelery.tasks.p_astro.rst
--rw-r--r--   0        0        0     2385 2024-03-23 00:10:57.595431 gwcelery-2.3.2/doc/gwcelery.tasks.raven.rst
--rw-r--r--   0        0        0      106 2024-03-23 00:10:57.595431 gwcelery-2.3.2/doc/gwcelery.tasks.rrt_utils.rst
--rw-r--r--   0        0        0      814 2024-03-23 00:10:57.596431 gwcelery-2.3.2/doc/gwcelery.tasks.rst
--rw-r--r--   0        0        0      100 2024-03-23 00:10:57.596431 gwcelery-2.3.2/doc/gwcelery.tasks.skymaps.rst
--rw-r--r--   0        0        0     7161 2024-03-23 00:10:57.596431 gwcelery-2.3.2/doc/gwcelery.tasks.superevents.rst
--rw-r--r--   0        0        0       97 2024-03-23 00:10:57.596431 gwcelery-2.3.2/doc/gwcelery.tools.condor.rst
--rw-r--r--   0        0        0       94 2024-03-23 00:10:57.596431 gwcelery-2.3.2/doc/gwcelery.tools.flask.rst
--rw-r--r--   0        0        0       97 2024-03-23 00:10:57.596431 gwcelery-2.3.2/doc/gwcelery.tools.nagios.rst
--rw-r--r--   0        0        0      185 2024-03-23 00:10:57.596431 gwcelery-2.3.2/doc/gwcelery.tools.rst
--rw-r--r--   0        0        0       73 2024-03-23 00:10:57.596431 gwcelery-2.3.2/doc/gwcelery.util.rst
--rw-r--r--   0        0        0      507 2024-03-23 00:10:57.596431 gwcelery-2.3.2/doc/gwcelery.voevent.rst
--rw-r--r--   0        0        0     3564 2024-03-23 00:10:57.596431 gwcelery-2.3.2/doc/htcondor.rst
--rw-r--r--   0        0        0     1576 2024-03-23 00:10:57.596431 gwcelery-2.3.2/doc/index.rst
--rw-r--r--   0        0        0      800 2024-03-23 00:10:57.597432 gwcelery-2.3.2/doc/make.bat
--rw-r--r--   0        0        0     5541 2024-03-23 00:10:57.597432 gwcelery-2.3.2/doc/monitoring.rst
--rw-r--r--   0        0        0     5405 2024-03-23 00:10:57.597432 gwcelery-2.3.2/doc/quickstart.rst
--rw-r--r--   0        0        0     1097 2024-03-23 00:10:57.597432 gwcelery-2.3.2/gwcelery/__init__.py
--rw-r--r--   0        0        0    18447 2024-03-23 00:10:57.597432 gwcelery-2.3.2/gwcelery/_version.py
--rw-r--r--   0        0        0    19514 2024-03-23 00:10:57.598431 gwcelery-2.3.2/gwcelery/conf/__init__.py
--rw-r--r--   0        0        0     1195 2024-03-23 00:10:57.598431 gwcelery-2.3.2/gwcelery/conf/dev.py
--rw-r--r--   0        0        0     1180 2024-03-23 00:10:57.598431 gwcelery-2.3.2/gwcelery/conf/minikube.py
--rw-r--r--   0        0        0     2178 2024-03-23 00:10:57.598431 gwcelery-2.3.2/gwcelery/conf/playground.py
--rw-r--r--   0        0        0     3687 2024-03-23 00:10:57.598431 gwcelery-2.3.2/gwcelery/conf/production.py
--rw-r--r--   0        0        0     2040 2024-03-23 00:10:57.598431 gwcelery-2.3.2/gwcelery/conf/test.py
--rw-r--r--   0        0        0        0 2024-03-23 00:10:57.763437 gwcelery-2.3.2/gwcelery/data/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 00:10:57.763437 gwcelery-2.3.2/gwcelery/data/first2years/__init__.py
--rw-r--r--   0        0        0   731421 2024-03-23 00:10:57.601431 gwcelery-2.3.2/gwcelery/data/first2years/gstlal.xml.gz
--rwxr-xr-x   0        0        0     3199 2024-03-23 00:10:57.602432 gwcelery-2.3.2/gwcelery/data/gwcelery.sub
--rw-r--r--   0        0        0      505 2024-03-23 00:10:57.602432 gwcelery-2.3.2/gwcelery/email/__init__.py
--rw-r--r--   0        0        0     3317 2024-03-23 00:10:57.602432 gwcelery-2.3.2/gwcelery/email/bootsteps.py
--rw-r--r--   0        0        0      995 2024-03-23 00:10:57.602432 gwcelery-2.3.2/gwcelery/email/signals.py
--rw-r--r--   0        0        0     1457 2024-03-23 00:10:57.602432 gwcelery-2.3.2/gwcelery/flask.py
--rw-r--r--   0        0        0      529 2024-03-23 00:10:57.602432 gwcelery-2.3.2/gwcelery/igwn_alert/__init__.py
--rw-r--r--   0        0        0     4484 2024-03-23 00:10:57.602432 gwcelery-2.3.2/gwcelery/igwn_alert/bootsteps.py
--rw-r--r--   0        0        0      608 2024-03-23 00:10:57.602432 gwcelery-2.3.2/gwcelery/igwn_alert/signals.py
--rw-r--r--   0        0        0      275 2024-03-23 00:10:57.603432 gwcelery-2.3.2/gwcelery/jinja.py
--rw-r--r--   0        0        0      305 2024-03-23 00:10:57.603432 gwcelery-2.3.2/gwcelery/kafka/__init__.py
--rw-r--r--   0        0        0    11839 2024-03-23 00:10:57.603432 gwcelery-2.3.2/gwcelery/kafka/bootsteps.py
--rw-r--r--   0        0        0      522 2024-03-23 00:10:57.603432 gwcelery-2.3.2/gwcelery/kafka/signals.py
--rw-r--r--   0        0        0     2567 2024-03-23 00:10:57.603432 gwcelery-2.3.2/gwcelery/sentry/__init__.py
--rw-r--r--   0        0        0       34 2024-03-23 00:10:57.603432 gwcelery-2.3.2/gwcelery/sentry/integrations/__init__.py
--rw-r--r--   0        0        0      832 2024-03-23 00:10:57.603432 gwcelery-2.3.2/gwcelery/sentry/integrations/condor.py
--rw-r--r--   0        0        0      836 2024-03-23 00:10:57.603432 gwcelery-2.3.2/gwcelery/sentry/integrations/requests.py
--rw-r--r--   0        0        0      939 2024-03-23 00:10:57.604432 gwcelery-2.3.2/gwcelery/sentry/integrations/subprocess.py
--rw-r--r--   0        0        0     1302 2024-03-23 00:10:57.604432 gwcelery-2.3.2/gwcelery/static/typeahead.css
--rw-r--r--   0        0        0     4124 2024-03-23 00:10:57.604432 gwcelery-2.3.2/gwcelery/static/vega/index.html
--rw-r--r--   0        0        0      515 2024-03-23 00:10:57.604432 gwcelery-2.3.2/gwcelery/tasks/__init__.py
--rw-r--r--   0        0        0    14457 2024-03-23 00:10:57.604432 gwcelery-2.3.2/gwcelery/tasks/alerts.py
--rw-r--r--   0        0        0     2540 2024-03-23 00:10:57.604432 gwcelery-2.3.2/gwcelery/tasks/bayestar.py
--rw-r--r--   0        0        0     1892 2024-03-23 00:10:57.604432 gwcelery-2.3.2/gwcelery/tasks/circulars.py
--rw-r--r--   0        0        0     7552 2024-03-23 00:10:57.605432 gwcelery-2.3.2/gwcelery/tasks/condor.py
--rw-r--r--   0        0        0     2692 2024-03-23 00:10:57.605432 gwcelery-2.3.2/gwcelery/tasks/core.py
--rw-r--r--   0        0        0    23090 2024-03-23 00:10:57.605432 gwcelery-2.3.2/gwcelery/tasks/detchar.py
--rw-r--r--   0        0        0     4903 2024-03-23 00:10:57.605432 gwcelery-2.3.2/gwcelery/tasks/em_bright.py
--rw-r--r--   0        0        0    29615 2024-03-23 00:10:57.605432 gwcelery-2.3.2/gwcelery/tasks/external_skymaps.py
--rw-r--r--   0        0        0    31983 2024-03-23 00:10:57.606432 gwcelery-2.3.2/gwcelery/tasks/external_triggers.py
--rw-r--r--   0        0        0     6841 2024-03-23 00:10:57.606432 gwcelery-2.3.2/gwcelery/tasks/first2years.py
--rw-r--r--   0        0        0    10693 2024-03-23 00:10:57.606432 gwcelery-2.3.2/gwcelery/tasks/first2years_external.py
--rw-r--r--   0        0        0     4832 2024-03-23 00:10:57.606432 gwcelery-2.3.2/gwcelery/tasks/gcn.py
--rw-r--r--   0        0        0    11080 2024-03-23 00:10:57.607432 gwcelery-2.3.2/gwcelery/tasks/gracedb.py
--rw-r--r--   0        0        0     6884 2024-03-23 00:10:57.607432 gwcelery-2.3.2/gwcelery/tasks/gwskynet.py
--rw-r--r--   0        0        0     2453 2024-03-23 00:10:57.607432 gwcelery-2.3.2/gwcelery/tasks/igwn_alert.py
--rw-r--r--   0        0        0    34985 2024-03-23 00:10:57.607432 gwcelery-2.3.2/gwcelery/tasks/inference.py
--rw-r--r--   0        0        0     1407 2024-03-23 00:10:57.607432 gwcelery-2.3.2/gwcelery/tasks/legacy_gracedb.py
--rw-r--r--   0        0        0     8556 2024-03-23 00:10:57.608432 gwcelery-2.3.2/gwcelery/tasks/notice_text.py
--rw-r--r--   0        0        0    57527 2024-03-23 00:10:57.608432 gwcelery-2.3.2/gwcelery/tasks/orchestrator.py
--rw-r--r--   0        0        0     5847 2024-03-23 00:10:57.608432 gwcelery-2.3.2/gwcelery/tasks/p_astro.py
--rw-r--r--   0        0        0    24536 2024-03-23 00:10:57.608432 gwcelery-2.3.2/gwcelery/tasks/raven.py
--rw-r--r--   0        0        0     2264 2024-03-23 00:10:57.609432 gwcelery-2.3.2/gwcelery/tasks/rrt_utils.py
--rw-r--r--   0        0        0     9510 2024-03-23 00:10:57.609432 gwcelery-2.3.2/gwcelery/tasks/skymaps.py
--rw-r--r--   0        0        0    25166 2024-03-23 00:10:57.609432 gwcelery-2.3.2/gwcelery/tasks/superevents.py
--rw-r--r--   0        0        0     1084 2024-03-23 00:10:57.609432 gwcelery-2.3.2/gwcelery/templates/fits_header.jinja2
--rw-r--r--   0        0        0    41294 2024-03-23 00:10:57.610432 gwcelery-2.3.2/gwcelery/templates/index.jinja2
--rw-r--r--   0        0        0     8505 2024-03-23 00:10:57.610432 gwcelery-2.3.2/gwcelery/templates/lalinference.jinja2
--rw-r--r--   0        0        0     9473 2024-03-23 00:10:57.610432 gwcelery-2.3.2/gwcelery/templates/rapidpe.jinja2
--rw-r--r--   0        0        0      472 2024-03-23 00:10:57.610432 gwcelery-2.3.2/gwcelery/templates/vector_table.jinja2
--rw-r--r--   0        0        0        0 2024-03-23 00:10:57.771437 gwcelery-2.3.2/gwcelery/tests/__init__.py
--rw-r--r--   0        0        0     4388 2024-03-23 00:10:57.610432 gwcelery-2.3.2/gwcelery/tests/conftest.py
--rw-r--r--   0        0        0      976 2024-03-23 00:10:57.610432 gwcelery-2.3.2/gwcelery/tests/data/G000012_S0040_preferred.json
--rw-r--r--   0        0        0     6258 2024-03-23 00:10:57.611432 gwcelery-2.3.2/gwcelery/tests/data/G298048-1-Initial.xml
--rw-r--r--   0        0        0      599 2024-03-23 00:10:57.611432 gwcelery-2.3.2/gwcelery/tests/data/G298048_log.json
--rw-r--r--   0        0        0      150 2024-03-23 00:10:57.611432 gwcelery-2.3.2/gwcelery/tests/data/H1L1V1-mean_counts-1126051217-61603201.json
--rw-r--r--   0        0        0      974 2024-03-23 00:10:57.611432 gwcelery-2.3.2/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json
--rw-r--r--   0        0        0    17572 2024-03-23 00:10:57.611432 gwcelery-2.3.2/gwcelery/tests/data/MS220722v.json
--rw-r--r--   0        0        0   777600 2024-03-23 00:10:57.617432 gwcelery-2.3.2/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits
--rw-r--r--   0        0        0     8232 2024-03-23 00:10:57.617432 gwcelery-2.3.2/gwcelery/tests/data/S230413b.json
--rw-r--r--   0        0        0     7255 2024-03-23 00:10:57.618432 gwcelery-2.3.2/gwcelery/tests/data/S230413g.json
--rw-r--r--   0        0        0     7721 2024-03-23 00:10:57.618432 gwcelery-2.3.2/gwcelery/tests/data/S230413h.json
--rw-r--r--   0        0        0     3387 2024-03-23 00:10:57.618432 gwcelery-2.3.2/gwcelery/tests/data/T0212_S0039_preferred.json
--rw-r--r--   0        0        0     3384 2024-03-23 00:10:57.618432 gwcelery-2.3.2/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json
--rw-r--r--   0        0        0     5210 2024-03-23 00:10:57.618432 gwcelery-2.3.2/gwcelery/tests/data/T0219_S0041_nopreferred.json
--rw-r--r--   0        0        0        0 2024-03-23 00:10:57.773437 gwcelery-2.3.2/gwcelery/tests/data/__init__.py
--rw-r--r--   0        0        0     2290 2024-03-23 00:10:57.618432 gwcelery-2.3.2/gwcelery/tests/data/agile_grb_gcn.xml
--rw-r--r--   0        0        0   854036 2024-03-23 00:10:57.624432 gwcelery-2.3.2/gwcelery/tests/data/coinc.xml
--rw-r--r--   0        0        0     6175 2024-03-23 00:10:57.624432 gwcelery-2.3.2/gwcelery/tests/data/externaltrigger_original_data.xml
--rw-r--r--   0        0        0     5482 2024-03-23 00:10:57.624432 gwcelery-2.3.2/gwcelery/tests/data/fermi_grb_gcn.xml
--rw-r--r--   0        0        0     5469 2024-03-23 00:10:57.624432 gwcelery-2.3.2/gwcelery/tests/data/fermi_initial_grb_gcn.xml
--rw-r--r--   0        0        0     5865 2024-03-23 00:10:57.625432 gwcelery-2.3.2/gwcelery/tests/data/fermi_noise_gcn.xml
--rw-r--r--   0        0        0     5864 2024-03-23 00:10:57.625432 gwcelery-2.3.2/gwcelery/tests/data/fermi_noise_gcn_2.xml
--rw-r--r--   0        0        0     1922 2024-03-23 00:10:57.625432 gwcelery-2.3.2/gwcelery/tests/data/fermi_subgrbtargeted_template.xml
--rw-r--r--   0        0        0     4914 2024-03-23 00:10:57.625432 gwcelery-2.3.2/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml
--rw-r--r--   0        0        0     4914 2024-03-23 00:10:57.625432 gwcelery-2.3.2/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml
--rw-r--r--   0        0        0     3407 2024-03-23 00:10:57.625432 gwcelery-2.3.2/gwcelery/tests/data/fits_header_result.html
--rw-r--r--   0        0        0      882 2024-03-23 00:10:57.625432 gwcelery-2.3.2/gwcelery/tests/data/gracedb_externaltrigger_log.json
--rw-r--r--   0        0        0      446 2024-03-23 00:10:57.625432 gwcelery-2.3.2/gwcelery/tests/data/gracedb_setrigger_log.json
--rw-r--r--   0        0        0      870 2024-03-23 00:10:57.625432 gwcelery-2.3.2/gwcelery/tests/data/igwn_alert_detchar.json
--rw-r--r--   0        0        0     2025 2024-03-23 00:10:57.625432 gwcelery-2.3.2/gwcelery/tests/data/igwn_alert_exttrig_creation.json
--rw-r--r--   0        0        0     2007 2024-03-23 00:10:57.626432 gwcelery-2.3.2/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json
--rw-r--r--   0        0        0      166 2024-03-23 00:10:57.626432 gwcelery-2.3.2/gwcelery/tests/data/igwn_alert_fits.json
--rw-r--r--   0        0        0      101 2024-03-23 00:10:57.626432 gwcelery-2.3.2/gwcelery/tests/data/igwn_alert_label_dqv.json
--rw-r--r--   0        0        0      743 2024-03-23 00:10:57.626432 gwcelery-2.3.2/gwcelery/tests/data/igwn_alert_psd.json
--rw-r--r--   0        0        0     2020 2024-03-23 00:10:57.626432 gwcelery-2.3.2/gwcelery/tests/data/igwn_alert_snews_creation.json
--rw-r--r--   0        0        0     2012 2024-03-23 00:10:57.626432 gwcelery-2.3.2/gwcelery/tests/data/igwn_alert_snews_test_creation.json
--rw-r--r--   0        0        0     2028 2024-03-23 00:10:57.626432 gwcelery-2.3.2/gwcelery/tests/data/igwn_alert_subgrb_creation.json
--rw-r--r--   0        0        0     1235 2024-03-23 00:10:57.626432 gwcelery-2.3.2/gwcelery/tests/data/igwn_alert_superevent_creation.json
--rw-r--r--   0        0        0      107 2024-03-23 00:10:57.626432 gwcelery-2.3.2/gwcelery/tests/data/igwn_alert_superevent_label.json
--rw-r--r--   0        0        0     5021 2024-03-23 00:10:57.626432 gwcelery-2.3.2/gwcelery/tests/data/igwn_alert_voevent.json
--rw-r--r--   0        0        0     4429 2024-03-23 00:10:57.626432 gwcelery-2.3.2/gwcelery/tests/data/integral_grb_gcn.xml
--rw-r--r--   0        0        0     4295 2024-03-23 00:10:57.627432 gwcelery-2.3.2/gwcelery/tests/data/integral_mdc_gcn.xml
--rw-r--r--   0        0        0     4451 2024-03-23 00:10:57.627432 gwcelery-2.3.2/gwcelery/tests/data/integral_test_gcn.xml
--rw-r--r--   0        0        0  1038044 2024-03-23 00:10:57.636433 gwcelery-2.3.2/gwcelery/tests/data/kafka_alert_fermi.json
--rw-r--r--   0        0        0  1038042 2024-03-23 00:10:57.638433 gwcelery-2.3.2/gwcelery/tests/data/kafka_alert_fermi_ignore.json
--rw-r--r--   0        0        0      806 2024-03-23 00:10:57.639433 gwcelery-2.3.2/gwcelery/tests/data/kafka_alert_swift.json
--rw-r--r--   0        0        0      743 2024-03-23 00:10:57.639433 gwcelery-2.3.2/gwcelery/tests/data/kafka_alert_swift_noloc.json
--rw-r--r--   0        0        0  1037630 2024-03-23 00:10:57.641433 gwcelery-2.3.2/gwcelery/tests/data/kafka_alert_swift_wskymap.json
--rw-r--r--   0        0        0        0 2024-03-23 00:10:57.775437 gwcelery-2.3.2/gwcelery/tests/data/llhoft/__init__.py
--rw-r--r--   0        0        0     8267 2024-03-23 00:10:57.643433 gwcelery-2.3.2/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf
--rw-r--r--   0        0        0        0 2024-03-23 00:10:57.775437 gwcelery-2.3.2/gwcelery/tests/data/llhoft/fail/L1/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 00:10:57.776437 gwcelery-2.3.2/gwcelery/tests/data/llhoft/fail/__init__.py
--rw-r--r--   0        0        0    14942 2024-03-23 00:10:57.643433 gwcelery-2.3.2/gwcelery/tests/data/llhoft/idqbad/H1/H-H1_O2_llhoft-1216577976-4.gwf
--rw-r--r--   0        0        0        0 2024-03-23 00:10:57.776437 gwcelery-2.3.2/gwcelery/tests/data/llhoft/omegascan/__init__.py
--rw-r--r--   0        0        0   516419 2024-03-23 00:10:57.645433 gwcelery-2.3.2/gwcelery/tests/data/llhoft/omegascan/scanme.gwf
--rw-r--r--   0        0        0    14950 2024-03-23 00:10:57.645433 gwcelery-2.3.2/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf
--rw-r--r--   0        0        0        0 2024-03-23 00:10:57.776437 gwcelery-2.3.2/gwcelery/tests/data/llhoft/pass/H1/__init__.py
--rw-r--r--   0        0        0        0 2024-03-23 00:10:57.776437 gwcelery-2.3.2/gwcelery/tests/data/llhoft/pass/__init__.py
--rw-r--r--   0        0        0    13099 2024-03-23 00:10:57.645433 gwcelery-2.3.2/gwcelery/tests/data/lvalert_event_creation.json
--rw-r--r--   0        0        0     9060 2024-03-23 00:10:57.645433 gwcelery-2.3.2/gwcelery/tests/data/lvalert_xmpp.xml
--rw-r--r--   0        0        0      864 2024-03-23 00:10:57.646433 gwcelery-2.3.2/gwcelery/tests/data/mock_superevent_object.json
--rw-r--r--   0        0        0   445440 2024-03-23 00:10:57.647433 gwcelery-2.3.2/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite
--rw-r--r--   0        0        0   294426 2024-03-23 00:10:57.649433 gwcelery-2.3.2/gwcelery/tests/data/psd.xml.gz
--rw-r--r--   0        0        0    11520 2024-03-23 00:10:57.649433 gwcelery-2.3.2/gwcelery/tests/data/rrt_small_area.fits
--rw-r--r--   0        0        0     2961 2024-03-23 00:10:57.649433 gwcelery-2.3.2/gwcelery/tests/data/sample_events.json
--rw-r--r--   0        0        0     3648 2024-03-23 00:10:57.649433 gwcelery-2.3.2/gwcelery/tests/data/samples.hdf5
--rw-r--r--   0        0        0      616 2024-03-23 00:10:57.649433 gwcelery-2.3.2/gwcelery/tests/data/scaler_set_all.pickle
--rw-r--r--   0        0        0     6169 2024-03-23 00:10:57.649433 gwcelery-2.3.2/gwcelery/tests/data/snews_gcn.xml
--rw-r--r--   0        0        0     6161 2024-03-23 00:10:57.649433 gwcelery-2.3.2/gwcelery/tests/data/snews_gcn_test.xml
--rw-r--r--   0        0        0     9583 2024-03-23 00:10:57.650433 gwcelery-2.3.2/gwcelery/tests/data/superevents.json
--rw-r--r--   0        0        0     7713 2024-03-23 00:10:57.650433 gwcelery-2.3.2/gwcelery/tests/data/swift_grb_gcn.xml
--rw-r--r--   0        0        0     1970 2024-03-23 00:10:57.650433 gwcelery-2.3.2/gwcelery/tests/data/swift_subgrbtargeted_template.xml
--rw-r--r--   0        0        0   581918 2024-03-23 00:10:57.653433 gwcelery-2.3.2/gwcelery/tests/data/test_classifier.pickle
--rw-r--r--   0        0        0      122 2024-03-23 00:10:57.653433 gwcelery-2.3.2/gwcelery/tests/data/updated_RapidPE_RIFT.p_astro.json
--rw-r--r--   0        0        0     4063 2024-03-23 00:10:57.653433 gwcelery-2.3.2/gwcelery/tests/process.py
--rw-r--r--   0        0        0     2307 2024-03-23 00:10:57.653433 gwcelery-2.3.2/gwcelery/tests/test_sentry.py
--rw-r--r--   0        0        0     1669 2024-03-23 00:10:57.653433 gwcelery-2.3.2/gwcelery/tests/test_tasks_alerts.py
--rw-r--r--   0        0        0     4815 2024-03-23 00:10:57.653433 gwcelery-2.3.2/gwcelery/tests/test_tasks_alerts_validate.py
--rw-r--r--   0        0        0     1428 2024-03-23 00:10:57.653433 gwcelery-2.3.2/gwcelery/tests/test_tasks_bayestar.py
--rw-r--r--   0        0        0     3172 2024-03-23 00:10:57.654433 gwcelery-2.3.2/gwcelery/tests/test_tasks_circulars.py
--rw-r--r--   0        0        0     4550 2024-03-23 00:10:57.654433 gwcelery-2.3.2/gwcelery/tests/test_tasks_condor.py
--rw-r--r--   0        0        0    17285 2024-03-23 00:10:57.654433 gwcelery-2.3.2/gwcelery/tests/test_tasks_detchar.py
--rw-r--r--   0        0        0     2317 2024-03-23 00:10:57.654433 gwcelery-2.3.2/gwcelery/tests/test_tasks_em_bright.py
--rw-r--r--   0        0        0    17442 2024-03-23 00:10:57.654433 gwcelery-2.3.2/gwcelery/tests/test_tasks_external_skymaps.py
--rw-r--r--   0        0        0    42927 2024-03-23 00:10:57.655433 gwcelery-2.3.2/gwcelery/tests/test_tasks_external_triggers.py
--rw-r--r--   0        0        0     1797 2024-03-23 00:10:57.655433 gwcelery-2.3.2/gwcelery/tests/test_tasks_first2years.py
--rw-r--r--   0        0        0     7026 2024-03-23 00:10:57.655433 gwcelery-2.3.2/gwcelery/tests/test_tasks_first2years_external.py
--rw-r--r--   0        0        0     1815 2024-03-23 00:10:57.655433 gwcelery-2.3.2/gwcelery/tests/test_tasks_gcn.py
--rw-r--r--   0        0        0     1616 2024-03-23 00:10:57.655433 gwcelery-2.3.2/gwcelery/tests/test_tasks_gcn_validate.py
--rw-r--r--   0        0        0     5728 2024-03-23 00:10:57.655433 gwcelery-2.3.2/gwcelery/tests/test_tasks_gracedb.py
--rw-r--r--   0        0        0     9664 2024-03-23 00:10:57.655433 gwcelery-2.3.2/gwcelery/tests/test_tasks_gwskynet.py
--rw-r--r--   0        0        0     3676 2024-03-23 00:10:57.656433 gwcelery-2.3.2/gwcelery/tests/test_tasks_igwn_alert.py
--rw-r--r--   0        0        0    28978 2024-03-23 00:10:57.656433 gwcelery-2.3.2/gwcelery/tests/test_tasks_inference.py
--rw-r--r--   0        0        0    50392 2024-03-23 00:10:57.656433 gwcelery-2.3.2/gwcelery/tests/test_tasks_orchestrator.py
--rw-r--r--   0        0        0     1647 2024-03-23 00:10:57.656433 gwcelery-2.3.2/gwcelery/tests/test_tasks_p_astro.py
--rw-r--r--   0        0        0    28405 2024-03-23 00:10:57.657433 gwcelery-2.3.2/gwcelery/tests/test_tasks_raven.py
--rw-r--r--   0        0        0     4696 2024-03-23 00:10:57.657433 gwcelery-2.3.2/gwcelery/tests/test_tasks_rrt_utils.py
--rw-r--r--   0        0        0     5520 2024-03-23 00:10:57.657433 gwcelery-2.3.2/gwcelery/tests/test_tasks_skymaps.py
--rw-r--r--   0        0        0    50557 2024-03-23 00:10:57.657433 gwcelery-2.3.2/gwcelery/tests/test_tasks_superevents.py
--rw-r--r--   0        0        0      637 2024-03-23 00:10:57.658433 gwcelery-2.3.2/gwcelery/tests/test_tempfile.py
--rw-r--r--   0        0        0     3520 2024-03-23 00:10:57.658433 gwcelery-2.3.2/gwcelery/tests/test_tools_condor.py
--rw-r--r--   0        0        0     1098 2024-03-23 00:10:57.658433 gwcelery-2.3.2/gwcelery/tests/test_tools_condor_submit_helper.py
--rw-r--r--   0        0        0      647 2024-03-23 00:10:57.658433 gwcelery-2.3.2/gwcelery/tests/test_tools_flask.py
--rw-r--r--   0        0        0    11271 2024-03-23 00:10:57.658433 gwcelery-2.3.2/gwcelery/tests/test_tools_nagios.py
--rw-r--r--   0        0        0      269 2024-03-23 00:10:57.658433 gwcelery-2.3.2/gwcelery/tests/test_util.py
--rw-r--r--   0        0        0    25205 2024-03-23 00:10:57.659433 gwcelery-2.3.2/gwcelery/tests/test_views.py
--rw-r--r--   0        0        0      216 2024-03-23 00:10:57.659433 gwcelery-2.3.2/gwcelery/tools/__init__.py
--rw-r--r--   0        0        0     2941 2024-03-23 00:10:57.659433 gwcelery-2.3.2/gwcelery/tools/condor.py
--rw-r--r--   0        0        0     1120 2024-03-23 00:10:57.659433 gwcelery-2.3.2/gwcelery/tools/condor_submit_helper.py
--rw-r--r--   0        0        0     1938 2024-03-23 00:10:57.659433 gwcelery-2.3.2/gwcelery/tools/flask.py
--rw-r--r--   0        0        0     9145 2024-03-23 00:10:57.659433 gwcelery-2.3.2/gwcelery/tools/nagios.py
--rw-r--r--   0        0        0      413 2024-03-23 00:10:57.660433 gwcelery-2.3.2/gwcelery/util/__init__.py
--rw-r--r--   0        0        0     1007 2024-03-23 00:10:57.660433 gwcelery-2.3.2/gwcelery/util/cmdline.py
--rw-r--r--   0        0        0      453 2024-03-23 00:10:57.660433 gwcelery-2.3.2/gwcelery/util/matplotlib.py
--rw-r--r--   0        0        0      390 2024-03-23 00:10:57.660433 gwcelery-2.3.2/gwcelery/util/proxy.py
--rw-r--r--   0        0        0      585 2024-03-23 00:10:57.660433 gwcelery-2.3.2/gwcelery/util/resources.py
--rw-r--r--   0        0        0      253 2024-03-23 00:10:57.660433 gwcelery-2.3.2/gwcelery/util/sphinx.py
--rw-r--r--   0        0        0      941 2024-03-23 00:10:57.660433 gwcelery-2.3.2/gwcelery/util/tempfile.py
--rw-r--r--   0        0        0    21881 2024-03-23 00:10:57.661434 gwcelery-2.3.2/gwcelery/views.py
--rw-r--r--   0        0        0      365 2024-03-23 00:10:57.661434 gwcelery-2.3.2/gwcelery/voevent/__init__.py
--rw-r--r--   0        0        0     6388 2024-03-23 00:10:57.661434 gwcelery-2.3.2/gwcelery/voevent/bootsteps.py
--rw-r--r--   0        0        0     1063 2024-03-23 00:10:57.661434 gwcelery-2.3.2/gwcelery/voevent/logging.py
--rw-r--r--   0        0        0      779 2024-03-23 00:10:57.661434 gwcelery-2.3.2/gwcelery/voevent/signals.py
--rw-r--r--   0        0        0      884 2024-03-23 00:10:57.661434 gwcelery-2.3.2/gwcelery/voevent/subscriber.py
--rw-r--r--   0        0        0     1454 2024-03-23 00:10:57.661434 gwcelery-2.3.2/gwcelery/voevent/util.py
--rw-r--r--   0        0        0     6499 2024-03-23 00:11:07.265740 gwcelery-2.3.2/pyproject.toml
--rw-r--r--   0        0        0     4666 1970-01-01 00:00:00.000000 gwcelery-2.3.2/PKG-INFO
+-rw-r--r--   0        0        0   108174 2024-04-02 01:14:25.802385 gwcelery-2.3.3/CHANGES.rst
+-rw-r--r--   0        0        0       64 2024-03-30 14:50:09.776096 gwcelery-2.3.3/CONTRIBUTING.rst
+-rw-r--r--   0        0        0    19716 2024-03-30 14:50:09.776096 gwcelery-2.3.3/LICENSE.rst
+-rw-r--r--   0        0        0     1351 2024-03-30 14:50:09.776096 gwcelery-2.3.3/README.rst
+-rw-r--r--   0        0        0      634 2024-03-30 14:50:09.776096 gwcelery-2.3.3/doc/Makefile
+-rw-r--r--   0        0        0   191486 2024-03-30 14:50:09.777096 gwcelery-2.3.3/doc/_static/acceptance-tests-checklist.png
+-rw-r--r--   0        0        0   241593 2024-03-30 14:50:09.778096 gwcelery-2.3.3/doc/_static/celeryevent-screenshot.png
+-rw-r--r--   0        0        0   206465 2024-03-30 14:50:09.779096 gwcelery-2.3.3/doc/_static/deployment-screenshot.png
+-rw-r--r--   0        0        0   161306 2024-03-30 14:50:09.780096 gwcelery-2.3.3/doc/_static/flask-screenshot.png
+-rw-r--r--   0        0        0   328056 2024-04-02 01:14:25.805385 gwcelery-2.3.3/doc/_static/flower-screenshot.png
+-rw-r--r--   0        0        0   114719 2024-03-30 14:50:09.783096 gwcelery-2.3.3/doc/_static/logo-0.5x.png
+-rw-r--r--   0        0        0   351955 2024-03-30 14:50:09.784096 gwcelery-2.3.3/doc/_static/logo.png
+-rw-r--r--   0        0        0   230777 2024-04-02 01:14:25.807386 gwcelery-2.3.3/doc/_static/sentry-screenshot.png
+-rwxr-xr-x   0        0        0     7356 2024-03-30 14:50:09.795096 gwcelery-2.3.3/doc/conf.py
+-rw-r--r--   0        0        0     4346 2024-03-30 14:50:09.795096 gwcelery-2.3.3/doc/configuration.rst
+-rw-r--r--   0        0        0     5698 2024-03-30 14:50:09.795096 gwcelery-2.3.3/doc/contributing.rst
+-rw-r--r--   0        0        0    10846 2024-03-30 14:50:09.796096 gwcelery-2.3.3/doc/deployment.rst
+-rw-r--r--   0        0        0    10308 2024-04-02 01:14:25.807386 gwcelery-2.3.3/doc/design.rst
+-rw-r--r--   0        0        0      563 2024-03-30 14:50:09.796096 gwcelery-2.3.3/doc/gwcelery.conf.rst
+-rw-r--r--   0        0        0      284 2024-03-30 14:50:09.796096 gwcelery-2.3.3/doc/gwcelery.email.rst
+-rw-r--r--   0        0        0      329 2024-03-30 14:50:09.796096 gwcelery-2.3.3/doc/gwcelery.igwn_alert.rst
+-rw-r--r--   0        0        0      227 2024-03-30 14:50:09.796096 gwcelery-2.3.3/doc/gwcelery.rst
+-rw-r--r--   0        0        0       79 2024-03-30 14:50:09.796096 gwcelery-2.3.3/doc/gwcelery.sentry.rst
+-rw-r--r--   0        0        0       97 2024-03-30 14:50:09.796096 gwcelery-2.3.3/doc/gwcelery.tasks.alerts.rst
+-rw-r--r--   0        0        0      103 2024-03-30 14:50:09.796096 gwcelery-2.3.3/doc/gwcelery.tasks.bayestar.rst
+-rw-r--r--   0        0        0      107 2024-03-30 14:50:09.796096 gwcelery-2.3.3/doc/gwcelery.tasks.circulars.rst
+-rw-r--r--   0        0        0       98 2024-03-30 14:50:09.796096 gwcelery-2.3.3/doc/gwcelery.tasks.condor.rst
+-rw-r--r--   0        0        0       91 2024-03-30 14:50:09.796096 gwcelery-2.3.3/doc/gwcelery.tasks.core.rst
+-rw-r--r--   0        0        0     2404 2024-03-30 14:50:09.796096 gwcelery-2.3.3/doc/gwcelery.tasks.detchar.rst
+-rw-r--r--   0        0        0     1110 2024-03-30 14:50:09.796096 gwcelery-2.3.3/doc/gwcelery.tasks.em_bright.rst
+-rw-r--r--   0        0        0      129 2024-03-30 14:50:09.796096 gwcelery-2.3.3/doc/gwcelery.tasks.external_skymaps.rst
+-rw-r--r--   0        0        0     9887 2024-04-02 01:14:25.807386 gwcelery-2.3.3/doc/gwcelery.tasks.external_triggers.rst
+-rw-r--r--   0        0        0      112 2024-03-30 14:50:09.797096 gwcelery-2.3.3/doc/gwcelery.tasks.first2years.rst
+-rw-r--r--   0        0        0      139 2024-03-30 14:50:09.797096 gwcelery-2.3.3/doc/gwcelery.tasks.first2years_external.rst
+-rw-r--r--   0        0        0       88 2024-03-30 14:50:09.797096 gwcelery-2.3.3/doc/gwcelery.tasks.gcn.rst
+-rw-r--r--   0        0        0      100 2024-03-30 14:50:09.797096 gwcelery-2.3.3/doc/gwcelery.tasks.gracedb.rst
+-rw-r--r--   0        0        0      103 2024-03-30 14:50:09.797096 gwcelery-2.3.3/doc/gwcelery.tasks.gwskynet.rst
+-rw-r--r--   0        0        0      109 2024-03-30 14:50:09.797096 gwcelery-2.3.3/doc/gwcelery.tasks.igwn_alert.rst
+-rw-r--r--   0        0        0      109 2024-03-30 14:50:09.797096 gwcelery-2.3.3/doc/gwcelery.tasks.inference.rst
+-rw-r--r--   0        0        0      121 2024-03-30 14:50:09.797096 gwcelery-2.3.3/doc/gwcelery.tasks.legacy_gracedb.rst
+-rw-r--r--   0        0        0      112 2024-03-30 14:50:09.797096 gwcelery-2.3.3/doc/gwcelery.tasks.notice_text.rst
+-rw-r--r--   0        0        0     8111 2024-03-30 14:50:09.797096 gwcelery-2.3.3/doc/gwcelery.tasks.orchestrator.rst
+-rw-r--r--   0        0        0      100 2024-03-30 14:50:09.797096 gwcelery-2.3.3/doc/gwcelery.tasks.p_astro.rst
+-rw-r--r--   0        0        0     2385 2024-03-30 14:50:09.797096 gwcelery-2.3.3/doc/gwcelery.tasks.raven.rst
+-rw-r--r--   0        0        0      106 2024-03-30 14:50:09.797096 gwcelery-2.3.3/doc/gwcelery.tasks.rrt_utils.rst
+-rw-r--r--   0        0        0      814 2024-03-30 14:50:09.797096 gwcelery-2.3.3/doc/gwcelery.tasks.rst
+-rw-r--r--   0        0        0      100 2024-03-30 14:50:09.797096 gwcelery-2.3.3/doc/gwcelery.tasks.skymaps.rst
+-rw-r--r--   0        0        0     7161 2024-03-30 14:50:09.797096 gwcelery-2.3.3/doc/gwcelery.tasks.superevents.rst
+-rw-r--r--   0        0        0       97 2024-03-30 14:50:09.797096 gwcelery-2.3.3/doc/gwcelery.tools.condor.rst
+-rw-r--r--   0        0        0       94 2024-03-30 14:50:09.797096 gwcelery-2.3.3/doc/gwcelery.tools.flask.rst
+-rw-r--r--   0        0        0       97 2024-03-30 14:50:09.798096 gwcelery-2.3.3/doc/gwcelery.tools.nagios.rst
+-rw-r--r--   0        0        0      185 2024-03-30 14:50:09.798096 gwcelery-2.3.3/doc/gwcelery.tools.rst
+-rw-r--r--   0        0        0       73 2024-03-30 14:50:09.798096 gwcelery-2.3.3/doc/gwcelery.util.rst
+-rw-r--r--   0        0        0      507 2024-03-30 14:50:09.798096 gwcelery-2.3.3/doc/gwcelery.voevent.rst
+-rw-r--r--   0        0        0     3564 2024-03-30 14:50:09.798096 gwcelery-2.3.3/doc/htcondor.rst
+-rw-r--r--   0        0        0     1576 2024-03-30 14:50:09.798096 gwcelery-2.3.3/doc/index.rst
+-rw-r--r--   0        0        0      800 2024-03-30 14:50:09.798096 gwcelery-2.3.3/doc/make.bat
+-rw-r--r--   0        0        0     5541 2024-04-02 01:14:25.807386 gwcelery-2.3.3/doc/monitoring.rst
+-rw-r--r--   0        0        0     5405 2024-03-30 14:50:09.798096 gwcelery-2.3.3/doc/quickstart.rst
+-rw-r--r--   0        0        0     1097 2024-03-30 14:50:09.798096 gwcelery-2.3.3/gwcelery/__init__.py
+-rw-r--r--   0        0        0    18447 2024-03-30 14:50:09.798096 gwcelery-2.3.3/gwcelery/_version.py
+-rw-r--r--   0        0        0    19514 2024-04-02 01:14:25.808385 gwcelery-2.3.3/gwcelery/conf/__init__.py
+-rw-r--r--   0        0        0     1195 2024-03-30 14:50:09.799096 gwcelery-2.3.3/gwcelery/conf/dev.py
+-rw-r--r--   0        0        0     1180 2024-03-30 14:50:09.799096 gwcelery-2.3.3/gwcelery/conf/minikube.py
+-rw-r--r--   0        0        0     2178 2024-03-30 14:50:09.799096 gwcelery-2.3.3/gwcelery/conf/playground.py
+-rw-r--r--   0        0        0     3687 2024-03-30 14:50:09.799096 gwcelery-2.3.3/gwcelery/conf/production.py
+-rw-r--r--   0        0        0     2040 2024-03-30 14:50:09.799096 gwcelery-2.3.3/gwcelery/conf/test.py
+-rw-r--r--   0        0        0        0 2024-04-02 01:14:26.210388 gwcelery-2.3.3/gwcelery/data/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 01:14:26.210388 gwcelery-2.3.3/gwcelery/data/first2years/__init__.py
+-rw-r--r--   0        0        0   731421 2024-03-30 14:50:09.801096 gwcelery-2.3.3/gwcelery/data/first2years/gstlal.xml.gz
+-rwxr-xr-x   0        0        0     3199 2024-03-30 14:50:09.801096 gwcelery-2.3.3/gwcelery/data/gwcelery.sub
+-rw-r--r--   0        0        0      505 2024-03-30 14:50:09.801096 gwcelery-2.3.3/gwcelery/email/__init__.py
+-rw-r--r--   0        0        0     3317 2024-04-02 01:14:25.808385 gwcelery-2.3.3/gwcelery/email/bootsteps.py
+-rw-r--r--   0        0        0      995 2024-03-30 14:50:09.801096 gwcelery-2.3.3/gwcelery/email/signals.py
+-rw-r--r--   0        0        0     1457 2024-03-30 14:50:09.802096 gwcelery-2.3.3/gwcelery/flask.py
+-rw-r--r--   0        0        0      529 2024-03-30 14:50:09.802096 gwcelery-2.3.3/gwcelery/igwn_alert/__init__.py
+-rw-r--r--   0        0        0     4484 2024-03-30 14:50:09.802096 gwcelery-2.3.3/gwcelery/igwn_alert/bootsteps.py
+-rw-r--r--   0        0        0      608 2024-03-30 14:50:09.802096 gwcelery-2.3.3/gwcelery/igwn_alert/signals.py
+-rw-r--r--   0        0        0      275 2024-03-30 14:50:09.802096 gwcelery-2.3.3/gwcelery/jinja.py
+-rw-r--r--   0        0        0      305 2024-03-30 14:50:09.802096 gwcelery-2.3.3/gwcelery/kafka/__init__.py
+-rw-r--r--   0        0        0    11839 2024-03-30 14:50:09.802096 gwcelery-2.3.3/gwcelery/kafka/bootsteps.py
+-rw-r--r--   0        0        0      522 2024-03-30 14:50:09.802096 gwcelery-2.3.3/gwcelery/kafka/signals.py
+-rw-r--r--   0        0        0     2567 2024-03-30 14:50:09.802096 gwcelery-2.3.3/gwcelery/sentry/__init__.py
+-rw-r--r--   0        0        0       34 2024-03-30 14:50:09.802096 gwcelery-2.3.3/gwcelery/sentry/integrations/__init__.py
+-rw-r--r--   0        0        0      832 2024-03-30 14:50:09.802096 gwcelery-2.3.3/gwcelery/sentry/integrations/condor.py
+-rw-r--r--   0        0        0      836 2024-03-30 14:50:09.802096 gwcelery-2.3.3/gwcelery/sentry/integrations/requests.py
+-rw-r--r--   0        0        0      939 2024-03-30 14:50:09.802096 gwcelery-2.3.3/gwcelery/sentry/integrations/subprocess.py
+-rw-r--r--   0        0        0     1302 2024-03-30 14:50:09.803096 gwcelery-2.3.3/gwcelery/static/typeahead.css
+-rw-r--r--   0        0        0     4124 2024-03-30 14:50:09.803096 gwcelery-2.3.3/gwcelery/static/vega/index.html
+-rw-r--r--   0        0        0      515 2024-03-30 14:50:09.803096 gwcelery-2.3.3/gwcelery/tasks/__init__.py
+-rw-r--r--   0        0        0    14457 2024-03-30 14:50:09.803096 gwcelery-2.3.3/gwcelery/tasks/alerts.py
+-rw-r--r--   0        0        0     2540 2024-03-30 14:50:09.803096 gwcelery-2.3.3/gwcelery/tasks/bayestar.py
+-rw-r--r--   0        0        0     1892 2024-03-30 14:50:09.803096 gwcelery-2.3.3/gwcelery/tasks/circulars.py
+-rw-r--r--   0        0        0     7552 2024-03-30 14:50:09.803096 gwcelery-2.3.3/gwcelery/tasks/condor.py
+-rw-r--r--   0        0        0     2692 2024-03-30 14:50:09.803096 gwcelery-2.3.3/gwcelery/tasks/core.py
+-rw-r--r--   0        0        0    23090 2024-03-30 14:50:09.803096 gwcelery-2.3.3/gwcelery/tasks/detchar.py
+-rw-r--r--   0        0        0     4903 2024-03-30 14:50:09.803096 gwcelery-2.3.3/gwcelery/tasks/em_bright.py
+-rw-r--r--   0        0        0    29615 2024-04-02 01:14:25.808385 gwcelery-2.3.3/gwcelery/tasks/external_skymaps.py
+-rw-r--r--   0        0        0    31983 2024-04-02 01:14:25.809386 gwcelery-2.3.3/gwcelery/tasks/external_triggers.py
+-rw-r--r--   0        0        0     6841 2024-03-30 14:50:09.804096 gwcelery-2.3.3/gwcelery/tasks/first2years.py
+-rw-r--r--   0        0        0    10693 2024-04-02 01:14:25.809386 gwcelery-2.3.3/gwcelery/tasks/first2years_external.py
+-rw-r--r--   0        0        0     4832 2024-03-30 14:50:09.804096 gwcelery-2.3.3/gwcelery/tasks/gcn.py
+-rw-r--r--   0        0        0    11080 2024-03-30 14:50:09.804096 gwcelery-2.3.3/gwcelery/tasks/gracedb.py
+-rw-r--r--   0        0        0     6884 2024-03-30 14:50:09.804096 gwcelery-2.3.3/gwcelery/tasks/gwskynet.py
+-rw-r--r--   0        0        0     2453 2024-03-30 14:50:09.804096 gwcelery-2.3.3/gwcelery/tasks/igwn_alert.py
+-rw-r--r--   0        0        0    34975 2024-04-02 01:14:25.809386 gwcelery-2.3.3/gwcelery/tasks/inference.py
+-rw-r--r--   0        0        0     1407 2024-03-30 14:50:09.805096 gwcelery-2.3.3/gwcelery/tasks/legacy_gracedb.py
+-rw-r--r--   0        0        0     8556 2024-03-30 14:50:09.805096 gwcelery-2.3.3/gwcelery/tasks/notice_text.py
+-rw-r--r--   0        0        0    57527 2024-03-30 14:50:09.805096 gwcelery-2.3.3/gwcelery/tasks/orchestrator.py
+-rw-r--r--   0        0        0     5847 2024-03-30 14:50:09.805096 gwcelery-2.3.3/gwcelery/tasks/p_astro.py
+-rw-r--r--   0        0        0    24536 2024-03-30 14:50:09.806096 gwcelery-2.3.3/gwcelery/tasks/raven.py
+-rw-r--r--   0        0        0     2264 2024-03-30 14:50:09.806096 gwcelery-2.3.3/gwcelery/tasks/rrt_utils.py
+-rw-r--r--   0        0        0     9510 2024-03-30 14:50:09.806096 gwcelery-2.3.3/gwcelery/tasks/skymaps.py
+-rw-r--r--   0        0        0    25166 2024-03-30 14:50:09.806096 gwcelery-2.3.3/gwcelery/tasks/superevents.py
+-rw-r--r--   0        0        0     1084 2024-03-30 14:50:09.806096 gwcelery-2.3.3/gwcelery/templates/fits_header.jinja2
+-rw-r--r--   0        0        0    41294 2024-03-30 14:50:09.806096 gwcelery-2.3.3/gwcelery/templates/index.jinja2
+-rw-r--r--   0        0        0     8505 2024-03-30 14:50:09.806096 gwcelery-2.3.3/gwcelery/templates/lalinference.jinja2
+-rw-r--r--   0        0        0     9473 2024-03-30 14:50:09.807096 gwcelery-2.3.3/gwcelery/templates/rapidpe.jinja2
+-rw-r--r--   0        0        0      472 2024-03-30 14:50:09.807096 gwcelery-2.3.3/gwcelery/templates/vector_table.jinja2
+-rw-r--r--   0        0        0        0 2024-04-02 01:14:26.213388 gwcelery-2.3.3/gwcelery/tests/__init__.py
+-rw-r--r--   0        0        0     4388 2024-03-30 14:50:09.807096 gwcelery-2.3.3/gwcelery/tests/conftest.py
+-rw-r--r--   0        0        0      976 2024-03-30 14:50:09.807096 gwcelery-2.3.3/gwcelery/tests/data/G000012_S0040_preferred.json
+-rw-r--r--   0        0        0     6258 2024-03-30 14:50:09.807096 gwcelery-2.3.3/gwcelery/tests/data/G298048-1-Initial.xml
+-rw-r--r--   0        0        0      599 2024-03-30 14:50:09.807096 gwcelery-2.3.3/gwcelery/tests/data/G298048_log.json
+-rw-r--r--   0        0        0      150 2024-03-30 14:50:09.807096 gwcelery-2.3.3/gwcelery/tests/data/H1L1V1-mean_counts-1126051217-61603201.json
+-rw-r--r--   0        0        0      974 2024-03-30 14:50:09.807096 gwcelery-2.3.3/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json
+-rw-r--r--   0        0        0    17572 2024-03-30 14:50:09.807096 gwcelery-2.3.3/gwcelery/tests/data/MS220722v.json
+-rw-r--r--   0        0        0   777600 2024-03-30 14:50:09.811096 gwcelery-2.3.3/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits
+-rw-r--r--   0        0        0     8232 2024-03-30 14:50:09.812096 gwcelery-2.3.3/gwcelery/tests/data/S230413b.json
+-rw-r--r--   0        0        0     7255 2024-03-30 14:50:09.812096 gwcelery-2.3.3/gwcelery/tests/data/S230413g.json
+-rw-r--r--   0        0        0     7721 2024-03-30 14:50:09.812096 gwcelery-2.3.3/gwcelery/tests/data/S230413h.json
+-rw-r--r--   0        0        0     3387 2024-03-30 14:50:09.812096 gwcelery-2.3.3/gwcelery/tests/data/T0212_S0039_preferred.json
+-rw-r--r--   0        0        0     3384 2024-03-30 14:50:09.812096 gwcelery-2.3.3/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json
+-rw-r--r--   0        0        0     5210 2024-03-30 14:50:09.812096 gwcelery-2.3.3/gwcelery/tests/data/T0219_S0041_nopreferred.json
+-rw-r--r--   0        0        0        0 2024-04-02 01:14:26.214388 gwcelery-2.3.3/gwcelery/tests/data/__init__.py
+-rw-r--r--   0        0        0     2290 2024-04-02 01:14:25.810386 gwcelery-2.3.3/gwcelery/tests/data/agile_grb_gcn.xml
+-rw-r--r--   0        0        0   854036 2024-03-30 14:50:09.816096 gwcelery-2.3.3/gwcelery/tests/data/coinc.xml
+-rw-r--r--   0        0        0     6175 2024-03-30 14:50:09.816096 gwcelery-2.3.3/gwcelery/tests/data/externaltrigger_original_data.xml
+-rw-r--r--   0        0        0     5482 2024-03-30 14:50:09.816096 gwcelery-2.3.3/gwcelery/tests/data/fermi_grb_gcn.xml
+-rw-r--r--   0        0        0     5469 2024-03-30 14:50:09.816096 gwcelery-2.3.3/gwcelery/tests/data/fermi_initial_grb_gcn.xml
+-rw-r--r--   0        0        0     5865 2024-03-30 14:50:09.816096 gwcelery-2.3.3/gwcelery/tests/data/fermi_noise_gcn.xml
+-rw-r--r--   0        0        0     5864 2024-03-30 14:50:09.816096 gwcelery-2.3.3/gwcelery/tests/data/fermi_noise_gcn_2.xml
+-rw-r--r--   0        0        0     1922 2024-03-30 14:50:09.817096 gwcelery-2.3.3/gwcelery/tests/data/fermi_subgrbtargeted_template.xml
+-rw-r--r--   0        0        0     4914 2024-03-30 14:50:09.817096 gwcelery-2.3.3/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml
+-rw-r--r--   0        0        0     4914 2024-03-30 14:50:09.817096 gwcelery-2.3.3/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml
+-rw-r--r--   0        0        0     3407 2024-03-30 14:50:09.817096 gwcelery-2.3.3/gwcelery/tests/data/fits_header_result.html
+-rw-r--r--   0        0        0      882 2024-03-30 14:50:09.817096 gwcelery-2.3.3/gwcelery/tests/data/gracedb_externaltrigger_log.json
+-rw-r--r--   0        0        0      446 2024-03-30 14:50:09.817096 gwcelery-2.3.3/gwcelery/tests/data/gracedb_setrigger_log.json
+-rw-r--r--   0        0        0      870 2024-03-30 14:50:09.817096 gwcelery-2.3.3/gwcelery/tests/data/igwn_alert_detchar.json
+-rw-r--r--   0        0        0     2025 2024-03-30 14:50:09.817096 gwcelery-2.3.3/gwcelery/tests/data/igwn_alert_exttrig_creation.json
+-rw-r--r--   0        0        0     2007 2024-03-30 14:50:09.817096 gwcelery-2.3.3/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json
+-rw-r--r--   0        0        0      166 2024-03-30 14:50:09.817096 gwcelery-2.3.3/gwcelery/tests/data/igwn_alert_fits.json
+-rw-r--r--   0        0        0      101 2024-03-30 14:50:09.817096 gwcelery-2.3.3/gwcelery/tests/data/igwn_alert_label_dqv.json
+-rw-r--r--   0        0        0      743 2024-03-30 14:50:09.817096 gwcelery-2.3.3/gwcelery/tests/data/igwn_alert_psd.json
+-rw-r--r--   0        0        0     2020 2024-03-30 14:50:09.817096 gwcelery-2.3.3/gwcelery/tests/data/igwn_alert_snews_creation.json
+-rw-r--r--   0        0        0     2012 2024-03-30 14:50:09.817096 gwcelery-2.3.3/gwcelery/tests/data/igwn_alert_snews_test_creation.json
+-rw-r--r--   0        0        0     2028 2024-03-30 14:50:09.818096 gwcelery-2.3.3/gwcelery/tests/data/igwn_alert_subgrb_creation.json
+-rw-r--r--   0        0        0     1235 2024-03-30 14:50:09.818096 gwcelery-2.3.3/gwcelery/tests/data/igwn_alert_superevent_creation.json
+-rw-r--r--   0        0        0      107 2024-03-30 14:50:09.818096 gwcelery-2.3.3/gwcelery/tests/data/igwn_alert_superevent_label.json
+-rw-r--r--   0        0        0     5021 2024-03-30 14:50:09.818096 gwcelery-2.3.3/gwcelery/tests/data/igwn_alert_voevent.json
+-rw-r--r--   0        0        0     4429 2024-03-30 14:50:09.818096 gwcelery-2.3.3/gwcelery/tests/data/integral_grb_gcn.xml
+-rw-r--r--   0        0        0     4295 2024-03-30 14:50:09.818096 gwcelery-2.3.3/gwcelery/tests/data/integral_mdc_gcn.xml
+-rw-r--r--   0        0        0     4451 2024-03-30 14:50:09.818096 gwcelery-2.3.3/gwcelery/tests/data/integral_test_gcn.xml
+-rw-r--r--   0        0        0  1038044 2024-03-30 14:50:09.824096 gwcelery-2.3.3/gwcelery/tests/data/kafka_alert_fermi.json
+-rw-r--r--   0        0        0  1038042 2024-03-30 14:50:09.827096 gwcelery-2.3.3/gwcelery/tests/data/kafka_alert_fermi_ignore.json
+-rw-r--r--   0        0        0      806 2024-03-30 14:50:09.827096 gwcelery-2.3.3/gwcelery/tests/data/kafka_alert_swift.json
+-rw-r--r--   0        0        0      743 2024-03-30 14:50:09.827096 gwcelery-2.3.3/gwcelery/tests/data/kafka_alert_swift_noloc.json
+-rw-r--r--   0        0        0  1037630 2024-03-30 14:50:09.828096 gwcelery-2.3.3/gwcelery/tests/data/kafka_alert_swift_wskymap.json
+-rw-r--r--   0        0        0        0 2024-04-02 01:14:26.215388 gwcelery-2.3.3/gwcelery/tests/data/llhoft/__init__.py
+-rw-r--r--   0        0        0     8267 2024-03-30 14:50:09.829096 gwcelery-2.3.3/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf
+-rw-r--r--   0        0        0        0 2024-04-02 01:14:26.215388 gwcelery-2.3.3/gwcelery/tests/data/llhoft/fail/L1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 01:14:26.215388 gwcelery-2.3.3/gwcelery/tests/data/llhoft/fail/__init__.py
+-rw-r--r--   0        0        0    14942 2024-03-30 14:50:09.829096 gwcelery-2.3.3/gwcelery/tests/data/llhoft/idqbad/H1/H-H1_O2_llhoft-1216577976-4.gwf
+-rw-r--r--   0        0        0        0 2024-04-02 01:14:26.215388 gwcelery-2.3.3/gwcelery/tests/data/llhoft/omegascan/__init__.py
+-rw-r--r--   0        0        0   516419 2024-03-30 14:50:09.830096 gwcelery-2.3.3/gwcelery/tests/data/llhoft/omegascan/scanme.gwf
+-rw-r--r--   0        0        0    14950 2024-03-30 14:50:09.830096 gwcelery-2.3.3/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf
+-rw-r--r--   0        0        0        0 2024-04-02 01:14:26.215388 gwcelery-2.3.3/gwcelery/tests/data/llhoft/pass/H1/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-02 01:14:26.215388 gwcelery-2.3.3/gwcelery/tests/data/llhoft/pass/__init__.py
+-rw-r--r--   0        0        0    13099 2024-03-30 14:50:09.831096 gwcelery-2.3.3/gwcelery/tests/data/lvalert_event_creation.json
+-rw-r--r--   0        0        0     9060 2024-03-30 14:50:09.831096 gwcelery-2.3.3/gwcelery/tests/data/lvalert_xmpp.xml
+-rw-r--r--   0        0        0      864 2024-03-30 14:50:09.831096 gwcelery-2.3.3/gwcelery/tests/data/mock_superevent_object.json
+-rw-r--r--   0        0        0   445440 2024-03-30 14:50:09.832096 gwcelery-2.3.3/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite
+-rw-r--r--   0        0        0   294426 2024-03-30 14:50:09.833096 gwcelery-2.3.3/gwcelery/tests/data/psd.xml.gz
+-rw-r--r--   0        0        0    11520 2024-03-30 14:50:09.833096 gwcelery-2.3.3/gwcelery/tests/data/rrt_small_area.fits
+-rw-r--r--   0        0        0     2961 2024-03-30 14:50:09.833096 gwcelery-2.3.3/gwcelery/tests/data/sample_events.json
+-rw-r--r--   0        0        0     3648 2024-03-30 14:50:09.834096 gwcelery-2.3.3/gwcelery/tests/data/samples.hdf5
+-rw-r--r--   0        0        0      616 2024-03-30 14:50:09.834096 gwcelery-2.3.3/gwcelery/tests/data/scaler_set_all.pickle
+-rw-r--r--   0        0        0     6169 2024-03-30 14:50:09.834096 gwcelery-2.3.3/gwcelery/tests/data/snews_gcn.xml
+-rw-r--r--   0        0        0     6161 2024-03-30 14:50:09.834096 gwcelery-2.3.3/gwcelery/tests/data/snews_gcn_test.xml
+-rw-r--r--   0        0        0     9583 2024-03-30 14:50:09.834096 gwcelery-2.3.3/gwcelery/tests/data/superevents.json
+-rw-r--r--   0        0        0     7713 2024-03-30 14:50:09.834096 gwcelery-2.3.3/gwcelery/tests/data/swift_grb_gcn.xml
+-rw-r--r--   0        0        0     1970 2024-03-30 14:50:09.834096 gwcelery-2.3.3/gwcelery/tests/data/swift_subgrbtargeted_template.xml
+-rw-r--r--   0        0        0   581918 2024-03-30 14:50:09.836096 gwcelery-2.3.3/gwcelery/tests/data/test_classifier.pickle
+-rw-r--r--   0        0        0      122 2024-03-30 14:50:09.836096 gwcelery-2.3.3/gwcelery/tests/data/updated_RapidPE_RIFT.p_astro.json
+-rw-r--r--   0        0        0     4063 2024-03-30 14:50:09.836096 gwcelery-2.3.3/gwcelery/tests/process.py
+-rw-r--r--   0        0        0     2307 2024-03-30 14:50:09.836096 gwcelery-2.3.3/gwcelery/tests/test_sentry.py
+-rw-r--r--   0        0        0     1669 2024-03-30 14:50:09.836096 gwcelery-2.3.3/gwcelery/tests/test_tasks_alerts.py
+-rw-r--r--   0        0        0     4815 2024-03-30 14:50:09.836096 gwcelery-2.3.3/gwcelery/tests/test_tasks_alerts_validate.py
+-rw-r--r--   0        0        0     1428 2024-03-30 14:50:09.836096 gwcelery-2.3.3/gwcelery/tests/test_tasks_bayestar.py
+-rw-r--r--   0        0        0     3172 2024-03-30 14:50:09.836096 gwcelery-2.3.3/gwcelery/tests/test_tasks_circulars.py
+-rw-r--r--   0        0        0     4550 2024-03-30 14:50:09.837096 gwcelery-2.3.3/gwcelery/tests/test_tasks_condor.py
+-rw-r--r--   0        0        0    17285 2024-03-30 14:50:09.837096 gwcelery-2.3.3/gwcelery/tests/test_tasks_detchar.py
+-rw-r--r--   0        0        0     2317 2024-03-30 14:50:09.837096 gwcelery-2.3.3/gwcelery/tests/test_tasks_em_bright.py
+-rw-r--r--   0        0        0    17442 2024-03-30 14:50:09.837096 gwcelery-2.3.3/gwcelery/tests/test_tasks_external_skymaps.py
+-rw-r--r--   0        0        0    42927 2024-04-02 01:14:25.811385 gwcelery-2.3.3/gwcelery/tests/test_tasks_external_triggers.py
+-rw-r--r--   0        0        0     1797 2024-03-30 14:50:09.837096 gwcelery-2.3.3/gwcelery/tests/test_tasks_first2years.py
+-rw-r--r--   0        0        0     7026 2024-03-30 14:50:09.837096 gwcelery-2.3.3/gwcelery/tests/test_tasks_first2years_external.py
+-rw-r--r--   0        0        0     1815 2024-03-30 14:50:09.837096 gwcelery-2.3.3/gwcelery/tests/test_tasks_gcn.py
+-rw-r--r--   0        0        0     1616 2024-03-30 14:50:09.837096 gwcelery-2.3.3/gwcelery/tests/test_tasks_gcn_validate.py
+-rw-r--r--   0        0        0     5728 2024-03-30 14:50:09.838096 gwcelery-2.3.3/gwcelery/tests/test_tasks_gracedb.py
+-rw-r--r--   0        0        0     9664 2024-03-30 14:50:09.838096 gwcelery-2.3.3/gwcelery/tests/test_tasks_gwskynet.py
+-rw-r--r--   0        0        0     3676 2024-03-30 14:50:09.838096 gwcelery-2.3.3/gwcelery/tests/test_tasks_igwn_alert.py
+-rw-r--r--   0        0        0    28973 2024-04-02 01:14:25.811385 gwcelery-2.3.3/gwcelery/tests/test_tasks_inference.py
+-rw-r--r--   0        0        0    50392 2024-03-30 14:50:09.838096 gwcelery-2.3.3/gwcelery/tests/test_tasks_orchestrator.py
+-rw-r--r--   0        0        0     1647 2024-03-30 14:50:09.838096 gwcelery-2.3.3/gwcelery/tests/test_tasks_p_astro.py
+-rw-r--r--   0        0        0    28405 2024-04-02 01:14:25.812386 gwcelery-2.3.3/gwcelery/tests/test_tasks_raven.py
+-rw-r--r--   0        0        0     4696 2024-03-30 14:50:09.839096 gwcelery-2.3.3/gwcelery/tests/test_tasks_rrt_utils.py
+-rw-r--r--   0        0        0     5520 2024-03-30 14:50:09.839096 gwcelery-2.3.3/gwcelery/tests/test_tasks_skymaps.py
+-rw-r--r--   0        0        0    50557 2024-03-30 14:50:09.839096 gwcelery-2.3.3/gwcelery/tests/test_tasks_superevents.py
+-rw-r--r--   0        0        0      637 2024-03-30 14:50:09.839096 gwcelery-2.3.3/gwcelery/tests/test_tempfile.py
+-rw-r--r--   0        0        0     3520 2024-03-30 14:50:09.839096 gwcelery-2.3.3/gwcelery/tests/test_tools_condor.py
+-rw-r--r--   0        0        0     1098 2024-03-30 14:50:09.839096 gwcelery-2.3.3/gwcelery/tests/test_tools_condor_submit_helper.py
+-rw-r--r--   0        0        0      647 2024-03-30 14:50:09.839096 gwcelery-2.3.3/gwcelery/tests/test_tools_flask.py
+-rw-r--r--   0        0        0    11271 2024-03-30 14:50:09.839096 gwcelery-2.3.3/gwcelery/tests/test_tools_nagios.py
+-rw-r--r--   0        0        0      269 2024-03-30 14:50:09.839096 gwcelery-2.3.3/gwcelery/tests/test_util.py
+-rw-r--r--   0        0        0    25205 2024-03-30 14:50:09.840096 gwcelery-2.3.3/gwcelery/tests/test_views.py
+-rw-r--r--   0        0        0      216 2024-03-30 14:50:09.840096 gwcelery-2.3.3/gwcelery/tools/__init__.py
+-rw-r--r--   0        0        0     2941 2024-03-30 14:50:09.840096 gwcelery-2.3.3/gwcelery/tools/condor.py
+-rw-r--r--   0        0        0     1120 2024-03-30 14:50:09.840096 gwcelery-2.3.3/gwcelery/tools/condor_submit_helper.py
+-rw-r--r--   0        0        0     1938 2024-03-30 14:50:09.840096 gwcelery-2.3.3/gwcelery/tools/flask.py
+-rw-r--r--   0        0        0     9145 2024-03-30 14:50:09.840096 gwcelery-2.3.3/gwcelery/tools/nagios.py
+-rw-r--r--   0        0        0      413 2024-03-30 14:50:09.840096 gwcelery-2.3.3/gwcelery/util/__init__.py
+-rw-r--r--   0        0        0     1007 2024-03-30 14:50:09.840096 gwcelery-2.3.3/gwcelery/util/cmdline.py
+-rw-r--r--   0        0        0      453 2024-03-30 14:50:09.840096 gwcelery-2.3.3/gwcelery/util/matplotlib.py
+-rw-r--r--   0        0        0      390 2024-03-30 14:50:09.840096 gwcelery-2.3.3/gwcelery/util/proxy.py
+-rw-r--r--   0        0        0      585 2024-03-30 14:50:09.840096 gwcelery-2.3.3/gwcelery/util/resources.py
+-rw-r--r--   0        0        0      253 2024-03-30 14:50:09.840096 gwcelery-2.3.3/gwcelery/util/sphinx.py
+-rw-r--r--   0        0        0      941 2024-03-30 14:50:09.840096 gwcelery-2.3.3/gwcelery/util/tempfile.py
+-rw-r--r--   0        0        0    21881 2024-03-30 14:50:09.841096 gwcelery-2.3.3/gwcelery/views.py
+-rw-r--r--   0        0        0      365 2024-03-30 14:50:09.841096 gwcelery-2.3.3/gwcelery/voevent/__init__.py
+-rw-r--r--   0        0        0     6388 2024-03-30 14:50:09.841096 gwcelery-2.3.3/gwcelery/voevent/bootsteps.py
+-rw-r--r--   0        0        0     1063 2024-03-30 14:50:09.841096 gwcelery-2.3.3/gwcelery/voevent/logging.py
+-rw-r--r--   0        0        0      779 2024-03-30 14:50:09.841096 gwcelery-2.3.3/gwcelery/voevent/signals.py
+-rw-r--r--   0        0        0      884 2024-03-30 14:50:09.841096 gwcelery-2.3.3/gwcelery/voevent/subscriber.py
+-rw-r--r--   0        0        0     1454 2024-03-30 14:50:09.841096 gwcelery-2.3.3/gwcelery/voevent/util.py
+-rw-r--r--   0        0        0     6499 2024-04-02 01:14:36.853459 gwcelery-2.3.3/pyproject.toml
+-rw-r--r--   0        0        0     4666 1970-01-01 00:00:00.000000 gwcelery-2.3.3/PKG-INFO
```

### Comparing `gwcelery-2.3.2/CHANGES.rst` & `gwcelery-2.3.3/CHANGES.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+2.3.3 "Champ" (2024-04-01)
+--------------------------
+
+-   Change Bilby accounting group user to cody.messick as temporary workaround
+    while KAGRA accounts are in flux.
+
 2.3.2 "Champ" (2024-03-22)
 --------------------------
 
 -   Enable public alerts on production.
 
 2.3.1 "Champ" (2024-03-22)
 --------------------------
```

### Comparing `gwcelery-2.3.2/LICENSE.rst` & `gwcelery-2.3.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/README.rst` & `gwcelery-2.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/doc/Makefile` & `gwcelery-2.3.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/doc/_static/acceptance-tests-checklist.png` & `gwcelery-2.3.3/doc/_static/acceptance-tests-checklist.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/doc/_static/celeryevent-screenshot.png` & `gwcelery-2.3.3/doc/_static/celeryevent-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/doc/_static/deployment-screenshot.png` & `gwcelery-2.3.3/doc/_static/deployment-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/doc/_static/flask-screenshot.png` & `gwcelery-2.3.3/doc/_static/flask-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/doc/_static/flower-screenshot.png` & `gwcelery-2.3.3/doc/_static/flower-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/doc/_static/logo-0.5x.png` & `gwcelery-2.3.3/doc/_static/logo-0.5x.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/doc/_static/logo.png` & `gwcelery-2.3.3/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/doc/_static/sentry-screenshot.png` & `gwcelery-2.3.3/doc/_static/sentry-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/doc/conf.py` & `gwcelery-2.3.3/doc/conf.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/doc/configuration.rst` & `gwcelery-2.3.3/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/doc/contributing.rst` & `gwcelery-2.3.3/doc/contributing.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/doc/deployment.rst` & `gwcelery-2.3.3/doc/deployment.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/doc/design.rst` & `gwcelery-2.3.3/doc/design.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/doc/gwcelery.conf.rst` & `gwcelery-2.3.3/doc/gwcelery.conf.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/doc/gwcelery.tasks.detchar.rst` & `gwcelery-2.3.3/doc/gwcelery.tasks.detchar.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/doc/gwcelery.tasks.em_bright.rst` & `gwcelery-2.3.3/doc/gwcelery.tasks.em_bright.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/doc/gwcelery.tasks.external_triggers.rst` & `gwcelery-2.3.3/doc/gwcelery.tasks.external_triggers.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/doc/gwcelery.tasks.orchestrator.rst` & `gwcelery-2.3.3/doc/gwcelery.tasks.orchestrator.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/doc/gwcelery.tasks.raven.rst` & `gwcelery-2.3.3/doc/gwcelery.tasks.raven.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/doc/gwcelery.tasks.rst` & `gwcelery-2.3.3/doc/gwcelery.tasks.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/doc/gwcelery.tasks.superevents.rst` & `gwcelery-2.3.3/doc/gwcelery.tasks.superevents.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/doc/htcondor.rst` & `gwcelery-2.3.3/doc/htcondor.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/doc/index.rst` & `gwcelery-2.3.3/doc/index.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/doc/make.bat` & `gwcelery-2.3.3/doc/make.bat`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/doc/monitoring.rst` & `gwcelery-2.3.3/doc/monitoring.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/doc/quickstart.rst` & `gwcelery-2.3.3/doc/quickstart.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/__init__.py` & `gwcelery-2.3.3/gwcelery/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/_version.py` & `gwcelery-2.3.3/gwcelery/_version.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/conf/__init__.py` & `gwcelery-2.3.3/gwcelery/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/conf/dev.py` & `gwcelery-2.3.3/gwcelery/conf/dev.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/conf/minikube.py` & `gwcelery-2.3.3/gwcelery/conf/minikube.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/conf/playground.py` & `gwcelery-2.3.3/gwcelery/conf/playground.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/conf/production.py` & `gwcelery-2.3.3/gwcelery/conf/production.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/conf/test.py` & `gwcelery-2.3.3/gwcelery/conf/test.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/data/first2years/gstlal.xml.gz` & `gwcelery-2.3.3/gwcelery/data/first2years/gstlal.xml.gz`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/data/gwcelery.sub` & `gwcelery-2.3.3/gwcelery/data/gwcelery.sub`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/email/bootsteps.py` & `gwcelery-2.3.3/gwcelery/email/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/email/signals.py` & `gwcelery-2.3.3/gwcelery/email/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/flask.py` & `gwcelery-2.3.3/gwcelery/flask.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/igwn_alert/__init__.py` & `gwcelery-2.3.3/gwcelery/igwn_alert/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/igwn_alert/bootsteps.py` & `gwcelery-2.3.3/gwcelery/igwn_alert/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/igwn_alert/signals.py` & `gwcelery-2.3.3/gwcelery/igwn_alert/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/kafka/bootsteps.py` & `gwcelery-2.3.3/gwcelery/kafka/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/kafka/signals.py` & `gwcelery-2.3.3/gwcelery/kafka/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/sentry/__init__.py` & `gwcelery-2.3.3/gwcelery/sentry/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/sentry/integrations/condor.py` & `gwcelery-2.3.3/gwcelery/sentry/integrations/condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/sentry/integrations/requests.py` & `gwcelery-2.3.3/gwcelery/sentry/integrations/requests.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/sentry/integrations/subprocess.py` & `gwcelery-2.3.3/gwcelery/sentry/integrations/subprocess.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/static/typeahead.css` & `gwcelery-2.3.3/gwcelery/static/typeahead.css`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/static/vega/index.html` & `gwcelery-2.3.3/gwcelery/static/vega/index.html`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tasks/__init__.py` & `gwcelery-2.3.3/gwcelery/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tasks/alerts.py` & `gwcelery-2.3.3/gwcelery/tasks/alerts.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tasks/bayestar.py` & `gwcelery-2.3.3/gwcelery/tasks/bayestar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tasks/circulars.py` & `gwcelery-2.3.3/gwcelery/tasks/circulars.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tasks/condor.py` & `gwcelery-2.3.3/gwcelery/tasks/condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tasks/core.py` & `gwcelery-2.3.3/gwcelery/tasks/core.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tasks/detchar.py` & `gwcelery-2.3.3/gwcelery/tasks/detchar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tasks/em_bright.py` & `gwcelery-2.3.3/gwcelery/tasks/em_bright.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tasks/external_skymaps.py` & `gwcelery-2.3.3/gwcelery/tasks/external_skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tasks/external_triggers.py` & `gwcelery-2.3.3/gwcelery/tasks/external_triggers.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tasks/first2years.py` & `gwcelery-2.3.3/gwcelery/tasks/first2years.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tasks/first2years_external.py` & `gwcelery-2.3.3/gwcelery/tasks/first2years_external.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tasks/gcn.py` & `gwcelery-2.3.3/gwcelery/tasks/gcn.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tasks/gracedb.py` & `gwcelery-2.3.3/gwcelery/tasks/gracedb.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tasks/gwskynet.py` & `gwcelery-2.3.3/gwcelery/tasks/gwskynet.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tasks/igwn_alert.py` & `gwcelery-2.3.3/gwcelery/tasks/igwn_alert.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tasks/inference.py` & `gwcelery-2.3.3/gwcelery/tasks/inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -253,15 +253,15 @@
 
     path_to_settings = os.path.join(rundir, 'settings.json')
     setup_arg = ['bilby_pipe_gracedb', '--webdir', path_to_webdir,
                  '--outdir', rundir, '--json', path_to_json,
                  '--psd-file', path_to_psd, '--settings', path_to_settings]
     settings = {'summarypages_arguments': {'gracedb': event['graceid'],
                                            'no_ligo_skymap': True},
-                'accounting_user': 'soichiro.morisaki'}
+                'accounting_user': 'cody.messick'}
     if app.conf['gracedb_host'] != 'gracedb.ligo.org':
         settings['queue'] = 'Online_PE_MDC'
     else:
         settings['queue'] = 'Online_PE'
         settings['accounting'] = 'ligo.prod.o4.cbc.pe.bilby'
     # FIXME: using live data for gracedb-test events should be reconsidered
     # when we have a better idea to differentiate MDC and real events.
@@ -865,15 +865,15 @@
             args += [f"--{key}"]
             for ifo in pesummary_kwargs[key]:
                 args += [f'{ifo}:{pesummary_kwargs[key][ifo]}']
         else:
             args += [f"--{key}", pesummary_kwargs[key]]
     condor_kwargs = dict(
         request_memory=16000, request_disk=5000, request_cpus=6,
-        accounting_group_user='soichiro.morisaki'
+        accounting_group_user='cody.messick'
     )
     if app.conf['gracedb_host'] != 'gracedb.ligo.org':
         condor_kwargs['accounting_group'] = 'ligo.dev.o4.cbc.pe.bilby'
         condor_kwargs['requirements'] = '((TARGET.Online_PE_MDC =?= True))'
         condor_kwargs['+Online_PE_MDC'] = True
         args += ["--disable_interactive", "--disable_expert"]
     else:
```

### Comparing `gwcelery-2.3.2/gwcelery/tasks/legacy_gracedb.py` & `gwcelery-2.3.3/gwcelery/tasks/legacy_gracedb.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tasks/notice_text.py` & `gwcelery-2.3.3/gwcelery/tasks/notice_text.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tasks/orchestrator.py` & `gwcelery-2.3.3/gwcelery/tasks/orchestrator.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tasks/p_astro.py` & `gwcelery-2.3.3/gwcelery/tasks/p_astro.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tasks/raven.py` & `gwcelery-2.3.3/gwcelery/tasks/raven.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tasks/rrt_utils.py` & `gwcelery-2.3.3/gwcelery/tasks/rrt_utils.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tasks/skymaps.py` & `gwcelery-2.3.3/gwcelery/tasks/skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tasks/superevents.py` & `gwcelery-2.3.3/gwcelery/tasks/superevents.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/templates/fits_header.jinja2` & `gwcelery-2.3.3/gwcelery/templates/fits_header.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/templates/index.jinja2` & `gwcelery-2.3.3/gwcelery/templates/index.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/templates/lalinference.jinja2` & `gwcelery-2.3.3/gwcelery/templates/lalinference.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/templates/rapidpe.jinja2` & `gwcelery-2.3.3/gwcelery/templates/rapidpe.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/conftest.py` & `gwcelery-2.3.3/gwcelery/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/G000012_S0040_preferred.json` & `gwcelery-2.3.3/gwcelery/tests/data/G000012_S0040_preferred.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/G298048-1-Initial.xml` & `gwcelery-2.3.3/gwcelery/tests/data/G298048-1-Initial.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/G298048_log.json` & `gwcelery-2.3.3/gwcelery/tests/data/G298048_log.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json` & `gwcelery-2.3.3/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/MS220722v.json` & `gwcelery-2.3.3/gwcelery/tests/data/MS220722v.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits` & `gwcelery-2.3.3/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/S230413b.json` & `gwcelery-2.3.3/gwcelery/tests/data/S230413b.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/S230413g.json` & `gwcelery-2.3.3/gwcelery/tests/data/S230413g.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/S230413h.json` & `gwcelery-2.3.3/gwcelery/tests/data/S230413h.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/T0212_S0039_preferred.json` & `gwcelery-2.3.3/gwcelery/tests/data/T0212_S0039_preferred.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json` & `gwcelery-2.3.3/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/T0219_S0041_nopreferred.json` & `gwcelery-2.3.3/gwcelery/tests/data/T0219_S0041_nopreferred.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/agile_grb_gcn.xml` & `gwcelery-2.3.3/gwcelery/tests/data/agile_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/coinc.xml` & `gwcelery-2.3.3/gwcelery/tests/data/coinc.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/externaltrigger_original_data.xml` & `gwcelery-2.3.3/gwcelery/tests/data/externaltrigger_original_data.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/fermi_grb_gcn.xml` & `gwcelery-2.3.3/gwcelery/tests/data/fermi_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/fermi_initial_grb_gcn.xml` & `gwcelery-2.3.3/gwcelery/tests/data/fermi_initial_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/fermi_noise_gcn.xml` & `gwcelery-2.3.3/gwcelery/tests/data/fermi_noise_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/fermi_noise_gcn_2.xml` & `gwcelery-2.3.3/gwcelery/tests/data/fermi_noise_gcn_2.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/fermi_subgrbtargeted_template.xml` & `gwcelery-2.3.3/gwcelery/tests/data/fermi_subgrbtargeted_template.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml` & `gwcelery-2.3.3/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml` & `gwcelery-2.3.3/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/fits_header_result.html` & `gwcelery-2.3.3/gwcelery/tests/data/fits_header_result.html`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/gracedb_externaltrigger_log.json` & `gwcelery-2.3.3/gwcelery/tests/data/gracedb_externaltrigger_log.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/igwn_alert_detchar.json` & `gwcelery-2.3.3/gwcelery/tests/data/igwn_alert_detchar.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/igwn_alert_exttrig_creation.json` & `gwcelery-2.3.3/gwcelery/tests/data/igwn_alert_exttrig_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json` & `gwcelery-2.3.3/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/igwn_alert_psd.json` & `gwcelery-2.3.3/gwcelery/tests/data/igwn_alert_psd.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/igwn_alert_snews_creation.json` & `gwcelery-2.3.3/gwcelery/tests/data/igwn_alert_snews_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/igwn_alert_snews_test_creation.json` & `gwcelery-2.3.3/gwcelery/tests/data/igwn_alert_snews_test_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/igwn_alert_subgrb_creation.json` & `gwcelery-2.3.3/gwcelery/tests/data/igwn_alert_subgrb_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/igwn_alert_superevent_creation.json` & `gwcelery-2.3.3/gwcelery/tests/data/igwn_alert_superevent_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/igwn_alert_voevent.json` & `gwcelery-2.3.3/gwcelery/tests/data/igwn_alert_voevent.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/integral_grb_gcn.xml` & `gwcelery-2.3.3/gwcelery/tests/data/integral_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/integral_mdc_gcn.xml` & `gwcelery-2.3.3/gwcelery/tests/data/integral_mdc_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/integral_test_gcn.xml` & `gwcelery-2.3.3/gwcelery/tests/data/integral_test_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/kafka_alert_fermi.json` & `gwcelery-2.3.3/gwcelery/tests/data/kafka_alert_fermi.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/kafka_alert_fermi_ignore.json` & `gwcelery-2.3.3/gwcelery/tests/data/kafka_alert_fermi_ignore.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/kafka_alert_swift.json` & `gwcelery-2.3.3/gwcelery/tests/data/kafka_alert_swift.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/kafka_alert_swift_noloc.json` & `gwcelery-2.3.3/gwcelery/tests/data/kafka_alert_swift_noloc.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/kafka_alert_swift_wskymap.json` & `gwcelery-2.3.3/gwcelery/tests/data/kafka_alert_swift_wskymap.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf` & `gwcelery-2.3.3/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/llhoft/idqbad/H1/H-H1_O2_llhoft-1216577976-4.gwf` & `gwcelery-2.3.3/gwcelery/tests/data/llhoft/idqbad/H1/H-H1_O2_llhoft-1216577976-4.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/llhoft/omegascan/scanme.gwf` & `gwcelery-2.3.3/gwcelery/tests/data/llhoft/omegascan/scanme.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf` & `gwcelery-2.3.3/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/lvalert_event_creation.json` & `gwcelery-2.3.3/gwcelery/tests/data/lvalert_event_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/lvalert_xmpp.xml` & `gwcelery-2.3.3/gwcelery/tests/data/lvalert_xmpp.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/mock_superevent_object.json` & `gwcelery-2.3.3/gwcelery/tests/data/mock_superevent_object.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite` & `gwcelery-2.3.3/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/psd.xml.gz` & `gwcelery-2.3.3/gwcelery/tests/data/psd.xml.gz`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/rrt_small_area.fits` & `gwcelery-2.3.3/gwcelery/tests/data/rrt_small_area.fits`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/sample_events.json` & `gwcelery-2.3.3/gwcelery/tests/data/sample_events.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/samples.hdf5` & `gwcelery-2.3.3/gwcelery/tests/data/samples.hdf5`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/scaler_set_all.pickle` & `gwcelery-2.3.3/gwcelery/tests/data/scaler_set_all.pickle`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/snews_gcn.xml` & `gwcelery-2.3.3/gwcelery/tests/data/snews_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/snews_gcn_test.xml` & `gwcelery-2.3.3/gwcelery/tests/data/snews_gcn_test.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/superevents.json` & `gwcelery-2.3.3/gwcelery/tests/data/superevents.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/swift_grb_gcn.xml` & `gwcelery-2.3.3/gwcelery/tests/data/swift_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/swift_subgrbtargeted_template.xml` & `gwcelery-2.3.3/gwcelery/tests/data/swift_subgrbtargeted_template.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/data/test_classifier.pickle` & `gwcelery-2.3.3/gwcelery/tests/data/test_classifier.pickle`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/process.py` & `gwcelery-2.3.3/gwcelery/tests/process.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_sentry.py` & `gwcelery-2.3.3/gwcelery/tests/test_sentry.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tasks_alerts.py` & `gwcelery-2.3.3/gwcelery/tests/test_tasks_alerts.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tasks_alerts_validate.py` & `gwcelery-2.3.3/gwcelery/tests/test_tasks_alerts_validate.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tasks_bayestar.py` & `gwcelery-2.3.3/gwcelery/tests/test_tasks_bayestar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tasks_circulars.py` & `gwcelery-2.3.3/gwcelery/tests/test_tasks_circulars.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tasks_condor.py` & `gwcelery-2.3.3/gwcelery/tests/test_tasks_condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tasks_detchar.py` & `gwcelery-2.3.3/gwcelery/tests/test_tasks_detchar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tasks_em_bright.py` & `gwcelery-2.3.3/gwcelery/tests/test_tasks_em_bright.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tasks_external_skymaps.py` & `gwcelery-2.3.3/gwcelery/tests/test_tasks_external_skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tasks_external_triggers.py` & `gwcelery-2.3.3/gwcelery/tests/test_tasks_external_triggers.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tasks_first2years.py` & `gwcelery-2.3.3/gwcelery/tests/test_tasks_first2years.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tasks_first2years_external.py` & `gwcelery-2.3.3/gwcelery/tests/test_tasks_first2years_external.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tasks_gcn.py` & `gwcelery-2.3.3/gwcelery/tests/test_tasks_gcn.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tasks_gcn_validate.py` & `gwcelery-2.3.3/gwcelery/tests/test_tasks_gcn_validate.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tasks_gracedb.py` & `gwcelery-2.3.3/gwcelery/tests/test_tasks_gracedb.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tasks_gwskynet.py` & `gwcelery-2.3.3/gwcelery/tests/test_tasks_gwskynet.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tasks_igwn_alert.py` & `gwcelery-2.3.3/gwcelery/tests/test_tasks_igwn_alert.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tasks_inference.py` & `gwcelery-2.3.3/gwcelery/tests/test_tasks_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -172,15 +172,15 @@
 
         path_to_settings = cmd[10]
         assert os.path.exists(path_to_settings)
         ans = {
             'summarypages_arguments': {'gracedb': event['graceid'],
                                        'no_ligo_skymap': True},
             'queue': 'Online_PE',
-            'accounting_user': 'soichiro.morisaki',
+            'accounting_user': 'cody.messick',
         }
         if host != 'gracedb.ligo.org':
             ans['queue'] = 'Online_PE_MDC'
         else:
             ans['accounting'] = 'ligo.prod.o4.cbc.pe.bilby'
         if mode == 'production':
             ans.update(
```

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tasks_orchestrator.py` & `gwcelery-2.3.3/gwcelery/tests/test_tasks_orchestrator.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tasks_p_astro.py` & `gwcelery-2.3.3/gwcelery/tests/test_tasks_p_astro.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tasks_raven.py` & `gwcelery-2.3.3/gwcelery/tests/test_tasks_raven.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tasks_rrt_utils.py` & `gwcelery-2.3.3/gwcelery/tests/test_tasks_rrt_utils.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tasks_skymaps.py` & `gwcelery-2.3.3/gwcelery/tests/test_tasks_skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tasks_superevents.py` & `gwcelery-2.3.3/gwcelery/tests/test_tasks_superevents.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tempfile.py` & `gwcelery-2.3.3/gwcelery/tests/test_tempfile.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tools_condor.py` & `gwcelery-2.3.3/gwcelery/tests/test_tools_condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tools_condor_submit_helper.py` & `gwcelery-2.3.3/gwcelery/tests/test_tools_condor_submit_helper.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tools_flask.py` & `gwcelery-2.3.3/gwcelery/tests/test_tools_flask.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_tools_nagios.py` & `gwcelery-2.3.3/gwcelery/tests/test_tools_nagios.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tests/test_views.py` & `gwcelery-2.3.3/gwcelery/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tools/condor.py` & `gwcelery-2.3.3/gwcelery/tools/condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tools/condor_submit_helper.py` & `gwcelery-2.3.3/gwcelery/tools/condor_submit_helper.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tools/flask.py` & `gwcelery-2.3.3/gwcelery/tools/flask.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/tools/nagios.py` & `gwcelery-2.3.3/gwcelery/tools/nagios.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/util/cmdline.py` & `gwcelery-2.3.3/gwcelery/util/cmdline.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/util/resources.py` & `gwcelery-2.3.3/gwcelery/util/resources.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/util/tempfile.py` & `gwcelery-2.3.3/gwcelery/util/tempfile.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/views.py` & `gwcelery-2.3.3/gwcelery/views.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/voevent/bootsteps.py` & `gwcelery-2.3.3/gwcelery/voevent/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/voevent/logging.py` & `gwcelery-2.3.3/gwcelery/voevent/logging.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/voevent/signals.py` & `gwcelery-2.3.3/gwcelery/voevent/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/voevent/subscriber.py` & `gwcelery-2.3.3/gwcelery/voevent/subscriber.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/gwcelery/voevent/util.py` & `gwcelery-2.3.3/gwcelery/voevent/util.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.3.2/pyproject.toml` & `gwcelery-2.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gwcelery"
-version = "2.3.2"
+version = "2.3.3"
 description = "Low-latency pipeline for annotating IGWN events"
 readme = "README.rst"
 authors = [
     "Deep Chatterjee <deep.chatterjee@ligo.org>",
     "Cody Messick <cody.messick@ligo.org>",
     "Geoffrey Mo <geoffrey.mo@ligo.org>",
     "Leo Singer <leo.singer@ligo.org>"
```

### Comparing `gwcelery-2.3.2/PKG-INFO` & `gwcelery-2.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwcelery
-Version: 2.3.2
+Version: 2.3.3
 Summary: Low-latency pipeline for annotating IGWN events
 Home-page: https://git.ligo.org/emfollow/gwcelery
 License: GPL-2.0+
 Author: Deep Chatterjee
 Author-email: deep.chatterjee@ligo.org
 Requires-Python: >=3.9,<3.12
 Classifier: Development Status :: 4 - Beta
```

