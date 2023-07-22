# Comparing `tmp/jaxip-0.7.1.tar.gz` & `tmp/jaxip-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxip-0.7.1.tar", last modified: Sat Jul 15 14:24:53 2023, max compression
+gzip compressed data, was "jaxip-0.7.2.tar", last modified: Sat Jul 22 19:34:47 2023, max compression
```

## Comparing `jaxip-0.7.1.tar` & `jaxip-0.7.2.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.847498 jaxip-0.7.1/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      166 2022-12-07 19:09:20.000000 jaxip-0.7.1/AUTHORS.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3491 2023-04-26 21:18:43.000000 jaxip-0.7.1/CONTRIBUTING.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      829 2023-07-15 14:24:44.000000 jaxip-0.7.1/HISTORY.rst
--rw-r--r--   0 hossein   (1000) hossein   (1000)     1523 2023-01-05 20:40:22.000000 jaxip-0.7.1/LICENSE
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      262 2022-12-07 20:18:56.000000 jaxip-0.7.1/MANIFEST.in
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5671 2023-07-15 14:24:53.847498 jaxip-0.7.1/PKG-INFO
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5084 2023-07-15 14:24:44.000000 jaxip-0.7.1/README.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.775498 jaxip-0.7.1/docs/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      606 2023-02-01 19:45:48.000000 jaxip-0.7.1/docs/Makefile
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.747497 jaxip-0.7.1/docs/_build/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.743497 jaxip-0.7.1/docs/_build/doctrees/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.779498 jaxip-0.7.1/docs/_build/doctrees/nbsphinx/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-07-15 14:16:39.000000 jaxip-0.7.1/docs/_build/doctrees/nbsphinx/notebooks_getting_started_38_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-07-15 14:16:39.000000 jaxip-0.7.1/docs/_build/doctrees/nbsphinx/notebooks_getting_started_45_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-07-15 14:16:39.000000 jaxip-0.7.1/docs/_build/doctrees/nbsphinx/notebooks_getting_started_51_0.png
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.747497 jaxip-0.7.1/docs/_build/html/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.783498 jaxip-0.7.1/docs/_build/html/_images/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-07-15 14:16:39.000000 jaxip-0.7.1/docs/_build/html/_images/notebooks_getting_started_38_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-07-15 14:16:39.000000 jaxip-0.7.1/docs/_build/html/_images/notebooks_getting_started_45_0.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-07-15 14:16:39.000000 jaxip-0.7.1/docs/_build/html/_images/notebooks_getting_started_51_0.png
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.783498 jaxip-0.7.1/docs/_build/html/_static/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      286 2023-04-26 21:14:06.000000 jaxip-0.7.1/docs/_build/html/_static/file.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.7.1/docs/_build/html/_static/minus.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.7.1/docs/_build/html/_static/plus.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-28 08:07:09.000000 jaxip-0.7.1/docs/authors.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     6459 2023-07-15 14:24:44.000000 jaxip-0.7.1/docs/conf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       33 2022-12-07 19:09:20.000000 jaxip-0.7.1/docs/contributing.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       77 2023-07-10 18:19:00.000000 jaxip-0.7.1/docs/examples.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-07 19:09:20.000000 jaxip-0.7.1/docs/history.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.783498 jaxip-0.7.1/docs/images/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    44314 2023-03-28 20:24:39.000000 jaxip-0.7.1/docs/images/flowchart.drawio.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    96759 2023-02-06 19:53:40.000000 jaxip-0.7.1/docs/images/water.png
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      315 2023-05-06 13:11:44.000000 jaxip-0.7.1/docs/index.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1864 2023-04-26 21:18:43.000000 jaxip-0.7.1/docs/installation.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      760 2023-07-15 14:16:29.000000 jaxip-0.7.1/docs/jaxip.atoms.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      495 2023-07-15 14:24:44.000000 jaxip-0.7.1/docs/jaxip.datasets.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1095 2023-07-15 14:16:30.000000 jaxip-0.7.1/docs/jaxip.descriptors.acsf.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      613 2023-07-15 14:16:30.000000 jaxip-0.7.1/docs/jaxip.descriptors.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      686 2023-07-15 14:16:30.000000 jaxip-0.7.1/docs/jaxip.models.nn.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      400 2023-07-15 14:16:30.000000 jaxip-0.7.1/docs/jaxip.models.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1290 2023-07-15 14:16:30.000000 jaxip-0.7.1/docs/jaxip.potentials.nnp.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      464 2023-07-15 14:16:30.000000 jaxip-0.7.1/docs/jaxip.potentials.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      961 2023-07-15 14:16:29.000000 jaxip-0.7.1/docs/jaxip.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      951 2023-07-15 14:16:30.000000 jaxip-0.7.1/docs/jaxip.simulation.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      915 2023-07-15 14:16:30.000000 jaxip-0.7.1/docs/jaxip.utils.rst
--rw-r--r--   0 hossein   (1000) hossein   (1000)      803 2023-01-05 20:40:22.000000 jaxip-0.7.1/docs/make.bat
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       52 2023-07-15 14:16:30.000000 jaxip-0.7.1/docs/modules.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       27 2022-12-20 21:49:36.000000 jaxip-0.7.1/docs/readme.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3833 2023-05-06 13:11:44.000000 jaxip-0.7.1/docs/theory.rst
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1158 2023-04-26 21:18:43.000000 jaxip-0.7.1/docs/usage.rst
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.787498 jaxip-0.7.1/jaxip/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      575 2023-05-06 13:11:44.000000 jaxip-0.7.1/jaxip/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      294 2023-07-15 14:24:44.000000 jaxip-0.7.1/jaxip/_version.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.799498 jaxip-0.7.1/jaxip/atoms/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      232 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/atoms/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1486 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/atoms/_structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3683 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/atoms/box.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     6639 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/atoms/element.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3354 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/atoms/neighbor.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    17758 2023-07-15 14:24:44.000000 jaxip-0.7.1/jaxip/atoms/structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1124 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/config.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.803498 jaxip-0.7.1/jaxip/datasets/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       84 2023-07-15 14:24:44.000000 jaxip-0.7.1/jaxip/datasets/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      408 2023-05-17 19:30:18.000000 jaxip-0.7.1/jaxip/datasets/dataset.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     6494 2023-07-15 14:24:44.000000 jaxip-0.7.1/jaxip/datasets/runner.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.807498 jaxip-0.7.1/jaxip/descriptors/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      130 2023-05-01 12:41:07.000000 jaxip-0.7.1/jaxip/descriptors/__init__.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.815498 jaxip-0.7.1/jaxip/descriptors/acsf/
--rw-r--r--   0 hossein   (1000) hossein   (1000)      400 2023-01-05 20:40:22.000000 jaxip-0.7.1/jaxip/descriptors/acsf/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5312 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/descriptors/acsf/_acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     7828 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/descriptors/acsf/acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2236 2023-05-17 19:30:18.000000 jaxip-0.7.1/jaxip/descriptors/acsf/angular.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2627 2023-05-17 19:30:18.000000 jaxip-0.7.1/jaxip/descriptors/acsf/cutoff.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1495 2023-05-17 19:30:18.000000 jaxip-0.7.1/jaxip/descriptors/acsf/radial.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1015 2023-05-17 19:30:18.000000 jaxip-0.7.1/jaxip/descriptors/acsf/symmetry.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      616 2023-05-17 19:30:18.000000 jaxip-0.7.1/jaxip/descriptors/descriptor.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     7467 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/descriptors/scaler.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3739 2023-05-01 12:41:07.000000 jaxip-0.7.1/jaxip/logger.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.815498 jaxip-0.7.1/jaxip/models/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       88 2023-05-08 16:51:03.000000 jaxip-0.7.1/jaxip/models/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      389 2023-05-17 19:30:18.000000 jaxip-0.7.1/jaxip/models/model.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.819498 jaxip-0.7.1/jaxip/models/nn/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      181 2023-05-08 16:51:03.000000 jaxip-0.7.1/jaxip/models/nn/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1125 2023-05-08 16:51:03.000000 jaxip-0.7.1/jaxip/models/nn/activation.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      604 2023-05-08 16:51:03.000000 jaxip-0.7.1/jaxip/models/nn/initializer.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2879 2023-07-15 14:24:44.000000 jaxip-0.7.1/jaxip/models/nn/network.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.823498 jaxip-0.7.1/jaxip/potentials/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      212 2023-05-17 19:30:18.000000 jaxip-0.7.1/jaxip/potentials/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1979 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/potentials/_energy.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      866 2023-05-01 12:41:07.000000 jaxip-0.7.1/jaxip/potentials/_force.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1844 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/potentials/atomic_potential.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.827498 jaxip-0.7.1/jaxip/potentials/nnp/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      238 2023-05-17 19:30:18.000000 jaxip-0.7.1/jaxip/potentials/nnp/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     9522 2023-07-15 14:24:44.000000 jaxip-0.7.1/jaxip/potentials/nnp/gradient_descent.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     9374 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/potentials/nnp/kalman_filter.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2576 2023-05-01 12:41:07.000000 jaxip-0.7.1/jaxip/potentials/nnp/metrics.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      542 2023-06-24 19:26:34.000000 jaxip-0.7.1/jaxip/potentials/nnp/nnp.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    19007 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/potentials/nnp/potential.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)    11345 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/potentials/nnp/settings.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3627 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/pytree.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.831498 jaxip-0.7.1/jaxip/simulation/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      296 2023-06-24 19:26:34.000000 jaxip-0.7.1/jaxip/simulation/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2143 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/simulation/lj.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4331 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/simulation/mc.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     9132 2023-07-15 14:24:44.000000 jaxip-0.7.1/jaxip/simulation/md.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2515 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/simulation/run.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      840 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/simulation/thermostat.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      766 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/types.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2573 2023-06-18 10:02:01.000000 jaxip-0.7.1/jaxip/units.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.835498 jaxip-0.7.1/jaxip/utils/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       73 2023-05-01 12:41:07.000000 jaxip-0.7.1/jaxip/utils/__init__.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1418 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/utils/attribute.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      585 2023-05-01 12:41:07.000000 jaxip-0.7.1/jaxip/utils/batch.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2012 2023-07-10 18:19:00.000000 jaxip-0.7.1/jaxip/utils/compare.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4410 2023-05-01 12:41:07.000000 jaxip-0.7.1/jaxip/utils/profiler.py
--rw-r--r--   0 hossein   (1000) hossein   (1000)      670 2023-01-18 21:30:52.000000 jaxip-0.7.1/jaxip/utils/tokenize.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.791498 jaxip-0.7.1/jaxip.egg-info/
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5671 2023-07-15 14:24:53.000000 jaxip-0.7.1/jaxip.egg-info/PKG-INFO
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3265 2023-07-15 14:24:53.000000 jaxip-0.7.1/jaxip.egg-info/SOURCES.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-07-15 14:24:53.000000 jaxip-0.7.1/jaxip.egg-info/dependency_links.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       41 2023-07-15 14:24:53.000000 jaxip-0.7.1/jaxip.egg-info/entry_points.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-07-15 14:24:23.000000 jaxip-0.7.1/jaxip.egg-info/not-zip-safe
--rw-rw-r--   0 hossein   (1000) hossein   (1000)       85 2023-07-15 14:24:53.000000 jaxip-0.7.1/jaxip.egg-info/requires.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)        6 2023-07-15 14:24:53.000000 jaxip-0.7.1/jaxip.egg-info/top_level.txt
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      137 2023-07-15 14:24:53.847498 jaxip-0.7.1/setup.cfg
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     1661 2023-03-22 21:56:02.000000 jaxip-0.7.1/setup.py
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.843498 jaxip-0.7.1/tests/
-drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-15 14:24:53.847498 jaxip-0.7.1/tests/.ipynb_checkpoints/
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.7.1/tests/.ipynb_checkpoints/h2o-checkpoint.data
--rw-r--r--   0 hossein   (1000) hossein   (1000)     9543 2023-01-26 17:53:14.000000 jaxip-0.7.1/tests/.ipynb_checkpoints/h2o-checkpoint.json
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-26 17:32:00.000000 jaxip-0.7.1/tests/.ipynb_checkpoints/input.h2o-checkpoint.data
--rw-r--r--   0 hossein   (1000) hossein   (1000)    23707 2023-03-19 08:54:39.000000 jaxip-0.7.1/tests/.ipynb_checkpoints/test-checkpoint.ipynb
--rw-r--r--   0 hossein   (1000) hossein   (1000)       35 2023-01-05 20:40:22.000000 jaxip-0.7.1/tests/__init__.py
--rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.7.1/tests/h2o.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2063 2023-03-14 20:01:39.000000 jaxip-0.7.1/tests/h2o.json
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      384 2023-07-15 14:18:33.000000 jaxip-0.7.1/tests/scaling.001.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      480 2023-07-15 14:18:33.000000 jaxip-0.7.1/tests/scaling.008.data
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5108 2023-07-10 18:19:00.000000 jaxip-0.7.1/tests/test_acsf.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2569 2023-07-10 18:19:00.000000 jaxip-0.7.1/tests/test_mc.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3137 2023-07-10 18:19:00.000000 jaxip-0.7.1/tests/test_md.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     4106 2023-07-10 18:19:00.000000 jaxip-0.7.1/tests/test_nn.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     3445 2023-07-10 18:19:00.000000 jaxip-0.7.1/tests/test_nnp.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5269 2023-07-15 14:24:44.000000 jaxip-0.7.1/tests/test_runner.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     2850 2023-07-10 18:19:00.000000 jaxip-0.7.1/tests/test_scaler.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)     5897 2023-07-10 18:19:00.000000 jaxip-0.7.1/tests/test_structure.py
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      793 2023-07-15 14:18:33.000000 jaxip-0.7.1/tests/weights.001.pkl
--rw-rw-r--   0 hossein   (1000) hossein   (1000)      813 2023-07-15 14:18:33.000000 jaxip-0.7.1/tests/weights.008.pkl
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-22 19:34:47.121147 jaxip-0.7.2/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      166 2022-12-07 19:09:20.000000 jaxip-0.7.2/AUTHORS.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3491 2023-04-26 21:18:43.000000 jaxip-0.7.2/CONTRIBUTING.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      829 2023-07-15 14:24:44.000000 jaxip-0.7.2/HISTORY.rst
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     1523 2023-01-05 20:40:22.000000 jaxip-0.7.2/LICENSE
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      262 2022-12-07 20:18:56.000000 jaxip-0.7.2/MANIFEST.in
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6200 2023-07-22 19:34:47.121147 jaxip-0.7.2/PKG-INFO
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5613 2023-07-22 19:34:04.000000 jaxip-0.7.2/README.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-22 19:34:47.037146 jaxip-0.7.2/docs/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      606 2023-02-01 19:45:48.000000 jaxip-0.7.2/docs/Makefile
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-22 19:34:46.997146 jaxip-0.7.2/docs/_build/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-22 19:34:46.997146 jaxip-0.7.2/docs/_build/doctrees/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-22 19:34:47.045146 jaxip-0.7.2/docs/_build/doctrees/nbsphinx/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-07-21 11:35:19.000000 jaxip-0.7.2/docs/_build/doctrees/nbsphinx/notebooks_getting_started_38_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-07-21 11:35:19.000000 jaxip-0.7.2/docs/_build/doctrees/nbsphinx/notebooks_getting_started_45_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-07-21 11:35:19.000000 jaxip-0.7.2/docs/_build/doctrees/nbsphinx/notebooks_getting_started_51_0.png
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-22 19:34:46.997146 jaxip-0.7.2/docs/_build/html/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-22 19:34:47.049146 jaxip-0.7.2/docs/_build/html/_images/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11011 2023-07-21 11:35:19.000000 jaxip-0.7.2/docs/_build/html/_images/notebooks_getting_started_38_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-07-21 11:35:19.000000 jaxip-0.7.2/docs/_build/html/_images/notebooks_getting_started_45_0.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    10043 2023-07-21 11:35:19.000000 jaxip-0.7.2/docs/_build/html/_images/notebooks_getting_started_51_0.png
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-22 19:34:47.053146 jaxip-0.7.2/docs/_build/html/_static/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      286 2023-04-26 21:14:06.000000 jaxip-0.7.2/docs/_build/html/_static/file.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.7.2/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       90 2023-04-26 21:14:06.000000 jaxip-0.7.2/docs/_build/html/_static/plus.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-28 08:07:09.000000 jaxip-0.7.2/docs/authors.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6598 2023-07-22 19:34:04.000000 jaxip-0.7.2/docs/conf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       33 2022-12-07 19:09:20.000000 jaxip-0.7.2/docs/contributing.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       87 2023-07-22 19:34:04.000000 jaxip-0.7.2/docs/examples.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       28 2022-12-07 19:09:20.000000 jaxip-0.7.2/docs/history.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-22 19:34:47.061147 jaxip-0.7.2/docs/images/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    44314 2023-03-28 20:24:39.000000 jaxip-0.7.2/docs/images/flowchart.drawio.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    96759 2023-02-06 19:53:40.000000 jaxip-0.7.2/docs/images/water.png
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      466 2023-07-22 19:34:04.000000 jaxip-0.7.2/docs/index.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1864 2023-04-26 21:18:43.000000 jaxip-0.7.2/docs/installation.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      760 2023-07-15 22:30:18.000000 jaxip-0.7.2/docs/jaxip.atoms.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      495 2023-07-15 22:30:18.000000 jaxip-0.7.2/docs/jaxip.datasets.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1095 2023-07-15 22:30:18.000000 jaxip-0.7.2/docs/jaxip.descriptors.acsf.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      613 2023-07-15 22:30:18.000000 jaxip-0.7.2/docs/jaxip.descriptors.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      686 2023-07-15 22:30:18.000000 jaxip-0.7.2/docs/jaxip.models.nn.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      400 2023-07-15 22:30:18.000000 jaxip-0.7.2/docs/jaxip.models.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1290 2023-07-15 22:30:19.000000 jaxip-0.7.2/docs/jaxip.potentials.nnp.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      464 2023-07-15 22:30:19.000000 jaxip-0.7.2/docs/jaxip.potentials.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      961 2023-07-21 11:35:01.000000 jaxip-0.7.2/docs/jaxip.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      951 2023-07-15 22:30:19.000000 jaxip-0.7.2/docs/jaxip.simulation.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      915 2023-07-15 22:30:19.000000 jaxip-0.7.2/docs/jaxip.utils.rst
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      803 2023-01-05 20:40:22.000000 jaxip-0.7.2/docs/make.bat
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       52 2023-07-21 11:35:01.000000 jaxip-0.7.2/docs/modules.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       27 2022-12-20 21:49:36.000000 jaxip-0.7.2/docs/readme.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3833 2023-05-06 13:11:44.000000 jaxip-0.7.2/docs/theory.rst
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1158 2023-04-26 21:18:43.000000 jaxip-0.7.2/docs/usage.rst
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-22 19:34:47.073147 jaxip-0.7.2/jaxip/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      556 2023-07-22 19:34:04.000000 jaxip-0.7.2/jaxip/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      294 2023-07-22 19:34:04.000000 jaxip-0.7.2/jaxip/_version.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-22 19:34:47.089147 jaxip-0.7.2/jaxip/atoms/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      232 2023-07-10 18:19:00.000000 jaxip-0.7.2/jaxip/atoms/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1486 2023-07-10 18:19:00.000000 jaxip-0.7.2/jaxip/atoms/_structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3787 2023-07-22 19:34:04.000000 jaxip-0.7.2/jaxip/atoms/box.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6639 2023-07-10 18:19:00.000000 jaxip-0.7.2/jaxip/atoms/element.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3354 2023-07-10 18:19:00.000000 jaxip-0.7.2/jaxip/atoms/neighbor.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    17762 2023-07-22 19:34:04.000000 jaxip-0.7.2/jaxip/atoms/structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1124 2023-07-10 18:19:00.000000 jaxip-0.7.2/jaxip/config.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-22 19:34:47.093147 jaxip-0.7.2/jaxip/datasets/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       84 2023-07-15 14:24:44.000000 jaxip-0.7.2/jaxip/datasets/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      408 2023-05-17 19:30:18.000000 jaxip-0.7.2/jaxip/datasets/dataset.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6494 2023-07-15 14:24:44.000000 jaxip-0.7.2/jaxip/datasets/runner.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-22 19:34:47.093147 jaxip-0.7.2/jaxip/descriptors/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      130 2023-07-22 19:34:04.000000 jaxip-0.7.2/jaxip/descriptors/__init__.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-22 19:34:47.097147 jaxip-0.7.2/jaxip/descriptors/acsf/
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      400 2023-01-05 20:40:22.000000 jaxip-0.7.2/jaxip/descriptors/acsf/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5312 2023-07-10 18:19:00.000000 jaxip-0.7.2/jaxip/descriptors/acsf/_acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     8147 2023-07-22 19:34:04.000000 jaxip-0.7.2/jaxip/descriptors/acsf/acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2236 2023-05-17 19:30:18.000000 jaxip-0.7.2/jaxip/descriptors/acsf/angular.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3901 2023-07-22 19:34:04.000000 jaxip-0.7.2/jaxip/descriptors/acsf/cutoff.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1495 2023-07-22 19:19:55.000000 jaxip-0.7.2/jaxip/descriptors/acsf/radial.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1015 2023-05-17 19:30:18.000000 jaxip-0.7.2/jaxip/descriptors/acsf/symmetry.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      616 2023-05-17 19:30:18.000000 jaxip-0.7.2/jaxip/descriptors/descriptor.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     7467 2023-07-10 18:19:00.000000 jaxip-0.7.2/jaxip/descriptors/scaler.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3739 2023-05-01 12:41:07.000000 jaxip-0.7.2/jaxip/logger.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-22 19:34:47.097147 jaxip-0.7.2/jaxip/models/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       88 2023-05-08 16:51:03.000000 jaxip-0.7.2/jaxip/models/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      389 2023-05-17 19:30:18.000000 jaxip-0.7.2/jaxip/models/model.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-22 19:34:47.097147 jaxip-0.7.2/jaxip/models/nn/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      181 2023-05-08 16:51:03.000000 jaxip-0.7.2/jaxip/models/nn/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1125 2023-05-08 16:51:03.000000 jaxip-0.7.2/jaxip/models/nn/activation.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      604 2023-05-08 16:51:03.000000 jaxip-0.7.2/jaxip/models/nn/initializer.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2879 2023-07-15 14:24:44.000000 jaxip-0.7.2/jaxip/models/nn/network.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-22 19:34:47.101147 jaxip-0.7.2/jaxip/potentials/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      212 2023-05-17 19:30:18.000000 jaxip-0.7.2/jaxip/potentials/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1979 2023-07-10 18:19:00.000000 jaxip-0.7.2/jaxip/potentials/_energy.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      866 2023-05-01 12:41:07.000000 jaxip-0.7.2/jaxip/potentials/_force.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1852 2023-07-22 19:34:04.000000 jaxip-0.7.2/jaxip/potentials/atomic_potential.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-22 19:34:47.101147 jaxip-0.7.2/jaxip/potentials/nnp/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      238 2023-05-17 19:30:18.000000 jaxip-0.7.2/jaxip/potentials/nnp/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     9522 2023-07-15 14:24:44.000000 jaxip-0.7.2/jaxip/potentials/nnp/gradient_descent.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     9374 2023-07-10 18:19:00.000000 jaxip-0.7.2/jaxip/potentials/nnp/kalman_filter.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2576 2023-05-01 12:41:07.000000 jaxip-0.7.2/jaxip/potentials/nnp/metrics.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      542 2023-06-24 19:26:34.000000 jaxip-0.7.2/jaxip/potentials/nnp/nnp.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    19075 2023-07-22 19:34:04.000000 jaxip-0.7.2/jaxip/potentials/nnp/potential.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)    11345 2023-07-10 18:19:00.000000 jaxip-0.7.2/jaxip/potentials/nnp/settings.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3626 2023-07-22 19:34:04.000000 jaxip-0.7.2/jaxip/pytree.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-22 19:34:47.105147 jaxip-0.7.2/jaxip/simulation/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      296 2023-06-24 19:26:34.000000 jaxip-0.7.2/jaxip/simulation/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2143 2023-07-10 18:19:00.000000 jaxip-0.7.2/jaxip/simulation/lj.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4331 2023-07-10 18:19:00.000000 jaxip-0.7.2/jaxip/simulation/mc.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     9132 2023-07-15 14:24:44.000000 jaxip-0.7.2/jaxip/simulation/md.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2515 2023-07-10 18:19:00.000000 jaxip-0.7.2/jaxip/simulation/run.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      840 2023-07-10 18:19:00.000000 jaxip-0.7.2/jaxip/simulation/thermostat.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      679 2023-07-22 19:34:04.000000 jaxip-0.7.2/jaxip/types.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2573 2023-06-18 10:02:01.000000 jaxip-0.7.2/jaxip/units.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-22 19:34:47.105147 jaxip-0.7.2/jaxip/utils/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       73 2023-05-01 12:41:07.000000 jaxip-0.7.2/jaxip/utils/__init__.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1418 2023-07-10 18:19:00.000000 jaxip-0.7.2/jaxip/utils/attribute.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      585 2023-05-01 12:41:07.000000 jaxip-0.7.2/jaxip/utils/batch.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2012 2023-07-10 18:19:00.000000 jaxip-0.7.2/jaxip/utils/compare.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4410 2023-05-01 12:41:07.000000 jaxip-0.7.2/jaxip/utils/profiler.py
+-rw-r--r--   0 hossein   (1000) hossein   (1000)      670 2023-01-18 21:30:52.000000 jaxip-0.7.2/jaxip/utils/tokenize.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-22 19:34:47.081147 jaxip-0.7.2/jaxip.egg-info/
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     6200 2023-07-22 19:34:46.000000 jaxip-0.7.2/jaxip.egg-info/PKG-INFO
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3265 2023-07-22 19:34:46.000000 jaxip-0.7.2/jaxip.egg-info/SOURCES.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-07-22 19:34:46.000000 jaxip-0.7.2/jaxip.egg-info/dependency_links.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       41 2023-07-22 19:34:46.000000 jaxip-0.7.2/jaxip.egg-info/entry_points.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        1 2023-07-22 19:34:46.000000 jaxip-0.7.2/jaxip.egg-info/not-zip-safe
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)       85 2023-07-22 19:34:46.000000 jaxip-0.7.2/jaxip.egg-info/requires.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)        6 2023-07-22 19:34:46.000000 jaxip-0.7.2/jaxip.egg-info/top_level.txt
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      137 2023-07-22 19:34:47.121147 jaxip-0.7.2/setup.cfg
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     1661 2023-03-22 21:56:02.000000 jaxip-0.7.2/setup.py
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-22 19:34:47.117147 jaxip-0.7.2/tests/
+drwxrwxr-x   0 hossein   (1000) hossein   (1000)        0 2023-07-22 19:34:47.121147 jaxip-0.7.2/tests/.ipynb_checkpoints/
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.7.2/tests/.ipynb_checkpoints/h2o-checkpoint.data
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     9543 2023-01-26 17:53:14.000000 jaxip-0.7.2/tests/.ipynb_checkpoints/h2o-checkpoint.json
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-26 17:32:00.000000 jaxip-0.7.2/tests/.ipynb_checkpoints/input.h2o-checkpoint.data
+-rw-r--r--   0 hossein   (1000) hossein   (1000)    23707 2023-03-19 08:54:39.000000 jaxip-0.7.2/tests/.ipynb_checkpoints/test-checkpoint.ipynb
+-rw-r--r--   0 hossein   (1000) hossein   (1000)       35 2023-01-05 20:40:22.000000 jaxip-0.7.2/tests/__init__.py
+-rw-r--r--   0 hossein   (1000) hossein   (1000)     3632 2022-12-27 18:25:19.000000 jaxip-0.7.2/tests/h2o.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2063 2023-03-14 20:01:39.000000 jaxip-0.7.2/tests/h2o.json
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      384 2023-07-22 18:48:21.000000 jaxip-0.7.2/tests/scaling.001.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      480 2023-07-22 18:48:21.000000 jaxip-0.7.2/tests/scaling.008.data
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5512 2023-07-22 19:34:04.000000 jaxip-0.7.2/tests/test_acsf.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2569 2023-07-10 18:19:00.000000 jaxip-0.7.2/tests/test_mc.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3137 2023-07-10 18:19:00.000000 jaxip-0.7.2/tests/test_md.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     4106 2023-07-10 18:19:00.000000 jaxip-0.7.2/tests/test_nn.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     3445 2023-07-10 18:19:00.000000 jaxip-0.7.2/tests/test_nnp.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5269 2023-07-15 14:24:44.000000 jaxip-0.7.2/tests/test_runner.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     2850 2023-07-10 18:19:00.000000 jaxip-0.7.2/tests/test_scaler.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)     5897 2023-07-10 18:19:00.000000 jaxip-0.7.2/tests/test_structure.py
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      793 2023-07-22 18:48:21.000000 jaxip-0.7.2/tests/weights.001.pkl
+-rw-rw-r--   0 hossein   (1000) hossein   (1000)      813 2023-07-22 18:48:21.000000 jaxip-0.7.2/tests/weights.008.pkl
```

### Comparing `jaxip-0.7.1/CONTRIBUTING.rst` & `jaxip-0.7.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/HISTORY.rst` & `jaxip-0.7.2/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/LICENSE` & `jaxip-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/PKG-INFO` & `jaxip-0.7.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxip
-Version: 0.7.1
+Version: 0.7.2
 Summary: JAX-based Interatomic Potential
 Home-page: https://github.com/hghcomphys/jaxip
 Author: Hossein Ghorbanfekr
 Author-email: hgh.comphys@gmail.com
 License: GNU General Public License v3
 Keywords: jaxip
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -36,23 +36,23 @@
         :target: https://jaxip.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 
 Description
 -----------
 Jaxip is an optimized Python library on basis of Google `JAX`_ that enables 
-development of emerging machine learning interatomic potentials 
-for use in computational physics, chemistry, and material science. 
+development of machine learning inter-atomic potentials 
+for use in computational physics and material science. 
 These potentials are necessary for conducting large-scale molecular 
 dynamics simulations of complex materials with ab initio accuracy.
 
 .. _JAX: https://github.com/google/jax
 
 
-See `documentation`_ for more information.
+See the `documentation`_ for more information.
 
 .. _documentation: https://jaxip.readthedocs.io/en/latest/readme.html
 
 
 Features
 --------
 * The design of Jaxip is `simple` and `flexible`, which makes it easy to incorporate atomic descriptors and potentials. 
@@ -70,102 +70,110 @@
 ------------
 To install Jaxip, run this command in your terminal:
 
 .. code-block:: console
 
     $ pip install jaxip
 
-For machines with an NVIDIA **GPU** please follow the installation
-`instruction <https://jaxip.readthedocs.io/en/latest/installation.html>`_ 
-on the documentation. 
+For machines with an NVIDIA **GPU** please follow the
+`installation <https://jaxip.readthedocs.io/en/latest/installation.html>`_ 
+instruction on the documentation. 
 
 
 Examples
 --------
 
------------------------------
-Defining an atomic descriptor
------------------------------
+---------------------------
+Defining an ACSF descriptor
+---------------------------
 This script demonstrates the process of evaluating an array of atomic-centered symmetry functions (`ACSF`_) 
 for a specific element, which can be utilized to evaluate the descriptor values for any structure. 
 The resulting values can then be used to construct a machine learning potential.
 
 .. _ACSF: https://aip.scitation.org/doi/10.1063/1.3553717
 
 
-
 .. code-block:: python
 
         from jaxip.datasets import RunnerDataset
         from jaxip.descriptors import ACSF
         from jaxip.descriptors.acsf import CutoffFunction, G2, G3
 
         # Read atomic structure dataset (e.g. water molecules)
         structures = RunnerDataset('input.data')
         structure = structures[0]
+        print(structure)
+        # >> Structure(natoms=12, elements=('H', 'O'), dtype=float32) 
 
-        # Define ACSF descriptor for hydrogen element
-        descriptor = ACSF(element='H')
-
-        # Add radial and angular symmetry functions
-        cfn = CutoffFunction(r_cutoff=12.0, cutoff_type='tanh')
+        # Define an ACSF descriptor for hydrogen element
+        # It includes two radial (G2) and angular (G3) symmetry functions
+        descriptor = ACSF('H')
+        cfn = CutoffFunction.from_cutoff_type(r_cutoff=12.0, cutoff_type='tanh')
         descriptor.add(G2(cfn, eta=0.5, r_shift=0.0), 'H')
         descriptor.add(G3(cfn, eta=0.001, zeta=2.0, lambda0=1.0, r_shift=12.0), 'H', 'O')
         print(descriptor)
+        # >> ACSF(central_element='H', symmetry_functions=2)
 
         values = descriptor(structure)
         print("Descriptor values:\n", values)
+        # >> Descriptor values:
+        # [[0.01952942 1.1310327 ]
+        # [0.01952756 1.0431229 ]
+        # ...
+        # [0.00228752 0.4144546 ]]
 
         gradient = descriptor.grad(structure, atom_index=0)
         print("Descriptor gradient:\n", gradient)
+        # >> Descriptor gradient:
+        # [[ 0.0464524  -0.05037863 -0.06146219]
+        # [-0.10481848 -0.01841717  0.04760207]]
 
 
--------------------------------------
-Training a machine learning potential
--------------------------------------
+-------------------------
+Training an NNP potential
+-------------------------
 This example illustrates how to quickly create a `high-dimensional neural network 
 potential` (`HDNNP`_) instance from an in input setting files and train it on input structures. 
 The trained potential can then be used to evaluate the energy and force components for new structures.
 
 .. _HDNNP: https://pubs.acs.org/doi/10.1021/acs.chemrev.0c00868
 
 
 .. code-block:: python
 
         from jaxip.datasets import RunnerDataset
         from jaxip.potentials import NeuralNetworkPotential
 
-        # Read atomic data
+        # Read atomic data in RuNNer format
         structures = RunnerDataset("input.data")
         structure = structures[0]
 
-        # Instantiate potential from input settings file
         nnp = NeuralNetworkPotential.from_file("input.nn")
 
-        # Fit descriptor scaler and model weights
         nnp.fit_scaler(structures)
         nnp.fit_model(structures)
-        nnp.save()
-
-        # Or loading from files
-        #nnp.load()
-
-        # Total energy
-        nnp(structure)
-
-        # Force components
-        nnp.compute_forces(structure)
+        # nnp.save()
+        # nnp.load()
 
+        total_energy = nnp(structure)
+        print(total_energy)
+        # >> -15.386198
+
+        forces = nnp.compute_forces(structure)
+        print(forces)
+        # >> [[ 1.6445214e-02 -4.1671786e-03  7.6140024e-02]
+        # [-6.4949177e-02 -4.2048577e-02  5.6018140e-02]
+        # ...
+        # [ 7.6149488e-03 -9.5360324e-02 -9.2892153e-03]]
 
 
 Example files: `input.data`_ and `input.nn`_
 
 .. _input.data: https://drive.google.com/file/d/1VMckgIv_OUvCOXQ0pYzaF5yl9AwR0rBy/view?usp=sharing
 .. _input.nn: https://drive.google.com/file/d/15Oq9gAJ2xXVMcHyWXlRukfJFevyVO7lI/view?usp=sharing
 
 
 
 License
 -------
-
 This project is licensed under the GNU General Public License (GPL) version 3 - 
 see the `LICENSE <https://github.com/hghcomphys/jaxip/blob/main/LICENSE>`_ file for details.
```

### Comparing `jaxip-0.7.1/README.rst` & `jaxip-0.7.2/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -18,23 +18,23 @@
         :target: https://jaxip.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 
 Description
 -----------
 Jaxip is an optimized Python library on basis of Google `JAX`_ that enables 
-development of emerging machine learning interatomic potentials 
-for use in computational physics, chemistry, and material science. 
+development of machine learning inter-atomic potentials 
+for use in computational physics and material science. 
 These potentials are necessary for conducting large-scale molecular 
 dynamics simulations of complex materials with ab initio accuracy.
 
 .. _JAX: https://github.com/google/jax
 
 
-See `documentation`_ for more information.
+See the `documentation`_ for more information.
 
 .. _documentation: https://jaxip.readthedocs.io/en/latest/readme.html
 
 
 Features
 --------
 * The design of Jaxip is `simple` and `flexible`, which makes it easy to incorporate atomic descriptors and potentials. 
@@ -52,102 +52,110 @@
 ------------
 To install Jaxip, run this command in your terminal:
 
 .. code-block:: console
 
     $ pip install jaxip
 
-For machines with an NVIDIA **GPU** please follow the installation
-`instruction <https://jaxip.readthedocs.io/en/latest/installation.html>`_ 
-on the documentation. 
+For machines with an NVIDIA **GPU** please follow the
+`installation <https://jaxip.readthedocs.io/en/latest/installation.html>`_ 
+instruction on the documentation. 
 
 
 Examples
 --------
 
------------------------------
-Defining an atomic descriptor
------------------------------
+---------------------------
+Defining an ACSF descriptor
+---------------------------
 This script demonstrates the process of evaluating an array of atomic-centered symmetry functions (`ACSF`_) 
 for a specific element, which can be utilized to evaluate the descriptor values for any structure. 
 The resulting values can then be used to construct a machine learning potential.
 
 .. _ACSF: https://aip.scitation.org/doi/10.1063/1.3553717
 
 
-
 .. code-block:: python
 
         from jaxip.datasets import RunnerDataset
         from jaxip.descriptors import ACSF
         from jaxip.descriptors.acsf import CutoffFunction, G2, G3
 
         # Read atomic structure dataset (e.g. water molecules)
         structures = RunnerDataset('input.data')
         structure = structures[0]
+        print(structure)
+        # >> Structure(natoms=12, elements=('H', 'O'), dtype=float32) 
 
-        # Define ACSF descriptor for hydrogen element
-        descriptor = ACSF(element='H')
-
-        # Add radial and angular symmetry functions
-        cfn = CutoffFunction(r_cutoff=12.0, cutoff_type='tanh')
+        # Define an ACSF descriptor for hydrogen element
+        # It includes two radial (G2) and angular (G3) symmetry functions
+        descriptor = ACSF('H')
+        cfn = CutoffFunction.from_cutoff_type(r_cutoff=12.0, cutoff_type='tanh')
         descriptor.add(G2(cfn, eta=0.5, r_shift=0.0), 'H')
         descriptor.add(G3(cfn, eta=0.001, zeta=2.0, lambda0=1.0, r_shift=12.0), 'H', 'O')
         print(descriptor)
+        # >> ACSF(central_element='H', symmetry_functions=2)
 
         values = descriptor(structure)
         print("Descriptor values:\n", values)
+        # >> Descriptor values:
+        # [[0.01952942 1.1310327 ]
+        # [0.01952756 1.0431229 ]
+        # ...
+        # [0.00228752 0.4144546 ]]
 
         gradient = descriptor.grad(structure, atom_index=0)
         print("Descriptor gradient:\n", gradient)
+        # >> Descriptor gradient:
+        # [[ 0.0464524  -0.05037863 -0.06146219]
+        # [-0.10481848 -0.01841717  0.04760207]]
 
 
--------------------------------------
-Training a machine learning potential
--------------------------------------
+-------------------------
+Training an NNP potential
+-------------------------
 This example illustrates how to quickly create a `high-dimensional neural network 
 potential` (`HDNNP`_) instance from an in input setting files and train it on input structures. 
 The trained potential can then be used to evaluate the energy and force components for new structures.
 
 .. _HDNNP: https://pubs.acs.org/doi/10.1021/acs.chemrev.0c00868
 
 
 .. code-block:: python
 
         from jaxip.datasets import RunnerDataset
         from jaxip.potentials import NeuralNetworkPotential
 
-        # Read atomic data
+        # Read atomic data in RuNNer format
         structures = RunnerDataset("input.data")
         structure = structures[0]
 
-        # Instantiate potential from input settings file
         nnp = NeuralNetworkPotential.from_file("input.nn")
 
-        # Fit descriptor scaler and model weights
         nnp.fit_scaler(structures)
         nnp.fit_model(structures)
-        nnp.save()
-
-        # Or loading from files
-        #nnp.load()
-
-        # Total energy
-        nnp(structure)
-
-        # Force components
-        nnp.compute_forces(structure)
+        # nnp.save()
+        # nnp.load()
 
+        total_energy = nnp(structure)
+        print(total_energy)
+        # >> -15.386198
+
+        forces = nnp.compute_forces(structure)
+        print(forces)
+        # >> [[ 1.6445214e-02 -4.1671786e-03  7.6140024e-02]
+        # [-6.4949177e-02 -4.2048577e-02  5.6018140e-02]
+        # ...
+        # [ 7.6149488e-03 -9.5360324e-02 -9.2892153e-03]]
 
 
 Example files: `input.data`_ and `input.nn`_
 
 .. _input.data: https://drive.google.com/file/d/1VMckgIv_OUvCOXQ0pYzaF5yl9AwR0rBy/view?usp=sharing
 .. _input.nn: https://drive.google.com/file/d/15Oq9gAJ2xXVMcHyWXlRukfJFevyVO7lI/view?usp=sharing
 
 
 
 License
 -------
-
 This project is licensed under the GNU General Public License (GPL) version 3 - 
 see the `LICENSE <https://github.com/hghcomphys/jaxip/blob/main/LICENSE>`_ file for details.
```

### Comparing `jaxip-0.7.1/docs/Makefile` & `jaxip-0.7.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/docs/_build/doctrees/nbsphinx/notebooks_getting_started_38_0.png` & `jaxip-0.7.2/docs/_build/doctrees/nbsphinx/notebooks_getting_started_38_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/docs/_build/doctrees/nbsphinx/notebooks_getting_started_45_0.png` & `jaxip-0.7.2/docs/_build/doctrees/nbsphinx/notebooks_getting_started_45_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/docs/_build/doctrees/nbsphinx/notebooks_getting_started_51_0.png` & `jaxip-0.7.2/docs/_build/doctrees/nbsphinx/notebooks_getting_started_51_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/docs/_build/html/_images/notebooks_getting_started_38_0.png` & `jaxip-0.7.2/docs/_build/html/_images/notebooks_getting_started_38_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/docs/_build/html/_images/notebooks_getting_started_45_0.png` & `jaxip-0.7.2/docs/_build/html/_images/notebooks_getting_started_45_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/docs/_build/html/_images/notebooks_getting_started_51_0.png` & `jaxip-0.7.2/docs/_build/html/_images/notebooks_getting_started_51_0.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/docs/conf.py` & `jaxip-0.7.2/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,20 @@
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = "English"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
-exclude_patterns = ["_build", "Thumbs.db", ".DS_Store", "**.ipynb_checkpoints"]
+exclude_patterns = [
+    "_build",
+    "Thumbs.db",
+    ".DS_Store",
+    "**.ipynb_checkpoints",
+]
 
 # The name of the Pygments (syntax highlighting) style to use.
 pygments_style = "sphinx"
 
 # If true, `todo` and `todoList` produce output, else they produce nothing.
 todo_include_todos = True
 
@@ -124,14 +129,18 @@
 # documentation.
 #
 html_theme_options = {
     # "search_bar_position": "sidebar",
     "github_url": "https://github.com/hghcomphys/jaxip",
 }
 
+html_context = {
+    "display_github": True,
+}
+
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
 html_static_path = ["_static"]
 
 
 # -- Options for HTMLHelp output ---------------------------------------
@@ -194,15 +203,15 @@
 texinfo_documents = [
     (
         master_doc,
         "jaxip",
         "Jaxip Documentation",
         author,
         "jaxip",
-        "One line description of project.",
+        "An optimized Python library for developing machine learning interatomic potentials, based on Google JAX.",
         "Miscellaneous",
     ),
 ]
 
 # autodoc_default_options = {
 #     "members": True,
 #     "member-order": "bysource",
@@ -219,13 +228,13 @@
 notebooks_dir = os.path.join(curdir, "notebooks")
 if os.path.exists(notebooks_dir):
     shutil.rmtree(notebooks_dir)
 os.makedirs(notebooks_dir, exist_ok=True)
 
 for filename in (
     "getting_started.ipynb",
-    "training_potential.ipynb",
+    "potential_training.ipynb",
 ):
     shutil.copyfile(  # copytree(
         os.path.join(curdir, "..", "examples", filename),
         os.path.join(curdir, "notebooks", filename),
     )
```

### Comparing `jaxip-0.7.1/docs/images/flowchart.drawio.png` & `jaxip-0.7.2/docs/images/flowchart.drawio.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/docs/images/water.png` & `jaxip-0.7.2/docs/images/water.png`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/docs/installation.rst` & `jaxip-0.7.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/docs/jaxip.atoms.rst` & `jaxip-0.7.2/docs/jaxip.atoms.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/docs/jaxip.descriptors.acsf.rst` & `jaxip-0.7.2/docs/jaxip.descriptors.acsf.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/docs/jaxip.descriptors.rst` & `jaxip-0.7.2/docs/jaxip.descriptors.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/docs/jaxip.models.nn.rst` & `jaxip-0.7.2/docs/jaxip.models.nn.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/docs/jaxip.potentials.nnp.rst` & `jaxip-0.7.2/docs/jaxip.potentials.nnp.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/docs/jaxip.rst` & `jaxip-0.7.2/docs/jaxip.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/docs/jaxip.simulation.rst` & `jaxip-0.7.2/docs/jaxip.simulation.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/docs/jaxip.utils.rst` & `jaxip-0.7.2/docs/jaxip.utils.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/docs/make.bat` & `jaxip-0.7.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/docs/theory.rst` & `jaxip-0.7.2/docs/theory.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/docs/usage.rst` & `jaxip-0.7.2/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/__init__.py` & `jaxip-0.7.2/jaxip/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 Jaxip - JAX-based Interatomic Potential
 =======================================
 
-Jaxip is an optimized Python library on basis of Google JAX that enables development of emerging 
-machine learning interatomic potentials for use in computational physics, chemistry, material 
-science. These potentials are necessary for conducting large-scale molecular dynamics simulations 
+Jaxip is an optimized Python library on basis of Google JAX that enables development of machine
+learning inter-atomic potentials for use in computational physics and material science.
+These potentials are necessary for conducting large-scale molecular dynamics simulations
 of complex materials with ab initio accuracy.
 """
 from jaxip._version import __version__ as version
 
 __author__ = """Hossein Ghorbanfekr"""
 __email__ = "hgh.comphys@gmail.com"
 __version__ = version
```

### Comparing `jaxip-0.7.1/jaxip/atoms/_structure.py` & `jaxip-0.7.2/jaxip/atoms/_structure.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/atoms/box.py` & `jaxip-0.7.2/jaxip/atoms/box.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from dataclasses import InitVar, dataclass
-from typing import Optional
+from __future__ import annotations
+
+from dataclasses import dataclass
+from typing import List, Optional
 
 import jax
 import jax.numpy as jnp
 
 from jaxip.logger import logger
 from jaxip.pytree import BaseJaxPytreeDataClass, register_jax_pytree_node
 from jaxip.types import Array, Dtype, _dtype
@@ -33,33 +35,31 @@
 
     .. warning::
         The current implementation only works for orthogonal cells
         and does not support triclinic cells.
     """
 
     lattice: Array
-    dtype: InitVar[Optional[Dtype]] = None
 
-    def __post_init__(self, dtype: Optional[Dtype] = None) -> None:
+    def __post_init__(self) -> None:
         """Post initialize simulation box (super-cell)."""
         logger.debug(f"Initializing {self}")
-        if dtype is None:
-            dtype = _dtype.FLOATX
-        try:
-            self.lattice = jnp.array(self.lattice, dtype=dtype).reshape(3, 3)
-        except ValueError:
-            logger.error(
-                f"Unexpected lattice matrix: {self.lattice}",
-                exception=ValueError,
-            )
+        self._assert_jit_static_attributes()
         self._assert_jit_dynamic_attributes(expected=("lattice",))
 
-    def __hash__(self) -> int:
-        """Enforce to use the parent class's hash method (JIT)."""
-        return super().__hash__()
+    @classmethod
+    def from_list(
+        cls,
+        data: List[float],
+        dtype: Optional[Dtype] = None,
+    ) -> Box:
+        if dtype is None:
+            dtype = _dtype.FLOATX
+        lattice = jnp.array(data, dtype=dtype).reshape(3, 3)
+        return Box(lattice)
 
     @jax.jit
     def apply_pbc(self, dx: Array) -> Array:
         """
         Apply the periodic boundary condition (PBC) on the provided position array.
 
         For this method to function correctly, it is essential that all atoms are
@@ -84,17 +84,14 @@
         :type x: Array
         :return: shifted atom positions
         :rtype: Array
         """
         logger.debug("Shift all atoms inside the simulation box")
         return _shift_inside_box(positions, self.lattice)
 
-    def __repr__(self) -> str:
-        return f"{self.__class__.__name__}(lattice={self.lattice})"
-
     @property
     def lx(self) -> Array:
         """Return length of cell in x-direction."""
         return self.lattice[0, 0]
 
     @property
     def ly(self) -> Array:
@@ -112,9 +109,23 @@
         return self.lattice.diagonal()
 
     @property
     def volume(self) -> Array:
         """Return volume of the box."""
         return jnp.prod(self.length)
 
+    @property
+    def dtype(self) -> Dtype:
+        return self.lattice.dtype
+
+    def __hash__(self) -> int:
+        """Enforce to use the parent class's hash method (JIT)."""
+        return super().__hash__()
+
+    def __repr__(self) -> str:
+        return (
+            f"{self.__class__.__name__}"
+            f"(lattice={self.lattice}, dtype={self.dtype})"
+        )
+
 
 register_jax_pytree_node(Box)
```

### Comparing `jaxip-0.7.1/jaxip/atoms/element.py` & `jaxip-0.7.2/jaxip/atoms/element.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/atoms/neighbor.py` & `jaxip-0.7.2/jaxip/atoms/neighbor.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/atoms/structure.py` & `jaxip-0.7.2/jaxip/atoms/structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -225,20 +225,20 @@
                     exception=KeyError,
                 )
         return arrays
 
     @classmethod
     def _init_box(
         cls,
-        lattice: List[List[float]],
+        lattice: List[float],
         dtype: Dtype,
     ) -> Optional[Box]:
         """Initialize simulation box from input lattice matrix."""
         if len(lattice) > 0:
-            return Box(lattice, dtype=dtype)
+            return Box.from_list(lattice, dtype=dtype)
         else:
             logger.debug("No lattice info were found")
 
     def update_neighbor(self, r_cutoff: Optional[float] = None) -> None:
         """
         Update the neighbor list, building it if required.
```

### Comparing `jaxip-0.7.1/jaxip/config.py` & `jaxip-0.7.2/jaxip/config.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/datasets/runner.py` & `jaxip-0.7.2/jaxip/datasets/runner.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/descriptors/acsf/_acsf.py` & `jaxip-0.7.2/jaxip/descriptors/acsf/_acsf.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/descriptors/acsf/acsf.py` & `jaxip-0.7.2/jaxip/descriptors/acsf/acsf.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,33 +7,39 @@
 from jaxip.atoms.structure import Structure
 from jaxip.descriptors.acsf._acsf import (
     _calculate_descriptor,
     _calculate_grad_descriptor_per_atom,
 )
 from jaxip.descriptors.acsf.angular import AngularSymmetryFunction
 from jaxip.descriptors.acsf.radial import RadialSymmetryFunction
-from jaxip.descriptors.acsf.symmetry import BaseSymmetryFunction, EnvironmentElements
+from jaxip.descriptors.acsf.symmetry import (
+    BaseSymmetryFunction,
+    EnvironmentElements,
+)
 from jaxip.descriptors.descriptor import DescriptorInterface
 from jaxip.logger import logger
 from jaxip.pytree import BaseJaxPytreeDataClass, register_jax_pytree_node
 from jaxip.types import Array, Element
 
 
 @dataclass
 class ACSF(BaseJaxPytreeDataClass, DescriptorInterface):
     """
-    Atom-centered Symmetry Function (`ACSF`_) descriptor.
+    Atom-centered Symmetry Function (`ACSF`_) descriptor captures
+    information about the distribution of neighboring
+    atoms around a central atom by considering both radial (two-body) and angular
+    (three-body) symmetry functions. Radial symmetry functions describe the distances
+    between the central atom and its neighbors, while angular symmetry functions capture
+    the angles formed by the central atom with pairs of neighboring atoms.
+
+    The ACSF descriptor is computed by summing the contributions of the `symmetry functions`
+    for all neighboring atoms within a specified cutoff distance. The values obtained from
+    these calculations represent a fingerprint of the local atomic environment and can
+    be used in various machine learning potentials.
 
-    ACSF describes the local environment of an atom (neighbor distributions).
-    It usually contains multiple combinations of `radial` (two-body)
-    and `angular` (three-body) symmetry functions.
-
-    .. note::
-        The ACSF is independent of input Structure
-        but it knows how to calculate the descriptor values for any given structures.
 
     Example
     -------
 
     .. code-block:: python
         :linenos:
 
@@ -51,58 +57,57 @@
         acsf.add(g2, 'O')
         acsf.add(g2, 'H')
         acsf.add(g3, 'H', 'H')
         acsf.add(g3, 'H', 'O')
 
         print(acsf)
 
-    This gives the following output:
+    Output:
 
     .. code-block:: bash
 
-        ACSF(element='O', num_symmetry_functions=4, r_cutoff=12.0)
+        ACSF(central_element='O', num_symmetry_functions=4, r_cutoff=12.0)
+
 
     .. _ACSF: https://compphysvienna.github.io/n2p2/topics/descriptors.html?highlight=symmetry%20function#
 
     """
 
-    element: str
+    central_element: str
     radial_symmetry_functions: Tuple[Tuple[EnvironmentElements, RadialSymmetryFunction]] = tuple()  # type: ignore
     angular_symmetry_functions: Tuple[Tuple[EnvironmentElements, AngularSymmetryFunction]] = tuple()  # type: ignore
 
-    def __hash__(self) -> int:
-        """Enforce to use the parent class's hash method (JIT)."""
-        return super().__hash__()
-
     def add(
         self,
         symmetry_function: BaseSymmetryFunction,
         neighbor_element_j: Element,
         neighbor_element_k: Optional[Element] = None,
     ) -> None:
         """Add the input symmetry function to the list of ACSFs."""
         if isinstance(symmetry_function, RadialSymmetryFunction):
             self.radial_symmetry_functions = self.radial_symmetry_functions + (
                 (
-                    EnvironmentElements(self.element, neighbor_element_j),
+                    EnvironmentElements(
+                        self.central_element, neighbor_element_j
+                    ),
                     symmetry_function,
                 ),
             )  # type: ignore
         elif isinstance(symmetry_function, AngularSymmetryFunction):
             self.angular_symmetry_functions = self.angular_symmetry_functions + (
                 (
                     EnvironmentElements(
-                        self.element, neighbor_element_j, neighbor_element_k  # type: ignore
+                        self.central_element, neighbor_element_j, neighbor_element_k  # type: ignore
                     ),
                     symmetry_function,
                 ),
             )
         else:
             logger.error(
-                f"Unknown input symmetry function type {symmetry_function}",
+                f"Unknown symmetry function type {symmetry_function}",
                 exception=TypeError,
             )
 
     def __call__(
         self,
         structure: Structure,
         atom_indices: Optional[Array] = None,
@@ -116,31 +121,29 @@
         of type the central element of the descriptor.
         :type atom_indices: Optional[Array], optional
         :return: descriptor values
         :rtype: Array
         """
 
         if self.num_symmetry_functions == 0:
-            logger.warning(
-                f"No symmetry function defined yet:"
-                f" radial={self.num_radial_symmetry_functions}"
-                f", angular={self.num_angular_symmetry_functions}"
-            )
+            logger.warning("No symmetry function was found")
 
         if atom_indices is None:
-            atom_indices = structure.select(self.element)
+            atom_indices = structure.select(self.central_element)
         else:
             atom_indices = jnp.atleast_1d(atom_indices)  # type: ignore
             # Check aid atom type match the central element
             if not jnp.all(
-                structure.element_map.element_to_atom_type[self.element]
+                structure.element_map.element_to_atom_type[
+                    self.central_element
+                ]
                 == structure.atom_types[atom_indices]
             ):
                 logger.error(
-                    f"Inconsistent central element '{self.element}': "
+                    f"Inconsistent central element '{self.central_element}': "
                     f" input atom indices={atom_indices}"
                     f" (atom_types='{int(structure.atom_types[atom_indices])}')",
                     exception=ValueError,
                 )
 
         return _calculate_descriptor(
             self,
@@ -190,15 +193,18 @@
     def num_angular_symmetry_functions(self) -> int:
         """Return number of `three-body` (angular) symmetry functions."""
         return len(self.angular_symmetry_functions)
 
     @property
     def num_symmetry_functions(self) -> int:
         """Return the total (`two-body` and `tree-body`) number of symmetry functions."""
-        return self.num_radial_symmetry_functions + self.num_angular_symmetry_functions
+        return (
+            self.num_radial_symmetry_functions
+            + self.num_angular_symmetry_functions
+        )
 
     @property
     def num_descriptors(self) -> int:
         return self.num_symmetry_functions
 
     @property
     def r_cutoff(self) -> float:  # type: ignore
@@ -211,17 +217,19 @@
                         self.radial_symmetry_functions,
                         self.angular_symmetry_functions,
                     ]
                 )
             ]
         )
 
+    def __hash__(self) -> int:
+        """Enforce to use the parent class's hash method (JIT)."""
+        return super().__hash__()
+
     def __repr__(self) -> str:
         return (
-            f"{self.__class__.__name__}(element='{self.element}'"
-            f", symmetry_functions={self.num_symmetry_functions}"
-            # f", r_cutoff={self.r_cutoff}"
-            ")"
+            f"{self.__class__.__name__}(central_element='{self.central_element}'"
+            f", symmetry_functions={self.num_symmetry_functions})"
         )
 
 
 register_jax_pytree_node(ACSF)
```

### Comparing `jaxip-0.7.1/jaxip/descriptors/acsf/angular.py` & `jaxip-0.7.2/jaxip/descriptors/acsf/angular.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/descriptors/acsf/radial.py` & `jaxip-0.7.2/jaxip/descriptors/acsf/radial.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/descriptors/acsf/symmetry.py` & `jaxip-0.7.2/jaxip/descriptors/acsf/symmetry.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/descriptors/descriptor.py` & `jaxip-0.7.2/jaxip/descriptors/descriptor.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/descriptors/scaler.py` & `jaxip-0.7.2/jaxip/descriptors/scaler.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/logger.py` & `jaxip-0.7.2/jaxip/logger.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/models/nn/activation.py` & `jaxip-0.7.2/jaxip/models/nn/activation.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/models/nn/initializer.py` & `jaxip-0.7.2/jaxip/models/nn/initializer.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/models/nn/network.py` & `jaxip-0.7.2/jaxip/models/nn/network.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/potentials/_energy.py` & `jaxip-0.7.2/jaxip/potentials/_energy.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/potentials/_force.py` & `jaxip-0.7.2/jaxip/potentials/_force.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/potentials/atomic_potential.py` & `jaxip-0.7.2/jaxip/potentials/atomic_potential.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,15 +34,15 @@
         It's only the total energy, sum of the atomic energies over all atom in the structure,
         which has actually physical meaning.
 
         :param params: model parameters
         :param structure: input structure
         :return: model energy output
         """
-        element: Element = self.descriptor.element  # type: ignore
+        element: Element = self.descriptor.central_element  # type: ignore
         aid: Array = structure.select(element)
 
         return _compute_atomic_energy(
             self,
             structure.positions[aid],
             params,
             structure.get_per_element_inputs()[element],
```

### Comparing `jaxip-0.7.1/jaxip/potentials/nnp/gradient_descent.py` & `jaxip-0.7.2/jaxip/potentials/nnp/gradient_descent.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/potentials/nnp/kalman_filter.py` & `jaxip-0.7.2/jaxip/potentials/nnp/kalman_filter.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/potentials/nnp/metrics.py` & `jaxip-0.7.2/jaxip/potentials/nnp/metrics.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/potentials/nnp/nnp.py` & `jaxip-0.7.2/jaxip/potentials/nnp/nnp.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/potentials/nnp/potential.py` & `jaxip-0.7.2/jaxip/potentials/nnp/potential.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,50 +184,50 @@
         # Add symmetry functions
         logger.debug("Registering symmetry functions (radial and angular)")
 
         for args in settings.symfunction_short:
             if args.acsf_type == 1:
                 descriptor[args.central_element].add(
                     symmetry_function=G1(
-                        CutoffFunction(
+                        CutoffFunction.from_cutoff_type(
                             r_cutoff=args.r_cutoff,
                             cutoff_type=settings.cutoff_type,
                         )
                     ),
                     neighbor_element_j=args.neighbor_element_j,
                 )
             elif args.acsf_type == 2:
                 descriptor[args.central_element].add(
                     symmetry_function=G2(
-                        CutoffFunction(
+                        CutoffFunction.from_cutoff_type(
                             r_cutoff=args.r_cutoff, cutoff_type=settings.cutoff_type
                         ),
                         eta=args.eta,
                         r_shift=args.r_shift,
                     ),
                     neighbor_element_j=args.neighbor_element_j,
                 )
             elif args.acsf_type == 3:
                 descriptor[args.central_element].add(
                     symmetry_function=G3(
-                        CutoffFunction(
+                        CutoffFunction.from_cutoff_type(
                             r_cutoff=args.r_cutoff, cutoff_type=settings.cutoff_type
                         ),
                         eta=args.eta,
                         zeta=args.zeta,  # type: ignore
                         lambda0=args.lambda0,  # type: ignore
                         r_shift=args.r_cutoff,
                     ),
                     neighbor_element_j=args.neighbor_element_j,
                     neighbor_element_k=args.neighbor_element_k,  # type: ignore
                 )
             elif args.acsf_type == 9:
                 descriptor[args.central_element].add(
                     symmetry_function=G9(
-                        CutoffFunction(
+                        CutoffFunction.from_cutoff_type(
                             r_cutoff=args.r_cutoff,
                             cutoff_type=settings.cutoff_type,
                         ),
                         eta=args.eta,
                         zeta=args.zeta,  # type: ignore
                         lambda0=args.lambda0,  # type: ignore
                         r_shift=args.r_shift,
```

### Comparing `jaxip-0.7.1/jaxip/potentials/nnp/settings.py` & `jaxip-0.7.2/jaxip/potentials/nnp/settings.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/pytree.py` & `jaxip-0.7.2/jaxip/pytree.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,15 +77,15 @@
         available: Tuple[str, ...],
         expected: Tuple[str, ...],
         tag: str = "",
     ) -> None:
         """Assert to ensure jit (static or dynamics) attributes are correctly identified."""
         if sorted(available) != sorted(expected):  # type: ignore
             logger.error(
-                f"Expecting JIT {tag} attributes: {expected} but got {available}",
+                f"JIT {tag} attributes: expected {expected} but got {available}",
                 exception=AssertionError,
             )
 
     @classmethod
     def _assert_jit_static_attributes(
         cls, expected: Tuple[str, ...] = tuple()
     ) -> None:
```

### Comparing `jaxip-0.7.1/jaxip/simulation/lj.py` & `jaxip-0.7.2/jaxip/simulation/lj.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/simulation/mc.py` & `jaxip-0.7.2/jaxip/simulation/mc.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/simulation/md.py` & `jaxip-0.7.2/jaxip/simulation/md.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/simulation/run.py` & `jaxip-0.7.2/jaxip/simulation/run.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/simulation/thermostat.py` & `jaxip-0.7.2/jaxip/simulation/thermostat.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/types.py` & `jaxip-0.7.2/jaxip/types.py`

 * *Files 19% similar despite different names*

```diff
@@ -24,12 +24,7 @@
     FLOATX: Dtype = jnp.float32
     INT: Dtype = jnp.int32
     UINT: Dtype = jnp.uint32
     INDEX: Dtype = jnp.int32
 
 
 _dtype = DataType()
-
-
-# def set_as_default(dtype: Dtype) -> None:
-#     global _dtype
-#     _dtype = dtype
```

### Comparing `jaxip-0.7.1/jaxip/units.py` & `jaxip-0.7.2/jaxip/units.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/utils/attribute.py` & `jaxip-0.7.2/jaxip/utils/attribute.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/utils/batch.py` & `jaxip-0.7.2/jaxip/utils/batch.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/utils/compare.py` & `jaxip-0.7.2/jaxip/utils/compare.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/utils/profiler.py` & `jaxip-0.7.2/jaxip/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip/utils/tokenize.py` & `jaxip-0.7.2/jaxip/utils/tokenize.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/jaxip.egg-info/PKG-INFO` & `jaxip-0.7.2/jaxip.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxip
-Version: 0.7.1
+Version: 0.7.2
 Summary: JAX-based Interatomic Potential
 Home-page: https://github.com/hghcomphys/jaxip
 Author: Hossein Ghorbanfekr
 Author-email: hgh.comphys@gmail.com
 License: GNU General Public License v3
 Keywords: jaxip
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -36,23 +36,23 @@
         :target: https://jaxip.readthedocs.io/en/latest/?version=latest
         :alt: Documentation Status
 
 
 Description
 -----------
 Jaxip is an optimized Python library on basis of Google `JAX`_ that enables 
-development of emerging machine learning interatomic potentials 
-for use in computational physics, chemistry, and material science. 
+development of machine learning inter-atomic potentials 
+for use in computational physics and material science. 
 These potentials are necessary for conducting large-scale molecular 
 dynamics simulations of complex materials with ab initio accuracy.
 
 .. _JAX: https://github.com/google/jax
 
 
-See `documentation`_ for more information.
+See the `documentation`_ for more information.
 
 .. _documentation: https://jaxip.readthedocs.io/en/latest/readme.html
 
 
 Features
 --------
 * The design of Jaxip is `simple` and `flexible`, which makes it easy to incorporate atomic descriptors and potentials. 
@@ -70,102 +70,110 @@
 ------------
 To install Jaxip, run this command in your terminal:
 
 .. code-block:: console
 
     $ pip install jaxip
 
-For machines with an NVIDIA **GPU** please follow the installation
-`instruction <https://jaxip.readthedocs.io/en/latest/installation.html>`_ 
-on the documentation. 
+For machines with an NVIDIA **GPU** please follow the
+`installation <https://jaxip.readthedocs.io/en/latest/installation.html>`_ 
+instruction on the documentation. 
 
 
 Examples
 --------
 
------------------------------
-Defining an atomic descriptor
------------------------------
+---------------------------
+Defining an ACSF descriptor
+---------------------------
 This script demonstrates the process of evaluating an array of atomic-centered symmetry functions (`ACSF`_) 
 for a specific element, which can be utilized to evaluate the descriptor values for any structure. 
 The resulting values can then be used to construct a machine learning potential.
 
 .. _ACSF: https://aip.scitation.org/doi/10.1063/1.3553717
 
 
-
 .. code-block:: python
 
         from jaxip.datasets import RunnerDataset
         from jaxip.descriptors import ACSF
         from jaxip.descriptors.acsf import CutoffFunction, G2, G3
 
         # Read atomic structure dataset (e.g. water molecules)
         structures = RunnerDataset('input.data')
         structure = structures[0]
+        print(structure)
+        # >> Structure(natoms=12, elements=('H', 'O'), dtype=float32) 
 
-        # Define ACSF descriptor for hydrogen element
-        descriptor = ACSF(element='H')
-
-        # Add radial and angular symmetry functions
-        cfn = CutoffFunction(r_cutoff=12.0, cutoff_type='tanh')
+        # Define an ACSF descriptor for hydrogen element
+        # It includes two radial (G2) and angular (G3) symmetry functions
+        descriptor = ACSF('H')
+        cfn = CutoffFunction.from_cutoff_type(r_cutoff=12.0, cutoff_type='tanh')
         descriptor.add(G2(cfn, eta=0.5, r_shift=0.0), 'H')
         descriptor.add(G3(cfn, eta=0.001, zeta=2.0, lambda0=1.0, r_shift=12.0), 'H', 'O')
         print(descriptor)
+        # >> ACSF(central_element='H', symmetry_functions=2)
 
         values = descriptor(structure)
         print("Descriptor values:\n", values)
+        # >> Descriptor values:
+        # [[0.01952942 1.1310327 ]
+        # [0.01952756 1.0431229 ]
+        # ...
+        # [0.00228752 0.4144546 ]]
 
         gradient = descriptor.grad(structure, atom_index=0)
         print("Descriptor gradient:\n", gradient)
+        # >> Descriptor gradient:
+        # [[ 0.0464524  -0.05037863 -0.06146219]
+        # [-0.10481848 -0.01841717  0.04760207]]
 
 
--------------------------------------
-Training a machine learning potential
--------------------------------------
+-------------------------
+Training an NNP potential
+-------------------------
 This example illustrates how to quickly create a `high-dimensional neural network 
 potential` (`HDNNP`_) instance from an in input setting files and train it on input structures. 
 The trained potential can then be used to evaluate the energy and force components for new structures.
 
 .. _HDNNP: https://pubs.acs.org/doi/10.1021/acs.chemrev.0c00868
 
 
 .. code-block:: python
 
         from jaxip.datasets import RunnerDataset
         from jaxip.potentials import NeuralNetworkPotential
 
-        # Read atomic data
+        # Read atomic data in RuNNer format
         structures = RunnerDataset("input.data")
         structure = structures[0]
 
-        # Instantiate potential from input settings file
         nnp = NeuralNetworkPotential.from_file("input.nn")
 
-        # Fit descriptor scaler and model weights
         nnp.fit_scaler(structures)
         nnp.fit_model(structures)
-        nnp.save()
-
-        # Or loading from files
-        #nnp.load()
-
-        # Total energy
-        nnp(structure)
-
-        # Force components
-        nnp.compute_forces(structure)
+        # nnp.save()
+        # nnp.load()
 
+        total_energy = nnp(structure)
+        print(total_energy)
+        # >> -15.386198
+
+        forces = nnp.compute_forces(structure)
+        print(forces)
+        # >> [[ 1.6445214e-02 -4.1671786e-03  7.6140024e-02]
+        # [-6.4949177e-02 -4.2048577e-02  5.6018140e-02]
+        # ...
+        # [ 7.6149488e-03 -9.5360324e-02 -9.2892153e-03]]
 
 
 Example files: `input.data`_ and `input.nn`_
 
 .. _input.data: https://drive.google.com/file/d/1VMckgIv_OUvCOXQ0pYzaF5yl9AwR0rBy/view?usp=sharing
 .. _input.nn: https://drive.google.com/file/d/15Oq9gAJ2xXVMcHyWXlRukfJFevyVO7lI/view?usp=sharing
 
 
 
 License
 -------
-
 This project is licensed under the GNU General Public License (GPL) version 3 - 
 see the `LICENSE <https://github.com/hghcomphys/jaxip/blob/main/LICENSE>`_ file for details.
```

### Comparing `jaxip-0.7.1/jaxip.egg-info/SOURCES.txt` & `jaxip-0.7.2/jaxip.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/setup.py` & `jaxip-0.7.2/setup.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/tests/.ipynb_checkpoints/h2o-checkpoint.data` & `jaxip-0.7.2/tests/.ipynb_checkpoints/h2o-checkpoint.data`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/tests/.ipynb_checkpoints/h2o-checkpoint.json` & `jaxip-0.7.2/tests/.ipynb_checkpoints/h2o-checkpoint.json`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/tests/.ipynb_checkpoints/input.h2o-checkpoint.data` & `jaxip-0.7.2/tests/.ipynb_checkpoints/input.h2o-checkpoint.data`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/tests/.ipynb_checkpoints/test-checkpoint.ipynb` & `jaxip-0.7.2/tests/.ipynb_checkpoints/test-checkpoint.ipynb`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/tests/h2o.data` & `jaxip-0.7.2/tests/h2o.data`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/tests/h2o.json` & `jaxip-0.7.2/tests/h2o.json`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/tests/test_acsf.py` & `jaxip-0.7.2/tests/test_acsf.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,44 +13,48 @@
 from jaxip.types import Array
 
 
 # @pytest.fixture
 def lj_acsf() -> ACSF:
     """Initialize using the `add` method."""
     acsf: ACSF = ACSF("Ne")
-    cfn: CutoffFunction = CutoffFunction(3.0, cutoff_type="tanhu")
+    cfn: CutoffFunction = CutoffFunction.from_cutoff_type(
+        r_cutoff=3.0, cutoff_type="tanhu"
+    )
     acsf.add(G2(cfn, eta=1.00, r_shift=0.00), "Ne")
     acsf.add(G2(cfn, eta=1.00, r_shift=0.25), "Ne")
     acsf.add(G2(cfn, eta=1.00, r_shift=0.50), "Ne")
     acsf.add(G2(cfn, eta=1.00, r_shift=0.75), "Ne")
     acsf.add(G2(cfn, eta=1.00, r_shift=1.00), "Ne")
     return acsf
 
 
 def h2o_acsf() -> ACSF:
     """Initialize directly from the radial and angular terms."""
     return ACSF(
-        element="O",
+        central_element="O",
         radial_symmetry_functions=(
             (
                 EnvironmentElements(central="O", neighbor_j="H"),
                 G2(
-                    cfn=CutoffFunction(
+                    cfn=CutoffFunction.from_cutoff_type(
                         r_cutoff=5.9043202, cutoff_type="tanhu"
                     ),  # r_cutoff = box.length / 2
                     r_shift=0.0,
                     eta=0.001,
                 ),
             ),
         ),
         angular_symmetry_functions=(
             (
-                EnvironmentElements(central="O", neighbor_j="H", neighbor_k="H"),
+                EnvironmentElements(
+                    central="O", neighbor_j="H", neighbor_k="H"
+                ),
                 G3(
-                    cfn=CutoffFunction(
+                    cfn=CutoffFunction.from_cutoff_type(
                         r_cutoff=5.9043202, cutoff_type="tanhu"
                     ),  # r_cutoff = box.length / 2
                     eta=0.07,
                     zeta=1.0,
                     lambda0=1.0,
                     r_shift=0.0,
                 ),
@@ -58,15 +62,18 @@
         ),
     )
 
 
 class TestACSF:
     lj_structure: Structure = Structure.from_dict(
         {
-            "positions": [[0.0, 0.0, 0.0], [0.588897275, 0.588897275, 0.588897275]],
+            "positions": [
+                [0.0, 0.0, 0.0],
+                [0.588897275, 0.588897275, 0.588897275],
+            ],
             "elements": ["Ne", "Ne"],
         }
     )
     h2o_structure: Structure = Structure.from_dict(
         {
             "lattice": [
                 [11.8086403654, 0.0, 0.0],
@@ -83,15 +90,28 @@
                 [-2.2136818837, 1.3673642557, 2.7768013741],
                 [-1.9466635812, -0.3397746484, 3.3828743394],
                 [-0.4559776878, 0.1681476423, -5.430449296],
                 [-1.2831542798, 4.5473991714, -2.294184217],
                 [-2.3516507887, 0.9376745482, -4.0756290424],
                 [-1.7819663898, 4.1957022409, -4.0621741923],
             ],
-            "elements": ["O", "H", "H", "O", "H", "H", "O", "H", "H", "O", "H", "H"],
+            "elements": [
+                "O",
+                "H",
+                "H",
+                "O",
+                "H",
+                "H",
+                "O",
+                "H",
+                "H",
+                "O",
+                "H",
+                "H",
+            ],
         }
     )
 
     @pytest.mark.parametrize(
         "acsf, expected",
         [
             (
@@ -101,15 +121,15 @@
         ],
     )
     def test_acsf_attributes(
         self,
         acsf: ACSF,
         expected: Tuple,
     ) -> None:
-        assert acsf.element == expected[0]
+        assert acsf.central_element == expected[0]
         assert acsf.num_radial_symmetry_functions == expected[1]
         assert acsf.num_angular_symmetry_functions == expected[2]
         assert acsf.num_symmetry_functions == expected[3]
         assert acsf.r_cutoff == expected[4]
 
     @pytest.mark.parametrize(
         "acsf, structure, expected",
@@ -157,8 +177,10 @@
     def test_acsf_with_pbc(
         self,
         acsf: ACSF,
         structure: Structure,
         expected: Array,
     ) -> None:
         assert acsf(structure).shape == expected[0]
-        assert jnp.allclose(acsf(structure, atom_indices=jnp.asarray(0)), expected[1])
+        assert jnp.allclose(
+            acsf(structure, atom_indices=jnp.asarray(0)), expected[1]
+        )
```

### Comparing `jaxip-0.7.1/tests/test_mc.py` & `jaxip-0.7.2/tests/test_mc.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/tests/test_md.py` & `jaxip-0.7.2/tests/test_md.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/tests/test_nn.py` & `jaxip-0.7.2/tests/test_nn.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/tests/test_nnp.py` & `jaxip-0.7.2/tests/test_nnp.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/tests/test_runner.py` & `jaxip-0.7.2/tests/test_runner.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/tests/test_scaler.py` & `jaxip-0.7.2/tests/test_scaler.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/tests/test_structure.py` & `jaxip-0.7.2/tests/test_structure.py`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/tests/weights.001.pkl` & `jaxip-0.7.2/tests/weights.001.pkl`

 * *Files identical despite different names*

### Comparing `jaxip-0.7.1/tests/weights.008.pkl` & `jaxip-0.7.2/tests/weights.008.pkl`

 * *Files identical despite different names*

