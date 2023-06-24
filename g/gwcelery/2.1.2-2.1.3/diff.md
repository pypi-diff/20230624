# Comparing `tmp/gwcelery-2.1.2.tar.gz` & `tmp/gwcelery-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwcelery-2.1.2.tar", max compression
+gzip compressed data, was "gwcelery-2.1.3.tar", max compression
```

## Comparing `gwcelery-2.1.2.tar` & `gwcelery-2.1.3.tar`

### file list

```diff
@@ -1,233 +1,239 @@
--rw-r--r--   0        0        0    96823 2023-06-09 18:39:41.376572 gwcelery-2.1.2/CHANGES.rst
--rw-r--r--   0        0        0       64 2023-06-09 18:39:41.376572 gwcelery-2.1.2/CONTRIBUTING.rst
--rw-r--r--   0        0        0    19716 2023-06-09 18:39:41.377572 gwcelery-2.1.2/LICENSE.rst
--rw-r--r--   0        0        0     1351 2023-06-09 18:39:41.377572 gwcelery-2.1.2/README.rst
--rw-r--r--   0        0        0      634 2023-06-09 18:39:41.377572 gwcelery-2.1.2/doc/Makefile
--rw-r--r--   0        0        0   191486 2023-06-09 18:39:41.379572 gwcelery-2.1.2/doc/_static/acceptance-tests-checklist.png
--rw-r--r--   0        0        0   241593 2023-06-09 18:39:41.380572 gwcelery-2.1.2/doc/_static/celeryevent-screenshot.png
--rw-r--r--   0        0        0   206465 2023-06-09 18:39:41.382572 gwcelery-2.1.2/doc/_static/deployment-screenshot.png
--rw-r--r--   0        0        0   161306 2023-06-09 18:39:41.383572 gwcelery-2.1.2/doc/_static/flask-screenshot.png
--rw-r--r--   0        0        0   328056 2023-06-09 18:39:41.386572 gwcelery-2.1.2/doc/_static/flower-screenshot.png
--rw-r--r--   0        0        0   114719 2023-06-09 18:39:41.387572 gwcelery-2.1.2/doc/_static/logo-0.5x.png
--rw-r--r--   0        0        0   351955 2023-06-09 18:39:41.390572 gwcelery-2.1.2/doc/_static/logo.png
--rw-r--r--   0        0        0   230777 2023-06-09 18:39:41.392572 gwcelery-2.1.2/doc/_static/sentry-screenshot.png
--rwxr-xr-x   0        0        0     7356 2023-06-09 18:39:41.392572 gwcelery-2.1.2/doc/conf.py
--rw-r--r--   0        0        0     4346 2023-06-09 18:39:41.392572 gwcelery-2.1.2/doc/configuration.rst
--rw-r--r--   0        0        0     5698 2023-06-09 18:39:41.392572 gwcelery-2.1.2/doc/contributing.rst
--rw-r--r--   0        0        0     7202 2023-06-09 18:39:41.392572 gwcelery-2.1.2/doc/deployment.rst
--rw-r--r--   0        0        0    10176 2023-06-09 18:39:41.392572 gwcelery-2.1.2/doc/design.rst
--rw-r--r--   0        0        0      486 2023-06-09 18:39:41.392572 gwcelery-2.1.2/doc/gwcelery.conf.rst
--rw-r--r--   0        0        0      284 2023-06-09 18:39:41.393572 gwcelery-2.1.2/doc/gwcelery.email.rst
--rw-r--r--   0        0        0      329 2023-06-09 18:39:41.393572 gwcelery-2.1.2/doc/gwcelery.igwn_alert.rst
--rw-r--r--   0        0        0      227 2023-06-09 18:39:41.393572 gwcelery-2.1.2/doc/gwcelery.rst
--rw-r--r--   0        0        0       79 2023-06-09 18:39:41.393572 gwcelery-2.1.2/doc/gwcelery.sentry.rst
--rw-r--r--   0        0        0       97 2023-06-09 18:39:41.393572 gwcelery-2.1.2/doc/gwcelery.tasks.alerts.rst
--rw-r--r--   0        0        0      103 2023-06-09 18:39:41.393572 gwcelery-2.1.2/doc/gwcelery.tasks.bayestar.rst
--rw-r--r--   0        0        0      107 2023-06-09 18:39:41.393572 gwcelery-2.1.2/doc/gwcelery.tasks.circulars.rst
--rw-r--r--   0        0        0       98 2023-06-09 18:39:41.393572 gwcelery-2.1.2/doc/gwcelery.tasks.condor.rst
--rw-r--r--   0        0        0     2404 2023-06-09 18:39:41.393572 gwcelery-2.1.2/doc/gwcelery.tasks.detchar.rst
--rw-r--r--   0        0        0     1110 2023-06-09 18:39:41.393572 gwcelery-2.1.2/doc/gwcelery.tasks.em_bright.rst
--rw-r--r--   0        0        0      129 2023-06-09 18:39:41.393572 gwcelery-2.1.2/doc/gwcelery.tasks.external_skymaps.rst
--rw-r--r--   0        0        0     6738 2023-06-09 18:39:41.393572 gwcelery-2.1.2/doc/gwcelery.tasks.external_triggers.rst
--rw-r--r--   0        0        0      112 2023-06-09 18:39:41.393572 gwcelery-2.1.2/doc/gwcelery.tasks.first2years.rst
--rw-r--r--   0        0        0       88 2023-06-09 18:39:41.394572 gwcelery-2.1.2/doc/gwcelery.tasks.gcn.rst
--rw-r--r--   0        0        0      100 2023-06-09 18:39:41.394572 gwcelery-2.1.2/doc/gwcelery.tasks.gracedb.rst
--rw-r--r--   0        0        0      109 2023-06-09 18:39:41.394572 gwcelery-2.1.2/doc/gwcelery.tasks.igwn_alert.rst
--rw-r--r--   0        0        0      109 2023-06-09 18:39:41.394572 gwcelery-2.1.2/doc/gwcelery.tasks.inference.rst
--rw-r--r--   0        0        0     8111 2023-06-09 18:39:41.394572 gwcelery-2.1.2/doc/gwcelery.tasks.orchestrator.rst
--rw-r--r--   0        0        0      100 2023-06-09 18:39:41.394572 gwcelery-2.1.2/doc/gwcelery.tasks.p_astro.rst
--rw-r--r--   0        0        0       94 2023-06-09 18:39:41.394572 gwcelery-2.1.2/doc/gwcelery.tasks.raven.rst
--rw-r--r--   0        0        0      628 2023-06-09 18:39:41.394572 gwcelery-2.1.2/doc/gwcelery.tasks.rst
--rw-r--r--   0        0        0      100 2023-06-09 18:39:41.394572 gwcelery-2.1.2/doc/gwcelery.tasks.skymaps.rst
--rw-r--r--   0        0        0     7161 2023-06-09 18:39:41.394572 gwcelery-2.1.2/doc/gwcelery.tasks.superevents.rst
--rw-r--r--   0        0        0       97 2023-06-09 18:39:41.394572 gwcelery-2.1.2/doc/gwcelery.tools.condor.rst
--rw-r--r--   0        0        0       94 2023-06-09 18:39:41.394572 gwcelery-2.1.2/doc/gwcelery.tools.flask.rst
--rw-r--r--   0        0        0       97 2023-06-09 18:39:41.395572 gwcelery-2.1.2/doc/gwcelery.tools.nagios.rst
--rw-r--r--   0        0        0      185 2023-06-09 18:39:41.395572 gwcelery-2.1.2/doc/gwcelery.tools.rst
--rw-r--r--   0        0        0       73 2023-06-09 18:39:41.395572 gwcelery-2.1.2/doc/gwcelery.util.rst
--rw-r--r--   0        0        0      507 2023-06-09 18:39:41.395572 gwcelery-2.1.2/doc/gwcelery.voevent.rst
--rw-r--r--   0        0        0     3564 2023-06-09 18:39:41.395572 gwcelery-2.1.2/doc/htcondor.rst
--rw-r--r--   0        0        0     1576 2023-06-09 18:39:41.395572 gwcelery-2.1.2/doc/index.rst
--rw-r--r--   0        0        0      800 2023-06-09 18:39:41.395572 gwcelery-2.1.2/doc/make.bat
--rw-r--r--   0        0        0     4416 2023-06-09 18:39:41.395572 gwcelery-2.1.2/doc/monitoring.rst
--rw-r--r--   0        0        0     5312 2023-06-09 18:39:41.395572 gwcelery-2.1.2/doc/quickstart.rst
--rw-r--r--   0        0        0     1149 2023-06-09 18:39:41.395572 gwcelery-2.1.2/gwcelery/__init__.py
--rw-r--r--   0        0        0    18447 2023-06-09 18:39:41.396572 gwcelery-2.1.2/gwcelery/_version.py
--rw-r--r--   0        0        0    16230 2023-06-09 18:39:41.396572 gwcelery-2.1.2/gwcelery/conf/__init__.py
--rw-r--r--   0        0        0     1014 2023-06-09 18:39:41.396572 gwcelery-2.1.2/gwcelery/conf/dev.py
--rw-r--r--   0        0        0      403 2023-06-09 18:39:41.396572 gwcelery-2.1.2/gwcelery/conf/development.py
--rw-r--r--   0        0        0     1289 2023-06-09 18:39:41.396572 gwcelery-2.1.2/gwcelery/conf/minikube.py
--rw-r--r--   0        0        0     1865 2023-06-09 18:39:41.396572 gwcelery-2.1.2/gwcelery/conf/playground.py
--rw-r--r--   0        0        0     3541 2023-06-09 18:39:41.396572 gwcelery-2.1.2/gwcelery/conf/production.py
--rw-r--r--   0        0        0     2040 2023-06-09 18:39:41.397572 gwcelery-2.1.2/gwcelery/conf/test.py
--rw-r--r--   0        0        0        0 2023-06-09 18:39:41.477573 gwcelery-2.1.2/gwcelery/data/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 18:39:41.478573 gwcelery-2.1.2/gwcelery/data/first2years/__init__.py
--rw-r--r--   0        0        0   731421 2023-06-09 18:39:41.400572 gwcelery-2.1.2/gwcelery/data/first2years/gstlal.xml.gz
--rwxr-xr-x   0        0        0     2809 2023-06-09 18:39:41.400572 gwcelery-2.1.2/gwcelery/data/gwcelery.sub
--rw-r--r--   0        0        0      505 2023-06-09 18:39:41.400572 gwcelery-2.1.2/gwcelery/email/__init__.py
--rw-r--r--   0        0        0     3317 2023-06-09 18:39:41.400572 gwcelery-2.1.2/gwcelery/email/bootsteps.py
--rw-r--r--   0        0        0      995 2023-06-09 18:39:41.400572 gwcelery-2.1.2/gwcelery/email/signals.py
--rw-r--r--   0        0        0     1457 2023-06-09 18:39:41.400572 gwcelery-2.1.2/gwcelery/flask.py
--rw-r--r--   0        0        0      529 2023-06-09 18:39:41.400572 gwcelery-2.1.2/gwcelery/igwn_alert/__init__.py
--rw-r--r--   0        0        0     4484 2023-06-09 18:39:41.401572 gwcelery-2.1.2/gwcelery/igwn_alert/bootsteps.py
--rw-r--r--   0        0        0      608 2023-06-09 18:39:41.401572 gwcelery-2.1.2/gwcelery/igwn_alert/signals.py
--rw-r--r--   0        0        0      275 2023-06-09 18:39:41.401572 gwcelery-2.1.2/gwcelery/jinja.py
--rw-r--r--   0        0        0      305 2023-06-09 18:39:41.401572 gwcelery-2.1.2/gwcelery/kafka/__init__.py
--rw-r--r--   0        0        0    10652 2023-06-09 18:39:41.401572 gwcelery-2.1.2/gwcelery/kafka/bootsteps.py
--rw-r--r--   0        0        0      522 2023-06-09 18:39:41.401572 gwcelery-2.1.2/gwcelery/kafka/signals.py
--rw-r--r--   0        0        0     2567 2023-06-09 18:39:41.401572 gwcelery-2.1.2/gwcelery/sentry/__init__.py
--rw-r--r--   0        0        0       34 2023-06-09 18:39:41.401572 gwcelery-2.1.2/gwcelery/sentry/integrations/__init__.py
--rw-r--r--   0        0        0      832 2023-06-09 18:39:41.401572 gwcelery-2.1.2/gwcelery/sentry/integrations/condor.py
--rw-r--r--   0        0        0      836 2023-06-09 18:39:41.401572 gwcelery-2.1.2/gwcelery/sentry/integrations/requests.py
--rw-r--r--   0        0        0      939 2023-06-09 18:39:41.402572 gwcelery-2.1.2/gwcelery/sentry/integrations/subprocess.py
--rw-r--r--   0        0        0     1302 2023-06-09 18:39:41.402572 gwcelery-2.1.2/gwcelery/static/typeahead.css
--rw-r--r--   0        0        0     4124 2023-06-09 18:39:41.402572 gwcelery-2.1.2/gwcelery/static/vega/index.html
--rw-r--r--   0        0        0      515 2023-06-09 18:39:41.402572 gwcelery-2.1.2/gwcelery/tasks/__init__.py
--rw-r--r--   0        0        0    13597 2023-06-09 18:39:41.402572 gwcelery-2.1.2/gwcelery/tasks/alerts.py
--rw-r--r--   0        0        0     2672 2023-06-09 18:39:41.402572 gwcelery-2.1.2/gwcelery/tasks/bayestar.py
--rw-r--r--   0        0        0     1535 2023-06-09 18:39:41.402572 gwcelery-2.1.2/gwcelery/tasks/circulars.py
--rw-r--r--   0        0        0     7502 2023-06-09 18:39:41.402572 gwcelery-2.1.2/gwcelery/tasks/condor.py
--rw-r--r--   0        0        0     2692 2023-06-09 18:39:41.403572 gwcelery-2.1.2/gwcelery/tasks/core.py
--rw-r--r--   0        0        0    23014 2023-06-09 18:39:41.403572 gwcelery-2.1.2/gwcelery/tasks/detchar.py
--rw-r--r--   0        0        0     4863 2023-06-09 18:39:41.403572 gwcelery-2.1.2/gwcelery/tasks/em_bright.py
--rw-r--r--   0        0        0    21775 2023-06-09 18:39:41.403572 gwcelery-2.1.2/gwcelery/tasks/external_skymaps.py
--rw-r--r--   0        0        0    23705 2023-06-09 18:39:41.404572 gwcelery-2.1.2/gwcelery/tasks/external_triggers.py
--rw-r--r--   0        0        0     6832 2023-06-09 18:39:41.404572 gwcelery-2.1.2/gwcelery/tasks/first2years.py
--rw-r--r--   0        0        0     6320 2023-06-09 18:39:41.404572 gwcelery-2.1.2/gwcelery/tasks/first2years_external.py
--rw-r--r--   0        0        0     4831 2023-06-09 18:39:41.404572 gwcelery-2.1.2/gwcelery/tasks/gcn.py
--rw-r--r--   0        0        0    11079 2023-06-09 18:39:41.404572 gwcelery-2.1.2/gwcelery/tasks/gracedb.py
--rw-r--r--   0        0        0     6105 2023-06-09 18:39:41.404572 gwcelery-2.1.2/gwcelery/tasks/gwskynet.py
--rw-r--r--   0        0        0     2453 2023-06-09 18:39:41.405572 gwcelery-2.1.2/gwcelery/tasks/igwn_alert.py
--rw-r--r--   0        0        0    33507 2023-06-09 18:39:41.405572 gwcelery-2.1.2/gwcelery/tasks/inference.py
--rw-r--r--   0        0        0     1406 2023-06-09 18:39:41.405572 gwcelery-2.1.2/gwcelery/tasks/legacy_gracedb.py
--rw-r--r--   0        0        0     7772 2023-06-09 18:39:41.405572 gwcelery-2.1.2/gwcelery/tasks/notice_text.py
--rw-r--r--   0        0        0    47203 2023-06-09 18:39:41.406572 gwcelery-2.1.2/gwcelery/tasks/orchestrator.py
--rw-r--r--   0        0        0     5796 2023-06-09 18:39:41.406572 gwcelery-2.1.2/gwcelery/tasks/p_astro.py
--rw-r--r--   0        0        0    20783 2023-06-09 18:39:41.406572 gwcelery-2.1.2/gwcelery/tasks/raven.py
--rw-r--r--   0        0        0     2242 2023-06-09 18:39:41.406572 gwcelery-2.1.2/gwcelery/tasks/rrt_utils.py
--rw-r--r--   0        0        0    12528 2023-06-09 18:39:41.407572 gwcelery-2.1.2/gwcelery/tasks/skymaps.py
--rw-r--r--   0        0        0    23631 2023-06-09 18:39:41.407572 gwcelery-2.1.2/gwcelery/tasks/superevents.py
--rw-r--r--   0        0        0     1084 2023-06-09 18:39:41.407572 gwcelery-2.1.2/gwcelery/templates/fits_header.jinja2
--rw-r--r--   0        0        0    35556 2023-06-09 18:39:41.408572 gwcelery-2.1.2/gwcelery/templates/index.jinja2
--rw-r--r--   0        0        0     8505 2023-06-09 18:39:41.408572 gwcelery-2.1.2/gwcelery/templates/lalinference.jinja2
--rw-r--r--   0        0        0     9511 2023-06-09 18:39:41.408572 gwcelery-2.1.2/gwcelery/templates/rapidpe.jinja2
--rw-r--r--   0        0        0      472 2023-06-09 18:39:41.408572 gwcelery-2.1.2/gwcelery/templates/vector_table.jinja2
--rw-r--r--   0        0        0        0 2023-06-09 18:39:41.480573 gwcelery-2.1.2/gwcelery/tests/__init__.py
--rw-r--r--   0        0        0     4388 2023-06-09 18:39:41.408572 gwcelery-2.1.2/gwcelery/tests/conftest.py
--rw-r--r--   0        0        0      976 2023-06-09 18:39:41.408572 gwcelery-2.1.2/gwcelery/tests/data/G000012_S0040_preferred.json
--rw-r--r--   0        0        0     6258 2023-06-09 18:39:41.408572 gwcelery-2.1.2/gwcelery/tests/data/G298048-1-Initial.xml
--rw-r--r--   0        0        0      599 2023-06-09 18:39:41.409572 gwcelery-2.1.2/gwcelery/tests/data/G298048_log.json
--rw-r--r--   0        0        0      150 2023-06-09 18:39:41.409572 gwcelery-2.1.2/gwcelery/tests/data/H1L1V1-mean_counts-1126051217-61603201.json
--rw-r--r--   0        0        0      974 2023-06-09 18:39:41.409572 gwcelery-2.1.2/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json
--rw-r--r--   0        0        0    17572 2023-06-09 18:39:41.409572 gwcelery-2.1.2/gwcelery/tests/data/MS220722v.xml
--rw-r--r--   0        0        0   777600 2023-06-09 18:39:41.415572 gwcelery-2.1.2/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits
--rw-r--r--   0        0        0     8220 2023-06-09 18:39:41.415572 gwcelery-2.1.2/gwcelery/tests/data/S230413b.json
--rw-r--r--   0        0        0     7255 2023-06-09 18:39:41.416572 gwcelery-2.1.2/gwcelery/tests/data/S230413g.json
--rw-r--r--   0        0        0     7721 2023-06-09 18:39:41.416572 gwcelery-2.1.2/gwcelery/tests/data/S230413h.json
--rw-r--r--   0        0        0     3387 2023-06-09 18:39:41.416572 gwcelery-2.1.2/gwcelery/tests/data/T0212_S0039_preferred.json
--rw-r--r--   0        0        0     3384 2023-06-09 18:39:41.416572 gwcelery-2.1.2/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json
--rw-r--r--   0        0        0     5210 2023-06-09 18:39:41.416572 gwcelery-2.1.2/gwcelery/tests/data/T0219_S0041_nopreferred.json
--rw-r--r--   0        0        0        0 2023-06-09 18:39:41.481573 gwcelery-2.1.2/gwcelery/tests/data/__init__.py
--rw-r--r--   0        0        0     2290 2023-06-09 18:39:41.416572 gwcelery-2.1.2/gwcelery/tests/data/agile_grb_gcn.xml
--rw-r--r--   0        0        0   854036 2023-06-09 18:39:41.422572 gwcelery-2.1.2/gwcelery/tests/data/coinc.xml
--rw-r--r--   0        0        0     6175 2023-06-09 18:39:41.422572 gwcelery-2.1.2/gwcelery/tests/data/externaltrigger_original_data.xml
--rw-r--r--   0        0        0     5482 2023-06-09 18:39:41.422572 gwcelery-2.1.2/gwcelery/tests/data/fermi_grb_gcn.xml
--rw-r--r--   0        0        0     5469 2023-06-09 18:39:41.422572 gwcelery-2.1.2/gwcelery/tests/data/fermi_initial_grb_gcn.xml
--rw-r--r--   0        0        0     5865 2023-06-09 18:39:41.422572 gwcelery-2.1.2/gwcelery/tests/data/fermi_noise_gcn.xml
--rw-r--r--   0        0        0     5864 2023-06-09 18:39:41.423572 gwcelery-2.1.2/gwcelery/tests/data/fermi_noise_gcn_2.xml
--rw-r--r--   0        0        0     4914 2023-06-09 18:39:41.423572 gwcelery-2.1.2/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml
--rw-r--r--   0        0        0     4914 2023-06-09 18:39:41.423572 gwcelery-2.1.2/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml
--rw-r--r--   0        0        0     3407 2023-06-09 18:39:41.423572 gwcelery-2.1.2/gwcelery/tests/data/fits_header_result.html
--rw-r--r--   0        0        0      882 2023-06-09 18:39:41.423572 gwcelery-2.1.2/gwcelery/tests/data/gracedb_externaltrigger_log.json
--rw-r--r--   0        0        0      446 2023-06-09 18:39:41.423572 gwcelery-2.1.2/gwcelery/tests/data/gracedb_setrigger_log.json
--rw-r--r--   0        0        0      870 2023-06-09 18:39:41.423572 gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_detchar.json
--rw-r--r--   0        0        0     2025 2023-06-09 18:39:41.423572 gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_exttrig_creation.json
--rw-r--r--   0        0        0     2007 2023-06-09 18:39:41.423572 gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json
--rw-r--r--   0        0        0      166 2023-06-09 18:39:41.424572 gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_fits.json
--rw-r--r--   0        0        0      101 2023-06-09 18:39:41.424572 gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_label_dqv.json
--rw-r--r--   0        0        0      743 2023-06-09 18:39:41.424572 gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_psd.json
--rw-r--r--   0        0        0     2020 2023-06-09 18:39:41.424572 gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_snews_creation.json
--rw-r--r--   0        0        0     2012 2023-06-09 18:39:41.424572 gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_snews_test_creation.json
--rw-r--r--   0        0        0     2028 2023-06-09 18:39:41.424572 gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_subgrb_creation.json
--rw-r--r--   0        0        0     1235 2023-06-09 18:39:41.424572 gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_superevent_creation.json
--rw-r--r--   0        0        0      107 2023-06-09 18:39:41.424572 gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_superevent_label.json
--rw-r--r--   0        0        0     5021 2023-06-09 18:39:41.424572 gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_voevent.json
--rw-r--r--   0        0        0     4429 2023-06-09 18:39:41.424572 gwcelery-2.1.2/gwcelery/tests/data/integral_grb_gcn.xml
--rw-r--r--   0        0        0     4295 2023-06-09 18:39:41.424572 gwcelery-2.1.2/gwcelery/tests/data/integral_mdc_gcn.xml
--rw-r--r--   0        0        0        0 2023-06-09 18:39:41.482573 gwcelery-2.1.2/gwcelery/tests/data/llhoft/__init__.py
--rw-r--r--   0        0        0     8267 2023-06-09 18:39:41.425572 gwcelery-2.1.2/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf
--rw-r--r--   0        0        0        0 2023-06-09 18:39:41.482573 gwcelery-2.1.2/gwcelery/tests/data/llhoft/fail/L1/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 18:39:41.482573 gwcelery-2.1.2/gwcelery/tests/data/llhoft/fail/__init__.py
--rw-r--r--   0        0        0    14942 2023-06-09 18:39:41.425572 gwcelery-2.1.2/gwcelery/tests/data/llhoft/idqbad/H1/H-H1_O2_llhoft-1216577976-4.gwf
--rw-r--r--   0        0        0        0 2023-06-09 18:39:41.482573 gwcelery-2.1.2/gwcelery/tests/data/llhoft/omegascan/__init__.py
--rw-r--r--   0        0        0   516419 2023-06-09 18:39:41.426572 gwcelery-2.1.2/gwcelery/tests/data/llhoft/omegascan/scanme.gwf
--rw-r--r--   0        0        0    14950 2023-06-09 18:39:41.427572 gwcelery-2.1.2/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf
--rw-r--r--   0        0        0        0 2023-06-09 18:39:41.482573 gwcelery-2.1.2/gwcelery/tests/data/llhoft/pass/H1/__init__.py
--rw-r--r--   0        0        0        0 2023-06-09 18:39:41.482573 gwcelery-2.1.2/gwcelery/tests/data/llhoft/pass/__init__.py
--rw-r--r--   0        0        0    13099 2023-06-09 18:39:41.427572 gwcelery-2.1.2/gwcelery/tests/data/lvalert_event_creation.json
--rw-r--r--   0        0        0     9060 2023-06-09 18:39:41.427572 gwcelery-2.1.2/gwcelery/tests/data/lvalert_xmpp.xml
--rw-r--r--   0        0        0      864 2023-06-09 18:39:41.427572 gwcelery-2.1.2/gwcelery/tests/data/mock_superevent_object.json
--rw-r--r--   0        0        0   445440 2023-06-09 18:39:41.429572 gwcelery-2.1.2/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite
--rw-r--r--   0        0        0   294426 2023-06-09 18:39:41.430572 gwcelery-2.1.2/gwcelery/tests/data/psd.xml.gz
--rw-r--r--   0        0        0    11520 2023-06-09 18:39:41.431573 gwcelery-2.1.2/gwcelery/tests/data/rrt_small_area.fits
--rw-r--r--   0        0        0     2964 2023-06-09 18:39:41.431573 gwcelery-2.1.2/gwcelery/tests/data/sample_events.json
--rw-r--r--   0        0        0     3648 2023-06-09 18:39:41.431573 gwcelery-2.1.2/gwcelery/tests/data/samples.hdf5
--rw-r--r--   0        0        0      616 2023-06-09 18:39:41.431573 gwcelery-2.1.2/gwcelery/tests/data/scaler_set_all.pickle
--rw-r--r--   0        0        0     6169 2023-06-09 18:39:41.431573 gwcelery-2.1.2/gwcelery/tests/data/snews_gcn.xml
--rw-r--r--   0        0        0     6161 2023-06-09 18:39:41.431573 gwcelery-2.1.2/gwcelery/tests/data/snews_gcn_test.xml
--rw-r--r--   0        0        0     9583 2023-06-09 18:39:41.431573 gwcelery-2.1.2/gwcelery/tests/data/superevents.json
--rw-r--r--   0        0        0     7713 2023-06-09 18:39:41.431573 gwcelery-2.1.2/gwcelery/tests/data/swift_grb_gcn.xml
--rw-r--r--   0        0        0   581918 2023-06-09 18:39:41.434573 gwcelery-2.1.2/gwcelery/tests/data/test_classifier.pickle
--rw-r--r--   0        0        0     4042 2023-06-09 18:39:41.434573 gwcelery-2.1.2/gwcelery/tests/process.py
--rw-r--r--   0        0        0     2307 2023-06-09 18:39:41.434573 gwcelery-2.1.2/gwcelery/tests/test_sentry.py
--rw-r--r--   0        0        0     1705 2023-06-09 18:39:41.434573 gwcelery-2.1.2/gwcelery/tests/test_tasks_alerts.py
--rw-r--r--   0        0        0     4916 2023-06-09 18:39:41.434573 gwcelery-2.1.2/gwcelery/tests/test_tasks_alerts_validate.py
--rw-r--r--   0        0        0     1439 2023-06-09 18:39:41.435572 gwcelery-2.1.2/gwcelery/tests/test_tasks_bayestar.py
--rw-r--r--   0        0        0     3007 2023-06-09 18:39:41.435572 gwcelery-2.1.2/gwcelery/tests/test_tasks_circulars.py
--rw-r--r--   0        0        0     4550 2023-06-09 18:39:41.435572 gwcelery-2.1.2/gwcelery/tests/test_tasks_condor.py
--rw-r--r--   0        0        0    16937 2023-06-09 18:39:41.435572 gwcelery-2.1.2/gwcelery/tests/test_tasks_detchar.py
--rw-r--r--   0        0        0     2317 2023-06-09 18:39:41.435572 gwcelery-2.1.2/gwcelery/tests/test_tasks_em_bright.py
--rw-r--r--   0        0        0    12322 2023-06-09 18:39:41.435572 gwcelery-2.1.2/gwcelery/tests/test_tasks_external_skymaps.py
--rw-r--r--   0        0        0    34773 2023-06-09 18:39:41.436572 gwcelery-2.1.2/gwcelery/tests/test_tasks_external_triggers.py
--rw-r--r--   0        0        0     1816 2023-06-09 18:39:41.436572 gwcelery-2.1.2/gwcelery/tests/test_tasks_first2years.py
--rw-r--r--   0        0        0     4555 2023-06-09 18:39:41.436572 gwcelery-2.1.2/gwcelery/tests/test_tasks_first2years_external.py
--rw-r--r--   0        0        0     1826 2023-06-09 18:39:41.436572 gwcelery-2.1.2/gwcelery/tests/test_tasks_gcn.py
--rw-r--r--   0        0        0     1655 2023-06-09 18:39:41.436572 gwcelery-2.1.2/gwcelery/tests/test_tasks_gcn_validate.py
--rw-r--r--   0        0        0     5739 2023-06-09 18:39:41.436572 gwcelery-2.1.2/gwcelery/tests/test_tasks_gracedb.py
--rw-r--r--   0        0        0     9591 2023-06-09 18:39:41.436572 gwcelery-2.1.2/gwcelery/tests/test_tasks_gwskynet.py
--rw-r--r--   0        0        0     3662 2023-06-09 18:39:41.436572 gwcelery-2.1.2/gwcelery/tests/test_tasks_igwn_alert.py
--rw-r--r--   0        0        0    24398 2023-06-09 18:39:41.437573 gwcelery-2.1.2/gwcelery/tests/test_tasks_inference.py
--rw-r--r--   0        0        0    33486 2023-06-09 18:39:41.437573 gwcelery-2.1.2/gwcelery/tests/test_tasks_orchestrator.py
--rw-r--r--   0        0        0     1647 2023-06-09 18:39:41.437573 gwcelery-2.1.2/gwcelery/tests/test_tasks_p_astro.py
--rw-r--r--   0        0        0    25523 2023-06-09 18:39:41.437573 gwcelery-2.1.2/gwcelery/tests/test_tasks_raven.py
--rw-r--r--   0        0        0     4724 2023-06-09 18:39:41.438573 gwcelery-2.1.2/gwcelery/tests/test_tasks_rrt_utils.py
--rw-r--r--   0        0        0     5035 2023-06-09 18:39:41.438573 gwcelery-2.1.2/gwcelery/tests/test_tasks_skymaps.py
--rw-r--r--   0        0        0    40274 2023-06-09 18:39:41.438573 gwcelery-2.1.2/gwcelery/tests/test_tasks_superevents.py
--rw-r--r--   0        0        0      637 2023-06-09 18:39:41.438573 gwcelery-2.1.2/gwcelery/tests/test_tempfile.py
--rw-r--r--   0        0        0     3520 2023-06-09 18:39:41.438573 gwcelery-2.1.2/gwcelery/tests/test_tools_condor.py
--rw-r--r--   0        0        0     1098 2023-06-09 18:39:41.438573 gwcelery-2.1.2/gwcelery/tests/test_tools_condor_submit_helper.py
--rw-r--r--   0        0        0      633 2023-06-09 18:39:41.438573 gwcelery-2.1.2/gwcelery/tests/test_tools_flask.py
--rw-r--r--   0        0        0     9668 2023-06-09 18:39:41.439572 gwcelery-2.1.2/gwcelery/tests/test_tools_nagios.py
--rw-r--r--   0        0        0      269 2023-06-09 18:39:41.439572 gwcelery-2.1.2/gwcelery/tests/test_util.py
--rw-r--r--   0        0        0    22656 2023-06-09 18:39:41.439572 gwcelery-2.1.2/gwcelery/tests/test_views.py
--rw-r--r--   0        0        0      216 2023-06-09 18:39:41.439572 gwcelery-2.1.2/gwcelery/tools/__init__.py
--rw-r--r--   0        0        0     2948 2023-06-09 18:39:41.439572 gwcelery-2.1.2/gwcelery/tools/condor.py
--rw-r--r--   0        0        0     1120 2023-06-09 18:39:41.439572 gwcelery-2.1.2/gwcelery/tools/condor_submit_helper.py
--rw-r--r--   0        0        0     1938 2023-06-09 18:39:41.439572 gwcelery-2.1.2/gwcelery/tools/flask.py
--rw-r--r--   0        0        0     6624 2023-06-09 18:39:41.439572 gwcelery-2.1.2/gwcelery/tools/nagios.py
--rw-r--r--   0        0        0      413 2023-06-09 18:39:41.439572 gwcelery-2.1.2/gwcelery/util/__init__.py
--rw-r--r--   0        0        0     1007 2023-06-09 18:39:41.439572 gwcelery-2.1.2/gwcelery/util/cmdline.py
--rw-r--r--   0        0        0      453 2023-06-09 18:39:41.440573 gwcelery-2.1.2/gwcelery/util/matplotlib.py
--rw-r--r--   0        0        0      390 2023-06-09 18:39:41.440573 gwcelery-2.1.2/gwcelery/util/proxy.py
--rw-r--r--   0        0        0      514 2023-06-09 18:39:41.440573 gwcelery-2.1.2/gwcelery/util/resources.py
--rw-r--r--   0        0        0      253 2023-06-09 18:39:41.440573 gwcelery-2.1.2/gwcelery/util/sphinx.py
--rw-r--r--   0        0        0      941 2023-06-09 18:39:41.440573 gwcelery-2.1.2/gwcelery/util/tempfile.py
--rw-r--r--   0        0        0    19407 2023-06-09 18:39:41.440573 gwcelery-2.1.2/gwcelery/views.py
--rw-r--r--   0        0        0      365 2023-06-09 18:39:41.440573 gwcelery-2.1.2/gwcelery/voevent/__init__.py
--rw-r--r--   0        0        0     6387 2023-06-09 18:39:41.440573 gwcelery-2.1.2/gwcelery/voevent/bootsteps.py
--rw-r--r--   0        0        0     1063 2023-06-09 18:39:41.440573 gwcelery-2.1.2/gwcelery/voevent/logging.py
--rw-r--r--   0        0        0      779 2023-06-09 18:39:41.441573 gwcelery-2.1.2/gwcelery/voevent/signals.py
--rw-r--r--   0        0        0      852 2023-06-09 18:39:41.441573 gwcelery-2.1.2/gwcelery/voevent/subscriber.py
--rw-r--r--   0        0        0     1454 2023-06-09 18:39:41.441573 gwcelery-2.1.2/gwcelery/voevent/util.py
--rw-r--r--   0        0        0     6107 2023-06-09 18:39:53.695639 gwcelery-2.1.2/pyproject.toml
--rw-r--r--   0        0        0     4524 1970-01-01 00:00:00.000000 gwcelery-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0    97744 2023-06-24 20:42:02.284535 gwcelery-2.1.3/CHANGES.rst
+-rw-r--r--   0        0        0       64 2023-06-24 20:42:02.284535 gwcelery-2.1.3/CONTRIBUTING.rst
+-rw-r--r--   0        0        0    19716 2023-06-24 20:42:02.284535 gwcelery-2.1.3/LICENSE.rst
+-rw-r--r--   0        0        0     1351 2023-06-24 20:42:02.284535 gwcelery-2.1.3/README.rst
+-rw-r--r--   0        0        0      634 2023-06-24 20:42:02.285535 gwcelery-2.1.3/doc/Makefile
+-rw-r--r--   0        0        0   191486 2023-06-24 20:42:02.286535 gwcelery-2.1.3/doc/_static/acceptance-tests-checklist.png
+-rw-r--r--   0        0        0   241593 2023-06-24 20:42:02.288535 gwcelery-2.1.3/doc/_static/celeryevent-screenshot.png
+-rw-r--r--   0        0        0   206465 2023-06-24 20:42:02.290535 gwcelery-2.1.3/doc/_static/deployment-screenshot.png
+-rw-r--r--   0        0        0   161306 2023-06-24 20:42:02.291535 gwcelery-2.1.3/doc/_static/flask-screenshot.png
+-rw-r--r--   0        0        0   328056 2023-06-24 20:42:02.294535 gwcelery-2.1.3/doc/_static/flower-screenshot.png
+-rw-r--r--   0        0        0   114719 2023-06-24 20:42:02.295535 gwcelery-2.1.3/doc/_static/logo-0.5x.png
+-rw-r--r--   0        0        0   351955 2023-06-24 20:42:02.298535 gwcelery-2.1.3/doc/_static/logo.png
+-rw-r--r--   0        0        0   230777 2023-06-24 20:42:02.300535 gwcelery-2.1.3/doc/_static/sentry-screenshot.png
+-rwxr-xr-x   0        0        0     7356 2023-06-24 20:42:02.300535 gwcelery-2.1.3/doc/conf.py
+-rw-r--r--   0        0        0     4346 2023-06-24 20:42:02.300535 gwcelery-2.1.3/doc/configuration.rst
+-rw-r--r--   0        0        0     5698 2023-06-24 20:42:02.300535 gwcelery-2.1.3/doc/contributing.rst
+-rw-r--r--   0        0        0     7202 2023-06-24 20:42:02.301535 gwcelery-2.1.3/doc/deployment.rst
+-rw-r--r--   0        0        0    10176 2023-06-24 20:42:02.301535 gwcelery-2.1.3/doc/design.rst
+-rw-r--r--   0        0        0      486 2023-06-24 20:42:02.301535 gwcelery-2.1.3/doc/gwcelery.conf.rst
+-rw-r--r--   0        0        0      284 2023-06-24 20:42:02.301535 gwcelery-2.1.3/doc/gwcelery.email.rst
+-rw-r--r--   0        0        0      329 2023-06-24 20:42:02.301535 gwcelery-2.1.3/doc/gwcelery.igwn_alert.rst
+-rw-r--r--   0        0        0      227 2023-06-24 20:42:02.301535 gwcelery-2.1.3/doc/gwcelery.rst
+-rw-r--r--   0        0        0       79 2023-06-24 20:42:02.301535 gwcelery-2.1.3/doc/gwcelery.sentry.rst
+-rw-r--r--   0        0        0       97 2023-06-24 20:42:02.301535 gwcelery-2.1.3/doc/gwcelery.tasks.alerts.rst
+-rw-r--r--   0        0        0      103 2023-06-24 20:42:02.301535 gwcelery-2.1.3/doc/gwcelery.tasks.bayestar.rst
+-rw-r--r--   0        0        0      107 2023-06-24 20:42:02.302535 gwcelery-2.1.3/doc/gwcelery.tasks.circulars.rst
+-rw-r--r--   0        0        0       98 2023-06-24 20:42:02.302535 gwcelery-2.1.3/doc/gwcelery.tasks.condor.rst
+-rw-r--r--   0        0        0     2404 2023-06-24 20:42:02.302535 gwcelery-2.1.3/doc/gwcelery.tasks.detchar.rst
+-rw-r--r--   0        0        0     1110 2023-06-24 20:42:02.302535 gwcelery-2.1.3/doc/gwcelery.tasks.em_bright.rst
+-rw-r--r--   0        0        0      129 2023-06-24 20:42:02.302535 gwcelery-2.1.3/doc/gwcelery.tasks.external_skymaps.rst
+-rw-r--r--   0        0        0     6738 2023-06-24 20:42:02.302535 gwcelery-2.1.3/doc/gwcelery.tasks.external_triggers.rst
+-rw-r--r--   0        0        0      112 2023-06-24 20:42:02.302535 gwcelery-2.1.3/doc/gwcelery.tasks.first2years.rst
+-rw-r--r--   0        0        0       88 2023-06-24 20:42:02.302535 gwcelery-2.1.3/doc/gwcelery.tasks.gcn.rst
+-rw-r--r--   0        0        0      100 2023-06-24 20:42:02.302535 gwcelery-2.1.3/doc/gwcelery.tasks.gracedb.rst
+-rw-r--r--   0        0        0      109 2023-06-24 20:42:02.302535 gwcelery-2.1.3/doc/gwcelery.tasks.igwn_alert.rst
+-rw-r--r--   0        0        0      109 2023-06-24 20:42:02.302535 gwcelery-2.1.3/doc/gwcelery.tasks.inference.rst
+-rw-r--r--   0        0        0     8111 2023-06-24 20:42:02.303535 gwcelery-2.1.3/doc/gwcelery.tasks.orchestrator.rst
+-rw-r--r--   0        0        0      100 2023-06-24 20:42:02.303535 gwcelery-2.1.3/doc/gwcelery.tasks.p_astro.rst
+-rw-r--r--   0        0        0       94 2023-06-24 20:42:02.303535 gwcelery-2.1.3/doc/gwcelery.tasks.raven.rst
+-rw-r--r--   0        0        0      628 2023-06-24 20:42:02.303535 gwcelery-2.1.3/doc/gwcelery.tasks.rst
+-rw-r--r--   0        0        0      100 2023-06-24 20:42:02.303535 gwcelery-2.1.3/doc/gwcelery.tasks.skymaps.rst
+-rw-r--r--   0        0        0     7161 2023-06-24 20:42:02.303535 gwcelery-2.1.3/doc/gwcelery.tasks.superevents.rst
+-rw-r--r--   0        0        0       97 2023-06-24 20:42:02.303535 gwcelery-2.1.3/doc/gwcelery.tools.condor.rst
+-rw-r--r--   0        0        0       94 2023-06-24 20:42:02.303535 gwcelery-2.1.3/doc/gwcelery.tools.flask.rst
+-rw-r--r--   0        0        0       97 2023-06-24 20:42:02.303535 gwcelery-2.1.3/doc/gwcelery.tools.nagios.rst
+-rw-r--r--   0        0        0      185 2023-06-24 20:42:02.304535 gwcelery-2.1.3/doc/gwcelery.tools.rst
+-rw-r--r--   0        0        0       73 2023-06-24 20:42:02.304535 gwcelery-2.1.3/doc/gwcelery.util.rst
+-rw-r--r--   0        0        0      507 2023-06-24 20:42:02.304535 gwcelery-2.1.3/doc/gwcelery.voevent.rst
+-rw-r--r--   0        0        0     3564 2023-06-24 20:42:02.304535 gwcelery-2.1.3/doc/htcondor.rst
+-rw-r--r--   0        0        0     1576 2023-06-24 20:42:02.304535 gwcelery-2.1.3/doc/index.rst
+-rw-r--r--   0        0        0      800 2023-06-24 20:42:02.304535 gwcelery-2.1.3/doc/make.bat
+-rw-r--r--   0        0        0     4416 2023-06-24 20:42:02.304535 gwcelery-2.1.3/doc/monitoring.rst
+-rw-r--r--   0        0        0     5312 2023-06-24 20:42:02.304535 gwcelery-2.1.3/doc/quickstart.rst
+-rw-r--r--   0        0        0     1149 2023-06-24 20:42:02.305535 gwcelery-2.1.3/gwcelery/__init__.py
+-rw-r--r--   0        0        0    18447 2023-06-24 20:42:02.305535 gwcelery-2.1.3/gwcelery/_version.py
+-rw-r--r--   0        0        0    16230 2023-06-24 20:42:02.305535 gwcelery-2.1.3/gwcelery/conf/__init__.py
+-rw-r--r--   0        0        0     1014 2023-06-24 20:42:02.305535 gwcelery-2.1.3/gwcelery/conf/dev.py
+-rw-r--r--   0        0        0      403 2023-06-24 20:42:02.306535 gwcelery-2.1.3/gwcelery/conf/development.py
+-rw-r--r--   0        0        0     1289 2023-06-24 20:42:02.306535 gwcelery-2.1.3/gwcelery/conf/minikube.py
+-rw-r--r--   0        0        0     1865 2023-06-24 20:42:02.306535 gwcelery-2.1.3/gwcelery/conf/playground.py
+-rw-r--r--   0        0        0     3541 2023-06-24 20:42:02.306535 gwcelery-2.1.3/gwcelery/conf/production.py
+-rw-r--r--   0        0        0     2040 2023-06-24 20:42:02.306535 gwcelery-2.1.3/gwcelery/conf/test.py
+-rw-r--r--   0        0        0        0 2023-06-24 20:42:02.427536 gwcelery-2.1.3/gwcelery/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-24 20:42:02.428536 gwcelery-2.1.3/gwcelery/data/first2years/__init__.py
+-rw-r--r--   0        0        0   731421 2023-06-24 20:42:02.309535 gwcelery-2.1.3/gwcelery/data/first2years/gstlal.xml.gz
+-rwxr-xr-x   0        0        0     2809 2023-06-24 20:42:02.310535 gwcelery-2.1.3/gwcelery/data/gwcelery.sub
+-rw-r--r--   0        0        0      505 2023-06-24 20:42:02.310535 gwcelery-2.1.3/gwcelery/email/__init__.py
+-rw-r--r--   0        0        0     3317 2023-06-24 20:42:02.310535 gwcelery-2.1.3/gwcelery/email/bootsteps.py
+-rw-r--r--   0        0        0      995 2023-06-24 20:42:02.310535 gwcelery-2.1.3/gwcelery/email/signals.py
+-rw-r--r--   0        0        0     1457 2023-06-24 20:42:02.310535 gwcelery-2.1.3/gwcelery/flask.py
+-rw-r--r--   0        0        0      529 2023-06-24 20:42:02.311535 gwcelery-2.1.3/gwcelery/igwn_alert/__init__.py
+-rw-r--r--   0        0        0     4484 2023-06-24 20:42:02.311535 gwcelery-2.1.3/gwcelery/igwn_alert/bootsteps.py
+-rw-r--r--   0        0        0      608 2023-06-24 20:42:02.311535 gwcelery-2.1.3/gwcelery/igwn_alert/signals.py
+-rw-r--r--   0        0        0      275 2023-06-24 20:42:02.311535 gwcelery-2.1.3/gwcelery/jinja.py
+-rw-r--r--   0        0        0      305 2023-06-24 20:42:02.311535 gwcelery-2.1.3/gwcelery/kafka/__init__.py
+-rw-r--r--   0        0        0    10652 2023-06-24 20:42:02.311535 gwcelery-2.1.3/gwcelery/kafka/bootsteps.py
+-rw-r--r--   0        0        0      522 2023-06-24 20:42:02.311535 gwcelery-2.1.3/gwcelery/kafka/signals.py
+-rw-r--r--   0        0        0     2567 2023-06-24 20:42:02.312535 gwcelery-2.1.3/gwcelery/sentry/__init__.py
+-rw-r--r--   0        0        0       34 2023-06-24 20:42:02.312535 gwcelery-2.1.3/gwcelery/sentry/integrations/__init__.py
+-rw-r--r--   0        0        0      832 2023-06-24 20:42:02.312535 gwcelery-2.1.3/gwcelery/sentry/integrations/condor.py
+-rw-r--r--   0        0        0      836 2023-06-24 20:42:02.312535 gwcelery-2.1.3/gwcelery/sentry/integrations/requests.py
+-rw-r--r--   0        0        0      939 2023-06-24 20:42:02.312535 gwcelery-2.1.3/gwcelery/sentry/integrations/subprocess.py
+-rw-r--r--   0        0        0     1302 2023-06-24 20:42:02.312535 gwcelery-2.1.3/gwcelery/static/typeahead.css
+-rw-r--r--   0        0        0     4124 2023-06-24 20:42:02.312535 gwcelery-2.1.3/gwcelery/static/vega/index.html
+-rw-r--r--   0        0        0      515 2023-06-24 20:42:02.312535 gwcelery-2.1.3/gwcelery/tasks/__init__.py
+-rw-r--r--   0        0        0    13597 2023-06-24 20:42:02.313535 gwcelery-2.1.3/gwcelery/tasks/alerts.py
+-rw-r--r--   0        0        0     2672 2023-06-24 20:42:02.313535 gwcelery-2.1.3/gwcelery/tasks/bayestar.py
+-rw-r--r--   0        0        0     1535 2023-06-24 20:42:02.313535 gwcelery-2.1.3/gwcelery/tasks/circulars.py
+-rw-r--r--   0        0        0     7502 2023-06-24 20:42:02.313535 gwcelery-2.1.3/gwcelery/tasks/condor.py
+-rw-r--r--   0        0        0     2692 2023-06-24 20:42:02.313535 gwcelery-2.1.3/gwcelery/tasks/core.py
+-rw-r--r--   0        0        0    22857 2023-06-24 20:42:02.314535 gwcelery-2.1.3/gwcelery/tasks/detchar.py
+-rw-r--r--   0        0        0     4865 2023-06-24 20:42:02.314535 gwcelery-2.1.3/gwcelery/tasks/em_bright.py
+-rw-r--r--   0        0        0    23428 2023-06-24 20:42:02.314535 gwcelery-2.1.3/gwcelery/tasks/external_skymaps.py
+-rw-r--r--   0        0        0    28634 2023-06-24 20:42:02.315535 gwcelery-2.1.3/gwcelery/tasks/external_triggers.py
+-rw-r--r--   0        0        0     6832 2023-06-24 20:42:02.315535 gwcelery-2.1.3/gwcelery/tasks/first2years.py
+-rw-r--r--   0        0        0     6320 2023-06-24 20:42:02.315535 gwcelery-2.1.3/gwcelery/tasks/first2years_external.py
+-rw-r--r--   0        0        0     4831 2023-06-24 20:42:02.315535 gwcelery-2.1.3/gwcelery/tasks/gcn.py
+-rw-r--r--   0        0        0    11079 2023-06-24 20:42:02.315535 gwcelery-2.1.3/gwcelery/tasks/gracedb.py
+-rw-r--r--   0        0        0     6105 2023-06-24 20:42:02.316535 gwcelery-2.1.3/gwcelery/tasks/gwskynet.py
+-rw-r--r--   0        0        0     2453 2023-06-24 20:42:02.316535 gwcelery-2.1.3/gwcelery/tasks/igwn_alert.py
+-rw-r--r--   0        0        0    33507 2023-06-24 20:42:02.316535 gwcelery-2.1.3/gwcelery/tasks/inference.py
+-rw-r--r--   0        0        0     1406 2023-06-24 20:42:02.317535 gwcelery-2.1.3/gwcelery/tasks/legacy_gracedb.py
+-rw-r--r--   0        0        0     7772 2023-06-24 20:42:02.317535 gwcelery-2.1.3/gwcelery/tasks/notice_text.py
+-rw-r--r--   0        0        0    47395 2023-06-24 20:42:02.317535 gwcelery-2.1.3/gwcelery/tasks/orchestrator.py
+-rw-r--r--   0        0        0     5796 2023-06-24 20:42:02.318535 gwcelery-2.1.3/gwcelery/tasks/p_astro.py
+-rw-r--r--   0        0        0    20783 2023-06-24 20:42:02.318535 gwcelery-2.1.3/gwcelery/tasks/raven.py
+-rw-r--r--   0        0        0     2242 2023-06-24 20:42:02.318535 gwcelery-2.1.3/gwcelery/tasks/rrt_utils.py
+-rw-r--r--   0        0        0    12528 2023-06-24 20:42:02.318535 gwcelery-2.1.3/gwcelery/tasks/skymaps.py
+-rw-r--r--   0        0        0    23631 2023-06-24 20:42:02.319535 gwcelery-2.1.3/gwcelery/tasks/superevents.py
+-rw-r--r--   0        0        0     1084 2023-06-24 20:42:02.319535 gwcelery-2.1.3/gwcelery/templates/fits_header.jinja2
+-rw-r--r--   0        0        0    35556 2023-06-24 20:42:02.319535 gwcelery-2.1.3/gwcelery/templates/index.jinja2
+-rw-r--r--   0        0        0     8505 2023-06-24 20:42:02.320536 gwcelery-2.1.3/gwcelery/templates/lalinference.jinja2
+-rw-r--r--   0        0        0     9511 2023-06-24 20:42:02.320536 gwcelery-2.1.3/gwcelery/templates/rapidpe.jinja2
+-rw-r--r--   0        0        0      472 2023-06-24 20:42:02.320536 gwcelery-2.1.3/gwcelery/templates/vector_table.jinja2
+-rw-r--r--   0        0        0        0 2023-06-24 20:42:02.430536 gwcelery-2.1.3/gwcelery/tests/__init__.py
+-rw-r--r--   0        0        0     4388 2023-06-24 20:42:02.320536 gwcelery-2.1.3/gwcelery/tests/conftest.py
+-rw-r--r--   0        0        0      976 2023-06-24 20:42:02.320536 gwcelery-2.1.3/gwcelery/tests/data/G000012_S0040_preferred.json
+-rw-r--r--   0        0        0     6258 2023-06-24 20:42:02.321535 gwcelery-2.1.3/gwcelery/tests/data/G298048-1-Initial.xml
+-rw-r--r--   0        0        0      599 2023-06-24 20:42:02.321535 gwcelery-2.1.3/gwcelery/tests/data/G298048_log.json
+-rw-r--r--   0        0        0      150 2023-06-24 20:42:02.321535 gwcelery-2.1.3/gwcelery/tests/data/H1L1V1-mean_counts-1126051217-61603201.json
+-rw-r--r--   0        0        0      974 2023-06-24 20:42:02.321535 gwcelery-2.1.3/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json
+-rw-r--r--   0        0        0    17572 2023-06-24 20:42:02.321535 gwcelery-2.1.3/gwcelery/tests/data/MS220722v.xml
+-rw-r--r--   0        0        0   777600 2023-06-24 20:42:02.328535 gwcelery-2.1.3/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits
+-rw-r--r--   0        0        0     8220 2023-06-24 20:42:02.328535 gwcelery-2.1.3/gwcelery/tests/data/S230413b.json
+-rw-r--r--   0        0        0     7255 2023-06-24 20:42:02.328535 gwcelery-2.1.3/gwcelery/tests/data/S230413g.json
+-rw-r--r--   0        0        0     7721 2023-06-24 20:42:02.328535 gwcelery-2.1.3/gwcelery/tests/data/S230413h.json
+-rw-r--r--   0        0        0     3387 2023-06-24 20:42:02.329535 gwcelery-2.1.3/gwcelery/tests/data/T0212_S0039_preferred.json
+-rw-r--r--   0        0        0     3384 2023-06-24 20:42:02.329535 gwcelery-2.1.3/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json
+-rw-r--r--   0        0        0     5210 2023-06-24 20:42:02.329535 gwcelery-2.1.3/gwcelery/tests/data/T0219_S0041_nopreferred.json
+-rw-r--r--   0        0        0        0 2023-06-24 20:42:02.431536 gwcelery-2.1.3/gwcelery/tests/data/__init__.py
+-rw-r--r--   0        0        0     2290 2023-06-24 20:42:02.329535 gwcelery-2.1.3/gwcelery/tests/data/agile_grb_gcn.xml
+-rw-r--r--   0        0        0   854036 2023-06-24 20:42:02.335535 gwcelery-2.1.3/gwcelery/tests/data/coinc.xml
+-rw-r--r--   0        0        0     6175 2023-06-24 20:42:02.336536 gwcelery-2.1.3/gwcelery/tests/data/externaltrigger_original_data.xml
+-rw-r--r--   0        0        0     5482 2023-06-24 20:42:02.336536 gwcelery-2.1.3/gwcelery/tests/data/fermi_grb_gcn.xml
+-rw-r--r--   0        0        0     5469 2023-06-24 20:42:02.336536 gwcelery-2.1.3/gwcelery/tests/data/fermi_initial_grb_gcn.xml
+-rw-r--r--   0        0        0     5865 2023-06-24 20:42:02.336536 gwcelery-2.1.3/gwcelery/tests/data/fermi_noise_gcn.xml
+-rw-r--r--   0        0        0     5864 2023-06-24 20:42:02.336536 gwcelery-2.1.3/gwcelery/tests/data/fermi_noise_gcn_2.xml
+-rw-r--r--   0        0        0     1914 2023-06-24 20:42:02.337535 gwcelery-2.1.3/gwcelery/tests/data/fermi_subgrbtargeted_template.xml
+-rw-r--r--   0        0        0     4914 2023-06-24 20:42:02.337535 gwcelery-2.1.3/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml
+-rw-r--r--   0        0        0     4914 2023-06-24 20:42:02.337535 gwcelery-2.1.3/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml
+-rw-r--r--   0        0        0     3407 2023-06-24 20:42:02.337535 gwcelery-2.1.3/gwcelery/tests/data/fits_header_result.html
+-rw-r--r--   0        0        0      882 2023-06-24 20:42:02.337535 gwcelery-2.1.3/gwcelery/tests/data/gracedb_externaltrigger_log.json
+-rw-r--r--   0        0        0      446 2023-06-24 20:42:02.337535 gwcelery-2.1.3/gwcelery/tests/data/gracedb_setrigger_log.json
+-rw-r--r--   0        0        0      870 2023-06-24 20:42:02.338535 gwcelery-2.1.3/gwcelery/tests/data/igwn_alert_detchar.json
+-rw-r--r--   0        0        0     2025 2023-06-24 20:42:02.338535 gwcelery-2.1.3/gwcelery/tests/data/igwn_alert_exttrig_creation.json
+-rw-r--r--   0        0        0     2007 2023-06-24 20:42:02.338535 gwcelery-2.1.3/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json
+-rw-r--r--   0        0        0      166 2023-06-24 20:42:02.338535 gwcelery-2.1.3/gwcelery/tests/data/igwn_alert_fits.json
+-rw-r--r--   0        0        0      101 2023-06-24 20:42:02.338535 gwcelery-2.1.3/gwcelery/tests/data/igwn_alert_label_dqv.json
+-rw-r--r--   0        0        0      743 2023-06-24 20:42:02.338535 gwcelery-2.1.3/gwcelery/tests/data/igwn_alert_psd.json
+-rw-r--r--   0        0        0     2020 2023-06-24 20:42:02.338535 gwcelery-2.1.3/gwcelery/tests/data/igwn_alert_snews_creation.json
+-rw-r--r--   0        0        0     2012 2023-06-24 20:42:02.339536 gwcelery-2.1.3/gwcelery/tests/data/igwn_alert_snews_test_creation.json
+-rw-r--r--   0        0        0     2028 2023-06-24 20:42:02.339536 gwcelery-2.1.3/gwcelery/tests/data/igwn_alert_subgrb_creation.json
+-rw-r--r--   0        0        0     1235 2023-06-24 20:42:02.339536 gwcelery-2.1.3/gwcelery/tests/data/igwn_alert_superevent_creation.json
+-rw-r--r--   0        0        0      107 2023-06-24 20:42:02.339536 gwcelery-2.1.3/gwcelery/tests/data/igwn_alert_superevent_label.json
+-rw-r--r--   0        0        0     5021 2023-06-24 20:42:02.339536 gwcelery-2.1.3/gwcelery/tests/data/igwn_alert_voevent.json
+-rw-r--r--   0        0        0     4429 2023-06-24 20:42:02.339536 gwcelery-2.1.3/gwcelery/tests/data/integral_grb_gcn.xml
+-rw-r--r--   0        0        0     4295 2023-06-24 20:42:02.339536 gwcelery-2.1.3/gwcelery/tests/data/integral_mdc_gcn.xml
+-rw-r--r--   0        0        0  1038043 2023-06-24 20:42:02.349536 gwcelery-2.1.3/gwcelery/tests/data/kafka_alert_fermi.json
+-rw-r--r--   0        0        0      806 2023-06-24 20:42:02.349536 gwcelery-2.1.3/gwcelery/tests/data/kafka_alert_swift.json
+-rw-r--r--   0        0        0      743 2023-06-24 20:42:02.349536 gwcelery-2.1.3/gwcelery/tests/data/kafka_alert_swift_noloc.json
+-rw-r--r--   0        0        0  1037630 2023-06-24 20:42:02.351535 gwcelery-2.1.3/gwcelery/tests/data/kafka_alert_swift_wskymap.json
+-rw-r--r--   0        0        0        0 2023-06-24 20:42:02.432536 gwcelery-2.1.3/gwcelery/tests/data/llhoft/__init__.py
+-rw-r--r--   0        0        0     8267 2023-06-24 20:42:02.355536 gwcelery-2.1.3/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf
+-rw-r--r--   0        0        0        0 2023-06-24 20:42:02.433536 gwcelery-2.1.3/gwcelery/tests/data/llhoft/fail/L1/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-24 20:42:02.433536 gwcelery-2.1.3/gwcelery/tests/data/llhoft/fail/__init__.py
+-rw-r--r--   0        0        0    14942 2023-06-24 20:42:02.355536 gwcelery-2.1.3/gwcelery/tests/data/llhoft/idqbad/H1/H-H1_O2_llhoft-1216577976-4.gwf
+-rw-r--r--   0        0        0        0 2023-06-24 20:42:02.433536 gwcelery-2.1.3/gwcelery/tests/data/llhoft/omegascan/__init__.py
+-rw-r--r--   0        0        0   516419 2023-06-24 20:42:02.357535 gwcelery-2.1.3/gwcelery/tests/data/llhoft/omegascan/scanme.gwf
+-rw-r--r--   0        0        0    14950 2023-06-24 20:42:02.357535 gwcelery-2.1.3/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf
+-rw-r--r--   0        0        0        0 2023-06-24 20:42:02.433536 gwcelery-2.1.3/gwcelery/tests/data/llhoft/pass/H1/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-24 20:42:02.433536 gwcelery-2.1.3/gwcelery/tests/data/llhoft/pass/__init__.py
+-rw-r--r--   0        0        0    13099 2023-06-24 20:42:02.357535 gwcelery-2.1.3/gwcelery/tests/data/lvalert_event_creation.json
+-rw-r--r--   0        0        0     9060 2023-06-24 20:42:02.357535 gwcelery-2.1.3/gwcelery/tests/data/lvalert_xmpp.xml
+-rw-r--r--   0        0        0      864 2023-06-24 20:42:02.358536 gwcelery-2.1.3/gwcelery/tests/data/mock_superevent_object.json
+-rw-r--r--   0        0        0   445440 2023-06-24 20:42:02.359536 gwcelery-2.1.3/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite
+-rw-r--r--   0        0        0   294426 2023-06-24 20:42:02.361536 gwcelery-2.1.3/gwcelery/tests/data/psd.xml.gz
+-rw-r--r--   0        0        0    11520 2023-06-24 20:42:02.361536 gwcelery-2.1.3/gwcelery/tests/data/rrt_small_area.fits
+-rw-r--r--   0        0        0     2964 2023-06-24 20:42:02.361536 gwcelery-2.1.3/gwcelery/tests/data/sample_events.json
+-rw-r--r--   0        0        0     3648 2023-06-24 20:42:02.361536 gwcelery-2.1.3/gwcelery/tests/data/samples.hdf5
+-rw-r--r--   0        0        0      616 2023-06-24 20:42:02.361536 gwcelery-2.1.3/gwcelery/tests/data/scaler_set_all.pickle
+-rw-r--r--   0        0        0     6169 2023-06-24 20:42:02.361536 gwcelery-2.1.3/gwcelery/tests/data/snews_gcn.xml
+-rw-r--r--   0        0        0     6161 2023-06-24 20:42:02.362536 gwcelery-2.1.3/gwcelery/tests/data/snews_gcn_test.xml
+-rw-r--r--   0        0        0     9583 2023-06-24 20:42:02.362536 gwcelery-2.1.3/gwcelery/tests/data/superevents.json
+-rw-r--r--   0        0        0     7713 2023-06-24 20:42:02.362536 gwcelery-2.1.3/gwcelery/tests/data/swift_grb_gcn.xml
+-rw-r--r--   0        0        0     1962 2023-06-24 20:42:02.362536 gwcelery-2.1.3/gwcelery/tests/data/swift_subgrbtargeted_template.xml
+-rw-r--r--   0        0        0   581918 2023-06-24 20:42:02.365536 gwcelery-2.1.3/gwcelery/tests/data/test_classifier.pickle
+-rw-r--r--   0        0        0     4042 2023-06-24 20:42:02.365536 gwcelery-2.1.3/gwcelery/tests/process.py
+-rw-r--r--   0        0        0     2307 2023-06-24 20:42:02.365536 gwcelery-2.1.3/gwcelery/tests/test_sentry.py
+-rw-r--r--   0        0        0     1705 2023-06-24 20:42:02.365536 gwcelery-2.1.3/gwcelery/tests/test_tasks_alerts.py
+-rw-r--r--   0        0        0     4916 2023-06-24 20:42:02.365536 gwcelery-2.1.3/gwcelery/tests/test_tasks_alerts_validate.py
+-rw-r--r--   0        0        0     1439 2023-06-24 20:42:02.365536 gwcelery-2.1.3/gwcelery/tests/test_tasks_bayestar.py
+-rw-r--r--   0        0        0     3007 2023-06-24 20:42:02.366536 gwcelery-2.1.3/gwcelery/tests/test_tasks_circulars.py
+-rw-r--r--   0        0        0     4550 2023-06-24 20:42:02.366536 gwcelery-2.1.3/gwcelery/tests/test_tasks_condor.py
+-rw-r--r--   0        0        0    16937 2023-06-24 20:42:02.366536 gwcelery-2.1.3/gwcelery/tests/test_tasks_detchar.py
+-rw-r--r--   0        0        0     2317 2023-06-24 20:42:02.366536 gwcelery-2.1.3/gwcelery/tests/test_tasks_em_bright.py
+-rw-r--r--   0        0        0    13802 2023-06-24 20:42:02.366536 gwcelery-2.1.3/gwcelery/tests/test_tasks_external_skymaps.py
+-rw-r--r--   0        0        0    39929 2023-06-24 20:42:02.367535 gwcelery-2.1.3/gwcelery/tests/test_tasks_external_triggers.py
+-rw-r--r--   0        0        0     1816 2023-06-24 20:42:02.367535 gwcelery-2.1.3/gwcelery/tests/test_tasks_first2years.py
+-rw-r--r--   0        0        0     4584 2023-06-24 20:42:02.367535 gwcelery-2.1.3/gwcelery/tests/test_tasks_first2years_external.py
+-rw-r--r--   0        0        0     1826 2023-06-24 20:42:02.367535 gwcelery-2.1.3/gwcelery/tests/test_tasks_gcn.py
+-rw-r--r--   0        0        0     1655 2023-06-24 20:42:02.367535 gwcelery-2.1.3/gwcelery/tests/test_tasks_gcn_validate.py
+-rw-r--r--   0        0        0     5739 2023-06-24 20:42:02.367535 gwcelery-2.1.3/gwcelery/tests/test_tasks_gracedb.py
+-rw-r--r--   0        0        0     9591 2023-06-24 20:42:02.367535 gwcelery-2.1.3/gwcelery/tests/test_tasks_gwskynet.py
+-rw-r--r--   0        0        0     3662 2023-06-24 20:42:02.368536 gwcelery-2.1.3/gwcelery/tests/test_tasks_igwn_alert.py
+-rw-r--r--   0        0        0    24398 2023-06-24 20:42:02.368536 gwcelery-2.1.3/gwcelery/tests/test_tasks_inference.py
+-rw-r--r--   0        0        0    33897 2023-06-24 20:42:02.368536 gwcelery-2.1.3/gwcelery/tests/test_tasks_orchestrator.py
+-rw-r--r--   0        0        0     1647 2023-06-24 20:42:02.368536 gwcelery-2.1.3/gwcelery/tests/test_tasks_p_astro.py
+-rw-r--r--   0        0        0    25523 2023-06-24 20:42:02.368536 gwcelery-2.1.3/gwcelery/tests/test_tasks_raven.py
+-rw-r--r--   0        0        0     4724 2023-06-24 20:42:02.369536 gwcelery-2.1.3/gwcelery/tests/test_tasks_rrt_utils.py
+-rw-r--r--   0        0        0     5035 2023-06-24 20:42:02.369536 gwcelery-2.1.3/gwcelery/tests/test_tasks_skymaps.py
+-rw-r--r--   0        0        0    40274 2023-06-24 20:42:02.369536 gwcelery-2.1.3/gwcelery/tests/test_tasks_superevents.py
+-rw-r--r--   0        0        0      637 2023-06-24 20:42:02.369536 gwcelery-2.1.3/gwcelery/tests/test_tempfile.py
+-rw-r--r--   0        0        0     3520 2023-06-24 20:42:02.369536 gwcelery-2.1.3/gwcelery/tests/test_tools_condor.py
+-rw-r--r--   0        0        0     1098 2023-06-24 20:42:02.369536 gwcelery-2.1.3/gwcelery/tests/test_tools_condor_submit_helper.py
+-rw-r--r--   0        0        0      633 2023-06-24 20:42:02.369536 gwcelery-2.1.3/gwcelery/tests/test_tools_flask.py
+-rw-r--r--   0        0        0     9668 2023-06-24 20:42:02.370535 gwcelery-2.1.3/gwcelery/tests/test_tools_nagios.py
+-rw-r--r--   0        0        0      269 2023-06-24 20:42:02.370535 gwcelery-2.1.3/gwcelery/tests/test_util.py
+-rw-r--r--   0        0        0    22656 2023-06-24 20:42:02.370535 gwcelery-2.1.3/gwcelery/tests/test_views.py
+-rw-r--r--   0        0        0      216 2023-06-24 20:42:02.370535 gwcelery-2.1.3/gwcelery/tools/__init__.py
+-rw-r--r--   0        0        0     2948 2023-06-24 20:42:02.370535 gwcelery-2.1.3/gwcelery/tools/condor.py
+-rw-r--r--   0        0        0     1120 2023-06-24 20:42:02.370535 gwcelery-2.1.3/gwcelery/tools/condor_submit_helper.py
+-rw-r--r--   0        0        0     1938 2023-06-24 20:42:02.370535 gwcelery-2.1.3/gwcelery/tools/flask.py
+-rw-r--r--   0        0        0     6624 2023-06-24 20:42:02.370535 gwcelery-2.1.3/gwcelery/tools/nagios.py
+-rw-r--r--   0        0        0      413 2023-06-24 20:42:02.371536 gwcelery-2.1.3/gwcelery/util/__init__.py
+-rw-r--r--   0        0        0     1007 2023-06-24 20:42:02.371536 gwcelery-2.1.3/gwcelery/util/cmdline.py
+-rw-r--r--   0        0        0      453 2023-06-24 20:42:02.371536 gwcelery-2.1.3/gwcelery/util/matplotlib.py
+-rw-r--r--   0        0        0      390 2023-06-24 20:42:02.371536 gwcelery-2.1.3/gwcelery/util/proxy.py
+-rw-r--r--   0        0        0      514 2023-06-24 20:42:02.371536 gwcelery-2.1.3/gwcelery/util/resources.py
+-rw-r--r--   0        0        0      253 2023-06-24 20:42:02.371536 gwcelery-2.1.3/gwcelery/util/sphinx.py
+-rw-r--r--   0        0        0      941 2023-06-24 20:42:02.371536 gwcelery-2.1.3/gwcelery/util/tempfile.py
+-rw-r--r--   0        0        0    19407 2023-06-24 20:42:02.371536 gwcelery-2.1.3/gwcelery/views.py
+-rw-r--r--   0        0        0      365 2023-06-24 20:42:02.371536 gwcelery-2.1.3/gwcelery/voevent/__init__.py
+-rw-r--r--   0        0        0     6387 2023-06-24 20:42:02.372536 gwcelery-2.1.3/gwcelery/voevent/bootsteps.py
+-rw-r--r--   0        0        0     1063 2023-06-24 20:42:02.372536 gwcelery-2.1.3/gwcelery/voevent/logging.py
+-rw-r--r--   0        0        0      779 2023-06-24 20:42:02.372536 gwcelery-2.1.3/gwcelery/voevent/signals.py
+-rw-r--r--   0        0        0      852 2023-06-24 20:42:02.372536 gwcelery-2.1.3/gwcelery/voevent/subscriber.py
+-rw-r--r--   0        0        0     1454 2023-06-24 20:42:02.372536 gwcelery-2.1.3/gwcelery/voevent/util.py
+-rw-r--r--   0        0        0     6099 2023-06-24 20:42:18.114587 gwcelery-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0     4530 1970-01-01 00:00:00.000000 gwcelery-2.1.3/PKG-INFO
```

### Comparing `gwcelery-2.1.2/CHANGES.rst` & `gwcelery-2.1.3/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,36 @@
 Changelog
 =========
 
+2.1.3 "Thunderbird" (2023-06-24)
+--------------------------------
+
+-   Update to celery version 5.3.
+
+-   Update ligo.em-bright to version 1.1.4.post2, ligo-followup-advocate
+    to version 1.2.4.
+
+-   Apply FROZEN_LABEL inside the handle_superevent as a part of the alert
+    canvas so that they are retries for RetryableHTTPErrors.
+
+-   Add ingestion of Fermi and Swift subthreshold targeted events. Generalize
+    shared creation and replacement workflow used by various external trigger
+    listeners into a single function.
+
+-   Handle HTTP Error raised while grabbing Fermi skymaps.
+
+-   Add handling for ValueErrors in detchar.check_vector to allow for frames
+    without the requested channel.
+
+-   Log failed omegascan exceptions to Sentry.
+
+-   Change logging level of StateVector reading errors in detchar.check_vector
+    back to log.exception now that https://github.com/gwpy/gwpy/issues/1211
+    is fixed.
+
 2.1.2 "Ogopogo" (2023-06-09)
 ----------------------------
 
 -   Update the low-significance threshold to be 2/day pre-trials factor. Update
     low-siginificance trials factors to 7.
 
 -   Do not apply HIGH_PROFILE label to less-significant alerts.
```

### Comparing `gwcelery-2.1.2/LICENSE.rst` & `gwcelery-2.1.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/README.rst` & `gwcelery-2.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/doc/Makefile` & `gwcelery-2.1.3/doc/Makefile`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/doc/_static/acceptance-tests-checklist.png` & `gwcelery-2.1.3/doc/_static/acceptance-tests-checklist.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/doc/_static/celeryevent-screenshot.png` & `gwcelery-2.1.3/doc/_static/celeryevent-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/doc/_static/deployment-screenshot.png` & `gwcelery-2.1.3/doc/_static/deployment-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/doc/_static/flask-screenshot.png` & `gwcelery-2.1.3/doc/_static/flask-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/doc/_static/flower-screenshot.png` & `gwcelery-2.1.3/doc/_static/flower-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/doc/_static/logo-0.5x.png` & `gwcelery-2.1.3/doc/_static/logo-0.5x.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/doc/_static/logo.png` & `gwcelery-2.1.3/doc/_static/logo.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/doc/_static/sentry-screenshot.png` & `gwcelery-2.1.3/doc/_static/sentry-screenshot.png`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/doc/conf.py` & `gwcelery-2.1.3/doc/conf.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/doc/configuration.rst` & `gwcelery-2.1.3/doc/configuration.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/doc/contributing.rst` & `gwcelery-2.1.3/doc/contributing.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/doc/deployment.rst` & `gwcelery-2.1.3/doc/deployment.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/doc/design.rst` & `gwcelery-2.1.3/doc/design.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/doc/gwcelery.tasks.detchar.rst` & `gwcelery-2.1.3/doc/gwcelery.tasks.detchar.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/doc/gwcelery.tasks.em_bright.rst` & `gwcelery-2.1.3/doc/gwcelery.tasks.em_bright.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/doc/gwcelery.tasks.external_triggers.rst` & `gwcelery-2.1.3/doc/gwcelery.tasks.external_triggers.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/doc/gwcelery.tasks.orchestrator.rst` & `gwcelery-2.1.3/doc/gwcelery.tasks.orchestrator.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/doc/gwcelery.tasks.rst` & `gwcelery-2.1.3/doc/gwcelery.tasks.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/doc/gwcelery.tasks.superevents.rst` & `gwcelery-2.1.3/doc/gwcelery.tasks.superevents.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/doc/htcondor.rst` & `gwcelery-2.1.3/doc/htcondor.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/doc/index.rst` & `gwcelery-2.1.3/doc/index.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/doc/make.bat` & `gwcelery-2.1.3/doc/make.bat`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/doc/monitoring.rst` & `gwcelery-2.1.3/doc/monitoring.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/doc/quickstart.rst` & `gwcelery-2.1.3/doc/quickstart.rst`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/__init__.py` & `gwcelery-2.1.3/gwcelery/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/_version.py` & `gwcelery-2.1.3/gwcelery/_version.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/conf/__init__.py` & `gwcelery-2.1.3/gwcelery/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/conf/dev.py` & `gwcelery-2.1.3/gwcelery/conf/dev.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/conf/minikube.py` & `gwcelery-2.1.3/gwcelery/conf/minikube.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/conf/playground.py` & `gwcelery-2.1.3/gwcelery/conf/playground.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/conf/production.py` & `gwcelery-2.1.3/gwcelery/conf/production.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/conf/test.py` & `gwcelery-2.1.3/gwcelery/conf/test.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/data/first2years/gstlal.xml.gz` & `gwcelery-2.1.3/gwcelery/data/first2years/gstlal.xml.gz`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/data/gwcelery.sub` & `gwcelery-2.1.3/gwcelery/data/gwcelery.sub`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/email/bootsteps.py` & `gwcelery-2.1.3/gwcelery/email/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/email/signals.py` & `gwcelery-2.1.3/gwcelery/email/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/flask.py` & `gwcelery-2.1.3/gwcelery/flask.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/igwn_alert/__init__.py` & `gwcelery-2.1.3/gwcelery/igwn_alert/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/igwn_alert/bootsteps.py` & `gwcelery-2.1.3/gwcelery/igwn_alert/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/igwn_alert/signals.py` & `gwcelery-2.1.3/gwcelery/igwn_alert/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/kafka/bootsteps.py` & `gwcelery-2.1.3/gwcelery/kafka/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/kafka/signals.py` & `gwcelery-2.1.3/gwcelery/kafka/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/sentry/__init__.py` & `gwcelery-2.1.3/gwcelery/sentry/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/sentry/integrations/condor.py` & `gwcelery-2.1.3/gwcelery/sentry/integrations/condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/sentry/integrations/requests.py` & `gwcelery-2.1.3/gwcelery/sentry/integrations/requests.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/sentry/integrations/subprocess.py` & `gwcelery-2.1.3/gwcelery/sentry/integrations/subprocess.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/static/typeahead.css` & `gwcelery-2.1.3/gwcelery/static/typeahead.css`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/static/vega/index.html` & `gwcelery-2.1.3/gwcelery/static/vega/index.html`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tasks/__init__.py` & `gwcelery-2.1.3/gwcelery/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tasks/alerts.py` & `gwcelery-2.1.3/gwcelery/tasks/alerts.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tasks/bayestar.py` & `gwcelery-2.1.3/gwcelery/tasks/bayestar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tasks/circulars.py` & `gwcelery-2.1.3/gwcelery/tasks/circulars.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tasks/condor.py` & `gwcelery-2.1.3/gwcelery/tasks/condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tasks/core.py` & `gwcelery-2.1.3/gwcelery/tasks/core.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tasks/detchar.py` & `gwcelery-2.1.3/gwcelery/tasks/detchar.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from celery.utils.log import get_task_logger
 from glue.lal import Cache
 from gwdatafind import find_urls
 from gwpy.timeseries import Bits, StateVector, TimeSeries
 from gwpy.plot import Plot
 import matplotlib.pyplot as plt
 import numpy as np
+import sentry_sdk
 
 from . import gracedb
 from ..import app
 from ..import _version
 from ..jinja import env
 from ..util import closing_figures
 
@@ -134,19 +135,20 @@
         ts = TimeSeries.read(cache, strain_name,
                              start=long_start, end=long_end).astype('float64')
         # Do q_transforms for the different durations
         qgrams = [ts.q_transform(
             frange=(20, 4096), gps=t0,
             outseg=(t0 - before, t0 + after), logf=True)
             for before, after in durs]
-    except (IndexError, FloatingPointError, ValueError):
+    except (IndexError, FloatingPointError, ValueError) as err:
         # data from cache can't be properly read, or data is weird
+        sentry_sdk.capture_exception(err)
         fig = plt.figure(figsize=(4, 1))
         plt.axis("off")
-        plt.text(0.5, 0.5, "Failed to create V1 omegascan",
+        plt.text(0.5, 0.5, f"Failed to create {ifo} omegascan",
                  horizontalalignment='center', verticalalignment='center',
                  fontsize=17)
     else:
         fig = Plot(*qgrams,
                    figsize=(12 * len(durs), 6),
                    geometry=(1, len(durs)),
                    yscale='log',
@@ -366,21 +368,16 @@
     else:
         logic_map = {'any': np.any, 'all': np.all}
     bitname = '{}:{}'
     if cache:
         try:
             statevector = StateVector.read(cache, channel,
                                            start=start, end=end, bits=bits)
-        except (IndexError, TypeError):
-            # FIXME: TypeError above is due to
-            # https://github.com/gwpy/gwpy/issues/1211
-            #
-            # FIXME: Change from log.exception to log.warning until this fixed,
-            # because it's saturating Sentry.
-            log.warning('Failed to read from low-latency frame files')
+        except (IndexError, TypeError, ValueError):
+            log.exception('Failed to read from low-latency frame files')
         else:
             # FIXME: In the playground environment, the Virgo state vector
             # channel is stored as a float. Is this also the case in the
             # production environment?
             statevector = statevector.astype(np.uint32)
             if len(statevector) > 0:  # statevector must not be empty
                 return {bitname.format(ifo_from_channel(channel), key):
```

### Comparing `gwcelery-2.1.2/gwcelery/tasks/em_bright.py` & `gwcelery-2.1.3/gwcelery/tasks/em_bright.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     {"HasNS": 0.014904901243599122, "HasRemnant": 0.0, "HasMassGap": 0.0}
 
     """
     from ligo.em_bright import em_bright
     with NamedTemporaryFile(content=posterior_file_content) as samplefile:
         filename = samplefile.name
         has_ns, has_remnant, has_massgap = em_bright.source_classification_pe(
-            filename, num_eos_draws=100, eos_seed=0
+            filename, num_eos_draws=10000, eos_seed=0
         )
     data = json.dumps({
         'HasNS': has_ns,
         'HasRemnant': has_remnant,
         'HasMassGap': has_massgap
     })
     return data
```

### Comparing `gwcelery-2.1.2/gwcelery/tasks/external_skymaps.py` & `gwcelery-2.1.3/gwcelery/tasks/external_skymaps.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """Create and upload external sky maps."""
 from astropy import units as u
 from astropy.coordinates import ICRS, SkyCoord
 import astropy_healpix as ah
 from astropy_healpix import HEALPix, pixel_resolution_to_nside
+from base64 import b64decode
 from celery import group
 #  import astropy.utils.data
 import numpy as np
 from ligo.skymap.io import fits
 from ligo.skymap.distance import parameters_to_marginal_moments
 from ligo.skymap.tool import ligo_skymap_combine
 import gcn
 import healpy as hp
 import io
 import lxml.etree
 import re
 import ssl
 import urllib
+from urllib.error import HTTPError
 
 from ..import app
 from . import gracedb
 from . import skymaps
 from ..util.cmdline import handling_system_exit
 from ..util.tempfile import NamedTemporaryFile
 from ..import _version
@@ -255,23 +257,23 @@
             heasarc_url = root.find('./What/Param[@name="LightCurve_URL"]'
                                     ).attrib['value']
             return re.sub(r'quicklook(.*)', 'current/', heasarc_url)
     raise ValueError('Not able to retrieve HEASARC link for {0}.'.format(
         external_id))
 
 
-@app.task(autoretry_for=(urllib.error.HTTPError,), retry_backoff=10,
-          retry_backoff_max=600)
+@app.task(autoretry_for=(gracedb.RetryableHTTPError,), retry_backoff=10,
+          max_retries=14)
 def get_external_skymap(link, search):
     """Download the Fermi sky map fits file and return the contents as a byte
     array. If GRB, will construct a HEASARC url, while if SubGRB, will use the
     link directly.
 
     If not available, will try again 10 seconds later, then 20, then 40, etc.
-    until up to 10 minutes after initial attempt.
+    until up to 15 minutes after initial attempt.
     """
     if search == 'GRB':
         # if Fermi GRB, determine final HEASARC link
         trigger_id = re.sub(r'.*\/(\D+?)(\d+)(\D+)\/.*', r'\2', link)
         skymap_name = 'glg_healpix_all_bn{0}_v00.fit'.format(trigger_id)
         skymap_link = link + skymap_name
     elif search in {'SubGRB', 'FromURL'}:
@@ -279,15 +281,61 @@
     #  FIXME: Under Anaconda on the LIGO Caltech computing cluster, Python
     #  (and curl, for that matter) fail to negotiate TLSv1.2 with
     #  heasarc.gsfc.nasa.gov
     context = ssl.create_default_context()
     context.options |= ssl.OP_NO_TLSv1_3
     #  return astropy.utils.data.get_file_contents(
     #      (skymap_link), encoding='binary', cache=False)
-    return urllib.request.urlopen(skymap_link, context=context).read()
+    try:
+        response = urllib.request.urlopen(skymap_link, context=context)
+        return response.read()
+    except HTTPError as e:
+        if e.code == 404:
+            raise gracedb.RetryableHTTPError("Failed to download the sky map."
+                                             "Retrying...")
+        else:
+            raise
+
+
+@app.task(shared=False)
+def read_upload_skymap_from_base64(event, skymap_str):
+    """Decode and upload 64base encoded sky maps from Kafka alerts"""
+
+    graceid = event['graceid']
+    ra = event['extra_attributes']['GRB']['ra']
+    dec = event['extra_attributes']['GRB']['dec']
+    skymap_filename = event['pipeline'].lower() + '_skymap.fits.gz'
+
+    # Decode base64 encoded string to bytes string
+    skymap_data = b64decode(skymap_str)
+
+    message = (
+        'Mollweide projection of <a href="/api/events/{graceid}/files/'
+        '{filename}">{filename}</a>').format(
+            graceid=graceid, filename=skymap_filename)
+
+    (
+        group(
+            gracedb.upload.si(skymap_data,
+                              skymap_filename,
+                              graceid,
+                              'Sky map uploaded from {}'.format(
+                                  event['pipeline']),
+                              ['sky_loc']),
+
+            skymaps.plot_allsky.si(skymap_data, ra=ra, dec=dec)
+            |
+            gracedb.upload.s(event['pipeline'].lower() + '_skymap.png',
+                             graceid,
+                             message,
+                             ['sky_loc'])
+        )
+        |
+        gracedb.create_label.si('EXT_SKYMAP_READY', graceid)
+    ).delay()
 
 
 @app.task(autoretry_for=(urllib.error.HTTPError, urllib.error.URLError,),
           retry_backoff=10, retry_backoff_max=1200)
 def get_upload_external_skymap(event, skymap_link=None):
     """If a Fermi sky map is not uploaded yet, tries to download one and upload
     to external event. If sky map is not available, passes so that this can be
@@ -301,15 +349,15 @@
 
     if search == 'GRB':
         external_skymap_canvas = (
             external_trigger_heasarc.si(graceid)
             |
             get_external_skymap.s(search)
         )
-    elif search in {'SubGRB', 'FromURL'}:
+    elif search in {'SubGRB', 'SubGRBTargeted', 'FromURL'}:
         external_skymap_canvas = get_external_skymap.si(skymap_link, search)
 
     skymap_filename = \
         ('external_from_url' if search == 'FromURL'
          else 'glg_healpix_all_bn_v00')
 
     fits_message = \
```

### Comparing `gwcelery-2.1.2/gwcelery/tasks/external_triggers.py` & `gwcelery-2.1.3/gwcelery/tasks/external_triggers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 from lxml import etree
 from urllib.parse import urlparse
 from celery import group
 from celery.utils.log import get_logger
+from pathlib import Path
 
 from ..import app
+from . import alerts
 from . import detchar
 from . import gcn
 from . import gracedb
 from . import external_skymaps
 from . import igwn_alert
 from . import raven
 
@@ -51,31 +53,22 @@
     event_observatory = 'SNEWS'
     if 'mdc-test_event' in root.attrib['ivorn'].lower():
         search = 'MDC'
     else:
         search = 'Supernova'
     query = 'group: External pipeline: {} grbevent.trigger_id = "{}"'.format(
         event_observatory, trig_id)
-    events = gracedb.get_events(query=query)
 
-    if events and ext_group == 'External':
-        # Only update event if real
-        assert len(events) == 1, 'Found more than one matching GraceDB entry'
-        event, = events
-        graceid = event['graceid']
-        canvas = gracedb.replace_event.s(graceid, payload)
-
-    else:
-        canvas = gracedb.create_event.s(filecontents=payload,
-                                        search=search,
-                                        group=ext_group,
-                                        pipeline=event_observatory)
-        canvas |= _launch_external_detchar.s()
-
-    canvas.delay()
+    (
+        gracedb.get_events.si(query=query)
+        |
+        _create_replace_external_event_and_skymap.s(
+            payload, search, event_observatory, ext_group=ext_group
+        )
+    ).delay()
 
 
 @gcn.handler(gcn.NoticeType.FERMI_GBM_ALERT,
              gcn.NoticeType.FERMI_GBM_FLT_POS,
              gcn.NoticeType.FERMI_GBM_GND_POS,
              gcn.NoticeType.FERMI_GBM_FIN_POS,
              gcn.NoticeType.SWIFT_BAT_GRB_POS_ACK,
@@ -158,76 +151,46 @@
         root.find("./What/Group[@name='Solution_Status']" +
                   "/Param[@name='StarTrack_Lost_Lock']")
     swift_veto = lost_lock is not None and lost_lock.attrib['value'] == 'true'
 
     #  Only send alerts if likely a GRB, is not a low-confidence early Fermi
     #  alert, and if not a Swift veto
     if not_likely_grb or initial_gbm_alert or swift_veto:
-        labels = ['NOT_GRB']
+        label = 'NOT_GRB'
     else:
-        labels = None
+        label = None
 
     ivorn = root.attrib['ivorn']
     if 'subthresh' in ivorn.lower():
         search = 'SubGRB'
     elif 'mdc-test_event' in ivorn.lower():
         search = 'MDC'
     else:
         search = 'GRB'
 
+    if search == 'SubGRB' and event_observatory == 'Fermi':
+        skymap_link = \
+            root.find("./What/Param[@name='HealPix_URL']").attrib['value']
+    else:
+        skymap_link = None
+
     query = 'group: External pipeline: {} grbevent.trigger_id = "{}"'.format(
         event_observatory, trig_id)
-    events = gracedb.get_events(query=query)
-
-    group_canvas = ()
-    if events and ext_group == 'External':
-        # Only update event if real
-        assert len(events) == 1, 'Found more than one matching GraceDB entry'
-        event, = events
-        graceid = event['graceid']
-        if labels:
-            canvas = gracedb.create_label.si(labels[0], graceid)
-        else:
-            canvas = gracedb.remove_label.si('NOT_GRB', graceid)
-
-        # Prevent SubGRBs from appending GRBs
-        if search == 'GRB':
-            # Replace event and pass already existing event dictionary
-            canvas |= gracedb.replace_event.si(graceid, payload)
-            canvas |= gracedb.get_event.si(graceid)
-        else:
-            return
-
-    else:
-        canvas = gracedb.create_event.s(filecontents=payload,
-                                        search=search,
-                                        group=ext_group,
-                                        pipeline=event_observatory,
-                                        labels=labels)
-        group_canvas += _launch_external_detchar.s(),
-
-    if search in {'GRB', 'MDC'}:
-        notice_date = root.find("./Who/Date").text
-        group_canvas += external_skymaps.create_upload_external_skymap.s(
-                      notice_type, notice_date),
-    if event_observatory == 'Fermi':
-        if search == 'SubGRB':
-            skymap_link = \
-                root.find("./What/Param[@name='HealPix_URL']").attrib['value']
-            group_canvas += \
-                external_skymaps.get_upload_external_skymap.s(skymap_link),
-        elif search == 'GRB':
-            skymap_link = None
-            group_canvas += \
-                external_skymaps.get_upload_external_skymap.s(skymap_link),
 
     (
-        canvas
+        gracedb.get_events.si(query=query)
         |
-        group(group_canvas)
+        _create_replace_external_event_and_skymap.s(
+            payload, search, event_observatory,
+            ext_group=ext_group, label=label,
+            notice_date=root.find("./Who/Date").text,
+            notice_type=notice_type,
+            skymap_link=skymap_link,
+            use_radec=search in {'GRB', 'MDC'}
+        )
     ).delay()
 
 
 @igwn_alert.handler('superevent',
                     'mdc_superevent',
                     'external_fermi',
                     'external_swift',
@@ -255,21 +218,14 @@
     """
     # Determine GraceDB ID
     graceid = alert['uid']
 
     # launch searches
     if alert['alert_type'] == 'new':
         if alert['object'].get('group') == 'External':
-            # Create and upload Swift sky map for the joint targeted
-            # sub-threshold search as agreed on in the MOU
-            if alert['object']['search'] == 'SubGRBTargeted' and \
-                    alert['object']['pipeline'] == 'Swift':
-                external_skymaps.create_upload_external_skymap(
-                    alert['object'], None, alert['object']['created'])
-
             # launch search with MDC events and exit
             if alert['object']['search'] == 'MDC':
                 raven.coincidence_search(graceid, alert['object'],
                                          group='CBC', se_searches=['MDC'])
                 raven.coincidence_search(graceid, alert['object'],
                                          group='Burst', se_searches=['MDC'])
                 return
@@ -471,14 +427,48 @@
                                          pipelines=['SNEWS'])
             elif search == 'Supernova':
                 raven.coincidence_search(graceid, alert['object'],
                                          group='Burst', searches=['Supernova'],
                                          pipelines=['SNEWS'])
 
 
+@alerts.handler('fermi',
+                'swift')
+def handle_targeted_kafka_alert(alert):
+    """Parse an alert sent via Kafka from a MOU partner in our joint
+    subthreshold targeted search.
+
+    Parameters
+    ----------
+    alert : dict
+        Kafka alert packet
+
+    """
+    # Convert alert to VOEvent format
+    # FIXME: This is required until native ingesting of kafka events in GraceDB
+    payload, pipeline, time, trig_id = _kafka_to_voevent(alert)
+
+    label = 'NOT_GRB' if alert['alert_type'] == "retraction" else None
+
+    # Look whether a previous event with the same ID exists
+    query = 'group: External pipeline: {} grbevent.trigger_id = "{}"'.format(
+        pipeline, trig_id)
+
+    (
+        gracedb.get_events.si(query=query)
+        |
+        _create_replace_external_event_and_skymap.s(
+            payload, 'SubGRBTargeted', pipeline,
+            label=label, notice_date=time,
+            skymap=alert.get('healpix_file'),
+            use_radec=('ra' in alert and 'dec' in alert)
+        )
+    ).delay()
+
+
 def _skymaps_are_ready(event, label, task):
     label_set = set(event['labels'])
     required_labels = REQUIRED_LABELS_BY_TASK[task]
     return required_labels.issubset(label_set) and label in required_labels
 
 
 def _get_superevent_ext_ids(graceid, event):
@@ -544,7 +534,166 @@
         # Create new updated combined sky map
         canvas |= external_skymaps.create_combined_skymap.si(
                       superevent['superevent_id'], ext_event['graceid'],
                       preferred_event=(
                           None if use_superevent
                           else superevent['preferred_event']))
     canvas.delay()
+
+
+@app.task(shared=False)
+def _create_replace_external_event_and_skymap(
+        events, payload, search, pipeline,
+        label=None, ext_group='External', notice_date=None, notice_type=None,
+        skymap=None, skymap_link=None, use_radec=False):
+    """Either create a new external event or replace an old one if applicable
+    Then either uploads a given sky map, try to download one given a link, or
+    create one given coordinates.
+
+    Parameters
+    ----------
+    events : list
+        List of external events sharing the same trigger ID
+    payload : str
+        VOEvent of event being considered
+    search : str
+        Search of external event
+    pipeline : str
+        Pipeline of external evevent
+    label : list
+        Label to be uploaded along with external event. If None, removes
+        'NOT_GRB' label from event
+    ext_group : str
+        Group of external event, 'External' or 'Test'
+    notice_date : str
+        Time and date of external event
+    notice_type : str
+        GCN Notice type of external event
+    skymap : str
+        Base64 encoded sky map
+    skymap_link : str
+        Link to external sky map to be downloaded
+    use_radec : bool
+        If true, try to create sky map using given coordinates
+
+    """
+    skymap_detchar_canvas = ()
+    # If previous event, try to append
+    if events and ext_group == 'External':
+        assert len(events) == 1, 'Found more than one matching GraceDB entry'
+        event, = events
+        graceid = event['graceid']
+        if label:
+            create_replace_canvas = gracedb.create_label.si(label, graceid)
+        else:
+            create_replace_canvas = gracedb.remove_label.si('NOT_GRB', graceid)
+
+        # Prevent SubGRBs from appending GRBs, also append if same search
+        if search == 'GRB' or search == event['search']:
+            # Replace event and pass already existing event dictionary
+            create_replace_canvas |= gracedb.replace_event.si(graceid, payload)
+            create_replace_canvas |= gracedb.get_event.si(graceid)
+        else:
+            # If not appending just exit
+            return
+
+    # If new event, create new entry in GraceDB and launch detchar
+    else:
+        create_replace_canvas = gracedb.create_event.si(
+            filecontents=payload,
+            search=search,
+            group=ext_group,
+            pipeline=pipeline,
+            labels=[label] if label else None)
+        skymap_detchar_canvas += _launch_external_detchar.s(),
+
+    # Use sky map if provided
+    if skymap:
+        skymap_detchar_canvas += \
+            external_skymaps.read_upload_skymap_from_base64.s(skymap),
+    else:
+        # Otherwise grab sky map from provided link
+        if skymap_link:
+            skymap_detchar_canvas += \
+                external_skymaps.get_upload_external_skymap.s(skymap_link),
+        # Otherwise if threshold Fermi try to grab sky map
+        elif pipeline == 'Fermi' and search == 'GRB':
+            skymap_detchar_canvas += \
+                external_skymaps.get_upload_external_skymap.s(None),
+        # Otherwise create sky map from given coordinates
+        if use_radec:
+            skymap_detchar_canvas += \
+                external_skymaps.create_upload_external_skymap.s(
+                    notice_type, notice_date),
+
+    (
+        create_replace_canvas
+        |
+        group(skymap_detchar_canvas)
+    ).delay()
+
+
+def _kafka_to_voevent(alert):
+    # Define basic values
+    pipeline = alert['mission']
+    trigger_time = alert['trigger_time']
+    alert_time = alert['alert_datetime']
+    far = alert['far']
+    integration_time = alert['rate_duration']
+    id = '_'.join(str(x) for x in alert['id'])
+
+    # sky localization may not be available
+    ra = alert.get('ra')
+    dec = alert.get('dec')
+    # Try to get dec first then ra, None if both misssing
+    error = alert.get('dec_uncertainty')
+    if error is None:
+        error = alert.get('ra_uncertainty')
+    # Argument should be list if not None
+    if isinstance(error, list):
+        error = error[0]
+    # if any missing sky map info, set to zeros so will be ignored later
+    if ra is None or dec is None or error is None:
+        ra, dec, error = 0., 0., 0.
+
+    # Load template
+    fname = str(Path(__file__).parent /
+                '../tests/data/{}_subgrbtargeted_template.xml'.format(
+                    pipeline.lower()))
+    root = etree.parse(fname)
+
+    # Update template values
+    # Change ivorn to indicate this is a subthreshold targeted event
+    root.xpath('.')[0].attrib['ivorn'] = \
+        'ivo://lvk.internal/{0}#targeted_subthreshold-{1}'.format(
+            pipeline.lower(), trigger_time).encode()
+
+    # Update ID
+    root.find("./What/Param[@name='TrigID']").attrib['value'] = \
+        id.encode()
+
+    # Change times to chosen time
+    root.find("./Who/Date").text = str(alert_time).encode()
+    root.find(("./WhereWhen/ObsDataLocation/"
+               "ObservationLocation/AstroCoords/Time/TimeInstant/"
+               "ISOTime")).text = str(trigger_time).encode()
+
+    root.find("./What/Param[@name='FAR']").attrib['value'] = \
+        str(far).encode()
+
+    root.find("./What/Param[@name='Integ_Time']").attrib['value'] = \
+        str(integration_time).encode()
+
+    # Sky position
+    root.find(("./WhereWhen/ObsDataLocation/"
+               "ObservationLocation/AstroCoords/Position2D/Value2/"
+               "C1")).text = str(ra).encode()
+    root.find(("./WhereWhen/ObsDataLocation/"
+               "ObservationLocation/AstroCoords/Position2D/Value2/"
+               "C2")).text = str(dec).encode()
+    root.find(("./WhereWhen/ObsDataLocation/"
+               "ObservationLocation/AstroCoords/Position2D/"
+               "Error2Radius")).text = str(error).encode()
+
+    return (etree.tostring(root, xml_declaration=True, encoding="UTF-8",
+                           pretty_print=True),
+            pipeline, trigger_time.replace('Z', ''), id)
```

### Comparing `gwcelery-2.1.2/gwcelery/tasks/first2years.py` & `gwcelery-2.1.3/gwcelery/tasks/first2years.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tasks/first2years_external.py` & `gwcelery-2.1.3/gwcelery/tasks/first2years_external.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tasks/gcn.py` & `gwcelery-2.1.3/gwcelery/tasks/gcn.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tasks/gracedb.py` & `gwcelery-2.1.3/gwcelery/tasks/gracedb.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tasks/gwskynet.py` & `gwcelery-2.1.3/gwcelery/tasks/gwskynet.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tasks/igwn_alert.py` & `gwcelery-2.1.3/gwcelery/tasks/igwn_alert.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tasks/inference.py` & `gwcelery-2.1.3/gwcelery/tasks/inference.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tasks/legacy_gracedb.py` & `gwcelery-2.1.3/gwcelery/tasks/legacy_gracedb.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tasks/notice_text.py` & `gwcelery-2.1.3/gwcelery/tasks/notice_text.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tasks/orchestrator.py` & `gwcelery-2.1.3/gwcelery/tasks/orchestrator.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,18 +131,20 @@
                 earlywarning_preliminary_alert.s(
                     alert, alert_type='less-significant')
             ).apply_async()
 
         # launch significant alert on SIGNIF_LOCKED
         elif label_name == superevents.SIGNIFICANT_LABEL:
             # ensure superevent is locked before starting alert workflow
+            r = chain()
             if superevents.FROZEN_LABEL not in alert['object']['labels']:
-                gracedb.create_label(superevents.FROZEN_LABEL, superevent_id)
+                r |= gracedb.create_label.si(superevents.FROZEN_LABEL,
+                                             superevent_id)
 
-            (
+            r |= (
                 gracedb.get_events.si(query)
                 |
                 superevents.select_preferred_event.s()
                 |
                 _update_superevent_and_return_event_dict.s(superevent_id)
                 |
                 _leave_log_message_and_return_event_dict.s(
@@ -161,15 +163,16 @@
                     superevent_id,
                     alert['object']['t_start'],
                     alert['object']['t_end']
                 )
                 |
                 earlywarning_preliminary_alert.s(
                     alert, alert_type='preliminary')
-            ).apply_async()
+            )
+            r.apply_async()
 
         # launch second preliminary on GCN_PRELIM_SENT
         elif label_name == 'GCN_PRELIM_SENT':
             (
                 identity.si().set(
                     # https://git.ligo.org/emfollow/gwcelery/-/issues/478
                     # FIXME: remove this task once https://github.com/celery/celery/issues/7851 is resolved  # noqa: E501
@@ -222,32 +225,35 @@
                 gracedb.upload.delay(
                     None, None, superevent_id,
                     "Superevent superseded by full BW event, skipping EW."
                 )
                 return
             # start the EW alert pipeline; is blocked by SIGNIF_LOCKED
             # ensure superevent is locked before starting pipeline
+            r = chain()
             if superevents.FROZEN_LABEL not in alert['object']['labels']:
-                gracedb.create_label(superevents.FROZEN_LABEL, superevent_id)
+                r |= gracedb.create_label.si(superevents.FROZEN_LABEL,
+                                             superevent_id)
 
-            (
+            r |= (
                 gracedb.get_events.si(query)
                 |
                 superevents.select_preferred_event.s()
                 |
                 _update_superevent_and_return_event_dict.s(superevent_id)
                 |
                 _leave_log_message_and_return_event_dict.s(
                     superevent_id,
                     "Superevent cleaned up before sending EW alert."
                 )
                 |
                 earlywarning_preliminary_alert.s(
                     alert, alert_type='earlywarning')
-            ).apply_async()
+            )
+            r.apply_async()
 
         # launch initial/retraction alert on ADVOK/ADVNO
         elif label_name == 'ADVOK':
             initial_alert((None, None, None), alert)
         elif label_name == 'ADVNO':
             retraction_alert(alert)
         elif label_name == 'ADVREQ':
```

### Comparing `gwcelery-2.1.2/gwcelery/tasks/p_astro.py` & `gwcelery-2.1.3/gwcelery/tasks/p_astro.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tasks/raven.py` & `gwcelery-2.1.3/gwcelery/tasks/raven.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tasks/rrt_utils.py` & `gwcelery-2.1.3/gwcelery/tasks/rrt_utils.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tasks/skymaps.py` & `gwcelery-2.1.3/gwcelery/tasks/skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tasks/superevents.py` & `gwcelery-2.1.3/gwcelery/tasks/superevents.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/templates/fits_header.jinja2` & `gwcelery-2.1.3/gwcelery/templates/fits_header.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/templates/index.jinja2` & `gwcelery-2.1.3/gwcelery/templates/index.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/templates/lalinference.jinja2` & `gwcelery-2.1.3/gwcelery/templates/lalinference.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/templates/rapidpe.jinja2` & `gwcelery-2.1.3/gwcelery/templates/rapidpe.jinja2`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/conftest.py` & `gwcelery-2.1.3/gwcelery/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/G000012_S0040_preferred.json` & `gwcelery-2.1.3/gwcelery/tests/data/G000012_S0040_preferred.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/G298048-1-Initial.xml` & `gwcelery-2.1.3/gwcelery/tests/data/G298048-1-Initial.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/G298048_log.json` & `gwcelery-2.1.3/gwcelery/tests/data/G298048_log.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json` & `gwcelery-2.1.3/gwcelery/tests/data/H1L1V1-pipeline-far_snr-thresholds.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/MS220722v.xml` & `gwcelery-2.1.3/gwcelery/tests/data/MS220722v.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits` & `gwcelery-2.1.3/gwcelery/tests/data/MS220722v_bayestar.multiorder.fits`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/S230413b.json` & `gwcelery-2.1.3/gwcelery/tests/data/S230413b.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/S230413g.json` & `gwcelery-2.1.3/gwcelery/tests/data/S230413g.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/S230413h.json` & `gwcelery-2.1.3/gwcelery/tests/data/S230413h.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/T0212_S0039_preferred.json` & `gwcelery-2.1.3/gwcelery/tests/data/T0212_S0039_preferred.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json` & `gwcelery-2.1.3/gwcelery/tests/data/T0212_S0039_preferred_single_ifo.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/T0219_S0041_nopreferred.json` & `gwcelery-2.1.3/gwcelery/tests/data/T0219_S0041_nopreferred.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/agile_grb_gcn.xml` & `gwcelery-2.1.3/gwcelery/tests/data/agile_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/coinc.xml` & `gwcelery-2.1.3/gwcelery/tests/data/coinc.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/externaltrigger_original_data.xml` & `gwcelery-2.1.3/gwcelery/tests/data/externaltrigger_original_data.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/fermi_grb_gcn.xml` & `gwcelery-2.1.3/gwcelery/tests/data/fermi_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/fermi_initial_grb_gcn.xml` & `gwcelery-2.1.3/gwcelery/tests/data/fermi_initial_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/fermi_noise_gcn.xml` & `gwcelery-2.1.3/gwcelery/tests/data/fermi_noise_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/fermi_noise_gcn_2.xml` & `gwcelery-2.1.3/gwcelery/tests/data/fermi_noise_gcn_2.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml` & `gwcelery-2.1.3/gwcelery/tests/data/fermi_subthresh_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml` & `gwcelery-2.1.3/gwcelery/tests/data/fermi_subthresh_grb_lowconfidence.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/fits_header_result.html` & `gwcelery-2.1.3/gwcelery/tests/data/fits_header_result.html`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/gracedb_externaltrigger_log.json` & `gwcelery-2.1.3/gwcelery/tests/data/gracedb_externaltrigger_log.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_detchar.json` & `gwcelery-2.1.3/gwcelery/tests/data/igwn_alert_detchar.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_exttrig_creation.json` & `gwcelery-2.1.3/gwcelery/tests/data/igwn_alert_exttrig_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json` & `gwcelery-2.1.3/gwcelery/tests/data/igwn_alert_exttrig_subgrb_targeted_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_psd.json` & `gwcelery-2.1.3/gwcelery/tests/data/igwn_alert_psd.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_snews_creation.json` & `gwcelery-2.1.3/gwcelery/tests/data/igwn_alert_snews_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_snews_test_creation.json` & `gwcelery-2.1.3/gwcelery/tests/data/igwn_alert_snews_test_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_subgrb_creation.json` & `gwcelery-2.1.3/gwcelery/tests/data/igwn_alert_subgrb_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_superevent_creation.json` & `gwcelery-2.1.3/gwcelery/tests/data/igwn_alert_superevent_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/igwn_alert_voevent.json` & `gwcelery-2.1.3/gwcelery/tests/data/igwn_alert_voevent.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/integral_grb_gcn.xml` & `gwcelery-2.1.3/gwcelery/tests/data/integral_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/integral_mdc_gcn.xml` & `gwcelery-2.1.3/gwcelery/tests/data/integral_mdc_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf` & `gwcelery-2.1.3/gwcelery/tests/data/llhoft/fail/L1/L-L1_O2_llhoft-1216577976-4.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/llhoft/idqbad/H1/H-H1_O2_llhoft-1216577976-4.gwf` & `gwcelery-2.1.3/gwcelery/tests/data/llhoft/idqbad/H1/H-H1_O2_llhoft-1216577976-4.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/llhoft/omegascan/scanme.gwf` & `gwcelery-2.1.3/gwcelery/tests/data/llhoft/omegascan/scanme.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf` & `gwcelery-2.1.3/gwcelery/tests/data/llhoft/pass/H1/H-H1_O2_llhoft-1216577976-4.gwf`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/lvalert_event_creation.json` & `gwcelery-2.1.3/gwcelery/tests/data/lvalert_event_creation.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/lvalert_xmpp.xml` & `gwcelery-2.1.3/gwcelery/tests/data/lvalert_xmpp.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/mock_superevent_object.json` & `gwcelery-2.1.3/gwcelery/tests/data/mock_superevent_object.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite` & `gwcelery-2.1.3/gwcelery/tests/data/p_astro_gstlal_trigger_db.sqlite`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/psd.xml.gz` & `gwcelery-2.1.3/gwcelery/tests/data/psd.xml.gz`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/rrt_small_area.fits` & `gwcelery-2.1.3/gwcelery/tests/data/rrt_small_area.fits`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/sample_events.json` & `gwcelery-2.1.3/gwcelery/tests/data/sample_events.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/samples.hdf5` & `gwcelery-2.1.3/gwcelery/tests/data/samples.hdf5`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/scaler_set_all.pickle` & `gwcelery-2.1.3/gwcelery/tests/data/scaler_set_all.pickle`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/snews_gcn.xml` & `gwcelery-2.1.3/gwcelery/tests/data/snews_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/snews_gcn_test.xml` & `gwcelery-2.1.3/gwcelery/tests/data/snews_gcn_test.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/superevents.json` & `gwcelery-2.1.3/gwcelery/tests/data/superevents.json`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/swift_grb_gcn.xml` & `gwcelery-2.1.3/gwcelery/tests/data/swift_grb_gcn.xml`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/data/test_classifier.pickle` & `gwcelery-2.1.3/gwcelery/tests/data/test_classifier.pickle`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/process.py` & `gwcelery-2.1.3/gwcelery/tests/process.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_sentry.py` & `gwcelery-2.1.3/gwcelery/tests/test_sentry.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tasks_alerts.py` & `gwcelery-2.1.3/gwcelery/tests/test_tasks_alerts.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tasks_alerts_validate.py` & `gwcelery-2.1.3/gwcelery/tests/test_tasks_alerts_validate.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tasks_bayestar.py` & `gwcelery-2.1.3/gwcelery/tests/test_tasks_bayestar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tasks_circulars.py` & `gwcelery-2.1.3/gwcelery/tests/test_tasks_circulars.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tasks_condor.py` & `gwcelery-2.1.3/gwcelery/tests/test_tasks_condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tasks_detchar.py` & `gwcelery-2.1.3/gwcelery/tests/test_tasks_detchar.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tasks_em_bright.py` & `gwcelery-2.1.3/gwcelery/tests/test_tasks_em_bright.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     assert res['HasMassGap'] == pytest.approx(0.0, abs=1e-3)
 
 
 @pytest.mark.parametrize(
         'posterior_samples,embright',
         [[[(1.2, 1.0, 0.0, 0.0, 100.0, 0.0, 0.0),
            (2.0, 0.5, 0.99, 0.99, 150.0, 0.0, 0.0)],
-          {'HasNS': 1.0, 'HasRemnant': 0.5, 'HasMassGap': 0.5}],
+          {'HasNS': 1.0, 'HasRemnant': 1.0, 'HasMassGap': 0.5}],
          [[(20., 12.0, 0.0, 0.0, 200.0, 0.0, 0.0),
            (22.0, 11.5, 0.80, 0.00, 250.0, 0.0, 0.0),
            (21.0, 10.0, 0.0, 0.0, 250, 0.0, 0.0)],
           {'HasNS': 0.0, 'HasRemnant': 0.0, 'HasMassGap': 0.0}]])
 def test_posterior_samples(posterior_samples, embright, socket_enabled):
     with NamedTemporaryFile() as f:
         filename = f.name
```

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tasks_external_skymaps.py` & `gwcelery-2.1.3/gwcelery/tests/test_tasks_external_skymaps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 from importlib import resources
 from unittest.mock import patch
 
 from astropy.table import Table
 import numpy as np
 import pytest
+from urllib.error import HTTPError
 
 from . import data
 from ..util import read_json
 from .test_tasks_skymaps import toy_fits_filecontents  # noqa: F401
 from .test_tasks_skymaps import toy_3d_fits_filecontents  # noqa: F401
 from ..tasks import external_skymaps
+from ..tasks import gracedb
 
 
 true_heasarc_link = ('http://heasarc.gsfc.nasa.gov/FTP/fermi/data/gbm/'
                      + 'triggers/2017/bn170817529/current/')
 true_skymap_link = true_heasarc_link + 'glg_healpix_all_bn170817529_v00.fit'
 
 
@@ -193,14 +195,36 @@
 @patch('urllib.request.urlopen')
 def test_get_external_skymap(mock_urlopen, search):
     """Assert that the correct call to astropy.get_file_contents is used"""
     external_skymaps.get_external_skymap(true_heasarc_link, search)
     mock_urlopen.assert_called_once()
 
 
+class File(object):
+    def close(self):
+        pass
+
+
+class HTTPError_404(object):
+    def __init__(self, *args, **kwargs):
+        pass
+
+    def read(self):
+        raise HTTPError('', 404, '', '', File)
+
+
+@pytest.mark.parametrize('search', ['GRB', 'SubGRB', 'FromURL'])
+@patch('urllib.request.urlopen', HTTPError_404)
+def test_get_external_skymap_404(search):
+    """Assert that when urllib.request raises 404 error, we raise
+    gracedb.RetryableHTTPError."""
+    with pytest.raises(gracedb.RetryableHTTPError):
+        external_skymaps.get_external_skymap(true_heasarc_link, search)
+
+
 @pytest.mark.parametrize('search', ['GRB', 'SubGRB', 'FromURL'])
 @patch('gwcelery.tasks.gracedb.upload.run')
 @patch('gwcelery.tasks.skymaps.plot_allsky.run')
 @patch('gwcelery.tasks.external_skymaps.get_external_skymap.run')
 @patch('gwcelery.tasks.external_skymaps.external_trigger_heasarc.run')
 def test_get_upload_external_skymap(mock_external_trigger_heasarc,
                                     mock_get_external_skymap,
@@ -308,7 +332,28 @@
     ext_event = {'graceid': graceid}
     external_skymaps.plot_overlap_integral(coinc_far_dict, superevent,
                                            ext_event)
     if expected_result:
         mock_upload.assert_called_once()
     else:
         mock_upload.assert_not_called()
+
+
+@patch('gwcelery.tasks.gracedb.upload.run')
+@patch('gwcelery.tasks.skymaps.plot_allsky.run')
+@patch('gwcelery.tasks.gracedb.create_label.run')
+def test_read_upload_skymap_from_base64(mock_create_label, mock_plot_allsky,
+                                        mock_gracedb_upload):
+    skymapb64 = read_json(
+                    data, 'kafka_alert_fermi.json'
+                )['healpix_file']
+    event = {'graceid': 'E1234',
+             'pipeline': 'Fermi',
+             'extra_attributes': {
+                 'GRB': {
+                     'ra': 14.5,
+                     'dec': -40.1}}}
+    external_skymaps.read_upload_skymap_from_base64(event, skymapb64)
+
+    mock_gracedb_upload.assert_called()
+    mock_plot_allsky.assert_called_once()
+    mock_create_label.assert_called_with('EXT_SKYMAP_READY', event['graceid'])
```

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tasks_external_triggers.py` & `gwcelery-2.1.3/gwcelery/tests/test_tasks_external_triggers.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,15 +91,15 @@
          'links': {
              'self': 'https://gracedb.ligo.org/events/E356793/'
                   }
          },
         gcn_type_dict[pipeline], time_dict[pipeline])
 
 
-@patch('gwcelery.tasks.gracedb.get_events', return_value=[])
+@patch('gwcelery.tasks.gracedb.get_events.run', return_value=[])
 @patch('gwcelery.tasks.gracedb.create_event.run', return_value={
     'graceid': 'E1', 'gpstime': 1, 'instruments': '', 'pipeline': 'Fermi',
     'search': 'SubGRB',
     'extra_attributes': {'GRB': {'trigger_duration': None, 'trigger_id': 123,
                                  'ra': 0., 'dec': 0., 'error_radius': 10.}},
     'links': {'self': 'https://gracedb.ligo.org/events/E356793/'}})
 @patch('gwcelery.tasks.detchar.check_vectors.run')
@@ -135,15 +135,15 @@
          'gbm_subthresh_578679393.215999_healpix.fits'))
 
 
 @pytest.mark.parametrize('filename',
                          ['fermi_noise_gcn.xml',
                           'fermi_noise_gcn_2.xml'])
 @patch('gwcelery.tasks.external_skymaps.get_upload_external_skymap.run')
-@patch('gwcelery.tasks.gracedb.get_events', return_value=[])
+@patch('gwcelery.tasks.gracedb.get_events.run', return_value=[])
 @patch('gwcelery.tasks.gracedb.create_event.run', return_value={
     'graceid': 'E1', 'gpstime': 1, 'instruments': '', 'pipeline': 'Fermi',
     'search': 'GRB',
     'extra_attributes': {'GRB': {'trigger_duration': 1, 'trigger_id': 123,
                                  'ra': 0., 'dec': 0., 'error_radius': 10.}},
     'links': {'self': 'https://gracedb.ligo.org/events/E356793/'}})
 @patch('gwcelery.tasks.detchar.check_vectors.run')
@@ -166,15 +166,15 @@
                                               labels=['NOT_GRB'])
     mock_check_vectors.assert_called_once()
     mock_get_upload_external_skymap.assert_called_once()
 
 
 @patch('gwcelery.tasks.external_skymaps.create_external_skymap')
 @patch('gwcelery.tasks.external_skymaps.get_upload_external_skymap.run')
-@patch('gwcelery.tasks.gracedb.get_events', return_value=[])
+@patch('gwcelery.tasks.gracedb.get_events.run', return_value=[])
 @patch('gwcelery.tasks.gracedb.create_event.run', return_value={
     'graceid': 'E1', 'gpstime': 1, 'instruments': '', 'pipeline': 'Fermi',
     'search': 'GRB',
     'extra_attributes': {'GRB': {'trigger_duration': 1, 'trigger_id': 123,
                                  'ra': 0., 'dec': 0., 'error_radius': 0.}},
     'links': {'self': 'https://gracedb.ligo.org/events/E356793/'}})
 @patch('gwcelery.tasks.detchar.check_vectors.run')
@@ -211,15 +211,15 @@
 @patch('gwcelery.tasks.gracedb.replace_event.run')
 @patch('gwcelery.tasks.gracedb.get_event.run', return_value=[{
     'graceid': 'E1', 'gpstime': 1, 'instruments': '', 'pipeline': 'Fermi',
     'search': 'GRB',
     'extra_attributes': {'GRB': {'trigger_duration': 1, 'trigger_id': 123,
                                  'ra': 0., 'dec': 0., 'error_radius': 10.}},
     'links': {'self': 'https://gracedb.ligo.org/events/E356793/'}}])
-@patch('gwcelery.tasks.gracedb.get_events', return_value=[{
+@patch('gwcelery.tasks.gracedb.get_events.run', return_value=[{
     'graceid': 'E1', 'gpstime': 1, 'instruments': '', 'pipeline': 'Fermi',
     'search': 'GRB',
     'extra_attributes': {'GRB': {'trigger_duration': 1, 'trigger_id': 123,
                                  'ra': 0., 'dec': 0., 'error_radius': 15.}},
     'links': {'self': 'https://gracedb.ligo.org/events/E356793/'}}])
 def test_handle_replace_grb_event(mock_get_event,
                                   mock_get_events,
@@ -570,15 +570,16 @@
 def test_handle_create_snews_event(mock_create_event,
                                    mock_upload, mock_json):
     text = resources.read_binary(data, 'snews_gcn.xml')
     external_triggers.handle_snews_gcn(payload=text)
     mock_create_event.assert_called_once_with(filecontents=text,
                                               search='Supernova',
                                               pipeline='SNEWS',
-                                              group='External')
+                                              group='External',
+                                              labels=None)
     calls = [
         call(
             '"dqrjson"', 'gwcelerydetcharcheckvectors-E1.json', 'E1',
             'DQR-compatible json generated from check_vectors results'),
         call(
             None, None, 'E1',
             ('Detector state for active instruments is unknown.\n{}'
@@ -595,16 +596,20 @@
                       'V1:GOOD_DATA_QUALITY_CAT1'])),
             ['data_quality'])
     ]
     mock_upload.assert_has_calls(calls, any_order=True)
 
 
 @patch('gwcelery.tasks.gracedb.replace_event.run')
-@patch('gwcelery.tasks.gracedb.get_events', return_value=[{'graceid': 'E1'}])
-def test_handle_replace_snews_event(mock_get_events, mock_replace_event):
+@patch('gwcelery.tasks.gracedb.remove_label.run')
+@patch('gwcelery.tasks.gracedb.get_events.run',
+       return_value=[{'graceid': 'E1', 'search': 'Supernova', 'gpstime': 100,
+                      'pipeline': 'SNEWS'}])
+def test_handle_replace_snews_event(mock_get_events, mock_remove_label,
+                                    mock_replace_event):
     text = resources.read_binary(data, 'snews_gcn.xml')
     external_triggers.handle_snews_gcn(payload=text)
     mock_replace_event.assert_called_once_with('E1', text)
 
 
 @patch('gwcelery.tasks.raven.coincidence_search')
 def test_handle_grb_exttrig_creation(mock_raven_coincidence_search):
@@ -644,18 +649,14 @@
     """Test dispatch of an IGWN alert message for an exttrig creation."""
     # Test IGWN alert payload.
     alert = read_json(data, 'igwn_alert_exttrig_subgrb_targeted_creation.json')
 
     # Run function under test
     external_triggers.handle_grb_igwn_alert(alert)
 
-    # Check that sky map is uploaded
-    mock_create_upload_external_skymap.assert_called_once_with(
-        alert['object'], None, alert['object']['created'])
-
     # Check that the correct tasks were dispatched.
     mock_raven_coincidence_search.assert_has_calls([
         call('E1234', alert['object'], group='Burst', se_searches=['Allsky']),
         call('E1234', alert['object'], group='CBC',
              searches=['SubGRB', 'SubGRBTargeted'],
              pipelines=['Swift'])])
 
@@ -736,14 +737,120 @@
 
     # Check that the correct tasks were dispatched.
     mock_raven_coincidence_search.assert_has_calls([
         call('S180616h', alert['object'], group='Burst', searches=['GRB'],
              se_searches=['Allsky'])])
 
 
+def _mock_get_events(query):
+    if "12345" in query:
+        return [{"graceid": "E12345", "search": "SubGRBTargeted"}]
+    else:
+        return {}
+
+
+@pytest.mark.parametrize('alert_type',
+                         ['initial', 'update', 'retraction'])
+@pytest.mark.parametrize('kafka_path',
+                         ['kafka_alert_fermi.json',
+                          'kafka_alert_swift.json',
+                          'kafka_alert_swift_noloc.json',
+                          'kafka_alert_swift_wskymap.json'])
+@patch('gwcelery.tasks.gracedb.create_event.run', return_value={
+    'graceid': 'E12345', 'gpstime': 100, 'pipeline': 'Fermi',
+    'extra_attributes': {'GRB': {'trigger_duration': 1, 'trigger_id': 123,
+                                 'ra': 10., 'dec': 20., 'error_radius': 10.}}})
+@patch('gwcelery.tasks.external_skymaps.create_upload_external_skymap.run')
+@patch('gwcelery.tasks.external_skymaps.get_upload_external_skymap.run')
+@patch('gwcelery.tasks.external_skymaps.read_upload_skymap_from_base64.run')
+@patch('gwcelery.tasks.gracedb.replace_event.run')
+@patch('gwcelery.tasks.gracedb.get_event.run',
+       return_value={'graceid': 'E12345'})
+@patch('gwcelery.tasks.gracedb.create_label.run')
+@patch('gwcelery.tasks.gracedb.get_events.run', side_effect=_mock_get_events)
+@patch('gwcelery.tasks.detchar.check_vectors.run')
+@patch('gwcelery.tasks.gracedb.upload.run')
+@patch('gwcelery.tasks.skymaps.plot_allsky.run')
+def test_handle_targeted_kafka_alert(mock_plot_allsky,
+                                     mock_gracedb_upload,
+                                     mock_check_vectors,
+                                     mock_get_events,
+                                     mock_create_label,
+                                     mock_get_event,
+                                     mock_replace_event,
+                                     mock_read_upload_skymap_from_base64,
+                                     mock_get_upload_external_skymap,
+                                     mock_create_upload_external_skymap,
+                                     mock_create_event,
+                                     alert_type, kafka_path):
+
+    alert = read_json(data, kafka_path)
+    alert["alert_type"] = alert_type
+    voevent_path = '{}_subgrbtargeted_template.xml'.format(
+        'fermi' if 'fermi' in kafka_path else 'swift')
+    no_loc = 'noloc' in kafka_path
+    replace_event = alert_type in ['update', 'retraction']
+    pipeline = 'Fermi' if 'fermi' in kafka_path else 'Swift'
+    # Update VOEvent with sky localization info or ID if needed
+    if no_loc or replace_event:
+        with resources.path(data, voevent_path) as p:
+            fname = str(p)
+        root = etree.parse(fname)
+        if no_loc:
+            # Set template to also be zeros if nothing in kafka alert
+            root.find(("./WhereWhen/ObsDataLocation/"
+                       "ObservationLocation/AstroCoords/Position2D/Value2/"
+                       "C1")).text = str(0.).encode()
+            root.find(("./WhereWhen/ObsDataLocation/"
+                       "ObservationLocation/AstroCoords/Position2D/Value2/"
+                       "C2")).text = str(0.).encode()
+            root.find(("./WhereWhen/ObsDataLocation/"
+                       "ObservationLocation/AstroCoords/Position2D/"
+                       "Error2Radius")).text = str(0.).encode()
+        if replace_event:
+            # Update ID so we can find a previous event and replace it
+            new_id = "12345"
+            root.find("./What/Param[@name='TrigID']").attrib['value'] = \
+                new_id.encode()
+            alert["id"] = [new_id]
+        text = etree.tostring(root, xml_declaration=True, encoding="UTF-8")
+        # Add back removed newline
+        text += b'\n'
+    # If no changes needed, read the file directly
+    else:
+        text = resources.read_binary(data, voevent_path)
+
+    # Send alert through handler
+    external_triggers.handle_targeted_kafka_alert(alert)
+
+    # Check either event was created or updated based on alert type
+    if replace_event:
+        mock_replace_event.assert_called_once_with("E12345", text)
+    else:
+        mock_create_event.assert_called_once_with(filecontents=text,
+                                                  search='SubGRBTargeted',
+                                                  pipeline=pipeline,
+                                                  group='External',
+                                                  labels=None)
+
+    # Ensure correct localization method used
+    if pipeline == 'Fermi' or 'wskymap' in kafka_path:
+        mock_read_upload_skymap_from_base64.assert_called()
+    elif 'noloc' in kafka_path:
+        mock_read_upload_skymap_from_base64.assert_not_called()
+        mock_create_upload_external_skymap.assert_not_called()
+    else:
+        mock_create_upload_external_skymap.assert_called_once()
+
+    if alert_type == "retraction":
+        mock_create_label.assert_called_once_with("NOT_GRB", "E12345")
+    else:
+        mock_create_label.assert_not_called()
+
+
 @pytest.mark.parametrize('path',
                          ['igwn_alert_superevent_creation.json',
                           'igwn_alert_exttrig_creation.json'])
 @patch('gwcelery.tasks.raven.coincidence_search')
 def test_handle_mdc_creation(mock_raven_coincidence_search,
                              path):
     """Test dispatch of an IGWN alert message for a CBC superevent creation."""
```

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tasks_first2years.py` & `gwcelery-2.1.3/gwcelery/tests/test_tasks_first2years.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tasks_first2years_external.py` & `gwcelery-2.1.3/gwcelery/tests/test_tasks_first2years_external.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     monkeypatch.setattr(
         'gwcelery.tasks.external_skymaps.get_upload_external_skymap.run',
         mock_get_upload_external_skymap)
     monkeypatch.setattr('gwcelery.tasks.detchar.check_vectors.run',
                         mock_check_vectors)
     monkeypatch.setattr('gwcelery.tasks.gracedb.create_event.run',
                         mock_create_event)
-    monkeypatch.setattr('gwcelery.tasks.gracedb.get_events',
+    monkeypatch.setattr('gwcelery.tasks.gracedb.get_events.run',
                         mock_get_events)
     monkeypatch.setattr(app.conf, 'gracedb_host', host)
     if group == 'Test':
         with pytest.raises(AssertionError):
             first2years_external.upload_external_event(alert)
         res = None
     else:
@@ -91,18 +91,19 @@
 
 
 @patch('gwcelery.tasks.detchar.check_vectors.run')
 @patch('gwcelery.tasks.gracedb.create_event.run', return_value={
     'graceid': 'M1', 'gpstime': 1, 'instruments': '', 'pipeline': 'SNEWS',
     'search': 'MDC',
     'links': {'self': 'https://gracedb.ligo.org/events/E356793/'}})
-@patch('gwcelery.tasks.gracedb.get_events', return_value=[])
+@patch('gwcelery.tasks.gracedb.get_events.run', return_value=[])
 def test_upload_snews_event(mock_get_events,
                             mock_create_event,
                             mock_check_vectors):
     event = first2years_external.upload_snews_event()
     mock_create_event.assert_called_once_with(
         filecontents=event,
         search='MDC',
         pipeline='SNEWS',
-        group='External')
+        group='External',
+        labels=None)
     mock_check_vectors.assert_called_once()
```

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tasks_gcn.py` & `gwcelery-2.1.3/gwcelery/tests/test_tasks_gcn.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tasks_gcn_validate.py` & `gwcelery-2.1.3/gwcelery/tests/test_tasks_gcn_validate.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tasks_gracedb.py` & `gwcelery-2.1.3/gwcelery/tests/test_tasks_gracedb.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tasks_gwskynet.py` & `gwcelery-2.1.3/gwcelery/tests/test_tasks_gwskynet.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tasks_igwn_alert.py` & `gwcelery-2.1.3/gwcelery/tests/test_tasks_igwn_alert.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tasks_inference.py` & `gwcelery-2.1.3/gwcelery/tests/test_tasks_inference.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tasks_orchestrator.py` & `gwcelery-2.1.3/gwcelery/tests/test_tasks_orchestrator.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,18 @@
      ['label_added', 'LOW_SIGNIF_PRELIM_SENT', 'CBC', 'gstlal', False, 1.e-9,
          ['H1', 'L1', 'V1'], 'S1234', ['EM_SelectedConfident']],
      ['label_added', 'LOW_SIGNIF_PRELIM_SENT', 'CBC', 'gstlal', False, 1.e-7,
          ['H1', 'L1', 'V1'], 'S1234', ['EM_Selected']],
      ['new', '', 'CBC', 'gstlal', False, 1.e-9, ['H1', 'L1'], 'S1234',
          ['LOW_SIGNIF_LOCKED']],
      ['label_added', 'EARLY_WARNING', 'CBC', 'gstlal', False, 1.e-10,
+         ['H1', 'L1', 'V1'], 'S1234', []],
+     ['label_added', 'EARLY_WARNING', 'CBC', 'gstlal', False, 1.e-10,
+         ['H1', 'L1', 'V1'], 'S1234', ['SIGNIF_LOCKED']],
+     ['label_added', 'SIGNIF_LOCKED', 'CBC', 'gstlal', False, 1.e-10,
          ['H1', 'L1', 'V1'], 'S1234', []]])
 def test_handle_superevent(monkeypatch, toy_3d_fits_filecontents,  # noqa: F811
                            alert_type, alert_label, group, pipeline,
                            offline, far, instruments, superevent_id,
                            superevent_labels):
     """Test a superevent is dispatched to the correct annotation task based on
     its preferred event's search group.
@@ -249,14 +253,17 @@
         update_superevent_task.assert_called_once()
         select_pipeline_preferred_event_task.assert_called_once()
         assert add_pipeline_preferred_event_task.call_count == len(
             select_pipeline_preferred_event_task.return_value
         )
 
     elif alert_label == 'SIGNIF_LOCKED':
+        if superevents.FROZEN_LABEL not in superevent_labels:
+            create_label.assert_has_calls(
+                [call(superevents.FROZEN_LABEL, superevent_id)])
         annotate_fits.assert_called_once()
         _event_info = get_event('G1234')  # this gets the preferred event info
         assert superevents.should_publish(_event_info)
         expose.assert_called_once_with(superevent_id)
         create_tag.assert_has_calls(
             [call('S1234-1-Preliminary.xml', 'public', superevent_id),
              call('em-bright-filename', 'public', superevent_id),
```

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tasks_p_astro.py` & `gwcelery-2.1.3/gwcelery/tests/test_tasks_p_astro.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tasks_raven.py` & `gwcelery-2.1.3/gwcelery/tests/test_tasks_raven.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tasks_rrt_utils.py` & `gwcelery-2.1.3/gwcelery/tests/test_tasks_rrt_utils.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tasks_skymaps.py` & `gwcelery-2.1.3/gwcelery/tests/test_tasks_skymaps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tasks_superevents.py` & `gwcelery-2.1.3/gwcelery/tests/test_tasks_superevents.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tempfile.py` & `gwcelery-2.1.3/gwcelery/tests/test_tempfile.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tools_condor.py` & `gwcelery-2.1.3/gwcelery/tests/test_tools_condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tools_condor_submit_helper.py` & `gwcelery-2.1.3/gwcelery/tests/test_tools_condor_submit_helper.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tools_flask.py` & `gwcelery-2.1.3/gwcelery/tests/test_tools_flask.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_tools_nagios.py` & `gwcelery-2.1.3/gwcelery/tests/test_tools_nagios.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tests/test_views.py` & `gwcelery-2.1.3/gwcelery/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tools/condor.py` & `gwcelery-2.1.3/gwcelery/tools/condor.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tools/condor_submit_helper.py` & `gwcelery-2.1.3/gwcelery/tools/condor_submit_helper.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tools/flask.py` & `gwcelery-2.1.3/gwcelery/tools/flask.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/tools/nagios.py` & `gwcelery-2.1.3/gwcelery/tools/nagios.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/util/cmdline.py` & `gwcelery-2.1.3/gwcelery/util/cmdline.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/util/resources.py` & `gwcelery-2.1.3/gwcelery/util/resources.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/util/tempfile.py` & `gwcelery-2.1.3/gwcelery/util/tempfile.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/views.py` & `gwcelery-2.1.3/gwcelery/views.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/voevent/bootsteps.py` & `gwcelery-2.1.3/gwcelery/voevent/bootsteps.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/voevent/logging.py` & `gwcelery-2.1.3/gwcelery/voevent/logging.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/voevent/signals.py` & `gwcelery-2.1.3/gwcelery/voevent/signals.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/voevent/subscriber.py` & `gwcelery-2.1.3/gwcelery/voevent/subscriber.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/gwcelery/voevent/util.py` & `gwcelery-2.1.3/gwcelery/voevent/util.py`

 * *Files identical despite different names*

### Comparing `gwcelery-2.1.2/pyproject.toml` & `gwcelery-2.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gwcelery"
-version = "2.1.2"
+version = "2.1.3"
 description = "Low-latency pipeline for annotating IGWN events"
 readme = "README.rst"
 authors = [
     "Deep Chatterjee <deep.chatterjee@ligo.org>",
     "Cody Messick <cody.messick@ligo.org>",
     "Geoffrey Mo <geoffrey.mo@ligo.org>",
     "Leo Singer <leo.singer@ligo.org>"
@@ -71,19 +71,19 @@
 hop-client = ">=0.7.0"  # https://github.com/scimma/hop-client/pull/176
 igwn-alert = ">=0.2.2"
 igwn-gwalert-schema = "^1.0.0"
 imapclient = "*"
 importlib-metadata = { version = "*"}
 jinja2 = ">=2.11.2"  # https://github.com/pallets/jinja/issues/1168
 lalsuite = ">=7.15"  # https://git.ligo.org/lscsoft/lalsuite/-/merge_requests/2120
-ligo-followup-advocate = ">=1.2.3"
+ligo-followup-advocate = ">=1.2.4"
 ligo-gracedb = ">=2.7.5"  # https://git.ligo.org/lscsoft/gracedb-client/-/issues/28
 ligo-raven = ">=3.2"
 ligo-segments = "*"
-"ligo.em-bright" = ">=1.1.3"  # https://git.ligo.org/emfollow/em-properties/em-bright/-/issues/34
+"ligo.em-bright" = ">=1.1.4.post2"  # https://git.ligo.org/emfollow/gwcelery/-/issues/653
 "ligo.skymap" = ">=1.0.4"  # https://git.ligo.org/lscsoft/ligo.skymap/-/merge_requests/299
 lscsoft-glue = "*"
 lxml = "*"
 matplotlib = "<3.7"  # Matplotlib changed an axes behaviour which breaks some of our plotting scripts. When gwpy has a new release, we can unpin this.
 numba = ">=0.56"  # Poetry update chooses an old version of numba and its deps that break the python3.9 and 3.10 build tests if this is not specified; dependence on numba comes from rift. Version chosen because it adds python 3.10 support. This requirement can be dropped here if RIFT adds it https://git.ligo.org/rapidpe-rift/rift/-/issues/24
 numpy = "*"
 p_astro = ">=1.0.1"  # https://git.ligo.org/lscsoft/p-astro/-/merge_requests/40
```

### Comparing `gwcelery-2.1.2/PKG-INFO` & `gwcelery-2.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwcelery
-Version: 2.1.2
+Version: 2.1.3
 Summary: Low-latency pipeline for annotating IGWN events
 Home-page: https://git.ligo.org/emfollow/gwcelery
 License: GPL-2.0+
 Author: Deep Chatterjee
 Author-email: deep.chatterjee@ligo.org
 Requires-Python: >=3.9,<3.11
 Classifier: Development Status :: 4 - Beta
@@ -42,20 +42,20 @@
 Requires-Dist: hop-client (>=0.7.0)
 Requires-Dist: igwn-alert (>=0.2.2)
 Requires-Dist: igwn-gwalert-schema (>=1.0.0,<2.0.0)
 Requires-Dist: imapclient
 Requires-Dist: importlib-metadata
 Requires-Dist: jinja2 (>=2.11.2)
 Requires-Dist: lalsuite (>=7.15)
-Requires-Dist: ligo-followup-advocate (>=1.2.3)
+Requires-Dist: ligo-followup-advocate (>=1.2.4)
 Requires-Dist: ligo-gracedb (>=2.7.5)
 Requires-Dist: ligo-raven (>=3.2)
 Requires-Dist: ligo-rrt-chat (>=0.1.1)
 Requires-Dist: ligo-segments
-Requires-Dist: ligo.em-bright (>=1.1.3)
+Requires-Dist: ligo.em-bright (>=1.1.4.post2)
 Requires-Dist: ligo.skymap (>=1.0.4)
 Requires-Dist: lscsoft-glue
 Requires-Dist: lxml
 Requires-Dist: matplotlib (<3.7)
 Requires-Dist: numba (>=0.56)
 Requires-Dist: numpy
 Requires-Dist: p_astro (>=1.0.1)
```

