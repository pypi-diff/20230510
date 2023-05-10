# Comparing `tmp/gwcelery-2.0.5.tar.gz` & `tmp/gwcelery-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwcelery-2.0.5.tar", max compression
+gzip compressed data, was "gwcelery-2.0.6.tar", max compression
```

## Comparing `gwcelery-2.0.5.tar` & `gwcelery-2.0.6.tar`

### file list

```diff
@@ -1,225 +1,229 @@
--rw-r--r--   0        0        0    90483 2023-04-20 23:28:05.189174 gwcelery-2.0.5/CHANGES.rst
--rw-r--r--   0        0        0       64 2023-04-20 23:28:05.189174 gwcelery-2.0.5/CONTRIBUTING.rst
--rw-r--r--   0        0        0    19716 2023-04-20 23:28:05.189174 gwcelery-2.0.5/LICENSE.rst
--rw-r--r--   0        0        0     1351 2023-04-20 23:28:05.189174 gwcelery-2.0.5/README.rst
--rw-r--r--   0        0        0      634 2023-04-20 23:28:05.189174 gwcelery-2.0.5/doc/Makefile
--rw-r--r--   0        0        0   191486 2023-04-20 23:28:05.190173 gwcelery-2.0.5/doc/_static/acceptance-tests-checklist.png
--rw-r--r--   0        0        0   241593 2023-04-20 23:28:05.191174 gwcelery-2.0.5/doc/_static/celeryevent-screenshot.png
--rw-r--r--   0        0        0   206465 2023-04-20 23:28:05.192174 gwcelery-2.0.5/doc/_static/deployment-screenshot.png
--rw-r--r--   0        0        0   161306 2023-04-20 23:28:05.194174 gwcelery-2.0.5/doc/_static/flask-screenshot.png
--rw-r--r--   0        0        0   328056 2023-04-20 23:28:05.195174 gwcelery-2.0.5/doc/_static/flower-screenshot.png
--rw-r--r--   0        0        0   114719 2023-04-20 23:28:05.196174 gwcelery-2.0.5/doc/_static/logo-0.5x.png
--rw-r--r--   0        0        0   351955 2023-04-20 23:28:05.198174 gwcelery-2.0.5/doc/_static/logo.png
--rw-r--r--   0        0        0   230777 2023-04-20 23:28:05.199174 gwcelery-2.0.5/doc/_static/sentry-screenshot.png
--rwxr-xr-x   0        0        0     7356 2023-04-20 23:28:05.200173 gwcelery-2.0.5/doc/conf.py
--rw-r--r--   0        0        0     3543 2023-04-20 23:28:05.200173 gwcelery-2.0.5/doc/configuration.rst
--rw-r--r--   0        0        0     5698 2023-04-20 23:28:05.200173 gwcelery-2.0.5/doc/contributing.rst
--rw-r--r--   0        0        0     7204 2023-04-20 23:28:05.200173 gwcelery-2.0.5/doc/deployment.rst
--rw-r--r--   0        0        0    10176 2023-04-20 23:28:05.200173 gwcelery-2.0.5/doc/design.rst
--rw-r--r--   0        0        0      486 2023-04-20 23:28:05.200173 gwcelery-2.0.5/doc/gwcelery.conf.rst
--rw-r--r--   0        0        0      284 2023-04-20 23:28:05.200173 gwcelery-2.0.5/doc/gwcelery.email.rst
--rw-r--r--   0        0        0      329 2023-04-20 23:28:05.200173 gwcelery-2.0.5/doc/gwcelery.igwn_alert.rst
--rw-r--r--   0        0        0      227 2023-04-20 23:28:05.200173 gwcelery-2.0.5/doc/gwcelery.rst
--rw-r--r--   0        0        0       79 2023-04-20 23:28:05.200173 gwcelery-2.0.5/doc/gwcelery.sentry.rst
--rw-r--r--   0        0        0       97 2023-04-20 23:28:05.200173 gwcelery-2.0.5/doc/gwcelery.tasks.alerts.rst
--rw-r--r--   0        0        0      103 2023-04-20 23:28:05.200173 gwcelery-2.0.5/doc/gwcelery.tasks.bayestar.rst
--rw-r--r--   0        0        0      107 2023-04-20 23:28:05.200173 gwcelery-2.0.5/doc/gwcelery.tasks.circulars.rst
--rw-r--r--   0        0        0       98 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.condor.rst
--rw-r--r--   0        0        0     2404 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.detchar.rst
--rw-r--r--   0        0        0     1110 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.em_bright.rst
--rw-r--r--   0        0        0      129 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.external_skymaps.rst
--rw-r--r--   0        0        0     6738 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.external_triggers.rst
--rw-r--r--   0        0        0      112 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.first2years.rst
--rw-r--r--   0        0        0       88 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.gcn.rst
--rw-r--r--   0        0        0      100 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.gracedb.rst
--rw-r--r--   0        0        0      109 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.igwn_alert.rst
--rw-r--r--   0        0        0      109 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.inference.rst
--rw-r--r--   0        0        0     8111 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.orchestrator.rst
--rw-r--r--   0        0        0      100 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.p_astro.rst
--rw-r--r--   0        0        0       94 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.raven.rst
--rw-r--r--   0        0        0      628 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.rst
--rw-r--r--   0        0        0      100 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.skymaps.rst
--rw-r--r--   0        0        0     7161 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tasks.superevents.rst
--rw-r--r--   0        0        0       97 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tools.condor.rst
--rw-r--r--   0        0        0       94 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tools.flask.rst
--rw-r--r--   0        0        0       97 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tools.nagios.rst
--rw-r--r--   0        0        0      185 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.tools.rst
--rw-r--r--   0        0        0       73 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.util.rst
--rw-r--r--   0        0        0      507 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/gwcelery.voevent.rst
--rw-r--r--   0        0        0     3564 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/htcondor.rst
--rw-r--r--   0        0        0     1576 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/index.rst
--rw-r--r--   0        0        0      800 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/make.bat
--rw-r--r--   0        0        0     4416 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/monitoring.rst
--rw-r--r--   0        0        0     5312 2023-04-20 23:28:05.201174 gwcelery-2.0.5/doc/quickstart.rst
--rw-r--r--   0        0        0     1149 2023-04-20 23:28:05.202174 gwcelery-2.0.5/gwcelery/__init__.py
--rw-r--r--   0        0        0    18447 2023-04-20 23:28:05.202174 gwcelery-2.0.5/gwcelery/_version.py
--rw-r--r--   0        0        0    14591 2023-04-20 23:28:05.202174 gwcelery-2.0.5/gwcelery/conf/__init__.py
--rw-r--r--   0        0        0      403 2023-04-20 23:28:05.202174 gwcelery-2.0.5/gwcelery/conf/development.py
--rw-r--r--   0        0        0     1026 2023-04-20 23:28:05.202174 gwcelery-2.0.5/gwcelery/conf/minikube.py
--rw-r--r--   0        0        0     1562 2023-04-20 23:28:05.202174 gwcelery-2.0.5/gwcelery/conf/playground.py
--rw-r--r--   0        0        0     3104 2023-04-20 23:28:05.202174 gwcelery-2.0.5/gwcelery/conf/production.py
--rw-r--r--   0        0        0     1044 2023-04-20 23:28:05.202174 gwcelery-2.0.5/gwcelery/conf/test.py
--rw-r--r--   0        0        0        0 2023-04-20 23:28:05.202174 gwcelery-2.0.5/gwcelery/data/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 23:28:05.202174 gwcelery-2.0.5/gwcelery/data/first2years/__init__.py
--rw-r--r--   0        0        0   731421 2023-04-20 23:28:05.204174 gwcelery-2.0.5/gwcelery/data/first2years/gstlal.xml.gz
--rwxr-xr-x   0        0        0     2519 2023-04-20 23:28:05.204174 gwcelery-2.0.5/gwcelery/data/gwcelery.sub
--rw-r--r--   0        0        0      505 2023-04-20 23:28:05.204174 gwcelery-2.0.5/gwcelery/email/__init__.py
--rw-r--r--   0        0        0     3317 2023-04-20 23:28:05.204174 gwcelery-2.0.5/gwcelery/email/bootsteps.py
--rw-r--r--   0        0        0      995 2023-04-20 23:28:05.204174 gwcelery-2.0.5/gwcelery/email/signals.py
--rw-r--r--   0        0        0     1457 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/flask.py
--rw-r--r--   0        0        0      529 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/igwn_alert/__init__.py
--rw-r--r--   0        0        0     4484 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/igwn_alert/bootsteps.py
--rw-r--r--   0        0        0      608 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/igwn_alert/signals.py
--rw-r--r--   0        0        0      275 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/jinja.py
--rw-r--r--   0        0        0      285 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/kafka/__init__.py
--rw-r--r--   0        0        0     6544 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/kafka/bootsteps.py
--rw-r--r--   0        0        0     2567 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/sentry/__init__.py
--rw-r--r--   0        0        0       34 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/sentry/integrations/__init__.py
--rw-r--r--   0        0        0      832 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/sentry/integrations/condor.py
--rw-r--r--   0        0        0      836 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/sentry/integrations/requests.py
--rw-r--r--   0        0        0      939 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/sentry/integrations/subprocess.py
--rw-r--r--   0        0        0     1302 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/static/typeahead.css
--rw-r--r--   0        0        0     4124 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/static/vega/index.html
--rw-r--r--   0        0        0      515 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/tasks/__init__.py
--rw-r--r--   0        0        0    11951 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/tasks/alerts.py
--rw-r--r--   0        0        0     2672 2023-04-20 23:28:05.205174 gwcelery-2.0.5/gwcelery/tasks/bayestar.py
--rw-r--r--   0        0        0     1296 2023-04-20 23:28:05.206174 gwcelery-2.0.5/gwcelery/tasks/circulars.py
--rw-r--r--   0        0        0     7502 2023-04-20 23:28:05.206174 gwcelery-2.0.5/gwcelery/tasks/condor.py
--rw-r--r--   0        0        0     2692 2023-04-20 23:28:05.206174 gwcelery-2.0.5/gwcelery/tasks/core.py
--rw-r--r--   0        0        0    20924 2023-04-20 23:28:05.206174 gwcelery-2.0.5/gwcelery/tasks/detchar.py
--rw-r--r--   0        0        0     4819 2023-04-20 23:28:05.206174 gwcelery-2.0.5/gwcelery/tasks/em_bright.py
--rw-r--r--   0        0        0    21902 2023-04-20 23:28:05.206174 gwcelery-2.0.5/gwcelery/tasks/external_skymaps.py
--rw-r--r--   0        0        0    22568 2023-04-20 23:28:05.206174 gwcelery-2.0.5/gwcelery/tasks/external_triggers.py
--rw-r--r--   0        0        0     6832 2023-04-20 23:28:05.206174 gwcelery-2.0.5/gwcelery/tasks/first2years.py
--rw-r--r--   0        0        0     6384 2023-04-20 23:28:05.206174 gwcelery-2.0.5/gwcelery/tasks/first2years_external.py
--rw-r--r--   0        0        0     4831 2023-04-20 23:28:05.206174 gwcelery-2.0.5/gwcelery/tasks/gcn.py
--rw-r--r--   0        0        0    11079 2023-04-20 23:28:05.206174 gwcelery-2.0.5/gwcelery/tasks/gracedb.py
--rw-r--r--   0        0        0     2453 2023-04-20 23:28:05.206174 gwcelery-2.0.5/gwcelery/tasks/igwn_alert.py
--rw-r--r--   0        0        0    30399 2023-04-20 23:28:05.207174 gwcelery-2.0.5/gwcelery/tasks/inference.py
--rw-r--r--   0        0        0     1396 2023-04-20 23:28:05.207174 gwcelery-2.0.5/gwcelery/tasks/legacy_gracedb.py
--rw-r--r--   0        0        0     7772 2023-04-20 23:28:05.207174 gwcelery-2.0.5/gwcelery/tasks/notice_text.py
--rw-r--r--   0        0        0    46448 2023-04-20 23:28:05.207174 gwcelery-2.0.5/gwcelery/tasks/orchestrator.py
--rw-r--r--   0        0        0     5796 2023-04-20 23:28:05.207174 gwcelery-2.0.5/gwcelery/tasks/p_astro.py
--rw-r--r--   0        0        0    19628 2023-04-20 23:28:05.207174 gwcelery-2.0.5/gwcelery/tasks/raven.py
--rw-r--r--   0        0        0    12528 2023-04-20 23:28:05.207174 gwcelery-2.0.5/gwcelery/tasks/skymaps.py
--rw-r--r--   0        0        0    23386 2023-04-20 23:28:05.208174 gwcelery-2.0.5/gwcelery/tasks/superevents.py
--rw-r--r--   0        0        0     1084 2023-04-20 23:28:05.208174 gwcelery-2.0.5/gwcelery/templates/fits_header.jinja2
--rw-r--r--   0        0        0    34059 2023-04-20 23:28:05.208174 gwcelery-2.0.5/gwcelery/templates/index.jinja2
--rw-r--r--   0        0        0     8505 2023-04-20 23:28:05.208174 gwcelery-2.0.5/gwcelery/templates/lalinference.jinja2
--rw-r--r--   0        0        0     8939 2023-04-20 23:28:05.208174 gwcelery-2.0.5/gwcelery/templates/rapidpe.jinja2
--rw-r--r--   0        0        0      806 2023-04-20 23:28:05.208174 gwcelery-2.0.5/gwcelery/templates/vector_table.jinja2
--rw-r--r--   0        0        0        0 2023-04-20 23:28:05.208174 gwcelery-2.0.5/gwcelery/tests/__init__.py
--rw-r--r--   0        0        0     4388 2023-04-20 23:28:05.208174 gwcelery-2.0.5/gwcelery/tests/conftest.py
--rw-r--r--   0        0        0      976 2023-04-20 23:28:05.208174 gwcelery-2.0.5/gwcelery/tests/data/G000012_S0040_preferred.json
--rw-r--r--   0        0        0     6258 2023-04-20 23:28:05.208174 gwcelery-2.0.5/gwcelery/tests/data/G298048-1-Initial.xml
--rw-r--r--   0        0        0      599 2023-04-20 23:28:05.208174 gwcelery-2.0.5/gwcelery/tests/data/G298048_log.json
--rw-r--r--   0        0        0      150 2023-04-20 23:28:05.209174 gwcelery-2.0.5/gwcelery/tests/data/H1L1V1-mean_counts-1126051217-61603201.json
--rw-r--r--   0        0        0      974 2023-04-20 23:28:05.209174 gwcelery-2.0.5/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json
--rw-r--r--   0        0        0    17572 2023-04-20 23:28:05.209174 gwcelery-2.0.5/gwcelery/tests/data/MS220722v.xml
--rw-r--r--   0        0        0   777600 2023-04-20 23:28:05.213173 gwcelery-2.0.5/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits
--rw-r--r--   0        0        0     8220 2023-04-20 23:28:05.214174 gwcelery-2.0.5/gwcelery/tests/data/S230413b.json
--rw-r--r--   0        0        0     7255 2023-04-20 23:28:05.214174 gwcelery-2.0.5/gwcelery/tests/data/S230413g.json
--rw-r--r--   0        0        0     7721 2023-04-20 23:28:05.214174 gwcelery-2.0.5/gwcelery/tests/data/S230413h.json
--rw-r--r--   0        0        0     3387 2023-04-20 23:28:05.214174 gwcelery-2.0.5/gwcelery/tests/data/T0212_S0039_preferred.json
--rw-r--r--   0        0        0     3384 2023-04-20 23:28:05.214174 gwcelery-2.0.5/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json
--rw-r--r--   0        0        0     5210 2023-04-20 23:28:05.214174 gwcelery-2.0.5/gwcelery/tests/data/T0219_S0041_nopreferred.json
--rw-r--r--   0        0        0        0 2023-04-20 23:28:05.214174 gwcelery-2.0.5/gwcelery/tests/data/__init__.py
--rw-r--r--   0        0        0     2290 2023-04-20 23:28:05.214174 gwcelery-2.0.5/gwcelery/tests/data/agile_grb_gcn.xml
--rw-r--r--   0        0        0   854036 2023-04-20 23:28:05.218174 gwcelery-2.0.5/gwcelery/tests/data/coinc.xml
--rw-r--r--   0        0        0     6175 2023-04-20 23:28:05.218174 gwcelery-2.0.5/gwcelery/tests/data/externaltrigger_original_data.xml
--rw-r--r--   0        0        0     5482 2023-04-20 23:28:05.218174 gwcelery-2.0.5/gwcelery/tests/data/fermi_grb_gcn.xml
--rw-r--r--   0        0        0     5469 2023-04-20 23:28:05.218174 gwcelery-2.0.5/gwcelery/tests/data/fermi_initial_grb_gcn.xml
--rw-r--r--   0        0        0     5865 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/fermi_noise_gcn.xml
--rw-r--r--   0        0        0     5864 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/fermi_noise_gcn_2.xml
--rw-r--r--   0        0        0     4914 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml
--rw-r--r--   0        0        0     4914 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml
--rw-r--r--   0        0        0     3407 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/fits_header_result.html
--rw-r--r--   0        0        0      882 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/gracedb_externaltrigger_log.json
--rw-r--r--   0        0        0      446 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/gracedb_setrigger_log.json
--rw-r--r--   0        0        0      870 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_detchar.json
--rw-r--r--   0        0        0     2025 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_exttrig_creation.json
--rw-r--r--   0        0        0     2007 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json
--rw-r--r--   0        0        0      166 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_fits.json
--rw-r--r--   0        0        0      101 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_label_dqv.json
--rw-r--r--   0        0        0      743 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_psd.json
--rw-r--r--   0        0        0     2020 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_snews_creation.json
--rw-r--r--   0        0        0     2012 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_snews_test_creation.json
--rw-r--r--   0        0        0     2028 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_subgrb_creation.json
--rw-r--r--   0        0        0     1235 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_superevent_creation.json
--rw-r--r--   0        0        0      107 2023-04-20 23:28:05.219174 gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_superevent_label.json
--rw-r--r--   0        0        0     5021 2023-04-20 23:28:05.220174 gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_voevent.json
--rw-r--r--   0        0        0     4429 2023-04-20 23:28:05.220174 gwcelery-2.0.5/gwcelery/tests/data/integral_grb_gcn.xml
--rw-r--r--   0        0        0     4295 2023-04-20 23:28:05.220174 gwcelery-2.0.5/gwcelery/tests/data/integral_mdc_gcn.xml
--rw-r--r--   0        0        0        0 2023-04-20 23:28:05.220174 gwcelery-2.0.5/gwcelery/tests/data/llhoft/__init__.py
--rw-r--r--   0        0        0    14622 2023-04-20 23:28:05.220174 gwcelery-2.0.5/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf
--rw-r--r--   0        0        0        0 2023-04-20 23:28:05.220174 gwcelery-2.0.5/gwcelery/tests/data/llhoft/fail/L1/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 23:28:05.220174 gwcelery-2.0.5/gwcelery/tests/data/llhoft/fail/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 23:28:05.220174 gwcelery-2.0.5/gwcelery/tests/data/llhoft/omegascan/__init__.py
--rw-r--r--   0        0        0   516419 2023-04-20 23:28:05.221174 gwcelery-2.0.5/gwcelery/tests/data/llhoft/omegascan/scanme.gwf
--rw-r--r--   0        0        0    14630 2023-04-20 23:28:05.221174 gwcelery-2.0.5/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf
--rw-r--r--   0        0        0        0 2023-04-20 23:28:05.221174 gwcelery-2.0.5/gwcelery/tests/data/llhoft/pass/H1/__init__.py
--rw-r--r--   0        0        0        0 2023-04-20 23:28:05.221174 gwcelery-2.0.5/gwcelery/tests/data/llhoft/pass/__init__.py
--rw-r--r--   0        0        0    13099 2023-04-20 23:28:05.221174 gwcelery-2.0.5/gwcelery/tests/data/lvalert_event_creation.json
--rw-r--r--   0        0        0     9060 2023-04-20 23:28:05.221174 gwcelery-2.0.5/gwcelery/tests/data/lvalert_xmpp.xml
--rw-r--r--   0        0        0      864 2023-04-20 23:28:05.221174 gwcelery-2.0.5/gwcelery/tests/data/mock_superevent_object.json
--rw-r--r--   0        0        0   445440 2023-04-20 23:28:05.223174 gwcelery-2.0.5/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite
--rw-r--r--   0        0        0   294426 2023-04-20 23:28:05.224174 gwcelery-2.0.5/gwcelery/tests/data/psd.xml.gz
--rw-r--r--   0        0        0     2964 2023-04-20 23:28:05.224174 gwcelery-2.0.5/gwcelery/tests/data/sample_events.json
--rw-r--r--   0        0        0     3648 2023-04-20 23:28:05.224174 gwcelery-2.0.5/gwcelery/tests/data/samples.hdf5
--rw-r--r--   0        0        0      616 2023-04-20 23:28:05.224174 gwcelery-2.0.5/gwcelery/tests/data/scaler_set_all.pickle
--rw-r--r--   0        0        0     6169 2023-04-20 23:28:05.224174 gwcelery-2.0.5/gwcelery/tests/data/snews_gcn.xml
--rw-r--r--   0        0        0     6161 2023-04-20 23:28:05.224174 gwcelery-2.0.5/gwcelery/tests/data/snews_gcn_test.xml
--rw-r--r--   0        0        0     9583 2023-04-20 23:28:05.224174 gwcelery-2.0.5/gwcelery/tests/data/superevents.json
--rw-r--r--   0        0        0     7713 2023-04-20 23:28:05.224174 gwcelery-2.0.5/gwcelery/tests/data/swift_grb_gcn.xml
--rw-r--r--   0        0        0   581918 2023-04-20 23:28:05.226173 gwcelery-2.0.5/gwcelery/tests/data/test_classifier.pickle
--rw-r--r--   0        0        0     4042 2023-04-20 23:28:05.226173 gwcelery-2.0.5/gwcelery/tests/process.py
--rw-r--r--   0        0        0     2307 2023-04-20 23:28:05.226173 gwcelery-2.0.5/gwcelery/tests/test_sentry.py
--rw-r--r--   0        0        0     1705 2023-04-20 23:28:05.226173 gwcelery-2.0.5/gwcelery/tests/test_tasks_alerts.py
--rw-r--r--   0        0        0     4916 2023-04-20 23:28:05.226173 gwcelery-2.0.5/gwcelery/tests/test_tasks_alerts_validate.py
--rw-r--r--   0        0        0     1439 2023-04-20 23:28:05.226173 gwcelery-2.0.5/gwcelery/tests/test_tasks_bayestar.py
--rw-r--r--   0        0        0     2416 2023-04-20 23:28:05.226173 gwcelery-2.0.5/gwcelery/tests/test_tasks_circulars.py
--rw-r--r--   0        0        0     4550 2023-04-20 23:28:05.226173 gwcelery-2.0.5/gwcelery/tests/test_tasks_condor.py
--rw-r--r--   0        0        0    11689 2023-04-20 23:28:05.227174 gwcelery-2.0.5/gwcelery/tests/test_tasks_detchar.py
--rw-r--r--   0        0        0     2287 2023-04-20 23:28:05.227174 gwcelery-2.0.5/gwcelery/tests/test_tasks_em_bright.py
--rw-r--r--   0        0        0    12265 2023-04-20 23:28:05.227174 gwcelery-2.0.5/gwcelery/tests/test_tasks_external_skymaps.py
--rw-r--r--   0        0        0    31976 2023-04-20 23:28:05.227174 gwcelery-2.0.5/gwcelery/tests/test_tasks_external_triggers.py
--rw-r--r--   0        0        0     1816 2023-04-20 23:28:05.227174 gwcelery-2.0.5/gwcelery/tests/test_tasks_first2years.py
--rw-r--r--   0        0        0     4555 2023-04-20 23:28:05.227174 gwcelery-2.0.5/gwcelery/tests/test_tasks_first2years_external.py
--rw-r--r--   0        0        0     1826 2023-04-20 23:28:05.227174 gwcelery-2.0.5/gwcelery/tests/test_tasks_gcn.py
--rw-r--r--   0        0        0     1655 2023-04-20 23:28:05.227174 gwcelery-2.0.5/gwcelery/tests/test_tasks_gcn_validate.py
--rw-r--r--   0        0        0     5739 2023-04-20 23:28:05.227174 gwcelery-2.0.5/gwcelery/tests/test_tasks_gracedb.py
--rw-r--r--   0        0        0     3662 2023-04-20 23:28:05.227174 gwcelery-2.0.5/gwcelery/tests/test_tasks_igwn_alert.py
--rw-r--r--   0        0        0    21517 2023-04-20 23:28:05.227174 gwcelery-2.0.5/gwcelery/tests/test_tasks_inference.py
--rw-r--r--   0        0        0    32509 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tests/test_tasks_orchestrator.py
--rw-r--r--   0        0        0     1647 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tests/test_tasks_p_astro.py
--rw-r--r--   0        0        0    25900 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tests/test_tasks_raven.py
--rw-r--r--   0        0        0     5035 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tests/test_tasks_skymaps.py
--rw-r--r--   0        0        0    39981 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tests/test_tasks_superevents.py
--rw-r--r--   0        0        0      637 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tests/test_tempfile.py
--rw-r--r--   0        0        0     3520 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tests/test_tools_condor.py
--rw-r--r--   0        0        0     1098 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tests/test_tools_condor_submit_helper.py
--rw-r--r--   0        0        0      633 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tests/test_tools_flask.py
--rw-r--r--   0        0        0     8067 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tests/test_tools_nagios.py
--rw-r--r--   0        0        0      269 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tests/test_util.py
--rw-r--r--   0        0        0    21450 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tests/test_views.py
--rw-r--r--   0        0        0      216 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tools/__init__.py
--rw-r--r--   0        0        0     2948 2023-04-20 23:28:05.228174 gwcelery-2.0.5/gwcelery/tools/condor.py
--rw-r--r--   0        0        0     1120 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/tools/condor_submit_helper.py
--rw-r--r--   0        0        0     1938 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/tools/flask.py
--rw-r--r--   0        0        0     5763 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/tools/nagios.py
--rw-r--r--   0        0        0      413 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/util/__init__.py
--rw-r--r--   0        0        0     1007 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/util/cmdline.py
--rw-r--r--   0        0        0      453 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/util/matplotlib.py
--rw-r--r--   0        0        0      390 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/util/proxy.py
--rw-r--r--   0        0        0      514 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/util/resources.py
--rw-r--r--   0        0        0      253 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/util/sphinx.py
--rw-r--r--   0        0        0      941 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/util/tempfile.py
--rw-r--r--   0        0        0    18472 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/views.py
--rw-r--r--   0        0        0      365 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/voevent/__init__.py
--rw-r--r--   0        0        0     6387 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/voevent/bootsteps.py
--rw-r--r--   0        0        0     1063 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/voevent/logging.py
--rw-r--r--   0        0        0      779 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/voevent/signals.py
--rw-r--r--   0        0        0      852 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/voevent/subscriber.py
--rw-r--r--   0        0        0     1454 2023-04-20 23:28:05.229174 gwcelery-2.0.5/gwcelery/voevent/util.py
--rw-r--r--   0        0        0     5901 2023-04-20 23:28:18.384198 gwcelery-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     4597 1970-01-01 00:00:00.000000 gwcelery-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0    92247 2023-05-10 21:15:58.258618 gwcelery-2.0.6/CHANGES.rst
+-rw-r--r--   0        0        0       64 2023-05-08 19:41:16.838727 gwcelery-2.0.6/CONTRIBUTING.rst
+-rw-r--r--   0        0        0    19716 2023-05-08 19:41:16.838727 gwcelery-2.0.6/LICENSE.rst
+-rw-r--r--   0        0        0     1351 2023-05-08 19:41:16.839727 gwcelery-2.0.6/README.rst
+-rw-r--r--   0        0        0      634 2023-05-08 19:41:16.839727 gwcelery-2.0.6/doc/Makefile
+-rw-r--r--   0        0        0   191486 2023-05-08 19:41:16.841727 gwcelery-2.0.6/doc/_static/acceptance-tests-checklist.png
+-rw-r--r--   0        0        0   241593 2023-05-08 19:41:16.842727 gwcelery-2.0.6/doc/_static/celeryevent-screenshot.png
+-rw-r--r--   0        0        0   206465 2023-05-08 19:41:16.844727 gwcelery-2.0.6/doc/_static/deployment-screenshot.png
+-rw-r--r--   0        0        0   161306 2023-05-08 19:41:16.845727 gwcelery-2.0.6/doc/_static/flask-screenshot.png
+-rw-r--r--   0        0        0   328056 2023-05-08 19:41:16.848727 gwcelery-2.0.6/doc/_static/flower-screenshot.png
+-rw-r--r--   0        0        0   114719 2023-05-08 19:41:16.849727 gwcelery-2.0.6/doc/_static/logo-0.5x.png
+-rw-r--r--   0        0        0   351955 2023-05-08 19:41:16.851727 gwcelery-2.0.6/doc/_static/logo.png
+-rw-r--r--   0        0        0   230777 2023-05-08 19:41:16.853727 gwcelery-2.0.6/doc/_static/sentry-screenshot.png
+-rwxr-xr-x   0        0        0     7356 2023-05-08 19:41:16.854728 gwcelery-2.0.6/doc/conf.py
+-rw-r--r--   0        0        0     4351 2023-05-08 19:41:16.854728 gwcelery-2.0.6/doc/configuration.rst
+-rw-r--r--   0        0        0     5698 2023-05-08 19:41:16.854728 gwcelery-2.0.6/doc/contributing.rst
+-rw-r--r--   0        0        0     7204 2023-05-08 19:41:16.854728 gwcelery-2.0.6/doc/deployment.rst
+-rw-r--r--   0        0        0    10176 2023-05-08 19:41:16.854728 gwcelery-2.0.6/doc/design.rst
+-rw-r--r--   0        0        0      486 2023-05-08 19:41:16.854728 gwcelery-2.0.6/doc/gwcelery.conf.rst
+-rw-r--r--   0        0        0      284 2023-05-08 19:41:16.855728 gwcelery-2.0.6/doc/gwcelery.email.rst
+-rw-r--r--   0        0        0      329 2023-05-08 19:41:16.855728 gwcelery-2.0.6/doc/gwcelery.igwn_alert.rst
+-rw-r--r--   0        0        0      227 2023-05-08 19:41:16.855728 gwcelery-2.0.6/doc/gwcelery.rst
+-rw-r--r--   0        0        0       79 2023-05-08 19:41:16.855728 gwcelery-2.0.6/doc/gwcelery.sentry.rst
+-rw-r--r--   0        0        0       97 2023-05-08 19:41:16.855728 gwcelery-2.0.6/doc/gwcelery.tasks.alerts.rst
+-rw-r--r--   0        0        0      103 2023-05-08 19:41:16.855728 gwcelery-2.0.6/doc/gwcelery.tasks.bayestar.rst
+-rw-r--r--   0        0        0      107 2023-05-08 19:41:16.855728 gwcelery-2.0.6/doc/gwcelery.tasks.circulars.rst
+-rw-r--r--   0        0        0       98 2023-05-08 19:41:16.855728 gwcelery-2.0.6/doc/gwcelery.tasks.condor.rst
+-rw-r--r--   0        0        0     2404 2023-05-08 19:41:16.855728 gwcelery-2.0.6/doc/gwcelery.tasks.detchar.rst
+-rw-r--r--   0        0        0     1110 2023-05-08 19:41:16.856728 gwcelery-2.0.6/doc/gwcelery.tasks.em_bright.rst
+-rw-r--r--   0        0        0      129 2023-05-08 19:41:16.856728 gwcelery-2.0.6/doc/gwcelery.tasks.external_skymaps.rst
+-rw-r--r--   0        0        0     6738 2023-05-08 19:41:16.856728 gwcelery-2.0.6/doc/gwcelery.tasks.external_triggers.rst
+-rw-r--r--   0        0        0      112 2023-05-08 19:41:16.856728 gwcelery-2.0.6/doc/gwcelery.tasks.first2years.rst
+-rw-r--r--   0        0        0       88 2023-05-08 19:41:16.856728 gwcelery-2.0.6/doc/gwcelery.tasks.gcn.rst
+-rw-r--r--   0        0        0      100 2023-05-08 19:41:16.856728 gwcelery-2.0.6/doc/gwcelery.tasks.gracedb.rst
+-rw-r--r--   0        0        0      109 2023-05-08 19:41:16.856728 gwcelery-2.0.6/doc/gwcelery.tasks.igwn_alert.rst
+-rw-r--r--   0        0        0      109 2023-05-08 19:41:16.856728 gwcelery-2.0.6/doc/gwcelery.tasks.inference.rst
+-rw-r--r--   0        0        0     8111 2023-05-08 19:41:16.856728 gwcelery-2.0.6/doc/gwcelery.tasks.orchestrator.rst
+-rw-r--r--   0        0        0      100 2023-05-08 19:41:16.856728 gwcelery-2.0.6/doc/gwcelery.tasks.p_astro.rst
+-rw-r--r--   0        0        0       94 2023-05-08 19:41:16.857728 gwcelery-2.0.6/doc/gwcelery.tasks.raven.rst
+-rw-r--r--   0        0        0      628 2023-05-08 19:41:16.857728 gwcelery-2.0.6/doc/gwcelery.tasks.rst
+-rw-r--r--   0        0        0      100 2023-05-08 19:41:16.857728 gwcelery-2.0.6/doc/gwcelery.tasks.skymaps.rst
+-rw-r--r--   0        0        0     7161 2023-05-08 19:41:16.857728 gwcelery-2.0.6/doc/gwcelery.tasks.superevents.rst
+-rw-r--r--   0        0        0       97 2023-05-08 19:41:16.857728 gwcelery-2.0.6/doc/gwcelery.tools.condor.rst
+-rw-r--r--   0        0        0       94 2023-05-08 19:41:16.857728 gwcelery-2.0.6/doc/gwcelery.tools.flask.rst
+-rw-r--r--   0        0        0       97 2023-05-08 19:41:16.857728 gwcelery-2.0.6/doc/gwcelery.tools.nagios.rst
+-rw-r--r--   0        0        0      185 2023-05-08 19:41:16.857728 gwcelery-2.0.6/doc/gwcelery.tools.rst
+-rw-r--r--   0        0        0       73 2023-05-08 19:41:16.857728 gwcelery-2.0.6/doc/gwcelery.util.rst
+-rw-r--r--   0        0        0      507 2023-05-08 19:41:16.857728 gwcelery-2.0.6/doc/gwcelery.voevent.rst
+-rw-r--r--   0        0        0     3564 2023-05-08 19:41:16.858728 gwcelery-2.0.6/doc/htcondor.rst
+-rw-r--r--   0        0        0     1576 2023-05-08 19:41:16.858728 gwcelery-2.0.6/doc/index.rst
+-rw-r--r--   0        0        0      800 2023-05-08 19:41:16.858728 gwcelery-2.0.6/doc/make.bat
+-rw-r--r--   0        0        0     4416 2023-05-08 19:41:16.858728 gwcelery-2.0.6/doc/monitoring.rst
+-rw-r--r--   0        0        0     5312 2023-05-08 19:41:16.858728 gwcelery-2.0.6/doc/quickstart.rst
+-rw-r--r--   0        0        0     1149 2023-05-08 19:41:16.858728 gwcelery-2.0.6/gwcelery/__init__.py
+-rw-r--r--   0        0        0    18447 2023-05-08 19:41:16.859728 gwcelery-2.0.6/gwcelery/_version.py
+-rw-r--r--   0        0        0    14975 2023-05-09 19:30:07.793112 gwcelery-2.0.6/gwcelery/conf/__init__.py
+-rw-r--r--   0        0        0      403 2023-05-08 19:41:16.859728 gwcelery-2.0.6/gwcelery/conf/development.py
+-rw-r--r--   0        0        0     1026 2023-05-08 19:41:16.859728 gwcelery-2.0.6/gwcelery/conf/minikube.py
+-rw-r--r--   0        0        0     1722 2023-05-08 19:41:16.859728 gwcelery-2.0.6/gwcelery/conf/playground.py
+-rw-r--r--   0        0        0     3541 2023-05-10 21:15:58.259619 gwcelery-2.0.6/gwcelery/conf/production.py
+-rw-r--r--   0        0        0     2040 2023-05-08 19:41:16.860728 gwcelery-2.0.6/gwcelery/conf/test.py
+-rw-r--r--   0        0        0        0 2023-05-10 21:15:58.344621 gwcelery-2.0.6/gwcelery/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 21:15:58.346621 gwcelery-2.0.6/gwcelery/data/first2years/__init__.py
+-rw-r--r--   0        0        0   731421 2023-05-08 19:41:16.863728 gwcelery-2.0.6/gwcelery/data/first2years/gstlal.xml.gz
+-rwxr-xr-x   0        0        0     2519 2023-05-08 19:41:16.863728 gwcelery-2.0.6/gwcelery/data/gwcelery.sub
+-rw-r--r--   0        0        0      505 2023-05-08 19:41:16.863728 gwcelery-2.0.6/gwcelery/email/__init__.py
+-rw-r--r--   0        0        0     3317 2023-05-08 19:41:16.863728 gwcelery-2.0.6/gwcelery/email/bootsteps.py
+-rw-r--r--   0        0        0      995 2023-05-08 19:41:16.863728 gwcelery-2.0.6/gwcelery/email/signals.py
+-rw-r--r--   0        0        0     1457 2023-05-08 19:41:16.863728 gwcelery-2.0.6/gwcelery/flask.py
+-rw-r--r--   0        0        0      529 2023-05-08 19:41:16.864728 gwcelery-2.0.6/gwcelery/igwn_alert/__init__.py
+-rw-r--r--   0        0        0     4484 2023-05-08 19:41:16.864728 gwcelery-2.0.6/gwcelery/igwn_alert/bootsteps.py
+-rw-r--r--   0        0        0      608 2023-05-08 19:41:16.864728 gwcelery-2.0.6/gwcelery/igwn_alert/signals.py
+-rw-r--r--   0        0        0      275 2023-05-08 19:41:16.864728 gwcelery-2.0.6/gwcelery/jinja.py
+-rw-r--r--   0        0        0      305 2023-05-08 19:41:16.864728 gwcelery-2.0.6/gwcelery/kafka/__init__.py
+-rw-r--r--   0        0        0    10431 2023-05-08 19:41:16.864728 gwcelery-2.0.6/gwcelery/kafka/bootsteps.py
+-rw-r--r--   0        0        0      522 2023-05-08 19:41:16.864728 gwcelery-2.0.6/gwcelery/kafka/signals.py
+-rw-r--r--   0        0        0     2567 2023-05-08 19:41:16.865728 gwcelery-2.0.6/gwcelery/sentry/__init__.py
+-rw-r--r--   0        0        0       34 2023-05-08 19:41:16.865728 gwcelery-2.0.6/gwcelery/sentry/integrations/__init__.py
+-rw-r--r--   0        0        0      832 2023-05-08 19:41:16.865728 gwcelery-2.0.6/gwcelery/sentry/integrations/condor.py
+-rw-r--r--   0        0        0      836 2023-05-08 19:41:16.865728 gwcelery-2.0.6/gwcelery/sentry/integrations/requests.py
+-rw-r--r--   0        0        0      939 2023-05-08 19:41:16.865728 gwcelery-2.0.6/gwcelery/sentry/integrations/subprocess.py
+-rw-r--r--   0        0        0     1302 2023-05-08 19:41:16.865728 gwcelery-2.0.6/gwcelery/static/typeahead.css
+-rw-r--r--   0        0        0     4124 2023-05-08 19:41:16.865728 gwcelery-2.0.6/gwcelery/static/vega/index.html
+-rw-r--r--   0        0        0      515 2023-05-08 19:41:16.865728 gwcelery-2.0.6/gwcelery/tasks/__init__.py
+-rw-r--r--   0        0        0    13067 2023-05-10 21:15:58.260619 gwcelery-2.0.6/gwcelery/tasks/alerts.py
+-rw-r--r--   0        0        0     2672 2023-05-08 19:41:16.866728 gwcelery-2.0.6/gwcelery/tasks/bayestar.py
+-rw-r--r--   0        0        0     1296 2023-05-08 19:41:16.866728 gwcelery-2.0.6/gwcelery/tasks/circulars.py
+-rw-r--r--   0        0        0     7502 2023-05-08 19:41:16.866728 gwcelery-2.0.6/gwcelery/tasks/condor.py
+-rw-r--r--   0        0        0     2692 2023-05-08 19:41:16.866728 gwcelery-2.0.6/gwcelery/tasks/core.py
+-rw-r--r--   0        0        0    21082 2023-05-09 03:39:39.191337 gwcelery-2.0.6/gwcelery/tasks/detchar.py
+-rw-r--r--   0        0        0     4863 2023-05-08 19:41:16.867728 gwcelery-2.0.6/gwcelery/tasks/em_bright.py
+-rw-r--r--   0        0        0    21951 2023-05-08 19:41:16.867728 gwcelery-2.0.6/gwcelery/tasks/external_skymaps.py
+-rw-r--r--   0        0        0    22552 2023-05-10 21:15:58.261619 gwcelery-2.0.6/gwcelery/tasks/external_triggers.py
+-rw-r--r--   0        0        0     6832 2023-05-08 19:41:16.867728 gwcelery-2.0.6/gwcelery/tasks/first2years.py
+-rw-r--r--   0        0        0     6384 2023-05-08 19:41:16.868728 gwcelery-2.0.6/gwcelery/tasks/first2years_external.py
+-rw-r--r--   0        0        0     4831 2023-05-08 19:41:16.868728 gwcelery-2.0.6/gwcelery/tasks/gcn.py
+-rw-r--r--   0        0        0    11079 2023-05-08 19:41:16.868728 gwcelery-2.0.6/gwcelery/tasks/gracedb.py
+-rw-r--r--   0        0        0     2453 2023-05-08 19:41:16.868728 gwcelery-2.0.6/gwcelery/tasks/igwn_alert.py
+-rw-r--r--   0        0        0    39761 2023-05-08 19:41:16.868728 gwcelery-2.0.6/gwcelery/tasks/inference.py
+-rw-r--r--   0        0        0     1406 2023-05-08 19:41:16.869728 gwcelery-2.0.6/gwcelery/tasks/legacy_gracedb.py
+-rw-r--r--   0        0        0     7772 2023-05-08 19:41:16.869728 gwcelery-2.0.6/gwcelery/tasks/notice_text.py
+-rw-r--r--   0        0        0    46680 2023-05-08 19:41:16.869728 gwcelery-2.0.6/gwcelery/tasks/orchestrator.py
+-rw-r--r--   0        0        0     5796 2023-05-08 19:41:16.870728 gwcelery-2.0.6/gwcelery/tasks/p_astro.py
+-rw-r--r--   0        0        0    19693 2023-05-08 19:41:16.870728 gwcelery-2.0.6/gwcelery/tasks/raven.py
+-rw-r--r--   0        0        0     2242 2023-05-08 19:41:16.870728 gwcelery-2.0.6/gwcelery/tasks/rrt_utils.py
+-rw-r--r--   0        0        0    12528 2023-05-08 19:41:16.870728 gwcelery-2.0.6/gwcelery/tasks/skymaps.py
+-rw-r--r--   0        0        0    23386 2023-05-08 19:41:16.871728 gwcelery-2.0.6/gwcelery/tasks/superevents.py
+-rw-r--r--   0        0        0     1084 2023-05-08 19:41:16.871728 gwcelery-2.0.6/gwcelery/templates/fits_header.jinja2
+-rw-r--r--   0        0        0    34059 2023-05-08 19:41:16.871728 gwcelery-2.0.6/gwcelery/templates/index.jinja2
+-rw-r--r--   0        0        0     8505 2023-05-08 19:41:16.872728 gwcelery-2.0.6/gwcelery/templates/lalinference.jinja2
+-rw-r--r--   0        0        0     8939 2023-05-08 19:41:16.872728 gwcelery-2.0.6/gwcelery/templates/rapidpe.jinja2
+-rw-r--r--   0        0        0      806 2023-05-08 19:41:16.872728 gwcelery-2.0.6/gwcelery/templates/vector_table.jinja2
+-rw-r--r--   0        0        0        0 2023-05-10 21:15:58.348621 gwcelery-2.0.6/gwcelery/tests/__init__.py
+-rw-r--r--   0        0        0     4388 2023-05-08 19:41:16.872728 gwcelery-2.0.6/gwcelery/tests/conftest.py
+-rw-r--r--   0        0        0      976 2023-05-08 19:41:16.872728 gwcelery-2.0.6/gwcelery/tests/data/G000012_S0040_preferred.json
+-rw-r--r--   0        0        0     6258 2023-05-08 19:41:16.873728 gwcelery-2.0.6/gwcelery/tests/data/G298048-1-Initial.xml
+-rw-r--r--   0        0        0      599 2023-05-08 19:41:16.873728 gwcelery-2.0.6/gwcelery/tests/data/G298048_log.json
+-rw-r--r--   0        0        0      150 2023-05-08 19:41:16.873728 gwcelery-2.0.6/gwcelery/tests/data/H1L1V1-mean_counts-1126051217-61603201.json
+-rw-r--r--   0        0        0      974 2023-05-08 19:41:16.873728 gwcelery-2.0.6/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json
+-rw-r--r--   0        0        0    17572 2023-05-08 19:41:16.873728 gwcelery-2.0.6/gwcelery/tests/data/MS220722v.xml
+-rw-r--r--   0        0        0   777600 2023-05-08 19:41:16.879728 gwcelery-2.0.6/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits
+-rw-r--r--   0        0        0     8220 2023-05-08 19:41:16.879728 gwcelery-2.0.6/gwcelery/tests/data/S230413b.json
+-rw-r--r--   0        0        0     7255 2023-05-08 19:41:16.880728 gwcelery-2.0.6/gwcelery/tests/data/S230413g.json
+-rw-r--r--   0        0        0     7721 2023-05-08 19:41:16.880728 gwcelery-2.0.6/gwcelery/tests/data/S230413h.json
+-rw-r--r--   0        0        0     3387 2023-05-08 19:41:16.880728 gwcelery-2.0.6/gwcelery/tests/data/T0212_S0039_preferred.json
+-rw-r--r--   0        0        0     3384 2023-05-08 19:41:16.880728 gwcelery-2.0.6/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json
+-rw-r--r--   0        0        0     5210 2023-05-08 19:41:16.880728 gwcelery-2.0.6/gwcelery/tests/data/T0219_S0041_nopreferred.json
+-rw-r--r--   0        0        0        0 2023-05-10 21:15:58.349621 gwcelery-2.0.6/gwcelery/tests/data/__init__.py
+-rw-r--r--   0        0        0     2290 2023-05-08 19:41:16.880728 gwcelery-2.0.6/gwcelery/tests/data/agile_grb_gcn.xml
+-rw-r--r--   0        0        0   854036 2023-05-08 19:41:16.886729 gwcelery-2.0.6/gwcelery/tests/data/coinc.xml
+-rw-r--r--   0        0        0     6175 2023-05-08 19:41:16.886729 gwcelery-2.0.6/gwcelery/tests/data/externaltrigger_original_data.xml
+-rw-r--r--   0        0        0     5482 2023-05-08 19:41:16.886729 gwcelery-2.0.6/gwcelery/tests/data/fermi_grb_gcn.xml
+-rw-r--r--   0        0        0     5469 2023-05-08 19:41:16.886729 gwcelery-2.0.6/gwcelery/tests/data/fermi_initial_grb_gcn.xml
+-rw-r--r--   0        0        0     5865 2023-05-08 19:41:16.887729 gwcelery-2.0.6/gwcelery/tests/data/fermi_noise_gcn.xml
+-rw-r--r--   0        0        0     5864 2023-05-08 19:41:16.887729 gwcelery-2.0.6/gwcelery/tests/data/fermi_noise_gcn_2.xml
+-rw-r--r--   0        0        0     4914 2023-05-08 19:41:16.887729 gwcelery-2.0.6/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml
+-rw-r--r--   0        0        0     4914 2023-05-08 19:41:16.887729 gwcelery-2.0.6/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml
+-rw-r--r--   0        0        0     3407 2023-05-08 19:41:16.887729 gwcelery-2.0.6/gwcelery/tests/data/fits_header_result.html
+-rw-r--r--   0        0        0      882 2023-05-08 19:41:16.887729 gwcelery-2.0.6/gwcelery/tests/data/gracedb_externaltrigger_log.json
+-rw-r--r--   0        0        0      446 2023-05-08 19:41:16.887729 gwcelery-2.0.6/gwcelery/tests/data/gracedb_setrigger_log.json
+-rw-r--r--   0        0        0      870 2023-05-08 19:41:16.887729 gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_detchar.json
+-rw-r--r--   0        0        0     2025 2023-05-08 19:41:16.888729 gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_exttrig_creation.json
+-rw-r--r--   0        0        0     2007 2023-05-08 19:41:16.888729 gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json
+-rw-r--r--   0        0        0      166 2023-05-08 19:41:16.888729 gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_fits.json
+-rw-r--r--   0        0        0      101 2023-05-08 19:41:16.888729 gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_label_dqv.json
+-rw-r--r--   0        0        0      743 2023-05-08 19:41:16.888729 gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_psd.json
+-rw-r--r--   0        0        0     2020 2023-05-08 19:41:16.888729 gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_snews_creation.json
+-rw-r--r--   0        0        0     2012 2023-05-08 19:41:16.888729 gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_snews_test_creation.json
+-rw-r--r--   0        0        0     2028 2023-05-08 19:41:16.889729 gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_subgrb_creation.json
+-rw-r--r--   0        0        0     1235 2023-05-08 19:41:16.889729 gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_superevent_creation.json
+-rw-r--r--   0        0        0      107 2023-05-08 19:41:16.889729 gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_superevent_label.json
+-rw-r--r--   0        0        0     5021 2023-05-08 19:41:16.889729 gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_voevent.json
+-rw-r--r--   0        0        0     4429 2023-05-08 19:41:16.889729 gwcelery-2.0.6/gwcelery/tests/data/integral_grb_gcn.xml
+-rw-r--r--   0        0        0     4295 2023-05-08 19:41:16.889729 gwcelery-2.0.6/gwcelery/tests/data/integral_mdc_gcn.xml
+-rw-r--r--   0        0        0        0 2023-05-10 21:15:58.350622 gwcelery-2.0.6/gwcelery/tests/data/llhoft/__init__.py
+-rw-r--r--   0        0        0    14622 2023-05-08 19:41:16.890729 gwcelery-2.0.6/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf
+-rw-r--r--   0        0        0        0 2023-05-10 21:15:58.350622 gwcelery-2.0.6/gwcelery/tests/data/llhoft/fail/L1/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 21:15:58.350622 gwcelery-2.0.6/gwcelery/tests/data/llhoft/fail/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 21:15:58.350622 gwcelery-2.0.6/gwcelery/tests/data/llhoft/omegascan/__init__.py
+-rw-r--r--   0        0        0   516419 2023-05-08 19:41:16.891729 gwcelery-2.0.6/gwcelery/tests/data/llhoft/omegascan/scanme.gwf
+-rw-r--r--   0        0        0    14630 2023-05-08 19:41:16.892729 gwcelery-2.0.6/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf
+-rw-r--r--   0        0        0        0 2023-05-10 21:15:58.350622 gwcelery-2.0.6/gwcelery/tests/data/llhoft/pass/H1/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-10 21:15:58.350622 gwcelery-2.0.6/gwcelery/tests/data/llhoft/pass/__init__.py
+-rw-r--r--   0        0        0    13099 2023-05-08 19:41:16.892729 gwcelery-2.0.6/gwcelery/tests/data/lvalert_event_creation.json
+-rw-r--r--   0        0        0     9060 2023-05-08 19:41:16.892729 gwcelery-2.0.6/gwcelery/tests/data/lvalert_xmpp.xml
+-rw-r--r--   0        0        0      864 2023-05-08 19:41:16.892729 gwcelery-2.0.6/gwcelery/tests/data/mock_superevent_object.json
+-rw-r--r--   0        0        0   445440 2023-05-08 19:41:16.894729 gwcelery-2.0.6/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite
+-rw-r--r--   0        0        0   294426 2023-05-08 19:41:16.895729 gwcelery-2.0.6/gwcelery/tests/data/psd.xml.gz
+-rw-r--r--   0        0        0    11520 2023-05-08 19:41:16.896729 gwcelery-2.0.6/gwcelery/tests/data/rrt_small_area.fits
+-rw-r--r--   0        0        0     2964 2023-05-08 19:41:16.896729 gwcelery-2.0.6/gwcelery/tests/data/sample_events.json
+-rw-r--r--   0        0        0     3648 2023-05-08 19:41:16.896729 gwcelery-2.0.6/gwcelery/tests/data/samples.hdf5
+-rw-r--r--   0        0        0      616 2023-05-08 19:41:16.896729 gwcelery-2.0.6/gwcelery/tests/data/scaler_set_all.pickle
+-rw-r--r--   0        0        0     6169 2023-05-08 19:41:16.896729 gwcelery-2.0.6/gwcelery/tests/data/snews_gcn.xml
+-rw-r--r--   0        0        0     6161 2023-05-08 19:41:16.896729 gwcelery-2.0.6/gwcelery/tests/data/snews_gcn_test.xml
+-rw-r--r--   0        0        0     9583 2023-05-08 19:41:16.896729 gwcelery-2.0.6/gwcelery/tests/data/superevents.json
+-rw-r--r--   0        0        0     7713 2023-05-08 19:41:16.896729 gwcelery-2.0.6/gwcelery/tests/data/swift_grb_gcn.xml
+-rw-r--r--   0        0        0   581918 2023-05-08 19:41:16.899729 gwcelery-2.0.6/gwcelery/tests/data/test_classifier.pickle
+-rw-r--r--   0        0        0     4042 2023-05-08 19:41:16.899729 gwcelery-2.0.6/gwcelery/tests/process.py
+-rw-r--r--   0        0        0     2307 2023-05-08 19:41:16.900729 gwcelery-2.0.6/gwcelery/tests/test_sentry.py
+-rw-r--r--   0        0        0     1705 2023-05-08 19:41:16.900729 gwcelery-2.0.6/gwcelery/tests/test_tasks_alerts.py
+-rw-r--r--   0        0        0     4916 2023-05-08 19:41:16.900729 gwcelery-2.0.6/gwcelery/tests/test_tasks_alerts_validate.py
+-rw-r--r--   0        0        0     1439 2023-05-08 19:41:16.900729 gwcelery-2.0.6/gwcelery/tests/test_tasks_bayestar.py
+-rw-r--r--   0        0        0     2416 2023-05-08 19:41:16.900729 gwcelery-2.0.6/gwcelery/tests/test_tasks_circulars.py
+-rw-r--r--   0        0        0     4550 2023-05-08 19:41:16.900729 gwcelery-2.0.6/gwcelery/tests/test_tasks_condor.py
+-rw-r--r--   0        0        0    11688 2023-05-08 19:41:16.901729 gwcelery-2.0.6/gwcelery/tests/test_tasks_detchar.py
+-rw-r--r--   0        0        0     2317 2023-05-08 19:41:16.901729 gwcelery-2.0.6/gwcelery/tests/test_tasks_em_bright.py
+-rw-r--r--   0        0        0    12322 2023-05-08 19:41:16.901729 gwcelery-2.0.6/gwcelery/tests/test_tasks_external_skymaps.py
+-rw-r--r--   0        0        0    32406 2023-05-10 21:15:58.262619 gwcelery-2.0.6/gwcelery/tests/test_tasks_external_triggers.py
+-rw-r--r--   0        0        0     1816 2023-05-08 19:41:16.901729 gwcelery-2.0.6/gwcelery/tests/test_tasks_first2years.py
+-rw-r--r--   0        0        0     4555 2023-05-08 19:41:16.901729 gwcelery-2.0.6/gwcelery/tests/test_tasks_first2years_external.py
+-rw-r--r--   0        0        0     1826 2023-05-08 19:41:16.902729 gwcelery-2.0.6/gwcelery/tests/test_tasks_gcn.py
+-rw-r--r--   0        0        0     1655 2023-05-08 19:41:16.902729 gwcelery-2.0.6/gwcelery/tests/test_tasks_gcn_validate.py
+-rw-r--r--   0        0        0     5739 2023-05-08 19:41:16.902729 gwcelery-2.0.6/gwcelery/tests/test_tasks_gracedb.py
+-rw-r--r--   0        0        0     3662 2023-05-08 19:41:16.902729 gwcelery-2.0.6/gwcelery/tests/test_tasks_igwn_alert.py
+-rw-r--r--   0        0        0    21593 2023-05-08 19:41:16.903729 gwcelery-2.0.6/gwcelery/tests/test_tasks_inference.py
+-rw-r--r--   0        0        0    33299 2023-05-08 19:41:16.903729 gwcelery-2.0.6/gwcelery/tests/test_tasks_orchestrator.py
+-rw-r--r--   0        0        0     1647 2023-05-08 19:41:16.903729 gwcelery-2.0.6/gwcelery/tests/test_tasks_p_astro.py
+-rw-r--r--   0        0        0    26044 2023-05-08 19:41:16.904729 gwcelery-2.0.6/gwcelery/tests/test_tasks_raven.py
+-rw-r--r--   0        0        0     4724 2023-05-08 19:41:16.904729 gwcelery-2.0.6/gwcelery/tests/test_tasks_rrt_utils.py
+-rw-r--r--   0        0        0     5035 2023-05-08 19:41:16.904729 gwcelery-2.0.6/gwcelery/tests/test_tasks_skymaps.py
+-rw-r--r--   0        0        0    39981 2023-05-08 19:41:16.904729 gwcelery-2.0.6/gwcelery/tests/test_tasks_superevents.py
+-rw-r--r--   0        0        0      637 2023-05-08 19:41:16.905729 gwcelery-2.0.6/gwcelery/tests/test_tempfile.py
+-rw-r--r--   0        0        0     3520 2023-05-08 19:41:16.905729 gwcelery-2.0.6/gwcelery/tests/test_tools_condor.py
+-rw-r--r--   0        0        0     1098 2023-05-08 19:41:16.905729 gwcelery-2.0.6/gwcelery/tests/test_tools_condor_submit_helper.py
+-rw-r--r--   0        0        0      633 2023-05-08 19:41:16.905729 gwcelery-2.0.6/gwcelery/tests/test_tools_flask.py
+-rw-r--r--   0        0        0     9658 2023-05-08 19:41:16.905729 gwcelery-2.0.6/gwcelery/tests/test_tools_nagios.py
+-rw-r--r--   0        0        0      269 2023-05-08 19:41:16.905729 gwcelery-2.0.6/gwcelery/tests/test_util.py
+-rw-r--r--   0        0        0    21450 2023-05-08 19:41:16.905729 gwcelery-2.0.6/gwcelery/tests/test_views.py
+-rw-r--r--   0        0        0      216 2023-05-08 19:41:16.906729 gwcelery-2.0.6/gwcelery/tools/__init__.py
+-rw-r--r--   0        0        0     2948 2023-05-08 19:41:16.906729 gwcelery-2.0.6/gwcelery/tools/condor.py
+-rw-r--r--   0        0        0     1120 2023-05-08 19:41:16.906729 gwcelery-2.0.6/gwcelery/tools/condor_submit_helper.py
+-rw-r--r--   0        0        0     1938 2023-05-08 19:41:16.906729 gwcelery-2.0.6/gwcelery/tools/flask.py
+-rw-r--r--   0        0        0     6624 2023-05-08 19:41:16.906729 gwcelery-2.0.6/gwcelery/tools/nagios.py
+-rw-r--r--   0        0        0      413 2023-05-08 19:41:16.906729 gwcelery-2.0.6/gwcelery/util/__init__.py
+-rw-r--r--   0        0        0     1007 2023-05-08 19:41:16.906729 gwcelery-2.0.6/gwcelery/util/cmdline.py
+-rw-r--r--   0        0        0      453 2023-05-08 19:41:16.906729 gwcelery-2.0.6/gwcelery/util/matplotlib.py
+-rw-r--r--   0        0        0      390 2023-05-08 19:41:16.907729 gwcelery-2.0.6/gwcelery/util/proxy.py
+-rw-r--r--   0        0        0      514 2023-05-08 19:41:16.907729 gwcelery-2.0.6/gwcelery/util/resources.py
+-rw-r--r--   0        0        0      253 2023-05-08 19:41:16.907729 gwcelery-2.0.6/gwcelery/util/sphinx.py
+-rw-r--r--   0        0        0      941 2023-05-08 19:41:16.907729 gwcelery-2.0.6/gwcelery/util/tempfile.py
+-rw-r--r--   0        0        0    18472 2023-05-08 19:41:16.907729 gwcelery-2.0.6/gwcelery/views.py
+-rw-r--r--   0        0        0      365 2023-05-08 19:41:16.907729 gwcelery-2.0.6/gwcelery/voevent/__init__.py
+-rw-r--r--   0        0        0     6387 2023-05-08 19:41:16.908729 gwcelery-2.0.6/gwcelery/voevent/bootsteps.py
+-rw-r--r--   0        0        0     1063 2023-05-08 19:41:16.908729 gwcelery-2.0.6/gwcelery/voevent/logging.py
+-rw-r--r--   0        0        0      779 2023-05-08 19:41:16.908729 gwcelery-2.0.6/gwcelery/voevent/signals.py
+-rw-r--r--   0        0        0      852 2023-05-08 19:41:16.908729 gwcelery-2.0.6/gwcelery/voevent/subscriber.py
+-rw-r--r--   0        0        0     1454 2023-05-08 19:41:16.908729 gwcelery-2.0.6/gwcelery/voevent/util.py
+-rw-r--r--   0        0        0     5956 2023-05-10 21:16:17.400233 gwcelery-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4628 1970-01-01 00:00:00.000000 gwcelery-2.0.6/PKG-INFO
```

### Comparing `gwcelery-2.0.5/CHANGES.rst` & `gwcelery-2.0.6/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,57 @@
 Changelog
 =========
 
+2.0.6 "Spaghetti Tree" (2023-05-10)
+-----------------------------------
+
+-   Add `HIGH_PROFILE` label for rapid response team.
+
+-   Ensure that external events are not already associated with a superevent
+    when triggering Raven off of superevents.
+
+-   Add minimum resolution for external sky maps.
+
+-   Remove clutter from omegascan pngs and lower dpi to 150 to reduce
+    file size.
+
+-   Retry GCN circular creation upon 408 or 409 errors, likely due to AWS
+    issues for GraceDB.
+
+-   Add Kafka consumer bootstep.
+
+-   Skip plotting sky map overlap integral if coinc_far_dict is empty, which
+    occurs for SNEWS coincidences.
+
+-   Update iDQ channel configuration for O4 iDQ channels. The playground
+    config will continue to use the O3 channels to support the O3 MDC replay.
+
+-   Update bilby settings. Set the chirp mass boundary between BNS and
+    potential NSBH to 1.465Msun, computed from component masses of 3Msun and
+    1Msun, and use low-spin IMRPhenomD below and high-spin IMRPhenomPv2 above.
+    For high mass triggers, use IMRPhenomXPHM. Use these "production" settings
+    by default for MDC and production analyses, and we no longer have multiple
+    bilby runs on a single event. Increase the time limit of condor job to 12
+    hours.
+
+-   Bump pesummary version to 1.0.0. Disable ligo skymap and use 6 cpus and
+    online-PE dedicated nodes to speed up the pesummary postprocess.
+
+-   Enable public alerts in production.
+
+-   Disable Kafka consumer bootstep in the production deployment.
+
+-   Fix bug where Kafka alerts were using combined sky map from the external
+    event rather than the superevent.
+
+-   Fix bug where the external sky map was created with out-of-date external
+    GCN information.
+
+-   Require em-bright >= 1.1.2.
+
 2.0.5 "Mothman" (2023-04-20)
 ----------------------------
 
 -   Add Mattermost channel creation for the RRT to discuss a superevent
     candidate.
 
 -   Use Online_PE_MDC nodes for bilby jobs on O3-Replay injections.
```

### Comparing `gwcelery-2.0.5/LICENSE.rst` & `gwcelery-2.0.6/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/README.rst` & `gwcelery-2.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/doc/Makefile` & `gwcelery-2.0.6/doc/Makefile`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/doc/_static/acceptance-tests-checklist.png` & `gwcelery-2.0.6/doc/_static/acceptance-tests-checklist.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/doc/_static/celeryevent-screenshot.png` & `gwcelery-2.0.6/doc/_static/celeryevent-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/doc/_static/deployment-screenshot.png` & `gwcelery-2.0.6/doc/_static/deployment-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/doc/_static/flask-screenshot.png` & `gwcelery-2.0.6/doc/_static/flask-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/doc/_static/flower-screenshot.png` & `gwcelery-2.0.6/doc/_static/flower-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/doc/_static/logo-0.5x.png` & `gwcelery-2.0.6/doc/_static/logo-0.5x.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/doc/_static/logo.png` & `gwcelery-2.0.6/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/doc/_static/sentry-screenshot.png` & `gwcelery-2.0.6/doc/_static/sentry-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/doc/conf.py` & `gwcelery-2.0.6/doc/conf.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/doc/configuration.rst` & `gwcelery-2.0.6/doc/configuration.rst`

 * *Files 17% similar despite different names*

```diff
@@ -46,14 +46,37 @@
 
 .. rubric:: IGWN Alert
 
 You must provide a valid username and password for :doc:`IGWN Alert <igwn-alert:index>`. You can request an
 account using the `SCiMMA Auth portal`_. To get started, see :doc:`IGWN Alert Userguide <igwn-alert:guide>`.
 The IGWN Alert username and password should be stored in your `netrc file`_.
 
+.. rubric:: Kafka
+
+You must provide a file named ``kafka_credential_map.json`` that maps
+deployment specific usernames for Kafka credentials to the logical names given
+in the configuration files. This file should be saved in the GWCelery XDG
+config directory (``${HOME}/.config/gwcelery/`` by default on many Linux and
+UNIX-like operating systems). An example file can be seen below::
+
+    {
+        "consumer": {
+            "fermi": "user_one",
+            "swift": "user_two"
+        },
+        "producer": {
+            "gcn": "user_one",
+            "scimma": "user_three"
+        }
+    }
+
+Note that one user can be specified multiple times. ``hop auth`` must have
+information about each user specified in this file. Every Kafka producer and
+consumer configuration key must have an entry in this file.
+
 .. _`LSC DataGrid Client`: https://www.lsc-group.phys.uwm.edu/lscdatagrid/doc/installclient.html
 .. _`obtain a robot certificate`: https://robots.ligo.org
 .. _`SCiMMA Auth portal`: https://my.hop.scimma.org/
 .. _`netrc file`: https://www.gnu.org/software/inetutils/manual/html_node/The-_002enetrc-file.html
 
 .. _redis-configuration:
```

### Comparing `gwcelery-2.0.5/doc/contributing.rst` & `gwcelery-2.0.6/doc/contributing.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/doc/deployment.rst` & `gwcelery-2.0.6/doc/deployment.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/doc/design.rst` & `gwcelery-2.0.6/doc/design.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/doc/gwcelery.tasks.detchar.rst` & `gwcelery-2.0.6/doc/gwcelery.tasks.detchar.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/doc/gwcelery.tasks.em_bright.rst` & `gwcelery-2.0.6/doc/gwcelery.tasks.em_bright.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/doc/gwcelery.tasks.external_triggers.rst` & `gwcelery-2.0.6/doc/gwcelery.tasks.external_triggers.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/doc/gwcelery.tasks.orchestrator.rst` & `gwcelery-2.0.6/doc/gwcelery.tasks.orchestrator.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/doc/gwcelery.tasks.rst` & `gwcelery-2.0.6/doc/gwcelery.tasks.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/doc/gwcelery.tasks.superevents.rst` & `gwcelery-2.0.6/doc/gwcelery.tasks.superevents.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/doc/htcondor.rst` & `gwcelery-2.0.6/doc/htcondor.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/doc/index.rst` & `gwcelery-2.0.6/doc/index.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/doc/make.bat` & `gwcelery-2.0.6/doc/make.bat`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/doc/monitoring.rst` & `gwcelery-2.0.6/doc/monitoring.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/doc/quickstart.rst` & `gwcelery-2.0.6/doc/quickstart.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/__init__.py` & `gwcelery-2.0.6/gwcelery/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/_version.py` & `gwcelery-2.0.6/gwcelery/_version.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/conf/__init__.py` & `gwcelery-2.0.6/gwcelery/conf/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -67,14 +67,24 @@
 
 gracedb_host = 'gracedb-playground.ligo.org'
 """GraceDB host."""
 
 create_mattermost_channel = False
 """Do not create Mattermost channel."""
 
+kafka_consumer_config = {
+    'fermi': {'url': 'kafka://kafka.test.gcn.nasa.gov/'
+              'fermi.gbm.targeted.private', 'suffix': 'json'},
+    'swift': {'url': 'kafka://kafka.test.gcn.nasa.gov/swift.bat.guano',
+              'suffix': 'json'}
+}
+"""Kafka consumer configuration details. The keys describe the senders of the
+messages to be consumed. The values are a dictionary of the URL to listen to
+and information about the message serializer."""
+
 voevent_broadcaster_address = ':5342'
 """The VOEvent broker will bind to this address to send GCNs.
 This should be a string of the form `host:port`. If `host` is empty,
 then listen on all available interfaces."""
 
 voevent_broadcaster_whitelist = []
 """List of hosts from which the broker will accept connections.
@@ -136,15 +146,15 @@
 
 early_warning_alert_far_threshold = 1 / (30 * 86400)
 """False alarm rate threshold for significant early warning alerts."""
 
 significant_alert_trials_factor = dict(cbc=5.0, burst=4.0)
 """Trials factor corresponding to trigger categories. For CBC and Burst, trials
 factor is the number of pipelines. CBC pipelines are gstlal, pycbc, mbta and
-spiir. Burst searches are cwb.allsky, cwb.bbh and cwb.imbh."""
+spiir. Burst searches are cwb.allsky, cwb.imbh, and olib."""
 
 preliminary_alert_trials_factor = dict(cbc=8.0, burst=8.0)
 """Trials factor for less significant alerts."""
 
 snews_gw_far_threshold = 1 / (3600 * 24)
 """Maximum false alarm rate for a superevent to send out a coincidence alert
 between an external SNEWS alert and the superevent."""
@@ -208,17 +218,17 @@
     'L1:DMT-DQ_VECTOR': 'dmt_dq_vector_bits',
     'H1:GDS-CALIB_STATE_VECTOR': 'ligo_state_vector_bits',
     'L1:GDS-CALIB_STATE_VECTOR': 'ligo_state_vector_bits',
     'V1:DQ_ANALYSIS_STATE_VECTOR': 'virgo_state_vector_bits'}
 """Low-latency h(t) state vector configuration. This is a dictionary consisting
 of a channel and its bitmask, as defined in :mod:`gwcelery.tasks.detchar`."""
 
-idq_channels = ['H1:IDQ-FAP_OVL_16_4096',
-                'L1:IDQ-FAP_OVL_16_4096']
-"""Low-latency iDQ false alarm probability channel names from O3 replay."""
+idq_channels = ['H1:IDQ-FAP_OVL_10_2048',
+                'L1:IDQ-FAP_OVL_10_2048']
+"""Low-latency iDQ false alarm probability channel names for O4."""
 
 idq_fap_thresh = 0.01
 """If FAP is below this threshold, and
 :obj:`~gwcelery.conf.idq_veto` for the pipeline is true, DQV will be labeled
 for the event.
 """
 
@@ -360,19 +370,16 @@
 MDC superevents an external MDC event is created."""
 
 joint_O3_replay_freq = 10
 """Determines how often an external replay event will be created near an
 superevent to test the RAVEN alert pipeline, i.e for every x
 O3 replay superevents an external MDC event is created."""
 
-bilby_default_mode = 'fast_test'
-"""Sampling mode of bilby"""
-
 condor_retry_kwargs = dict(
-    max_retries=45, retry_backoff=True, retry_jitter=False,
+    max_retries=80, retry_backoff=True, retry_jitter=False,
     retry_backoff_max=600
 )
 """Retry settings of condor.submit task. With these settings, a condor job is
-no longer tracked ~6 hours after it starts."""
+no longer tracked ~12 hours after it starts."""
 
 # Delete imported modules so that they do not pollute the config object
 del os, getpass
```

### Comparing `gwcelery-2.0.5/gwcelery/conf/minikube.py` & `gwcelery-2.0.6/gwcelery/conf/minikube.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/conf/playground.py` & `gwcelery-2.0.6/gwcelery/conf/playground.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,7 +32,11 @@
 If empty, then completely disable the broker's broadcast capability."""
 
 voevent_receiver_address = '50.116.49.68:8094'
 """The VOEvent listener will connect to this address to receive GCNs. For
 options, see `GCN's list of available VOEvent servers
 <https://gcn.gsfc.nasa.gov/voevent.html#tc2>`_. If this is an empty string,
 then completely disable the GCN listener."""
+
+idq_channels = ['H1:IDQ-FAP_OVL_16_4096',
+                'L1:IDQ-FAP_OVL_16_4096']
+"""Low-latency iDQ false alarm probability channel names for O3 replay."""
```

### Comparing `gwcelery-2.0.5/gwcelery/conf/production.py` & `gwcelery-2.0.6/gwcelery/conf/production.py`

 * *Files 21% similar despite different names*

```diff
@@ -29,14 +29,23 @@
                'suffix': 'avro', 'skymap_encoder': lambda _: _},
     'gcn': {'url': 'kafka://kafka.gcn.nasa.gov/igwn.gwalert',
             'suffix': 'json', 'skymap_encoder': lambda b:
             b64encode(b).decode('utf-8')}
 }
 """Kafka broker configuration details"""
 
+# FIXME kafka_consumer_config is only empty here as a safety precaution for
+# ER15 production deployment. We need to deploy a new release because we need
+# to enable alerts, but we haven't tested the Kafka consumer bootsteps enough
+# to deploy them on production yet.
+kafka_consumer_config = {}
+"""Kafka consumer configuration details. The keys describe the senders of the
+messages to be consumed. The values are a dictionary of the URL to listen to
+and information about the message serializer."""
+
 voevent_broadcaster_address = ':5341'
 """The VOEvent broker will bind to this address to send GCNs.
 This should be a string of the form `host:port`. If `host` is empty,
 then listen on all available interfaces."""
 
 voevent_broadcaster_whitelist = ['capella2.gsfc.nasa.gov']
 """List of hosts from which the broker will accept connections.
@@ -57,34 +66,31 @@
                             'L1': 'L1_HOFT_C00',
                             'V1': 'V1Online'}
 """Types of high latency frames used in Parameter Estimation
 (see :mod:`gwcelery.tasks.inference`) and in cache creation for detchar
 checks (see :mod:`gwcelery.tasks.detchar`).
 """
 
-idq_channels = ['H1:IDQ-FAP_OVL_16_4096',
-                'L1:IDQ-FAP_OVL_16_4096']
+idq_channels = ['H1:IDQ-FAP_OVL_10_2048',
+                'L1:IDQ-FAP_OVL_10_2048']
 """Low-latency iDQ false alarm probability channel names from live O3 frames"""
 
 strain_channel_names = {'H1': 'H1:GDS-CALIB_STRAIN_CLEAN',
                         'L1': 'L1:GDS-CALIB_STRAIN_CLEAN',
                         'V1': 'V1:Hrec_hoft_16384Hz'}
 """Names of h(t) channels used in Parameter Estimation (see
 :mod:`gwcelery.tasks.inference`)"""
 
 sentry_environment = 'production'
 """Record this `environment tag
 <https://docs.sentry.io/enriching-error-data/environments/>`_ in Sentry log
 messages."""
 
-only_alert_for_mdc = True
+only_alert_for_mdc = False
 """If True, then only sends alerts for MDC events. Useful for times outside
 of observing runs."""
 
-bilby_default_mode = 'production'
-"""Sampling mode of bilby"""
-
 condor_retry_kwargs = dict(
     max_retries=None, retry_backoff=True, retry_jitter=True,
     retry_backoff_max=600
 )
 """Retry settings of condor.submit task."""
```

### Comparing `gwcelery-2.0.5/gwcelery/data/first2years/gstlal.xml.gz` & `gwcelery-2.0.6/gwcelery/data/first2years/gstlal.xml.gz`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/data/gwcelery.sub` & `gwcelery-2.0.6/gwcelery/data/gwcelery.sub`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/email/bootsteps.py` & `gwcelery-2.0.6/gwcelery/email/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/email/signals.py` & `gwcelery-2.0.6/gwcelery/email/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/flask.py` & `gwcelery-2.0.6/gwcelery/flask.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/igwn_alert/__init__.py` & `gwcelery-2.0.6/gwcelery/igwn_alert/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/igwn_alert/bootsteps.py` & `gwcelery-2.0.6/gwcelery/igwn_alert/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/igwn_alert/signals.py` & `gwcelery-2.0.6/gwcelery/igwn_alert/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/sentry/__init__.py` & `gwcelery-2.0.6/gwcelery/sentry/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/sentry/integrations/condor.py` & `gwcelery-2.0.6/gwcelery/sentry/integrations/condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/sentry/integrations/requests.py` & `gwcelery-2.0.6/gwcelery/sentry/integrations/requests.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/sentry/integrations/subprocess.py` & `gwcelery-2.0.6/gwcelery/sentry/integrations/subprocess.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/static/typeahead.css` & `gwcelery-2.0.6/gwcelery/static/typeahead.css`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/static/vega/index.html` & `gwcelery-2.0.6/gwcelery/static/vega/index.html`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tasks/__init__.py` & `gwcelery-2.0.6/gwcelery/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tasks/alerts.py` & `gwcelery-2.0.6/gwcelery/tasks/alerts.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,57 @@
 
 from astropy import time
 from celery import group
 from celery.utils.log import get_logger
 import numpy as np
 
 from ..import app
+from .core import DispatchHandler
 from . import gracedb
+from ..kafka.signals import kafka_record_consumed
 
 log = get_logger(__name__)
 
 
+class _KafkaDispatchHandler(DispatchHandler):
+
+    def process_args(self, name, record):
+        return name, (record,), {}
+
+
+handler = _KafkaDispatchHandler()
+r"""Function decorator to register a handler callback for specified Kafka URLs.
+The decorated function is turned into a Celery task, which will be
+automatically called whenever a message is received from a matching URL.
+
+Parameters
+----------
+\*keys
+    List of keys from :obj:`gwcelery.conf.kafka_consumer_config`
+    associated with Kafka topics to listen to messages to.
+\*\*kwargs
+    Additional keyword arguments for :meth:`celery.Celery.task`.
+
+Examples
+--------
+Declare a new handler like this::
+
+    # Assumes kafka_consumer_config dictionary has 'fermi_swift' key
+    @alerts.handler('fermi_swift')
+    def handle_swift(record):
+        # record is a dict that contains the contents of the message
+        # do work here...
+"""
+
+
+@kafka_record_consumed.connect
+def _on_kafka_record_consumed(name, record, **kwargs):
+    handler.dispatch(name, record)
+
+
 def _create_base_alert_dict(classification, superevent, alert_type):
     '''Create the base of the alert dictionary, with all contents except the
     skymap and the external coinc information.'''
     # NOTE Everything that comes through this code path will be marked as
     # public. However, MDC events with this flag are not made public on
     # GraceDB-playground and GraceDB-test.
     # Re time_created: Dont need better than second precision for alert times
@@ -106,15 +144,15 @@
 
 @gracedb.task(shared=False)
 def _add_external_coinc_to_alert(alert_dict, superevent,
                                  combined_skymap_filename):
     external_event = gracedb.get_event(superevent['em_type'])
     if combined_skymap_filename:
         combined_skymap = gracedb.download(combined_skymap_filename,
-                                           superevent['em_type'])
+                                           superevent['superevent_id'])
     else:
         combined_skymap = None
     alert_dict['external_coinc'] = {
         'gcn_notice_id':
             int(external_event['extra_attributes']['GRB']['trigger_id']),
         'ivorn': external_event['extra_attributes']['GRB']['ivorn'],
         'observatory': external_event['pipeline'],
@@ -132,17 +170,17 @@
 def _upload_notice(self, payload, brokerhost, superevent_id):
     '''
     Upload serialized alert notice to GraceDB
     '''
     config = self.app.conf['kafka_alert_config'][brokerhost]
     kafka_writer = self.app.conf['kafka_streams'][brokerhost]
 
-    # FIXME Drop get_payload_input method once
+    # FIXME Drop get_payload_content method once
     # https://github.com/scimma/hop-client/pull/190 is merged
-    alert_dict = kafka_writer.get_payload_input(payload)
+    alert_dict = kafka_writer.get_payload_content(payload)
     message = 'Kafka alert notice sent to {}'.format(config['url'])
 
     filename = '{}-{}.{}'.format(
         alert_dict['superevent_id'],
         alert_dict['alert_type'].lower(),
         config['suffix']
     )
```

### Comparing `gwcelery-2.0.5/gwcelery/tasks/bayestar.py` & `gwcelery-2.0.6/gwcelery/tasks/bayestar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tasks/circulars.py` & `gwcelery-2.0.6/gwcelery/tasks/circulars.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tasks/condor.py` & `gwcelery-2.0.6/gwcelery/tasks/condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tasks/core.py` & `gwcelery-2.0.6/gwcelery/tasks/core.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tasks/detchar.py` & `gwcelery-2.0.6/gwcelery/tasks/detchar.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,26 +141,29 @@
     except (IndexError, FloatingPointError, ValueError):
         # data from cache can't be properly read, or data is weird
         fig = plt.figure()
         plt.axis("off")
         plt.text(0.1, 0.45, f"Failed to create {ifo} omegascan", fontsize=17)
     else:
         fig = Plot(*qgrams,
-                   figsize=(12 * len(durs), 5),
+                   figsize=(12 * len(durs), 6),
                    geometry=(1, len(durs)),
                    yscale='log',
                    method='pcolormesh',
                    cmap='viridis')
-        for ax in fig.axes:
-            fig.colorbar(ax=ax, label='Normalized energy', clim=(0, 30))
+        for i, ax in enumerate(fig.axes):
+            if i in [1, 2]:
+                ax.set_ylabel('')
+            if i == 2:
+                fig.colorbar(ax=ax, label='Normalized energy', clim=(0, 30))
             ax.set_epoch(t0)
         fig.suptitle(f'Omegascans of {strain_name} at {t0}', fontweight="bold")
-
+    plt.subplots_adjust(wspace=0.08)
     outfile = io.BytesIO()
-    fig.savefig(outfile, format='png', dpi=300)
+    fig.savefig(outfile, format='png', dpi=150, bbox_inches='tight')
     return outfile.getvalue()
 
 
 @app.task(shared=False)
 def omegascan(t0, graceid):
     """Create omegascan for a certain event.
 
@@ -412,15 +415,15 @@
     Returns
     -------
     event : dict
         Details of the event, reflecting any labels that were added.
 
     """
     # Skip early warning events (ie queries for times before now)
-    if start > Time.now().gps:
+    if end > Time.now().gps:
         log.info("Skipping detchar checks because %s is in the future",
                  event['graceid'])
         return event
 
     # Skip MDC events.
     if event.get('search') == 'MDC':
         log.info("Skipping detchar checks because %s is an MDC",
```

### Comparing `gwcelery-2.0.5/gwcelery/tasks/em_bright.py` & `gwcelery-2.0.6/gwcelery/tasks/em_bright.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 """Qualitative source properties for CBC events."""
 import io
 import json
 from matplotlib import pyplot as plt
 
-from ligo.em_bright import em_bright
-
 from celery.utils.log import get_task_logger
 
 from ..import app
 from . import gracedb, igwn_alert
 from .p_astro import _format_prob
 from ..util import closing_figures, NamedTemporaryFile
 
@@ -103,14 +101,15 @@
     Examples
     --------
     >>> em_bright_posterior_samples(GraceDb().files('S190930s',
     ... 'Bilby.posterior_samples.hdf5').read())
     {"HasNS": 0.014904901243599122, "HasRemnant": 0.0, "HasMassGap": 0.0}
 
     """
+    from ligo.em_bright import em_bright
     with NamedTemporaryFile(content=posterior_file_content) as samplefile:
         filename = samplefile.name
         has_ns, has_remnant, has_massgap = em_bright.source_classification_pe(
             filename, num_eos_draws=100, eos_seed=0
         )
     data = json.dumps({
         'HasNS': has_ns,
@@ -146,14 +145,15 @@
         and `HasMassGap`` probabilities
 
     Examples
     --------
     >>> em_bright.source_properties(2.0, 1.0, 0.0, 0.0, 10.)
     '{"HasNS": 1.0, "HasRemnant": 1.0, "HasMassGap"}'
     """
+    from ligo.em_bright import em_bright
     p_ns, p_em, p_mg = em_bright.source_classification(
         mass1, mass2, spin1z, spin2z, snr
     )
 
     data = json.dumps({
         'HasNS': p_ns,
         'HasRemnant': p_em,
```

### Comparing `gwcelery-2.0.5/gwcelery/tasks/external_skymaps.py` & `gwcelery-2.0.6/gwcelery/tasks/external_skymaps.py`

 * *Files 2% similar despite different names*

```diff
@@ -375,15 +375,16 @@
     """
     max_nside = 2048
     if error:
         # Correct 90% containment to 1-sigma for Swift
         if pipeline == 'Swift':
             error /= np.sqrt(-2 * np.log1p(-.9))
         error_radius = error * u.deg
-        nside = pixel_resolution_to_nside(error_radius, round='up')
+        # Use minimum nside of 256
+        nside = max(pixel_resolution_to_nside(error_radius, round='up'), 256)
     else:
         nside = np.inf
     if nside >= max_nside:
         nside = max_nside
 
         #  Find the one pixel the event can localized to
         hpx = HEALPix(nside, 'ring', frame=ICRS())
@@ -549,15 +550,15 @@
         superevent dictionary
     ext_event : dict
         external event dictionary
     var_label : str
         The variable symbol used in plotting
 
     """
-    if coinc_far_dict['skymap_overlap'] is None:
+    if coinc_far_dict.get('skymap_overlap') is None:
         return
     if superevent['em_type'] != ext_event['graceid'] and \
             'RAVEN_ALERT' in superevent['labels']:
         return
 
     superevent_id = superevent['superevent_id']
     ext_id = ext_event['graceid']
```

### Comparing `gwcelery-2.0.5/gwcelery/tasks/external_triggers.py` & `gwcelery-2.0.6/gwcelery/tasks/external_triggers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from lxml import etree
 from urllib.parse import urlparse
 from celery import group
 from celery.utils.log import get_logger
 
 from ..import app
-from .core import identity
 from . import detchar
 from . import gcn
 from . import gracedb
 from . import external_skymaps
 from . import igwn_alert
 from . import raven
 
@@ -190,15 +189,15 @@
         else:
             canvas = gracedb.remove_label.si('NOT_GRB', graceid)
 
         # Prevent SubGRBs from appending GRBs
         if search == 'GRB':
             # Replace event and pass already existing event dictionary
             canvas |= gracedb.replace_event.si(graceid, payload)
-            canvas |= identity.si(event)
+            canvas |= gracedb.get_event.si(graceid)
         else:
             return
 
     else:
         canvas = gracedb.create_event.s(filecontents=payload,
                                         search=search,
                                         group=ext_group,
```

### Comparing `gwcelery-2.0.5/gwcelery/tasks/first2years.py` & `gwcelery-2.0.6/gwcelery/tasks/first2years.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tasks/first2years_external.py` & `gwcelery-2.0.6/gwcelery/tasks/first2years_external.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tasks/gcn.py` & `gwcelery-2.0.6/gwcelery/tasks/gcn.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tasks/gracedb.py` & `gwcelery-2.0.6/gwcelery/tasks/gracedb.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tasks/igwn_alert.py` & `gwcelery-2.0.6/gwcelery/tasks/igwn_alert.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tasks/inference.py` & `gwcelery-2.0.6/gwcelery/tasks/inference.py`

 * *Files 19% similar despite different names*

```diff
@@ -250,16 +250,206 @@
             message='Failed to prepare DAG for lalinference', tags='pe'
         )
         raise
 
     return os.path.join(rundir, 'multidag.dag')
 
 
+def _dump_phenomd_settings(path):
+    settings = {
+        "likelihood_args": {
+            "likelihood_type": "ROQGravitationalWaveTransient",
+            "minimum_frequency": 20,
+            "maximum_frequency": 1024,
+            "roq_scale_factor": 1,
+            "waveform_approximant": "IMRPhenomD",
+        },
+        "likelihood_parameter_bounds": {
+            "mass_ratio_min": 0.125,
+            "a_1_max": 0.05,
+            "a_2_max": 0.05,
+            "spin_template": "aligned",
+        },
+        "trigger_dependent": {
+            "range": {
+                "chirp_mass": [
+                    [0.6, 1.012], [1.012, 1.54], [1.54, 2.31], [2.31, 4.0]
+                ],
+            },
+            "likelihood_args": [
+                {"roq_linear_matrix":
+                    "/home/roq/IMRPhenomD/lowspin_fhigh1024/basis_512s.hdf5",
+                 "roq_quadratic_matrix":
+                    "/home/roq/IMRPhenomD/lowspin_fhigh1024/basis_512s.hdf5",
+                 "duration": 512},
+                {"roq_linear_matrix":
+                    "/home/roq/IMRPhenomD/lowspin_fhigh1024/basis_256s.hdf5",
+                 "roq_quadratic_matrix":
+                    "/home/roq/IMRPhenomD/lowspin_fhigh1024/basis_256s.hdf5",
+                 "duration": 256},
+                {"roq_linear_matrix":
+                    "/home/roq/IMRPhenomD/lowspin_fhigh1024/basis_128s.hdf5",
+                 "roq_quadratic_matrix":
+                    "/home/roq/IMRPhenomD/lowspin_fhigh1024/basis_128s.hdf5",
+                 "duration": 128},
+                {"roq_linear_matrix":
+                    "/home/roq/IMRPhenomD/lowspin_fhigh1024/basis_64s.hdf5",
+                 "roq_quadratic_matrix":
+                    "/home/roq/IMRPhenomD/lowspin_fhigh1024/basis_64s.hdf5",
+                 "duration": 64}
+            ],
+            "likelihood_parameter_bounds": [
+                {"chirp_mass_min": 0.6, "chirp_mass_max": 1.1},
+                {"chirp_mass_min": 0.92, "chirp_mass_max": 1.7},
+                {"chirp_mass_min": 1.4, "chirp_mass_max": 2.6},
+                {"chirp_mass_min": 2.1, "chirp_mass_max": 4.0}
+            ],
+        },
+    }
+    with open(path, 'w') as f:
+        json.dump(settings, f, indent=2)
+
+
+def _dump_high_mass_ratio_pv2_settings(path):
+    settings = {
+        "likelihood_args": {
+            "likelihood_type": "ROQGravitationalWaveTransient",
+            "minimum_frequency": 20,
+            "maximum_frequency": 1024,
+            "roq_scale_factor": 1,
+            "waveform_approximant": "IMRPhenomPv2",
+        },
+        "likelihood_parameter_bounds": {
+            "mass_ratio_min": 0.05,
+            "a_1_max": 0.99,
+            "a_2_max": 0.99,
+            "spin_template": "precessing",
+        },
+        "trigger_dependent": {
+            "range": {
+                "chirp_mass": [[1.4, 2.31], [2.31, 3.63], [3.63, 5.72],
+                               [5.72, 9.57], [9.57, 21]],
+            },
+            "likelihood_args": [
+                {"roq_linear_matrix":
+                    "/home/roq/IMRPhenomPv2/low_mass_ratio/basis_128s.hdf5",
+                 "roq_quadratic_matrix":
+                    "/home/roq/IMRPhenomPv2/low_mass_ratio/basis_128s.hdf5",
+                 "duration": 128},
+                {
+                    "roq_linear_matrix":
+                        "/home/roq/IMRPhenomPv2/low_mass_ratio/basis_64s.hdf5",
+                    "roq_quadratic_matrix":
+                        "/home/roq/IMRPhenomPv2/low_mass_ratio/basis_64s.hdf5",
+                    "duration": 64,
+                },
+                {
+                    "roq_linear_matrix":
+                        "/home/roq/IMRPhenomPv2/low_mass_ratio/basis_32s.hdf5",
+                    "roq_quadratic_matrix":
+                        "/home/roq/IMRPhenomPv2/low_mass_ratio/basis_32s.hdf5",
+                    "duration": 32,
+                },
+                {
+                    "roq_linear_matrix":
+                        "/home/roq/IMRPhenomPv2/low_mass_ratio/basis_16s.hdf5",
+                    "roq_quadratic_matrix":
+                        "/home/roq/IMRPhenomPv2/low_mass_ratio/basis_16s.hdf5",
+                    "duration": 16,
+                },
+                {
+                    "roq_linear_matrix":
+                        "/home/roq/IMRPhenomPv2/low_mass_ratio/basis_8s.hdf5",
+                    "roq_quadratic_matrix":
+                        "/home/roq/IMRPhenomPv2/low_mass_ratio/basis_8s.hdf5",
+                    "duration": 8,
+                },
+            ],
+            "likelihood_parameter_bounds": [
+                {"chirp_mass_min": 1.4, "chirp_mass_max": 2.6},
+                {"chirp_mass_min": 2.1, "chirp_mass_max": 4.0},
+                {"chirp_mass_min": 3.3, "chirp_mass_max": 6.3},
+                {"chirp_mass_min": 5.2, "chirp_mass_max": 11.0},
+                {"chirp_mass_min": 8.7, "chirp_mass_max": 21.0},
+            ],
+        },
+    }
+    with open(path, 'w') as f:
+        json.dump(settings, f, indent=2)
+
+
+def _dump_xphm_settings(path):
+    settings = {
+        "likelihood_args": {
+            "likelihood_type": "ROQGravitationalWaveTransient",
+            "minimum_frequency": 20,
+            "maximum_frequency": 4096,
+            "reference_frequency": 20,
+            "roq_scale_factor": 1,
+            "waveform_approximant": "IMRPhenomXPHM",
+            "waveform_arguments_dict": {"PhenomXHMReleaseVersion": 122019},
+            "phase_marginalization": False,
+        },
+        "likelihood_parameter_bounds": {
+            "mass_ratio_min": 0.05,
+            "a_1_max": 0.99,
+            "a_2_max": 0.99,
+            "spin_template": "precessing",
+        },
+        "trigger_dependent": {
+            "range": {
+                "chirp_mass": [[10.03, 16], [16, 25],
+                               [25, 45], [45, np.inf]],
+            },
+            "likelihood_args": [
+                {
+                    "roq_linear_matrix":
+                        "/home/roq/IMRPhenomXPHM/basis_32s.hdf5",
+                    "roq_quadratic_matrix":
+                        "/home/roq/IMRPhenomXPHM/basis_32s.hdf5",
+                    "duration": 32,
+                },
+                {
+                    "roq_linear_matrix":
+                        "/home/roq/IMRPhenomXPHM/basis_16s.hdf5",
+                    "roq_quadratic_matrix":
+                        "/home/roq/IMRPhenomXPHM/basis_16s.hdf5",
+                    "duration": 16,
+                },
+                {
+                    "roq_linear_matrix":
+                        "/home/roq/IMRPhenomXPHM/basis_8s.hdf5",
+                    "roq_quadratic_matrix":
+                        "/home/roq/IMRPhenomXPHM/basis_8s.hdf5",
+                    "duration": 8,
+                },
+                {
+                    "roq_linear_matrix":
+                        "/home/roq/IMRPhenomXPHM/basis_4s.hdf5",
+                    "roq_quadratic_matrix":
+                        "/home/roq/IMRPhenomXPHM/basis_4s.hdf5",
+                    "duration": 4,
+                },
+            ],
+            "likelihood_parameter_bounds": [
+                {"chirp_mass_min": 10.03, "chirp_mass_max": 19.04},
+                {"chirp_mass_min": 13, "chirp_mass_max": 31.85},
+                {"chirp_mass_min": 20, "chirp_mass_max": 62.86},
+                {"chirp_mass_min": 30, "chirp_mass_max": 200},
+            ],
+        },
+    }
+    with open(path, 'w') as f:
+        json.dump(settings, f, indent=2)
+
+
 @app.task(shared=False)
-def _setup_dag_for_bilby(coinc, rundir, event, superevent_id, mode):
+def _setup_dag_for_bilby(
+    coinc, rundir, event, superevent_id, mode="production"
+):
     """Create DAG for a bilby run and return the path to DAG.
 
     Parameters
     ----------
     coinc : bytes
         Byte contents of ``coinc.xml``. The PSD is expected to be embedded.
     rundir : str
@@ -267,27 +457,28 @@
     event : dict
         The json contents of a target G event retrieved from
         gracedb.get_event(), whose mass and spin information are used to
         determine analysis settings.
     superevent_id : str
         The GraceDB ID of a target superevent
     mode : str
-        Analysis mode
+        Analysis mode, allowed options are "production" and "fast_test",
+        default is "production".
 
     Returns
     -------
     path_to_dag : str
         The path to the .dag file
 
     Notes
     -----
     `--channel-dict o3replay` is added to bilby_pipe_gracedb arguments when the
-    gracedb host is different from `gracedb.ligo.org`. Condor queue is set to
-    `Online_PE` if gracedb host is `gracedb.ligo.org`, and `Online_PE_MDC`
-    otherwise.
+    gracedb host is different from `gracedb.ligo.org` or
+    `gracedb-test.ligo.org`. Condor queue is set to `Online_PE` if gracedb host
+    is `gracedb.ligo.org`, and `Online_PE_MDC` otherwise.
 
     """
     path_to_json = os.path.join(rundir, 'event.json')
     with open(path_to_json, 'w') as f:
         json.dump(event, f, indent=2)
 
     path_to_psd = os.path.join(rundir, 'coinc.xml')
@@ -303,70 +494,94 @@
                  '--outdir', rundir, '--json', path_to_json,
                  '--psd-file', path_to_psd, '--settings', path_to_settings]
     settings = {'summarypages_arguments': {'gracedb': event['graceid'],
                                            'no_ligo_skymap': True},
                 'accounting_user': 'soichiro.morisaki'}
     if app.conf['gracedb_host'] != 'gracedb.ligo.org':
         settings['queue'] = 'Online_PE_MDC'
-        setup_arg += ['--channel-dict', 'o3replay']
     else:
         settings['queue'] = 'Online_PE'
+    # FIXME: using live data for gracedb-test events should be reconsidered
+    # when we have a better idea to differentiate MDC and real events.
+    if app.conf['gracedb_host'] not in [
+        'gracedb.ligo.org', 'gracedb-test.ligo.org'
+    ]:
+        setup_arg += ['--channel-dict', 'o3replay']
 
-    if mode == 'quick_bns':
-        setup_arg += ['--cbc-likelihood-mode', 'lowspin_phenomd_narrowmc_roq']
-        settings.update(
-            {'sampler_kwargs': {'naccept': 10, 'nlive': 500,
-                                'npool': 24, 'sample': 'acceptance-walk'},
-             'n_parallel': 2,
-             'request_cpus': 24,
-             'spline_calibration_nodes': 10,
-             'request_memory_generation': 8.0}
+    trigger_chirp_mass = event['extra_attributes']['CoincInspiral']['mchirp']
+    if trigger_chirp_mass < 0.6:
+        raise ValueError(
+            "No bilby settings available for trigger chirp mass of"
+            f" {trigger_chirp_mass}Msun."
         )
+    if mode == 'production':
+        settings.update(
+            {
+                'sampler_kwargs': {'naccept': 60, 'nlive': 500,
+                                   'npool': 24, 'sample': 'acceptance-walk'},
+                'n_parallel': 2,
+                'request_cpus': 24,
+                'spline_calibration_nodes': 10,
+                'request_memory_generation': 8.0
+            }
+        )
+        # use low-spin IMRPhenomD below chirp mass of m1=3Msun, m2=1Msun
+        # assuming binary neutron star
+        if trigger_chirp_mass < 1.465:
+            likelihood_mode = os.path.join(rundir, "likelihood_mode.json")
+            _dump_phenomd_settings(likelihood_mode)
+            settings['sampler_kwargs']['naccept'] = 10
+        # use IMRPhenomPv2 with mass ratio upper bound of 8 below chirp mass of
+        # m1=8Msun, m2=1Msun
+        elif trigger_chirp_mass < 2.243:
+            likelihood_mode = 'phenompv2_bns_roq'
+        # use IMRPhenomPv2 with mass ratio upper bound of 20 in chirp-mass
+        # range where IMRPhenomXPHM ROQ bases are not available
+        elif trigger_chirp_mass < 12:
+            likelihood_mode = os.path.join(rundir, "likelihood_mode.json")
+            _dump_high_mass_ratio_pv2_settings(likelihood_mode)
+        else:
+            likelihood_mode = os.path.join(rundir, "likelihood_mode.json")
+            _dump_xphm_settings(likelihood_mode)
+            settings['request_memory_generation'] = 16.0
+        setup_arg += ['--cbc-likelihood-mode', likelihood_mode]
     elif mode == 'fast_test':
-        # use pv2_nrtidalv2 below chirp mass of m1=3Msun, m2=1Msun
-        if event['extra_attributes']['CoincInspiral']['mchirp'] < 1.465:
-            setup_arg += ['--cbc-likelihood-mode', 'phenompv2nrtidalv2_roq']
-            settings['request_memory_generation'] = 8.0
-        # use bns-mass pv2 basis for chirp mass range where it is available
-        elif event['extra_attributes']['CoincInspiral']['mchirp'] < 3.9:
+        setup_arg += ["--sampler-kwargs", "FastTest"]
+        if trigger_chirp_mass < 3.9:
             setup_arg += ['--cbc-likelihood-mode', 'phenompv2_bns_roq']
             settings['request_memory_generation'] = 8.0
-        settings.update(
-            {'sampler_kwargs': {'naccept': 60, 'nlive': 500,
-                                'npool': 24, 'sample': 'acceptance-walk'},
-             'n_parallel': 2,
-             'request_cpus': 24,
-             'spline_calibration_nodes': 10}
-        )
-    elif mode != 'production':
+    else:
         raise ValueError(f"mode: {mode} not recognized.")
 
     with open(path_to_settings, 'w') as f:
         json.dump(settings, f, indent=2)
 
     try:
         subprocess.run(setup_arg, capture_output=True, check=True)
     except subprocess.CalledProcessError as e:
         contents = b'args:\n' + json.dumps(e.args[1]).encode('utf-8') + \
                    b'\n\nstdout:\n' + e.stdout + b'\n\nstderr:\n' + e.stderr
         gracedb.upload.delay(
             filecontents=contents, filename='bilby_dag.log',
             graceid=superevent_id,
-            message=f'Failed to prepare DAG for {mode} bilby', tags='pe'
+            message=f'Failed to prepare DAG for {mode}-mode bilby', tags='pe'
         )
         raise
     else:
         # Uploads bilby ini file to GraceDB
         with open(os.path.join(rundir, 'bilby_config.ini'), 'r') as f:
             ini_contents = f.read()
+        if mode == 'production':
+            filename = 'bilby_config.ini'
+        else:
+            filename = f'bilby_{mode}_config.ini'
         gracedb.upload.delay(
-            ini_contents, filename=f'bilby_{mode}_config.ini',
-            graceid=superevent_id,
-            message=(f'Automatically generated {mode} Bilby configuration file'
-                     ' for this event.'),
+            ini_contents, filename=filename, graceid=superevent_id,
+            message=(f'Automatically generated {mode}-mode Bilby configuration'
+                     ' file for this event.'),
             tags='pe')
 
     path_to_dag, = glob.glob(os.path.join(rundir, 'submit/dag*.submit'))
     return path_to_dag
 
 
 @app.task(shared=False)
@@ -673,25 +888,28 @@
     -------
     tasks : canvas
         The work-flow for uploading Bilby results
 
     """
     # convert bilby sample file into one compatible with ligo-skymap
     samples_dir = os.path.join(rundir, 'final_result')
-    samples_filename = f'Bilby.{mode}.posterior_samples.hdf5'
+    if mode == 'production':
+        samples_filename = 'Bilby.posterior_samples.hdf5'
+    else:
+        samples_filename = f'Bilby.{mode}.posterior_samples.hdf5'
     out_samples = os.path.join(samples_dir, samples_filename)
     in_samples, = glob.glob(os.path.join(samples_dir, '*result.hdf5'))
     subprocess.run(
         ['bilby_pipe_to_ligo_skymap_samples', in_samples, '--out', out_samples]
     )
 
     with open(out_samples, 'rb') as f:
         canvas = gracedb.upload.si(
             f.read(), samples_filename,
-            superevent_id, f'{mode} Bilby posterior samples', 'pe')
+            superevent_id, f'{mode}-mode Bilby posterior samples', 'pe')
 
     # pesummary
     pesummary_kwargs = {}
     path_to_ini, = glob.glob(os.path.join(rundir, "*_complete.ini"))
     pesummary_kwargs["config"] = path_to_ini
     config_parser = BilbyConfigFileParser()
     with open(path_to_ini, "r") as f:
@@ -716,15 +934,15 @@
     )
     canvas = group(
         canvas,
         _pesummary_task(webdir, in_samples, **pesummary_kwargs)
         |
         gracedb.upload.si(
             None, None, superevent_id,
-            'PESummary page for {mode} Bilby is available '
+            'PESummary page for {mode}-mode Bilby is available '
             f'<a href={url}>here</a>'
         )
     )
 
     return canvas
 
 
@@ -774,35 +992,49 @@
     **pesummary_kwargs
         Extra arguments of summarypages
 
     Returns
     -------
     celery task
 
+    Notes
+    -----
+    `--disable_interactive --disable_expert` are added and `--redshift_method
+    exact --evolve_spins_forwards` are not added to `summarypages` arguments
+    when the gracedb host is different from `gracedb.ligo.org`. Condor queue is
+    set to `Online_PE` if gracedb host is `gracedb.ligo.org`, and
+    `Online_PE_MDC` otherwise.
+
     """
     args = [
-        "summarypages", "--webdir", webdir, "--samples", samples,
-        "--gw", "--redshift_method", "exact", "--evolve_spins_fowards"
+        "summarypages", "--webdir", webdir, "--samples", samples, "--gw",
+        "--no_ligo_skymap", "--multi_process", "6"
     ]
     for key in pesummary_kwargs:
         if key in ["psd", "calibration"]:
             args += [f"--{key}"]
             for ifo in pesummary_kwargs[key]:
                 args += [f'{ifo}:{pesummary_kwargs[key][ifo]}']
         else:
             args += [f"--{key}", pesummary_kwargs[key]]
+    condor_kwargs = dict(
+        request_memory=16000, request_disk=5000, request_cpus=6,
+        accounting_group_user='soichiro.morisaki'
+    )
     if app.conf['gracedb_host'] != 'gracedb.ligo.org':
-        queue = 'Online_PE_MDC'
+        condor_kwargs['accounting_group'] = 'ligo.dev.o4.cbc.pe.bilby'
+        condor_kwargs['requirements'] = '((TARGET.Online_PE_MDC =?= True))'
+        condor_kwargs['+Online_PE_MDC'] = True
+        args += ["--disable_interactive", "--disable_expert"]
     else:
-        queue = 'Online_PE'
-    return condor.check_output.si(
-        args, request_memory=16000, request_disk=5000, queue=queue,
-        accounting_group="ligo.dev.o4.cbc.pe.bilby",
-        accounting_group_user="soichiro.morisaki",
-    )
+        condor_kwargs['accounting_group'] = 'ligo.prod.o4.cbc.pe.bilby'
+        condor_kwargs['requirements'] = '((TARGET.Online_PE =?= True))'
+        condor_kwargs['+Online_PE'] = True
+        args += ["--redshift_method", "exact", "--evolve_spins_forwards"]
+    return condor.check_output.si(args, **condor_kwargs)
 
 
 @app.task(ignore_result=True, shared=False)
 def start_pe(frametype_dict, event, superevent_id, pe_pipeline):
     """Run Parameter Estimation on a given event.
 
     Parameters
@@ -823,21 +1055,18 @@
     # make an event directory
     pipeline_dir = os.path.expanduser('~/.cache/{}'.format(pe_pipeline))
     mkpath(pipeline_dir)
     event_dir = os.path.join(pipeline_dir, superevent_id)
     os.mkdir(event_dir)
 
     if pe_pipeline == 'bilby':
-        modes = [app.conf['bilby_default_mode']]
-        # add quick-bns mode if chirp mass is lower than that of 3Msun-3Msun
-        if event['extra_attributes']['CoincInspiral']['mchirp'] < 2.62:
-            modes += ['quick_bns']
+        modes = ["production"]
         rundirs = [os.path.join(event_dir, m) for m in modes]
         kwargs_list = [{'bilby_mode': m} for m in modes]
-        analyses = [f'{m} bilby' for m in modes]
+        analyses = [f'{m}-mode bilby' for m in modes]
     else:
         rundirs = [event_dir]
         kwargs_list = [{}]
         analyses = [pe_pipeline]
 
     for rundir, kwargs, analysis in zip(rundirs, kwargs_list, analyses):
         mkpath(rundir)
```

### Comparing `gwcelery-2.0.5/gwcelery/tasks/legacy_gracedb.py` & `gwcelery-2.0.6/gwcelery/tasks/legacy_gracedb.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     504 (Gateway Timeout).
     """
     @functools.wraps(f)
     def wrapper(*args, **kwargs):
         try:
             return f(*args, **kwargs)
         except rest.HTTPError as e:
-            if e.status in {429, 502, 503, 504}:
+            if e.status in {408, 409, 429, 502, 503, 504}:
                 raise RetryableHTTPError(e.status, e.reason, e.message)
             else:
                 raise
 
     return wrapper
```

### Comparing `gwcelery-2.0.5/gwcelery/tasks/notice_text.py` & `gwcelery-2.0.6/gwcelery/tasks/notice_text.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tasks/orchestrator.py` & `gwcelery-2.0.6/gwcelery/tasks/orchestrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from . import em_bright
 from . import external_skymaps
 from . import gcn
 from . import gracedb
 from . import inference
 from . import igwn_alert
 from . import p_astro
+from . import rrt_utils
 from . import skymaps
 from . import superevents
 
 from ligo.rrt_chat import channel_creation
 
 
 @igwn_alert.handler('superevent',
@@ -1081,14 +1082,19 @@
     # For kafka alerts the analogous field is set in alerts.py.
     # (see comment before defining kafka_alert_canvas)
     voevent_significance = 0 if alert_type == 'less-significant' else 1
 
     if filecontents and not combined_skymap_filename:
         skymap, em_bright, p_astro = filecontents
 
+        # check high profile and apply label if true
+        high_profile_canvas = rrt_utils.check_high_profile.si(
+            skymap, em_bright, p_astro, superevent
+        )
+
         download_andor_expose_group = []
 
         voevent_canvas = _create_voevent.si(
             (em_bright, p_astro),
             superevent_id,
             alert_type_voevent,
             Significant=voevent_significance,
@@ -1110,14 +1116,15 @@
         )
     else:
         # Download em_bright and p_astro files here for voevent
         download_andor_expose_group = [
             gracedb.download.si(em_bright_filename, superevent_id),
             gracedb.download.si(p_astro_filename, superevent_id),
         ]
+        high_profile_canvas = identity.si()
 
         voevent_canvas = _create_voevent.s(
             superevent_id,
             alert_type_voevent,
             Significant=voevent_significance,
             skymap_filename=skymap_filename,
             internal=False,
@@ -1160,29 +1167,29 @@
 
     sent_label_canvas = identity.si()
     if alert_type == 'less-significant':
         sent_label_canvas = gracedb.create_label.si(
             'LOW_SIGNIF_PRELIM_SENT',
             superevent_id
         )
-    elif alert_type == 'preliminary' or \
-            alert_type == 'earlywarning':
+    elif alert_type == 'preliminary':
         sent_label_canvas = gracedb.create_label.si(
             'GCN_PRELIM_SENT',
             superevent_id
         )
 
     canvas = (
         group(download_andor_expose_group)
         |
         group(voevent_canvas, kafka_alert_canvas)
         |
         group(
             sent_label_canvas,
             circular_canvas,
+            high_profile_canvas
         )
     )
 
     canvas.apply_async()
 
 
 @gracedb.task(ignore_result=True, shared=False)
```

### Comparing `gwcelery-2.0.5/gwcelery/tasks/p_astro.py` & `gwcelery-2.0.6/gwcelery/tasks/p_astro.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tasks/raven.py` & `gwcelery-2.0.6/gwcelery/tasks/raven.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,18 +217,18 @@
             superevent = alert_object
             ext_event = result
         else:
             superevent_id = result['superevent_id']
             exttrig_id = gracedb_id
             superevent = result
             ext_event = alert_object
-            # Don't continue if it is a different superevent than previous one.
-            if ext_event['superevent'] is not None \
-                    and ext_event['superevent'] != superevent['superevent_id']:
-                return
+        # Don't continue if it is a different superevent than previous one.
+        if ext_event['superevent'] is not None \
+                and ext_event['superevent'] != superevent['superevent_id']:
+            return
 
         canvas = (
             gracedb.add_event_to_superevent.si(superevent_id, exttrig_id)
             |
             calculate_coincidence_far.si(superevent, ext_event, tl, th)
             |
             update_coinc_far.s(superevent, ext_event)
@@ -432,14 +432,16 @@
             not is_test_event and no_previous_alert:
         messages.append(('RAVEN: publishing criteria met for {0}-{1}. '
                          'Triggering RAVEN alert'.format(
                              preferred_gwevent_id, ext_id)))
         (
             gracedb.create_label.si('RAVEN_ALERT', superevent_id)
             |
+            gracedb.create_label.si('HIGH_PROFILE', superevent_id)
+            |
             gracedb.create_label.si('RAVEN_ALERT', ext_id)
             |
             gracedb.create_label.si('RAVEN_ALERT', preferred_gwevent_id)
         ).delay()
     if not pass_far_threshold:
         messages.append(('RAVEN: publishing criteria not met for {0}-{1},'
                          ' {2} FAR (w/ trials) too large '
```

### Comparing `gwcelery-2.0.5/gwcelery/tasks/skymaps.py` & `gwcelery-2.0.6/gwcelery/tasks/skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tasks/superevents.py` & `gwcelery-2.0.6/gwcelery/tasks/superevents.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/templates/fits_header.jinja2` & `gwcelery-2.0.6/gwcelery/templates/fits_header.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/templates/index.jinja2` & `gwcelery-2.0.6/gwcelery/templates/index.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/templates/lalinference.jinja2` & `gwcelery-2.0.6/gwcelery/templates/lalinference.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/templates/rapidpe.jinja2` & `gwcelery-2.0.6/gwcelery/templates/rapidpe.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/templates/vector_table.jinja2` & `gwcelery-2.0.6/gwcelery/templates/vector_table.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/conftest.py` & `gwcelery-2.0.6/gwcelery/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/G000012_S0040_preferred.json` & `gwcelery-2.0.6/gwcelery/tests/data/G000012_S0040_preferred.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/G298048-1-Initial.xml` & `gwcelery-2.0.6/gwcelery/tests/data/G298048-1-Initial.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/G298048_log.json` & `gwcelery-2.0.6/gwcelery/tests/data/G298048_log.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json` & `gwcelery-2.0.6/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/MS220722v.xml` & `gwcelery-2.0.6/gwcelery/tests/data/MS220722v.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits` & `gwcelery-2.0.6/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/S230413b.json` & `gwcelery-2.0.6/gwcelery/tests/data/S230413b.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/S230413g.json` & `gwcelery-2.0.6/gwcelery/tests/data/S230413g.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/S230413h.json` & `gwcelery-2.0.6/gwcelery/tests/data/S230413h.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/T0212_S0039_preferred.json` & `gwcelery-2.0.6/gwcelery/tests/data/T0212_S0039_preferred.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json` & `gwcelery-2.0.6/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/T0219_S0041_nopreferred.json` & `gwcelery-2.0.6/gwcelery/tests/data/T0219_S0041_nopreferred.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/agile_grb_gcn.xml` & `gwcelery-2.0.6/gwcelery/tests/data/agile_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/coinc.xml` & `gwcelery-2.0.6/gwcelery/tests/data/coinc.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/externaltrigger_original_data.xml` & `gwcelery-2.0.6/gwcelery/tests/data/externaltrigger_original_data.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/fermi_grb_gcn.xml` & `gwcelery-2.0.6/gwcelery/tests/data/fermi_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/fermi_initial_grb_gcn.xml` & `gwcelery-2.0.6/gwcelery/tests/data/fermi_initial_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/fermi_noise_gcn.xml` & `gwcelery-2.0.6/gwcelery/tests/data/fermi_noise_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/fermi_noise_gcn_2.xml` & `gwcelery-2.0.6/gwcelery/tests/data/fermi_noise_gcn_2.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml` & `gwcelery-2.0.6/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml` & `gwcelery-2.0.6/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/fits_header_result.html` & `gwcelery-2.0.6/gwcelery/tests/data/fits_header_result.html`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/gracedb_externaltrigger_log.json` & `gwcelery-2.0.6/gwcelery/tests/data/gracedb_externaltrigger_log.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_detchar.json` & `gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_detchar.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_exttrig_creation.json` & `gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_exttrig_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json` & `gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_psd.json` & `gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_psd.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_snews_creation.json` & `gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_snews_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_snews_test_creation.json` & `gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_snews_test_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_subgrb_creation.json` & `gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_subgrb_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_superevent_creation.json` & `gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_superevent_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/igwn_alert_voevent.json` & `gwcelery-2.0.6/gwcelery/tests/data/igwn_alert_voevent.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/integral_grb_gcn.xml` & `gwcelery-2.0.6/gwcelery/tests/data/integral_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/integral_mdc_gcn.xml` & `gwcelery-2.0.6/gwcelery/tests/data/integral_mdc_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf` & `gwcelery-2.0.6/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/llhoft/omegascan/scanme.gwf` & `gwcelery-2.0.6/gwcelery/tests/data/llhoft/omegascan/scanme.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf` & `gwcelery-2.0.6/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/lvalert_event_creation.json` & `gwcelery-2.0.6/gwcelery/tests/data/lvalert_event_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/lvalert_xmpp.xml` & `gwcelery-2.0.6/gwcelery/tests/data/lvalert_xmpp.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/mock_superevent_object.json` & `gwcelery-2.0.6/gwcelery/tests/data/mock_superevent_object.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite` & `gwcelery-2.0.6/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/psd.xml.gz` & `gwcelery-2.0.6/gwcelery/tests/data/psd.xml.gz`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/sample_events.json` & `gwcelery-2.0.6/gwcelery/tests/data/sample_events.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/samples.hdf5` & `gwcelery-2.0.6/gwcelery/tests/data/samples.hdf5`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/scaler_set_all.pickle` & `gwcelery-2.0.6/gwcelery/tests/data/scaler_set_all.pickle`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/snews_gcn.xml` & `gwcelery-2.0.6/gwcelery/tests/data/snews_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/snews_gcn_test.xml` & `gwcelery-2.0.6/gwcelery/tests/data/snews_gcn_test.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/superevents.json` & `gwcelery-2.0.6/gwcelery/tests/data/superevents.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/swift_grb_gcn.xml` & `gwcelery-2.0.6/gwcelery/tests/data/swift_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/data/test_classifier.pickle` & `gwcelery-2.0.6/gwcelery/tests/data/test_classifier.pickle`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/process.py` & `gwcelery-2.0.6/gwcelery/tests/process.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_sentry.py` & `gwcelery-2.0.6/gwcelery/tests/test_sentry.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_tasks_alerts.py` & `gwcelery-2.0.6/gwcelery/tests/test_tasks_alerts.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_tasks_alerts_validate.py` & `gwcelery-2.0.6/gwcelery/tests/test_tasks_alerts_validate.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_tasks_bayestar.py` & `gwcelery-2.0.6/gwcelery/tests/test_tasks_bayestar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_tasks_circulars.py` & `gwcelery-2.0.6/gwcelery/tests/test_tasks_circulars.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_tasks_condor.py` & `gwcelery-2.0.6/gwcelery/tests/test_tasks_condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_tasks_detchar.py` & `gwcelery-2.0.6/gwcelery/tests/test_tasks_detchar.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,27 +72,27 @@
 
 @patch('gwcelery.tasks.detchar.create_cache', return_value=[expected_path])
 def test_make_omegascan_worked(mock_create_cache, scan_strainname):
     durs = [(1, 1), (1, 1), (1, 1)]
     t0 = 1126259463
     png = detchar.make_omegascan('H1', t0, durs)
     pngarray = plt.imread(BytesIO(png))
-    # Test to see that the png is taller than 1400 pixels, indicating
+    # Test to see that the png is wider than 2000 pixels, indicating
     # presence of omegascan(s)
-    assert plt.imshow(pngarray).get_extent()[2] > 1400
+    assert plt.imshow(pngarray).get_extent()[1] > 850
 
 
 @patch('gwcelery.tasks.detchar.create_cache', return_value=[])
 def test_make_omegascan_failed(mock_create_cache, scan_strainname):
     durs = [(1, 1), (1, 1), (1, 1)]
     t0 = 1126259463
     png = detchar.make_omegascan('H1', t0, durs)
     pngarray = plt.imread(BytesIO(png))
-    # Test to see that the png is shorter than 1500 pixels
-    assert plt.imshow(pngarray).get_extent()[2] < 1500
+    # Test to see that the png is narrower than 2000 pixels
+    assert plt.imshow(pngarray).get_extent()[1] < 2000
 
 
 @patch('gwcelery.tasks.detchar.make_omegascan.run',
        return_value=BytesIO().getvalue())
 @patch('gwcelery.tasks.gracedb.upload.run')
 def test_omegascan(mock_upload, mock_fig):
     t0 = 1126259463
```

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_tasks_em_bright.py` & `gwcelery-2.0.6/gwcelery/tests/test_tasks_em_bright.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
         'em_bright.json',
         'TS123456'
     )
     mock_plot.assert_called_once_with('mock_em_bright')
     mock_upload.assert_called_once()
 
 
-def test_classifier():
+def test_classifier(socket_enabled):
     res = json.loads(em_bright.source_properties(
         1.355607, 1.279483, 0.0, 0.0, 15.6178))
     assert res['HasNS'] == pytest.approx(1.0, abs=1e-3)
     assert res['HasRemnant'] == pytest.approx(1.0, abs=1e-3)
     assert res['HasMassGap'] == pytest.approx(0.0, abs=1e-3)
 
 
@@ -43,15 +43,15 @@
         [[[(1.2, 1.0, 0.0, 0.0, 100.0, 0.0, 0.0),
            (2.0, 0.5, 0.99, 0.99, 150.0, 0.0, 0.0)],
           {'HasNS': 1.0, 'HasRemnant': 0.5, 'HasMassGap': 0.5}],
          [[(20., 12.0, 0.0, 0.0, 200.0, 0.0, 0.0),
            (22.0, 11.5, 0.80, 0.00, 250.0, 0.0, 0.0),
            (21.0, 10.0, 0.0, 0.0, 250, 0.0, 0.0)],
           {'HasNS': 0.0, 'HasRemnant': 0.0, 'HasMassGap': 0.0}]])
-def test_posterior_samples(posterior_samples, embright):
+def test_posterior_samples(posterior_samples, embright, socket_enabled):
     with NamedTemporaryFile() as f:
         filename = f.name
         with h5py.File(f, 'r+') as tmp_h5:
             data = np.array(
                     posterior_samples,
                     dtype=[('chirp_mass', '<f8'), ('mass_ratio', '<f8'),
                            ('a_1', '<f8'), ('a_2', '<f8'),
```

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_tasks_external_skymaps.py` & `gwcelery-2.0.6/gwcelery/tests/test_tasks_external_skymaps.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,21 +292,22 @@
 
 @pytest.mark.parametrize(
     'em_type,graceid,labels,expected_result',
     [[None, 'E1', [], True],
      ['E1', 'E1', [], True],
      ['E1', 'E2', [], True],
      ['E1', 'E1', ['RAVEN_ALERT'], True],
-     ['E1', 'E2', ['RAVEN_ALERT'], False]]
+     ['E1', 'E2', ['RAVEN_ALERT'], False],
+     [None, 'E3', [], False]]
 )
 @patch('gwcelery.tasks.gracedb.upload.run')
 def test_plot_overlap_integral(mock_upload,
                                em_type, graceid, labels, expected_result):
 
-    coinc_far_dict = {'skymap_overlap': 1e2}
+    coinc_far_dict = {'skymap_overlap': 1e2} if graceid != 'E3' else {}
     superevent = {'superevent_id': 'S1', 'em_type': em_type, 'labels': labels}
     ext_event = {'graceid': graceid}
     external_skymaps.plot_overlap_integral(coinc_far_dict, superevent,
                                            ext_event)
     if expected_result:
         mock_upload.assert_called_once()
     else:
```

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_tasks_external_triggers.py` & `gwcelery-2.0.6/gwcelery/tests/test_tasks_external_triggers.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,21 +205,28 @@
                           'fermi_noise_gcn.xml',
                           'fermi_subthresh_grb_gcn.xml'])
 @patch('gwcelery.tasks.external_skymaps.create_upload_external_skymap.run')
 @patch('gwcelery.tasks.external_skymaps.get_upload_external_skymap.run')
 @patch('gwcelery.tasks.gracedb.create_label.run')
 @patch('gwcelery.tasks.gracedb.remove_label.run')
 @patch('gwcelery.tasks.gracedb.replace_event.run')
-@patch('gwcelery.tasks.gracedb.get_events', return_value=[{
+@patch('gwcelery.tasks.gracedb.get_event.run', return_value=[{
     'graceid': 'E1', 'gpstime': 1, 'instruments': '', 'pipeline': 'Fermi',
     'search': 'GRB',
     'extra_attributes': {'GRB': {'trigger_duration': 1, 'trigger_id': 123,
                                  'ra': 0., 'dec': 0., 'error_radius': 10.}},
     'links': {'self': 'https://gracedb.ligo.org/events/E356793/'}}])
-def test_handle_replace_grb_event(mock_get_events,
+@patch('gwcelery.tasks.gracedb.get_events', return_value=[{
+    'graceid': 'E1', 'gpstime': 1, 'instruments': '', 'pipeline': 'Fermi',
+    'search': 'GRB',
+    'extra_attributes': {'GRB': {'trigger_duration': 1, 'trigger_id': 123,
+                                 'ra': 0., 'dec': 0., 'error_radius': 15.}},
+    'links': {'self': 'https://gracedb.ligo.org/events/E356793/'}}])
+def test_handle_replace_grb_event(mock_get_event,
+                                  mock_get_events,
                                   mock_replace_event, mock_remove_label,
                                   mock_create_label,
                                   mock_get_upload_external_skymap,
                                   mock_create_upload_external_skymap,
                                   filename):
     text = resources.read_binary(data, filename)
     external_triggers.handle_grb_gcn(payload=text)
```

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_tasks_first2years.py` & `gwcelery-2.0.6/gwcelery/tests/test_tasks_first2years.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_tasks_first2years_external.py` & `gwcelery-2.0.6/gwcelery/tests/test_tasks_first2years_external.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_tasks_gcn.py` & `gwcelery-2.0.6/gwcelery/tests/test_tasks_gcn.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_tasks_gcn_validate.py` & `gwcelery-2.0.6/gwcelery/tests/test_tasks_gcn_validate.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_tasks_gracedb.py` & `gwcelery-2.0.6/gwcelery/tests/test_tasks_gracedb.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_tasks_igwn_alert.py` & `gwcelery-2.0.6/gwcelery/tests/test_tasks_igwn_alert.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_tasks_inference.py` & `gwcelery-2.0.6/gwcelery/tests/test_tasks_inference.py`

 * *Files 6% similar despite different names*

```diff
@@ -174,16 +174,16 @@
     upload.assert_called_once()
 
 
 @pytest.mark.parametrize(
     "host,mode,mc",
     product(
         ['gracedb-playground.ligo.org', 'gracedb.ligo.org'],
-        ['fast_test', 'quick_bns', 'production'],
-        [10, 3, 1]
+        ['production', 'fast_test'],
+        [30, 10, 3, 2, 1, 0.1]
     )
 )
 def test_setup_dag_for_bilby(monkeypatch, tmp_path, host, mode, mc):
     psd = b'psd'
     rundir = str(tmp_path)
     event = {'gpstime': 1187008882, 'graceid': 'G1234',
              'extra_attributes': {'CoincInspiral': {'mchirp': mc}}}
@@ -207,43 +207,53 @@
             assert event == json.load(f)
 
         path_to_psd = cmd[8]
         assert os.path.exists(path_to_psd)
         with open(path_to_psd, 'rb') as f:
             assert f.read() == psd
 
+        if mode == "fast_test":
+            assert "FastTest" in cmd
+
         path_to_settings = cmd[10]
         assert os.path.exists(path_to_settings)
         ans = {
             'summarypages_arguments': {'gracedb': event['graceid'],
                                        'no_ligo_skymap': True},
             'queue': 'Online_PE',
             'accounting_user': 'soichiro.morisaki'
         }
         if host != 'gracedb.ligo.org':
             ans['queue'] = 'Online_PE_MDC'
-        if mode == 'quick_bns':
+        if mode == 'production':
             ans.update(
-                {'sampler_kwargs': {'naccept': 10, 'nlive': 500,
+                {'sampler_kwargs': {'naccept': 60, 'nlive': 500,
                                     'npool': 24, 'sample': 'acceptance-walk'},
                  'n_parallel': 2,
                  'request_cpus': 24,
                  'spline_calibration_nodes': 10,
                  'request_memory_generation': 8.0}
             )
-        elif mode == 'fast_test':
-            if mc < 3.9:
-                ans['request_memory_generation'] = 8.0
-            ans.update(
-                {'sampler_kwargs': {'naccept': 60, 'nlive': 500,
-                                    'npool': 24, 'sample': 'acceptance-walk'},
-                 'n_parallel': 2,
-                 'request_cpus': 24,
-                 'spline_calibration_nodes': 10}
-            )
+            if 1.465 < mc < 2.243:
+                assert 'phenompv2_bns_roq' in cmd
+            else:
+                path_to_mode = cmd[cmd.index("--cbc-likelihood-mode") + 1]
+                assert os.path.exists(path_to_mode)
+                with open(path_to_mode, 'r') as f:
+                    w = json.load(f)["likelihood_args"]["waveform_approximant"]
+                if 0.6 < mc < 1.465:
+                    assert w == "IMRPhenomD"
+                    ans['sampler_kwargs']['naccept'] = 10
+                elif mc < 11.033:
+                    assert w == "IMRPhenomPv2"
+                else:
+                    assert w == "IMRPhenomXPHM"
+                    ans['request_memory_generation'] = 16.0
+        elif mode == 'fast_test' and mc < 3.9:
+            ans['request_memory_generation'] = 8.0
         with open(path_to_settings, 'r') as f:
             assert json.load(f) == ans
 
         with open(os.path.join(rundir, 'bilby_config.ini'), 'w') as f:
             f.write(ini)
         dir = os.path.join(rundir, 'submit')
         os.mkdir(dir)
@@ -253,27 +263,35 @@
     def _upload(filecontents, filename, graceid, message, tags):
         assert filecontents == ini
 
     upload = Mock(side_effect=_upload)
     monkeypatch.setattr('subprocess.run', _subprocess_run)
     monkeypatch.setattr('gwcelery.tasks.gracedb.upload.run', upload)
 
-    path_to_dag = inference._setup_dag_for_bilby(psd, rundir, event, sid, mode)
+    if mc < 0.6:
+        with pytest.raises(ValueError):
+            inference._setup_dag_for_bilby(psd, rundir, event, sid, mode)
+    else:
+        path_to_dag = inference._setup_dag_for_bilby(
+            psd, rundir, event, sid, mode
+        )
 
-    assert os.path.exists(path_to_dag)
-    with open(path_to_dag, 'r') as f:
-        assert f.read() == dag
-    upload.assert_called_once()
+        assert os.path.exists(path_to_dag)
+        with open(path_to_dag, 'r') as f:
+            assert f.read() == dag
+        upload.assert_called_once()
 
 
 def test_setup_dag_for_bilby_unknown_mode(tmp_path):
     with pytest.raises(ValueError):
         inference._setup_dag_for_bilby(
             b'psd', str(tmp_path),
-            {'gpstime': 1187008882, 'graceid': 'G1234'}, 'S1234', 'unknown'
+            {'gpstime': 1187008882, 'graceid': 'G1234',
+             'extra_attributes': {'CoincInspiral': {'mchirp': 1}}},
+            'S1234', 'unknown'
         )
 
 
 def test_setup_dag_for_rapidpe(monkeypatch, tmp_path):
     rundir = str(tmp_path)
     dag_filename = 'event_all_iterations.dag'
     dag_content = 'rapidpe dag'
@@ -306,15 +324,16 @@
         Mock(return_value='./cal_file.txt'))
 
     rundir = str(tmp_path)
     event = {
         'gpstime': 1187008882,
         'graceid': 'G1234',
         'extra_attributes': {'SingleInspiral':
-                             [{'mass1': 1.4, 'mass2': 1.4, 'mchirp': 1.2}]}
+                             [{'mass1': 1.4, 'mass2': 1.4, 'mchirp': 1.2}],
+                             'CoincInspiral': {'mchirp': 1}}
     }
     with pytest.raises(subprocess.CalledProcessError):
         if pipeline == 'lalinference':
             inference._setup_dag_for_lalinference(
                 b'coinc', rundir, event, 'S1234', {})
         elif pipeline == 'bilby':
             inference._setup_dag_for_bilby(
@@ -405,16 +424,23 @@
 
     inference.job_error_notification(
         None, exc, 'test', 'S1234', str(tmp_path), 'lalinference')
     assert upload.call_count == len(filenames) + 1
 
 
 @pytest.mark.parametrize(
-    'pipeline', ['lalinference', 'bilby', 'rapidpe', 'my_awesome_pipeline'])
-def test_dag_finished(monkeypatch, tmp_path, pipeline):
+    'pipeline,host',
+    product(
+        ['lalinference', 'bilby_production', 'bilby_fast_test', 'rapidpe',
+         'my_awesome_pipeline'],
+        ['gracedb-playground.ligo.org', 'gracedb.ligo.org']
+    )
+)
+def test_dag_finished(monkeypatch, tmp_path, pipeline, host):
+    monkeypatch.setitem(app.conf, 'gracedb_host', host)
     sid = 'S1234'
     rundir = str(tmp_path / 'rundir')
     resultdir = str(tmp_path / 'rundir/result')
     sampledir = str(tmp_path / 'rundir/final_result')
     pe_results_path = str(tmp_path / 'public_html/online_pe')
     monkeypatch.setitem(app.conf, 'pe_results_path', pe_results_path)
     pe_results_path = os.path.join(pe_results_path, sid, pipeline)
@@ -425,77 +451,88 @@
 
     upload = Mock()
     create_label = Mock()
     monkeypatch.setattr('gwcelery.tasks.gracedb.upload.run', upload)
     monkeypatch.setattr('gwcelery.tasks.gracedb.create_label.run',
                         create_label)
 
-    if pipeline in ['lalinference', 'bilby', 'rapidpe']:
+    if pipeline in [
+        'lalinference', 'bilby_production', 'bilby_fast_test', 'rapidpe'
+    ]:
         kwargs = {}
         if pipeline == 'lalinference':
             paths = [os.path.join(rundir,
                                   'lalinference_1187008756-1187008882.dag'),
                      os.path.join(rundir, 'glitch_median_PSD_forLI_H1.dat'),
                      os.path.join(rundir, 'glitch_median_PSD_forLI_L1.dat'),
                      os.path.join(rundir, 'glitch_median_PSD_forLI_V1.dat'),
                      os.path.join(rundir, 'posterior_samples.hdf5'),
                      os.path.join(pe_results_path, 'extrinsic.png'),
                      os.path.join(pe_results_path, 'intrinsic.png'),
                      os.path.join(pe_results_path, 'posplots.html')]
-        elif pipeline == 'bilby':
+        elif pipeline in ['bilby_production', 'bilby_fast_test']:
+            kwargs['bilby_mode'] = pipeline[6:]
+            pipeline = 'bilby'
+
             input_sample = os.path.join(sampledir, "test_result.hdf5")
             with open(input_sample, 'wb') as f:
                 f.write(b'result')
 
+            samplename = f'Bilby.{kwargs["bilby_mode"]}.posterior_samples.hdf5'
+            if kwargs["bilby_mode"] == "production":
+                samplename = 'Bilby.posterior_samples.hdf5'
+            paths = [os.path.join(sampledir, samplename)]
+
             def _subprocess_run(cmd):
                 assert os.path.exists(cmd[1])
+                assert cmd[3] == paths[0]
 
             monkeypatch.setattr(
                 'subprocess.run', Mock(side_effect=_subprocess_run))
 
-            kwargs['bilby_mode'] = 'production'
-            paths = [os.path.join(sampledir,
-                                  'Bilby.production.posterior_samples.hdf5')]
-
             path_to_bilby_config = os.path.join(rundir, "bilby_complete.ini")
             with open(path_to_bilby_config, "w") as f:
                 f.write(
                     "spline-calibration-envelope-dict="
                     "{'H1': 'H1_cal.txt', 'L1': 'L1_cal.txt'}\n"
                     "psd-dict={'H1': 'H1_psd.txt', 'L1': 'L1_psd.txt'}\n"
                     "waveform-approximant=IMRPhenomPv2\n"
                     "minimum-frequency=20\n"
                     "reference-frequency=100\n"
                     "webdir=webdir"
                 )
 
             def mock_check_output(args, **kwargs):
-                assert args == [
+                ans = [
                     "summarypages", "--webdir", "webdir/pesummary",
                     "--samples", os.path.join(sampledir, 'test_result.hdf5'),
-                    "--gw", "--redshift_method", "exact",
-                    "--evolve_spins_fowards",
-                    "--config", path_to_bilby_config,
-                    "--psd", "H1:H1_psd.txt", "L1:L1_psd.txt",
-                    "--calibration", "H1:H1_cal.txt", "L1:L1_cal.txt",
-                    "--approximant", "IMRPhenomPv2",
+                    "--gw", "--no_ligo_skymap", "--multi_process", "6",
+                    "--config", path_to_bilby_config, "--psd", "H1:H1_psd.txt",
+                    "L1:L1_psd.txt", "--calibration", "H1:H1_cal.txt",
+                    "L1:L1_cal.txt", "--approximant", "IMRPhenomPv2",
                     "--f_low", "20", "--f_ref", "100"
                 ]
+                if host != 'gracedb.ligo.org':
+                    ans += ["--disable_interactive", "--disable_expert"]
+                else:
+                    ans += [
+                        "--redshift_method", "exact", "--evolve_spins_forwards"
+                    ]
+                assert args == ans
 
             monkeypatch.setattr(
                 'gwcelery.tasks.condor.check_output.run', mock_check_output)
 
         else:
             paths = []
         for path in paths:
             with open(path, 'wb') as f:
                 f.write(b'result')
 
-        inference.dag_finished(
-            rundir, sid, pipeline, bilby_mode='production')
+        inference.dag_finished(rundir, sid, pipeline, **kwargs)
 
         if pipeline == 'rapidpe':
             upload.assert_called_once()
         elif pipeline == 'bilby':
             # +1 corresponds to pesummary link
             assert upload.call_count == len(paths) + 1
         else:
@@ -507,15 +544,17 @@
             create_label.assert_not_called()
 
     else:
         with pytest.raises(NotImplementedError):
             inference.dag_finished(rundir, sid, pipeline)
 
 
-def test_start_pe(monkeypatch, tmp_path):
+@pytest.mark.parametrize(
+    'pipeline', ['lalinference', 'bilby', 'rapidpe'])
+def test_start_pe(monkeypatch, tmp_path, pipeline):
     path_to_sub = 'pe.dag.condor.sub'
 
     @app.task
     def mock_task():
         return path_to_sub
 
     dag_prepare_task = Mock(return_value=mock_task.s())
@@ -530,55 +569,11 @@
                         Mock(return_value=str(tmp_path)))
     monkeypatch.setattr('gwcelery.tasks.inference.dag_prepare_task',
                         dag_prepare_task)
     monkeypatch.setattr('gwcelery.tasks.condor.submit.run', condor_submit)
     monkeypatch.setattr('gwcelery.tasks.inference.dag_finished.run',
                         dag_finished)
 
-    inference.start_pe({}, {'graceid': 'G1234'}, 'S1234', 'lalinference')
+    inference.start_pe({}, {'graceid': 'G1234'}, 'S1234', pipeline)
     dag_prepare_task.assert_called_once()
     condor_submit.assert_called_once()
     dag_finished.assert_called_once()
-
-
-def test_start_pe_multiple_bilby(monkeypatch, tmp_path):
-    path_to_sub = 'pe.dag.condor.sub'
-
-    def mock_dag_prepare_task(
-        rundir, event, superevent_id, pe_pipeline, frametype_dict=None,
-        **kwargs
-    ):
-        assert 'bilby_mode' in kwargs
-
-        @app.task
-        def mock_task():
-            return path_to_sub
-
-        return mock_task.s()
-
-    def mock_condor_submit(path):
-        assert path == path_to_sub
-
-    def mock_dag_finished(rundir, superevent_id, pe_pipeline, **kwargs):
-        assert 'bilby_mode' in kwargs
-
-    dag_prepare_task = Mock(side_effect=mock_dag_prepare_task)
-    condor_submit = Mock(side_effect=mock_condor_submit)
-    dag_finished = Mock(side_effect=mock_dag_finished)
-
-    monkeypatch.setattr('gwcelery.tasks.gracedb.upload.run', Mock())
-    monkeypatch.setattr('distutils.dir_util.mkpath',
-                        Mock(return_value=str(tmp_path)))
-    monkeypatch.setattr('gwcelery.tasks.inference.dag_prepare_task',
-                        dag_prepare_task)
-    monkeypatch.setattr('gwcelery.tasks.condor.submit.run', condor_submit)
-    monkeypatch.setattr('gwcelery.tasks.inference.dag_finished.run',
-                        dag_finished)
-
-    event = {
-        'graceid': 'G1234',
-        'extra_attributes': {'CoincInspiral': {'mchirp': 1}}
-    }
-    inference.start_pe({}, event, 'S1234', 'bilby')
-    assert dag_prepare_task.call_count == 2
-    assert condor_submit.call_count == 2
-    assert dag_finished.call_count == 2
```

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_tasks_orchestrator.py` & `gwcelery-2.0.6/gwcelery/tests/test_tasks_orchestrator.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,17 @@
      ['label_added', 'LOW_SIGNIF_LOCKED', 'CBC', 'gstlal', False, 1.e-10,
          ['H1', 'L1', 'V1'], 'S1234', ['EARLY_WARNING']],
      ['label_added', 'LOW_SIGNIF_PRELIM_SENT', 'CBC', 'gstlal', False, 1.e-9,
          ['H1', 'L1', 'V1'], 'S1234', ['EM_SelectedConfident']],
      ['label_added', 'LOW_SIGNIF_PRELIM_SENT', 'CBC', 'gstlal', False, 1.e-7,
          ['H1', 'L1', 'V1'], 'S1234', ['EM_Selected']],
      ['new', '', 'CBC', 'gstlal', False, 1.e-9, ['H1', 'L1'], 'S1234',
-         ['LOW_SIGNIF_LOCKED']]])
+         ['LOW_SIGNIF_LOCKED']],
+     ['label_added', 'EARLY_WARNING', 'CBC', 'gstlal', False, 1.e-10,
+         ['H1', 'L1', 'V1'], 'S1234', []]])
 def test_handle_superevent(monkeypatch, toy_3d_fits_filecontents,  # noqa: F811
                            alert_type, alert_label, group, pipeline,
                            offline, far, instruments, superevent_id,
                            superevent_labels):
     """Test a superevent is dispatched to the correct annotation task based on
     its preferred event's search group.
     """
@@ -137,14 +139,15 @@
     else:
         raven_coinc = True
 
     create_initial_circular = Mock()
     create_emcoinc_circular = Mock()
     expose = Mock()
     rrt_channel_creation = Mock()
+    check_high_profile = Mock()
     annotate_fits = Mock(return_value=None)
     # FIXME: remove logic of mocking return value
     # when live worker testing is enabled
     proceed_if_not_blocked_by = Mock(return_value=None) if \
         alert_label == 'LOW_SIGNIF_PRELIM_SENT' and \
         'EM_SelectedConfident' in superevent_labels else \
         Mock(return_value=(('skymap', 'skymap-filename'),
@@ -225,14 +228,16 @@
         select_pipeline_preferred_event_task
     )
     monkeypatch.setattr('gwcelery.tasks.detchar.omegascan.run', omegascan)
     monkeypatch.setattr('gwcelery.tasks.detchar.check_vectors.run',
                         check_vectors)
     monkeypatch.setattr('gwcelery.tasks.orchestrator.channel_creation.'
                         'rrt_channel_creation', rrt_channel_creation)
+    monkeypatch.setattr('gwcelery.tasks.rrt_utils.check_high_profile.run',
+                        check_high_profile)
     monkeypatch.setattr(app.conf, 'create_mattermost_channel', True)
     # Run function under test
     orchestrator.handle_superevent(alert)
 
     if alert_label == 'GCN_PRELIM_SENT':
         dqr_request_label = list(
             filter(
@@ -266,65 +271,77 @@
         #     create_voevent.assert_called_once_with(
         #         'S1234', 'preliminary', BBH=0.02, BNS=0.94, NSBH=0.03,
         #         ProbHasNS=0.0, ProbHasRemnant=0.0, Terrestrial=0.01,
         #         internal=False, open_alert=True,
         #         skymap_filename='bayestar.fits.gz', skymap_type='bayestar')
         gcn_send.assert_called_once()
         alerts_send.assert_called_once()
+        check_high_profile.assert_called_once()
+        assert call(
+            'GCN_PRELIM_SENT', superevent_id) in create_label.call_args_list
+
         if raven_coinc:
             create_emcoinc_circular.assert_called_once()
         else:
             create_initial_circular.assert_called_once()
 
     elif alert_label == 'EARLY_WARNING':
         if 'SIGNIF_LOCKED' in superevent_labels:
             expose.assert_not_called()
             alerts_send.assert_not_called()
             gcn_send.assert_not_called()
             create_tag.assert_not_called()
             create_initial_circular.assert_not_called()
+            check_high_profile.assert_not_called()
         else:
             annotate_fits.assert_called_once()
             update_superevent_task.assert_called_once_with(
                 'S1234', preferred_event='G1234'
             )
             expose.assert_called_once_with('S1234')
             create_tag.assert_has_calls(
                 [call('S1234-1-Preliminary.xml', 'public', 'S1234'),
                  call('em-bright-filename', 'public', 'S1234'),
                  call('p-astro-filename', 'public', 'S1234'),
                  call('skymap-filename', 'public', 'S1234')],
                 any_order=True
             )
+            assert call('GCN_PRELIM_SENT', superevent_id) \
+                not in create_label.call_args_list
+
     elif alert_label == 'LOW_SIGNIF_LOCKED':
         if ('SIGNIF_LOCKED' in superevent_labels) or \
                 ('EARLY_WARNING' in superevent_labels):
             expose.assert_not_called()
             alerts_send.assert_not_called()
             gcn_send.assert_not_called()
             create_tag.assert_not_called()
             create_initial_circular.assert_not_called()
+            check_high_profile.assert_not_called()
         else:
             annotate_fits.assert_called_once()
             # no superevent clean up needed
             update_superevent_task.assert_not_called()
             # no circular creation for less-significant alerts
             create_initial_circular.assert_not_called()
             create_emcoinc_circular.assert_not_called()
+            assert call('LOW_SIGNIF_PRELIM_SENT', superevent_id) \
+                in create_label.call_args_list
     elif alert_label == 'ADVREQ':
         rrt_channel_creation.assert_called_once_with(
             superevent_id,
             app.conf['gracedb_host'])
     elif alert_label == 'LOW_SIGNIF_PRELIM_SENT':
         if 'EM_SelectedConfident' in superevent_labels:
             expose.assert_not_called()
             alerts_send.assert_not_called()
             gcn_send.assert_not_called()
             create_tag.assert_not_called()
             create_initial_circular.assert_not_called()
+            check_high_profile.assert_not_called()
         else:
             # check alert type is less-significant
             _files, _superevent, _alert_type = alerts_send.call_args.args
             assert _alert_type == 'less-significant'
 
     if alert_type == 'new' and group == 'CBC':
         query_data.assert_called_once()
```

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_tasks_p_astro.py` & `gwcelery-2.0.6/gwcelery/tests/test_tasks_p_astro.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_tasks_raven.py` & `gwcelery-2.0.6/gwcelery/tests/test_tasks_raven.py`

 * *Files 0% similar despite different names*

```diff
@@ -280,14 +280,16 @@
             result['space_coinc_far'] = None
             result['overlap_integral'] = None
     else:
         alert_object['superevent_id'] = graceid
         alert_object['time_coinc_far'] = 1e-5
         alert_object['space_coinc_far'] = None
         alert_object['overlap_integral'] = None
+        for result in raven_search_results:
+            result['superevent'] = None
     raven.raven_pipeline(raven_search_results, graceid, alert_object, tl, th,
                          group)
 
     coinc_calls = []
     label_calls = []
     update_calls = []
     plot_calls = []
@@ -619,14 +621,15 @@
     ext_event = _mock_get_event(ext_id)
     preferred_id = superevent['preferred_event']
     raven.trigger_raven_alert(coinc_far_json, superevent,
                               graceid, ext_event, group)
 
     if expected_result:
         label_calls = [call('RAVEN_ALERT', superevent_id),
+                       call('HIGH_PROFILE', superevent_id),
                        call('RAVEN_ALERT', ext_id),
                        call('RAVEN_ALERT', preferred_id)]
         mock_create_label.assert_has_calls(label_calls)
     else:
         mock_create_label.assert_not_called()
```

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_tasks_skymaps.py` & `gwcelery-2.0.6/gwcelery/tests/test_tasks_skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_tasks_superevents.py` & `gwcelery-2.0.6/gwcelery/tests/test_tasks_superevents.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_tempfile.py` & `gwcelery-2.0.6/gwcelery/tests/test_tempfile.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_tools_condor.py` & `gwcelery-2.0.6/gwcelery/tests/test_tools_condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_tools_condor_submit_helper.py` & `gwcelery-2.0.6/gwcelery/tests/test_tools_condor_submit_helper.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_tools_flask.py` & `gwcelery-2.0.6/gwcelery/tests/test_tools_flask.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_tools_nagios.py` & `gwcelery-2.0.6/gwcelery/tests/test_tools_nagios.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,24 +32,33 @@
 
 def test_nagios(capsys, monkeypatch, request, socket_enabled, starter,
                 tmp_path):
     mock_igwn_alert_client = Mock()
     mock_hop_stream_object = Mock()
     mock_hop_stream_object.configure_mock(**{'close.return_value': None})
     mock_hop_stream = Mock(return_value=mock_hop_stream_object)
+    mock_get_auth = Mock()
     mock_list_topics = Mock()
     unix_socket = str(tmp_path / 'redis.sock')
     broker_url = f'redis+socket://{unix_socket}'
 
     monkeypatch.setattr('hop.io.Stream.open', mock_hop_stream)
     monkeypatch.setattr('igwn_alert.client', mock_igwn_alert_client)
+    monkeypatch.setattr('gwcelery.kafka.bootsteps.KafkaBase.get_auth',
+                        mock_get_auth)
     monkeypatch.setattr('gwcelery.kafka.bootsteps.list_topics',
                         mock_list_topics)
     monkeypatch.setitem(app.conf, 'broker_url', broker_url)
     monkeypatch.setitem(app.conf, 'result_backend', broker_url)
+    monkeypatch.setitem(app.conf, 'kafka_consumer_config', {
+        'swift': {
+            'url': 'kafka://kafka.gcn.nasa.gov/swift.bat.guano',
+            'suffix': 'json'
+        }
+    })
 
     # no broker
 
     with pytest.raises(SystemExit) as excinfo:
         main(['gwcelery', 'nagios'])
     assert excinfo.value.code == nagios.NagiosPluginStatus.CRITICAL
     out, err = capsys.readouterr()
@@ -185,14 +194,39 @@
                                    'igwn-alert-topics':
                                    expected_igwn_alert_topics,
                                    'kafka_topic_up':
                                    {'kafka://kafka.scimma.org/gwalert-test':
                                     True},
                                    'kafka_delivery_failures':
                                    {'kafka://kafka.scimma.org/gwalert-test':
-                                    False}}}))  # noqa: E501
+                                    False},
+                                   'active_kafka_consumers': set()}}))
+
+    with pytest.raises(SystemExit) as excinfo:
+        main(['gwcelery', 'nagios'])
+    assert excinfo.value.code == nagios.NagiosPluginStatus.CRITICAL
+    out, err = capsys.readouterr()
+    assert 'CRITICAL: Not all Kafka consumer bootstep topics are active' \
+           in out
+
+    expected_kafka_consumer_topics = \
+        nagios.get_expected_kafka_consumer_bootstep_names(app)
+    monkeypatch.setattr(
+        'celery.app.control.Inspect.stats',
+        Mock(return_value={'foo': {'voevent-broker-peers': ['127.0.0.1'],
+                                   'voevent-receiver-peers': ['127.0.0.1'],
+                                   'igwn-alert-topics':
+                                   expected_igwn_alert_topics,
+                                   'kafka_topic_up':
+                                   {'kafka://kafka.scimma.org/gwalert-test':
+                                    True},
+                                   'kafka_delivery_failures':
+                                   {'kafka://kafka.scimma.org/gwalert-test':
+                                    False},
+                                   'active_kafka_consumers':
+                                   expected_kafka_consumer_topics}}))
 
     with pytest.raises(SystemExit) as excinfo:
         main(['gwcelery', 'nagios'])
     assert excinfo.value.code == nagios.NagiosPluginStatus.OK
     out, err = capsys.readouterr()
     assert 'OK: Running normally' in out
```

### Comparing `gwcelery-2.0.5/gwcelery/tests/test_views.py` & `gwcelery-2.0.6/gwcelery/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tools/condor.py` & `gwcelery-2.0.6/gwcelery/tools/condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tools/condor_submit_helper.py` & `gwcelery-2.0.6/gwcelery/tools/condor_submit_helper.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tools/flask.py` & `gwcelery-2.0.6/gwcelery/tools/flask.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/tools/nagios.py` & `gwcelery-2.0.6/gwcelery/tools/nagios.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,14 +79,27 @@
     stats = inspector.stats()
     undelievered_messages = \
         {kafka_url for stat in stats.values() for kafka_url, active_flag in
          stat.get('kafka_delivery_failures', {}).items() if active_flag}
     return undelievered_messages
 
 
+def get_active_kafka_consumer_bootstep_names(inspector):
+    stats = inspector.stats()
+    active_kafka_consumer_urls = {consumer for stat in stats.values() for
+                                  consumer in stat.get(
+                                      'active_kafka_consumers', ()
+                                  )}
+    return active_kafka_consumer_urls
+
+
+def get_expected_kafka_consumer_bootstep_names(app):
+    return {name for name in app.conf['kafka_consumer_config'].keys()}
+
+
 def get_celery_queue_length(app):
     return app.backend.client.llen("celery")
 
 
 def check_status(app):
     connection = app.connection()
     try:
@@ -144,14 +157,22 @@
 
     celery_queue_length = get_celery_queue_length(app)
     if celery_queue_length > 50:
         raise NagiosCriticalError(
             'Tasks are piled up in Celery queue') from AssertionError(
                 'Length of celery queue is {}'.format(celery_queue_length))
 
+    active = get_active_kafka_consumer_bootstep_names(inspector)
+    expected = get_expected_kafka_consumer_bootstep_names(app)
+    missing = expected - active
+    if missing:
+        raise NagiosCriticalError('Not all Kafka consumer bootstep topics are '
+                                  'active') \
+            from AssertionError('Missing urls: ' + ', '.join(missing))
+
 
 @click.command(help=__doc__)
 @click.pass_context
 def nagios(ctx):
     try:
         check_status(ctx.obj.app)
     except NagiosCriticalError as e:
```

### Comparing `gwcelery-2.0.5/gwcelery/util/cmdline.py` & `gwcelery-2.0.6/gwcelery/util/cmdline.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/util/resources.py` & `gwcelery-2.0.6/gwcelery/util/resources.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/util/tempfile.py` & `gwcelery-2.0.6/gwcelery/util/tempfile.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/views.py` & `gwcelery-2.0.6/gwcelery/views.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/voevent/bootsteps.py` & `gwcelery-2.0.6/gwcelery/voevent/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/voevent/logging.py` & `gwcelery-2.0.6/gwcelery/voevent/logging.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/voevent/signals.py` & `gwcelery-2.0.6/gwcelery/voevent/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/voevent/subscriber.py` & `gwcelery-2.0.6/gwcelery/voevent/subscriber.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/gwcelery/voevent/util.py` & `gwcelery-2.0.6/gwcelery/voevent/util.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.0.5/pyproject.toml` & `gwcelery-2.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gwcelery"
-version = "2.0.5"
+version = "2.0.6"
 description = "Low-latency pipeline for annotating IGWN events"
 readme = "README.rst"
 authors = [
     "Deep Chatterjee <deep.chatterjee@ligo.org>",
     "Cody Messick <cody.messick@ligo.org>",
     "Geoffrey Mo <geoffrey.mo@ligo.org>",
     "Leo Singer <leo.singer@ligo.org>"
@@ -74,25 +74,26 @@
 importlib-metadata = { version = "*"}
 jinja2 = ">=2.11.2"  # https://github.com/pallets/jinja/issues/1168
 lalsuite = ">=6.82"  # https://git.ligo.org/lscsoft/lalsuite/-/issues/414
 ligo-followup-advocate = ">=1.2.1"
 ligo-gracedb = ">=2.7.5"  # https://git.ligo.org/lscsoft/gracedb-client/-/issues/28
 ligo-raven = ">=3.1"
 ligo-segments = "*"
-"ligo.em-bright" = ">=1.1.1"  # https://git.ligo.org/emfollow/em-properties/em-bright/-/issues/23
+"ligo.em-bright" = ">=1.1.2"  # https://git.ligo.org/computing/sccb/-/issues/1166
 "ligo.skymap" = ">=1.0.4"  # https://git.ligo.org/lscsoft/ligo.skymap/-/merge_requests/299
 lscsoft-glue = "*"
 lxml = "*"
 matplotlib = "<3.7"  # Matplotlib changed an axes behaviour which breaks some of our plotting scripts. When gwpy has a new release, we can unpin this.
 numba = ">=0.56"  # Poetry update chooses an old version of numba and its deps that break the python3.9 and 3.10 build tests if this is not specified; dependence on numba comes from rift. Version chosen because it adds python 3.10 support. This requirement can be dropped here if RIFT adds it https://git.ligo.org/rapidpe-rift/rift/-/issues/24
 numpy = "*"
 p_astro = ">=1.0.1"  # https://git.ligo.org/lscsoft/p-astro/-/merge_requests/40
-pesummary = "*"
+pesummary = ">=1.0.0"  # https://git.ligo.org/computing/sccb/-/issues/1182
 pygcn = ">=1.0.1"
 python-ligo-lw = "^1.8.3"
+pyxdg = "*"
 rapid-pe = ">=0.0.6"  # https://git.ligo.org/computing/sccb/-/issues/1154
 rapidpe-rift-pipe = ">=0.0.12"  # https://git.ligo.org/computing/sccb/-/issues/1155
 redis = "!=4.5.2,!=4.5.3"  # https://git.ligo.org/emfollow/gwcelery/-/issues/556
 RIFT = ">=0.0.15.7"
 scipy = "<1.10"  # https://github.com/astropy/astropy/issues/14230
 safe-netrc = "*"
 sentry-sdk = {version = "*", extras = ["flask", "tornado"]}
```

### Comparing `gwcelery-2.0.5/PKG-INFO` & `gwcelery-2.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwcelery
-Version: 2.0.5
+Version: 2.0.6
 Summary: Low-latency pipeline for annotating IGWN events
 Home-page: https://git.ligo.org/emfollow/gwcelery
 License: GPL-2.0+
 Author: Deep Chatterjee
 Author-email: deep.chatterjee@ligo.org
 Requires-Python: >=3.9,<3.11
 Classifier: Development Status :: 4 - Beta
@@ -49,30 +49,31 @@
 Requires-Dist: jinja2 (>=2.11.2)
 Requires-Dist: lalsuite (>=6.82)
 Requires-Dist: ligo-followup-advocate (>=1.2.1)
 Requires-Dist: ligo-gracedb (>=2.7.5)
 Requires-Dist: ligo-raven (>=3.1)
 Requires-Dist: ligo-rrt-chat (>=0.1.1)
 Requires-Dist: ligo-segments
-Requires-Dist: ligo.em-bright (>=1.1.1)
+Requires-Dist: ligo.em-bright (>=1.1.2)
 Requires-Dist: ligo.skymap (>=1.0.4)
 Requires-Dist: lscsoft-glue
 Requires-Dist: lxml
 Requires-Dist: matplotlib (<3.7)
 Requires-Dist: numba (>=0.56)
 Requires-Dist: numpy
 Requires-Dist: p_astro (>=1.0.1)
 Requires-Dist: pep517 ; extra == "doc"
-Requires-Dist: pesummary
+Requires-Dist: pesummary (>=1.0.0)
 Requires-Dist: pygcn (>=1.0.1)
 Requires-Dist: pytest-celery ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: pytest-flask ; extra == "test"
 Requires-Dist: pytest-socket ; extra == "test"
 Requires-Dist: python-ligo-lw (>=1.8.3,<2.0.0)
+Requires-Dist: pyxdg
 Requires-Dist: rapid-pe (>=0.0.6)
 Requires-Dist: rapidpe-rift-pipe (>=0.0.12)
 Requires-Dist: redis (!=4.5.2,!=4.5.3)
 Requires-Dist: safe-netrc
 Requires-Dist: scipy (<1.10)
 Requires-Dist: sentry-sdk[flask,tornado]
 Requires-Dist: service-identity
```

