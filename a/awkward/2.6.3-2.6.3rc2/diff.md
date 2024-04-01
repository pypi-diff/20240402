# Comparing `tmp/awkward-2.6.3.tar.gz` & `tmp/awkward-2.6.3rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Mon Apr  1 18:26:47 2024, max compression
+gzip compressed data, last modified: Thu Mar 21 23:08:24 2024, max compression
```

## Comparing `awkward-2.6.3.tar` & `awkward-2.6.3rc2.tar`

### file list

```diff
@@ -1,1458 +1,1455 @@
--rw-r--r--   0        0        0     1889 2024-04-01 18:26:47.000000 awkward-2.6.3/CITATION.cff
--rw-r--r--   0        0        0    14355 2024-04-01 18:26:47.000000 awkward-2.6.3/CONTRIBUTING.md
--rw-r--r--   0        0        0    26295 2024-04-01 18:26:47.000000 awkward-2.6.3/README.md
--rw-r--r--   0        0        0      173 2024-04-01 18:26:47.000000 awkward-2.6.3/juliapkg.json
--rw-r--r--   0        0        0      393 2024-04-01 18:26:47.000000 awkward-2.6.3/requirements-test-full.txt
--rw-r--r--   0        0        0      105 2024-04-01 18:26:47.000000 awkward-2.6.3/requirements-test-minimal.txt
--rw-r--r--   0        0        0     8686 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/_toc.yml
--rw-r--r--   0        0        0     7735 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/conf.py
--rw-r--r--   0        0        0      346 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/environment.yml.cog
--rw-r--r--   0        0        0     3469 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/index.md
--rw-r--r--   0        0        0    11690 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/prepare_docstrings.py
--rw-r--r--   0        0        0     4448 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/redirects-user-guide.json
--rw-r--r--   0        0        0    11440 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/redirects.json
--rw-r--r--   0        0        0       33 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/requirements-wasm.txt
--rw-r--r--   0        0        0      571 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/requirements.txt
--rw-r--r--   0        0        0      825 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/switcher.json
--rw-r--r--   0        0        0      942 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/_static/css/awkward.css
--rw-r--r--   0        0        0      355 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/_static/css/try-awkward-array.css
-lrwxr-xr-x   0        0        0        0 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/_static/image/logo-300px-white.png -> ../../../docs-img/logo/logo-300px-white.png
-lrwxr-xr-x   0        0        0        0 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/_static/image/logo-300px.png -> ../../../docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0      469 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/_templates/funding.html
--rw-r--r--   0        0        0      474 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/_templates/redirect.html
--rw-r--r--   0        0        0   245975 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/data/y77d-th95.json
--rw-r--r--   0        0        0     2968 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/getting-started/community-tutorials.md
--rw-r--r--   0        0        0     4654 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/getting-started/index.md
--rw-r--r--   0        0        0     3346 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/getting-started/papers-and-talks.md
--rw-r--r--   0        0        0       93 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/getting-started/try-awkward-array.md
-lrwxr-xr-x   0        0        0        0 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/getting-started/demo/example-reduction-sum.svg -> ../../../docs-img/diagrams/example-reduction-sum.svg
--rw-r--r--   0        0        0    13128 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/getting-started/demo/what-is-an-awkward-array.ipynb
-lrwxr-xr-x   0        0        0        0 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/image/awkward-1-0-layers.svg -> ../../docs-img/diagrams/awkward-1-0-layers.svg
-lrwxr-xr-x   0        0        0        0 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/image/bikeroutes-scaling.svg -> ../../docs-img/plots/bikeroutes-scaling.svg
-lrwxr-xr-x   0        0        0        0 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/image/desire-path.jpg -> ../../docs-img/photos/desire-path.jpg
-lrwxr-xr-x   0        0        0        0 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/image/example-array.svg -> ../../docs-img/diagrams/example-array.svg
--rw-r--r--   0        0        0    17067 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/image/example-hierarchy.svg
-lrwxr-xr-x   0        0        0        0 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/image/example-reduction-sum-only.svg -> ../../docs-img/diagrams/example-reduction-sum-only.svg
-lrwxr-xr-x   0        0        0        0 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/image/example-reduction-sum.svg -> ../../docs-img/diagrams/example-reduction-sum.svg
-lrwxr-xr-x   0        0        0        0 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/image/favicon.ico -> ../../docs-img/logo/favicon.ico
-lrwxr-xr-x   0        0        0        0 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/image/github-issues-documentation.png -> ../../docs-img/screenshots/github-issues-documentation.png
-lrwxr-xr-x   0        0        0        0 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/image/how-it-works.svg -> ../../docs-img/diagrams/how-it-works.svg
-lrwxr-xr-x   0        0        0        0 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/image/logo-300px.png -> ../../docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0    24232 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/reference/ak.behavior.md
--rw-r--r--   0        0        0     1426 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/reference/ak.builder.ArrayBuilder.rst
--rw-r--r--   0        0        0    64727 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/reference/awkwardforth.rst
--rw-r--r--   0        0        0      271 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/reference/index.md
--rw-r--r--   0        0        0     9491 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/reference/toctree.txt
--rw-r--r--   0        0        0   214211 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/samples/Android.head.log.gz
--rw-r--r--   0        0        0     8320 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/10-minutes-to-awkward-array.md
--rw-r--r--   0        0        0      926 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-combinatorics-best-match.md
--rw-r--r--   0        0        0      930 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-combinatorics-cartesian-combinations.md
--rw-r--r--   0        0        0      263 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-combinatorics.md
--rw-r--r--   0        0        0     8335 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-convert-arrow.md
--rw-r--r--   0        0        0     6323 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-convert-buffers.md
--rw-r--r--   0        0        0     2455 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-convert-json.md
--rw-r--r--   0        0        0    13475 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-convert-numpy.md
--rw-r--r--   0        0        0     7182 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-convert-pandas.md
--rw-r--r--   0        0        0    18472 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-convert-python.md
--rw-r--r--   0        0        0     3554 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-convert-rdataframe.md
--rw-r--r--   0        0        0      271 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-convert.md
--rw-r--r--   0        0        0    11973 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-create-arraybuilder.md
--rw-r--r--   0        0        0    36902 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-create-constructors.md
--rw-r--r--   0        0        0     7383 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-create-lists.md
--rw-r--r--   0        0        0     7456 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-create-missing.md
--rw-r--r--   0        0        0    11542 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-create-records.md
--rw-r--r--   0        0        0     4093 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-create-strings.md
--rw-r--r--   0        0        0     4364 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-create-unflatten-group.md
--rw-r--r--   0        0        0      267 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-create.md
--rw-r--r--   0        0        0      834 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-examine-checking-validity.md
--rw-r--r--   0        0        0     2919 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-examine-list-fields.md
--rw-r--r--   0        0        0      848 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-examine-simple-slicing.md
--rw-r--r--   0        0        0      838 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-examine-single-item.md
--rw-r--r--   0        0        0     6778 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-examine-type.md
--rw-r--r--   0        0        0      269 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-examine.md
--rw-r--r--   0        0        0      844 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-filter-cut-mask.md
--rw-r--r--   0        0        0     3889 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-filter-masked.md
--rw-r--r--   0        0        0      840 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-filter-num.md
--rw-r--r--   0        0        0     7955 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-filter-ragged.md
--rw-r--r--   0        0        0      265 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-filter.md
--rw-r--r--   0        0        0      818 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-math-argminmax.md
--rw-r--r--   0        0        0      822 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-math-broadcasting.md
--rw-r--r--   0        0        0      828 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-math-gpu.md
--rw-r--r--   0        0        0      838 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-math-numpy.md
--rw-r--r--   0        0        0      846 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-math-reducing.md
--rw-r--r--   0        0        0      870 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-math-statistics.md
--rw-r--r--   0        0        0      265 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-math.md
--rw-r--r--   0        0        0     3411 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-restructure-add-fields.md
--rw-r--r--   0        0        0      842 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-restructure-concatenate.md
--rw-r--r--   0        0        0    19083 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-restructure-flatten.md
--rw-r--r--   0        0        0     7568 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-restructure-pad.md
--rw-r--r--   0        0        0      852 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-restructure-rename-records.md
--rw-r--r--   0        0        0      832 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-restructure-sort.md
--rw-r--r--   0        0        0     9624 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-restructure-zip-project.md
--rw-r--r--   0        0        0      273 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-restructure.md
--rw-r--r--   0        0        0     2599 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-specialize-differentiate-jax.md
--rw-r--r--   0        0        0      870 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-specialize-in-numba.md
--rw-r--r--   0        0        0      838 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-specialize-lorentz.md
--rw-r--r--   0        0        0      874 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-specialize-override-numpy.md
--rw-r--r--   0        0        0      870 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-specialize-subclass.md
--rw-r--r--   0        0        0      277 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-specialize.md
--rw-r--r--   0        0        0    10650 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-strings-extract-substrings.md
--rw-r--r--   0        0        0     5030 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-strings-read-binary.md
--rw-r--r--   0        0        0     5734 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-strings-split-and-join.md
--rw-r--r--   0        0        0    11694 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-use-header-only-layoutbuilder.md
--rw-r--r--   0        0        0     7580 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-use-in-cpp-cppyy.ipynb
--rw-r--r--   0        0        0      277 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-use-in-cpp.md
--rw-r--r--   0        0        0      900 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-use-in-numba-arraybuilder.md
--rw-r--r--   0        0        0     9973 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-use-in-numba-cuda.ipynb
--rw-r--r--   0        0        0      900 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-use-in-numba-features.md
--rw-r--r--   0        0        0      279 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/how-to-use-in-numba.md
--rw-r--r--   0        0        0      344 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/index.md
--rw-r--r--   0        0        0        0 2024-04-01 18:26:47.000000 awkward-2.6.3/docs/user-guide/requirements.txt
--rw-r--r--   0        0        0   367587 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/panel-data-analysts.png
--rw-r--r--   0        0        0   794465 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/panel-data-analysts.svg
--rw-r--r--   0        0        0   140700 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/panel-developers.png
--rw-r--r--   0        0        0   328307 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/panel-developers.svg
--rw-r--r--   0        0        0    73584 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/panel-doxygen.png
--rw-r--r--   0        0        0    58179 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/panel-sphinx.png
--rw-r--r--   0        0        0   127063 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/panel-tutorials-alternate.png
--rw-r--r--   0        0        0   173327 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/panel-tutorials.png
--rw-r--r--   0        0        0    12541 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/awkward-1-0-layers.pdf
--rw-r--r--   0        0        0    65246 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/awkward-1-0-layers.png
--rw-r--r--   0        0        0    41004 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/awkward-1-0-layers.svg
--rw-r--r--   0        0        0    14946 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/awkward-timeline.pdf
--rw-r--r--   0        0        0   125180 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/awkward-timeline.png
--rw-r--r--   0        0        0    70209 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/awkward-timeline.svg
--rw-r--r--   0        0        0   436595 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/awkward-uproot-timeline-pip-github.png
--rw-r--r--   0        0        0   426911 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg
--rw-r--r--   0        0        0   335955 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/awkward-uproot-timeline-pip.png
--rw-r--r--   0        0        0   325268 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/awkward-uproot-timeline-pip.svg
--rw-r--r--   0        0        0   129696 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/awkward-uproot-timeline.png
--rw-r--r--   0        0        0   120554 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/awkward-uproot-timeline.svg
--rw-r--r--   0        0        0     5208 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/cartoon-broadcasting.png
--rw-r--r--   0        0        0    25065 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/cartoon-broadcasting.svg
--rw-r--r--   0        0        0     5754 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/cartoon-cartesian.png
--rw-r--r--   0        0        0    32616 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/cartoon-cartesian.svg
--rw-r--r--   0        0        0     9584 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/cartoon-combinations.png
--rw-r--r--   0        0        0    39524 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/cartoon-combinations.svg
--rw-r--r--   0        0        0    10808 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/cartoon-schematic.png
--rw-r--r--   0        0        0    25779 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/cartoon-schematic.svg
--rw-r--r--   0        0        0    18178 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/example-array.svg
--rw-r--r--   0        0        0    36024 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/example-hierarchy.png
--rw-r--r--   0        0        0    17092 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/example-hierarchy.svg
--rw-r--r--   0        0        0    21120 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/example-reduction-sum-only.svg
--rw-r--r--   0        0        0    29325 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/example-reduction-sum.svg
--rw-r--r--   0        0        0    55553 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/example-reduction.png
--rw-r--r--   0        0        0    21631 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/example-reduction.svg
--rw-r--r--   0        0        0    10978 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/git-strategy.pdf
--rw-r--r--   0        0        0    58904 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/git-strategy.png
--rw-r--r--   0        0        0    28990 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/git-strategy.svg
--rw-r--r--   0        0        0   113587 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/how-it-works-muons.png
--rw-r--r--   0        0        0    57471 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/how-it-works-muons.svg
--rw-r--r--   0        0        0    58475 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/how-it-works.svg
--rw-r--r--   0        0        0    63989 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/sorting-axis.svg
--rw-r--r--   0        0        0   124038 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/reducers/all.svg
--rw-r--r--   0        0        0   128558 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/reducers/any.svg
--rw-r--r--   0        0        0   134490 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/reducers/argmax.svg
--rw-r--r--   0        0        0   133192 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/reducers/argmin.svg
--rw-r--r--   0        0        0   106277 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/reducers/count.svg
--rw-r--r--   0        0        0   116417 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/reducers/count_nonzero.svg
--rw-r--r--   0        0        0   111789 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/reducers/max.svg
--rw-r--r--   0        0        0   109239 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/reducers/min.svg
--rw-r--r--   0        0        0   124702 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/reducers/product.svg
--rw-r--r--   0        0        0   108897 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/diagrams/reducers/sum.svg
--rw-r--r--   0        0        0     8347 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/logo/favicon.ico
--rw-r--r--   0        0        0     8984 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/logo/logo-300px-white.png
--rw-r--r--   0        0        0    11964 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0    24707 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/logo/logo-600px.png
--rw-r--r--   0        0        0    18767 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/logo/logo.svg
--rw-r--r--   0        0        0    90413 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/photos/desire-path.jpg
--rw-r--r--   0        0        0    52113 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/plots/awkward-0-popularity.pdf
--rw-r--r--   0        0        0   146109 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/plots/awkward-0-popularity.png
--rw-r--r--   0        0        0   147576 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/plots/awkward-0-popularity.svg
--rw-r--r--   0        0        0    26938 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/plots/bikeroutes-scaling.svg
--rw-r--r--   0        0        0     8891 2024-04-01 18:26:47.000000 awkward-2.6.3/docs-img/screenshots/github-issues-documentation.png
--rw-r--r--   0        0        0     1288 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/__init__.py
--rw-r--r--   0        0        0     1210 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_attrs.py
--rw-r--r--   0        0        0     5709 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_behavior.py
--rw-r--r--   0        0        0    36351 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_broadcasting.py
--rw-r--r--   0        0        0     1293 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_categorical.py
--rw-r--r--   0        0        0     2849 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_dispatch.py
--rw-r--r--   0        0        0    13568 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_do.py
--rw-r--r--   0        0        0    15027 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_errors.py
--rw-r--r--   0        0        0      370 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_ext.py
--rw-r--r--   0        0        0     5876 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_kernels.py
--rw-r--r--   0        0        0    11380 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_layout.py
--rw-r--r--   0        0        0    10016 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_lookup.py
--rw-r--r--   0        0        0     8477 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_operators.py
--rw-r--r--   0        0        0     5023 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_parameters.py
--rw-r--r--   0        0        0     3746 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_pickle.py
--rw-r--r--   0        0        0    13901 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_prettyprint.py
--rw-r--r--   0        0        0    29470 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_reducers.py
--rw-r--r--   0        0        0     1490 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_regularize.py
--rw-r--r--   0        0        0     1212 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_singleton.py
--rw-r--r--   0        0        0    23669 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_slicing.py
--rw-r--r--   0        0        0      732 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_typetracer.py
--rw-r--r--   0        0        0     1451 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_typing.py
--rw-r--r--   0        0        0     2411 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_util.py
--rw-r--r--   0        0        0      790 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_v2.py
--rw-r--r--   0        0        0      231 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/builder.py
--rw-r--r--   0        0        0      922 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/cppyy.py
--rw-r--r--   0        0        0      290 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/errors.py
--rw-r--r--   0        0        0      269 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/forth.py
--rw-r--r--   0        0        0   112732 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/highlevel.py
--rw-r--r--   0        0        0     9627 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/index.py
--rw-r--r--   0        0        0     4073 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/jax.py
--rw-r--r--   0        0        0     8386 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/record.py
--rw-r--r--   0        0        0     8239 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/typetracer.py
--rw-r--r--   0        0        0       84 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_backends/__init__.py
--rw-r--r--   0        0        0     1916 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_backends/backend.py
--rw-r--r--   0        0        0     1288 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_backends/cupy.py
--rw-r--r--   0        0        0     4246 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_backends/dispatch.py
--rw-r--r--   0        0        0     1318 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_backends/jax.py
--rw-r--r--   0        0        0      973 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_backends/numpy.py
--rw-r--r--   0        0        0     1454 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_backends/typetracer.py
--rw-r--r--   0        0        0       84 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/__init__.py
--rw-r--r--   0        0        0    32644 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/avro.py
--rw-r--r--   0        0        0    53565 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cling.py
--rw-r--r--   0        0        0      484 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/dlpack.py
--rw-r--r--   0        0        0      983 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/hist.py
--rw-r--r--   0        0        0     4701 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/numexpr.py
--rw-r--r--   0        0        0    16958 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/numpy.py
--rw-r--r--   0        0        0    40019 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/pyarrow.py
--rw-r--r--   0        0        0     8546 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/__init__.py
--rw-r--r--   0        0        0   284416 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/_kernel_signatures.py
--rw-r--r--   0        0        0     2333 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu
--rw-r--r--   0        0        0     4085 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu
--rw-r--r--   0        0        0     1959 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu
--rw-r--r--   0        0        0     2259 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu
--rw-r--r--   0        0        0     1756 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_numnull.cu
--rw-r--r--   0        0        0      637 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu
--rw-r--r--   0        0        0     2540 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu
--rw-r--r--   0        0        0     2474 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu
--rw-r--r--   0        0        0     2678 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu
--rw-r--r--   0        0        0      549 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu
--rw-r--r--   0        0        0     2661 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu
--rw-r--r--   0        0        0     2114 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_nones_as_index.cu
--rw-r--r--   0        0        0      590 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill.cu
--rw-r--r--   0        0        0      502 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu
--rw-r--r--   0        0        0     2353 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu
--rw-r--r--   0        0        0     3316 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_none2empty.cu
--rw-r--r--   0        0        0     2371 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu
--rw-r--r--   0        0        0     2684 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu
--rw-r--r--   0        0        0     2229 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_index_of_nulls.cu
--rw-r--r--   0        0        0     1707 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_numnull.cu
--rw-r--r--   0        0        0     1961 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_numnull_parents.cu
--rw-r--r--   0        0        0      468 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_numnull_unique_64.cu
--rw-r--r--   0        0        0      550 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu
--rw-r--r--   0        0        0     2535 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_ranges_carry_next_64.cu
--rw-r--r--   0        0        0     2865 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_ranges_next_64.cu
--rw-r--r--   0        0        0     2433 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu
--rw-r--r--   0        0        0      580 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu
--rw-r--r--   0        0        0     2339 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu
--rw-r--r--   0        0        0     2543 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu
--rw-r--r--   0        0        0      884 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu
--rw-r--r--   0        0        0      836 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu
--rw-r--r--   0        0        0     2005 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu
--rw-r--r--   0        0        0     3835 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_broadcast_tooffsets.cu
--rw-r--r--   0        0        0     3234 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_combinations_length.cu
--rw-r--r--   0        0        0     2434 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu
--rw-r--r--   0        0        0      715 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_fill.cu
--rw-r--r--   0        0        0     2006 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_carrylen.cu
--rw-r--r--   0        0        0     3305 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_descend.cu
--rw-r--r--   0        0        0     1484 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu
--rw-r--r--   0        0        0     2810 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_numvalid.cu
--rw-r--r--   0        0        0     1720 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu
--rw-r--r--   0        0        0     1663 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array_advanced.cu
--rw-r--r--   0        0        0      958 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_at.cu
--rw-r--r--   0        0        0     1815 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_range_counts.cu
--rw-r--r--   0        0        0      695 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_range_spreadadvanced.cu
--rw-r--r--   0        0        0      617 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_localindex.cu
--rw-r--r--   0        0        0     2026 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_min_range.cu
--rw-r--r--   0        0        0     2067 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_rpad_and_clip_length_axis1.cu
--rw-r--r--   0        0        0     2712 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_rpad_axis1.cu
--rw-r--r--   0        0        0     1076 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu
--rw-r--r--   0        0        0     2525 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_drop_none_indexes.cu
--rw-r--r--   0        0        0      595 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu
--rw-r--r--   0        0        0     1106 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_local_preparenext_64.cu
--rw-r--r--   0        0        0      693 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_local_nextparents_64.cu
--rw-r--r--   0        0        0     2240 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_nonlocal_maxcount_offsetscopy_64.cu
--rw-r--r--   0        0        0     2045 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_nonlocal_nextstarts_64.cu
--rw-r--r--   0        0        0      974 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu
--rw-r--r--   0        0        0     1525 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu
--rw-r--r--   0        0        0     2302 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_length_axis1.cu
--rw-r--r--   0        0        0     1118 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_toRegularArray.cu
--rw-r--r--   0        0        0     2383 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu
--rw-r--r--   0        0        0      497 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill.cu
--rw-r--r--   0        0        0     1755 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_pad_zero_to_length.cu
--rw-r--r--   0        0        0      645 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu
--rw-r--r--   0        0        0      704 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu
--rw-r--r--   0        0        0      577 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu
--rw-r--r--   0        0        0      639 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu
--rw-r--r--   0        0        0      811 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu
--rw-r--r--   0        0        0      773 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu
--rw-r--r--   0        0        0      690 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu
--rw-r--r--   0        0        0      909 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_regularize.cu
--rw-r--r--   0        0        0      814 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu
--rw-r--r--   0        0        0      699 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu
--rw-r--r--   0        0        0      651 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu
--rw-r--r--   0        0        0      556 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu
--rw-r--r--   0        0        0     1946 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_reduce_local_nextparents.cu
--rw-r--r--   0        0        0     2353 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_reduce_nonlocal_preparenext.cu
--rw-r--r--   0        0        0      825 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_rpad_and_clip_axis1.cu
--rw-r--r--   0        0        0      520 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillindex.cu
--rw-r--r--   0        0        0      479 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillindex_count.cu
--rw-r--r--   0        0        0      503 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu
--rw-r--r--   0        0        0      540 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_filltags.cu
--rw-r--r--   0        0        0      487 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_filltags_const.cu
--rw-r--r--   0        0        0     2195 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu
--rw-r--r--   0        0        0      864 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_regular_index_getsize.cu
--rw-r--r--   0        0        0      893 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_simplify.cu
--rw-r--r--   0        0        0      709 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_simplify_one.cu
--rw-r--r--   0        0        0     1221 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu
--rw-r--r--   0        0        0      652 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis0.cu
--rw-r--r--   0        0        0      544 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu
--rw-r--r--   0        0        0      417 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_localindex.cu
--rw-r--r--   0        0        0      721 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu
--rw-r--r--   0        0        0     1910 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu
--rw-r--r--   0        0        0     1819 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu
--rw-r--r--   0        0        0     2756 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu
--rw-r--r--   0        0        0     2935 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu
--rw-r--r--   0        0        0     1830 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu
--rw-r--r--   0        0        0     1830 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu
--rw-r--r--   0        0        0     2890 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu
--rw-r--r--   0        0        0     2670 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu
--rw-r--r--   0        0        0     2873 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu
--rw-r--r--   0        0        0     3015 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu
--rw-r--r--   0        0        0     3015 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu
--rw-r--r--   0        0        0     2337 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_sorting_ranges.cu
--rw-r--r--   0        0        0     1873 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_sorting_ranges_length.cu
--rw-r--r--   0        0        0     4774 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu
--rw-r--r--   0        0        0     1624 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/header-only/awkward/BuilderOptions.h
--rw-r--r--   0        0        0    19818 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/header-only/awkward/GrowableBuffer.h
--rw-r--r--   0        0        0    84571 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/header-only/awkward/LayoutBuilder.h
--rw-r--r--   0        0        0     9545 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/header-only/awkward/utils.h
--rw-r--r--   0        0        0      367 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/jax/__init__.py
--rw-r--r--   0        0        0    11453 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/jax/reducers.py
--rw-r--r--   0        0        0     5980 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/jax/trees.py
--rw-r--r--   0        0        0       84 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/numba/__init__.py
--rw-r--r--   0        0        0    36568 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/numba/arrayview.py
--rw-r--r--   0        0        0     1264 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/numba/arrayview_cuda.py
--rw-r--r--   0        0        0    32515 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/numba/builder.py
--rw-r--r--   0        0        0     9730 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/numba/growablebuffer.py
--rw-r--r--   0        0        0    52143 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/numba/layout.py
--rw-r--r--   0        0        0    43392 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/numba/layoutbuilder.py
--rw-r--r--   0        0        0       84 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/rdataframe/__init__.py
--rw-r--r--   0        0        0     9411 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/rdataframe/from_rdataframe.py
--rw-r--r--   0        0        0     9954 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/rdataframe/to_rdataframe.py
--rw-r--r--   0        0        0     1483 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h
--rw-r--r--   0        0        0        0 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_meta/__init__.py
--rw-r--r--   0        0        0     1424 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_meta/bitmaskedmeta.py
--rw-r--r--   0        0        0     1425 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_meta/bytemaskedmeta.py
--rw-r--r--   0        0        0      966 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_meta/emptymeta.py
--rw-r--r--   0        0        0     1412 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_meta/indexedmeta.py
--rw-r--r--   0        0        0     1463 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_meta/indexedoptionmeta.py
--rw-r--r--   0        0        0     1824 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_meta/listmeta.py
--rw-r--r--   0        0        0     1834 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_meta/listoffsetmeta.py
--rw-r--r--   0        0        0     3760 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_meta/meta.py
--rw-r--r--   0        0        0     1310 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_meta/numpymeta.py
--rw-r--r--   0        0        0     4085 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_meta/recordmeta.py
--rw-r--r--   0        0        0     1945 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_meta/regularmeta.py
--rw-r--r--   0        0        0     3065 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_meta/unionmeta.py
--rw-r--r--   0        0        0     1435 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_meta/unmaskedmeta.py
--rw-r--r--   0        0        0     1350 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_nplikes/__init__.py
--rw-r--r--   0        0        0     3152 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_nplikes/array_like.py
--rw-r--r--   0        0        0    23468 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_nplikes/array_module.py
--rw-r--r--   0        0        0     5706 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_nplikes/cupy.py
--rw-r--r--   0        0        0     1615 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_nplikes/dispatch.py
--rw-r--r--   0        0        0     2529 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_nplikes/jax.py
--rw-r--r--   0        0        0     2086 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_nplikes/numpy.py
--rw-r--r--   0        0        0    12698 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_nplikes/numpy_like.py
--rw-r--r--   0        0        0     4553 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_nplikes/placeholder.py
--rw-r--r--   0        0        0     2402 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_nplikes/shape.py
--rw-r--r--   0        0        0    60519 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_nplikes/typetracer.py
--rw-r--r--   0        0        0     2648 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/_nplikes/ufuncs.py
--rw-r--r--   0        0        0       84 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/behaviors/__init__.py
--rw-r--r--   0        0        0      186 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/behaviors/categorical.py
--rw-r--r--   0        0        0     3931 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/behaviors/mixins.py
--rw-r--r--   0        0        0      250 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/behaviors/string.py
--rw-r--r--   0        0        0     1018 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/contents/__init__.py
--rw-r--r--   0        0        0    28854 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/contents/bitmaskedarray.py
--rw-r--r--   0        0        0    42368 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/contents/bytemaskedarray.py
--rw-r--r--   0        0        0    43592 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/contents/content.py
--rw-r--r--   0        0        0    13977 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/contents/emptyarray.py
--rw-r--r--   0        0        0    43371 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/contents/indexedarray.py
--rw-r--r--   0        0        0    66660 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/contents/indexedoptionarray.py
--rw-r--r--   0        0        0    63078 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/contents/listarray.py
--rw-r--r--   0        0        0    88691 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/contents/listoffsetarray.py
--rw-r--r--   0        0        0    49445 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/contents/numpyarray.py
--rw-r--r--   0        0        0    46575 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/contents/recordarray.py
--rw-r--r--   0        0        0    58528 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/contents/regulararray.py
--rw-r--r--   0        0        0    60274 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/contents/unionarray.py
--rw-r--r--   0        0        0    20007 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/contents/unmaskedarray.py
--rw-r--r--   0        0        0      994 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/forms/__init__.py
--rw-r--r--   0        0        0     6344 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/forms/bitmaskedform.py
--rw-r--r--   0        0        0     5562 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/forms/bytemaskedform.py
--rw-r--r--   0        0        0     3485 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/forms/emptyform.py
--rw-r--r--   0        0        0    22946 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/forms/form.py
--rw-r--r--   0        0        0     5940 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/forms/indexedform.py
--rw-r--r--   0        0        0     5298 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/forms/indexedoptionform.py
--rw-r--r--   0        0        0     5387 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/forms/listform.py
--rw-r--r--   0        0        0     4627 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/forms/listoffsetform.py
--rw-r--r--   0        0        0     8044 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/forms/numpyform.py
--rw-r--r--   0        0        0     6693 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/forms/recordform.py
--rw-r--r--   0        0        0     4692 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/forms/regularform.py
--rw-r--r--   0        0        0     6650 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/forms/unionform.py
--rw-r--r--   0        0        0     4376 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/forms/unmaskedform.py
--rw-r--r--   0        0        0     9532 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/numba/__init__.py
--rw-r--r--   0        0        0    23941 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/numba/layoutbuilder.py
--rw-r--r--   0        0        0     5243 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/__init__.py
--rw-r--r--   0        0        0     3391 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_all.py
--rw-r--r--   0        0        0     8574 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_almost_equal.py
--rw-r--r--   0        0        0     1902 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_angle.py
--rw-r--r--   0        0        0     3394 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_any.py
--rw-r--r--   0        0        0     4426 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_argcartesian.py
--rw-r--r--   0        0        0     3792 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_argcombinations.py
--rw-r--r--   0        0        0     5771 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_argmax.py
--rw-r--r--   0        0        0     5632 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_argmin.py
--rw-r--r--   0        0        0     3241 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_argsort.py
--rw-r--r--   0        0        0     1141 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_backend.py
--rw-r--r--   0        0        0     9915 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_broadcast_arrays.py
--rw-r--r--   0        0        0     7278 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_broadcast_fields.py
--rw-r--r--   0        0        0    15811 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_cartesian.py
--rw-r--r--   0        0        0     1709 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_categories.py
--rw-r--r--   0        0        0     8091 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_combinations.py
--rw-r--r--   0        0        0    26808 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_concatenate.py
--rw-r--r--   0        0        0     2773 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_copy.py
--rw-r--r--   0        0        0     6533 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_corr.py
--rw-r--r--   0        0        0     4619 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_count.py
--rw-r--r--   0        0        0     3418 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_count_nonzero.py
--rw-r--r--   0        0        0     5733 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_covar.py
--rw-r--r--   0        0        0     4745 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_drop_none.py
--rw-r--r--   0        0        0    50491 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_enforce_type.py
--rw-r--r--   0        0        0     1175 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_fields.py
--rw-r--r--   0        0        0     4667 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_fill_none.py
--rw-r--r--   0        0        0     3523 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_firsts.py
--rw-r--r--   0        0        0     7810 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_flatten.py
--rw-r--r--   0        0        0     3214 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_from_arrow.py
--rw-r--r--   0        0        0      785 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_from_arrow_schema.py
--rw-r--r--   0        0        0     2629 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_from_avro_file.py
--rw-r--r--   0        0        0    16560 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_from_buffers.py
--rw-r--r--   0        0        0     1876 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_from_categorical.py
--rw-r--r--   0        0        0     1591 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_from_cupy.py
--rw-r--r--   0        0        0     3009 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_from_dlpack.py
--rw-r--r--   0        0        0     2437 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_from_feather.py
--rw-r--r--   0        0        0     4080 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_from_iter.py
--rw-r--r--   0        0        0     1667 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_from_jax.py
--rw-r--r--   0        0        0    28871 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_from_json.py
--rw-r--r--   0        0        0     2206 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_from_numpy.py
--rw-r--r--   0        0        0    11541 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_from_parquet.py
--rw-r--r--   0        0        0     3163 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_from_rdataframe.py
--rw-r--r--   0        0        0     3083 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_from_regular.py
--rw-r--r--   0        0        0     9235 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_full_like.py
--rw-r--r--   0        0        0     1713 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_imag.py
--rw-r--r--   0        0        0      951 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_is_categorical.py
--rw-r--r--   0        0        0     2606 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_is_none.py
--rw-r--r--   0        0        0      921 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_is_tuple.py
--rw-r--r--   0        0        0      965 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_is_valid.py
--rw-r--r--   0        0        0     2640 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_isclose.py
--rw-r--r--   0        0        0     8525 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_linear_fit.py
--rw-r--r--   0        0        0     3434 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_local_index.py
--rw-r--r--   0        0        0     4720 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_mask.py
--rw-r--r--   0        0        0     6035 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_max.py
--rw-r--r--   0        0        0     9367 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_mean.py
--rw-r--r--   0        0        0     3699 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_merge_option_of_records.py
--rw-r--r--   0        0        0    12416 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_merge_union_of_records.py
--rw-r--r--   0        0        0     3114 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_metadata_from_parquet.py
--rw-r--r--   0        0        0     6057 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_min.py
--rw-r--r--   0        0        0     5248 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_moment.py
--rw-r--r--   0        0        0     2033 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_nan_to_none.py
--rw-r--r--   0        0        0     5461 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_nan_to_num.py
--rw-r--r--   0        0        0     4200 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_num.py
--rw-r--r--   0        0        0     1992 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_ones_like.py
--rw-r--r--   0        0        0     4431 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_pad_none.py
--rw-r--r--   0        0        0     1844 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_parameters.py
--rw-r--r--   0        0        0     5149 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_prod.py
--rw-r--r--   0        0        0     4573 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_ptp.py
--rw-r--r--   0        0        0     2470 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_ravel.py
--rw-r--r--   0        0        0     1708 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_real.py
--rw-r--r--   0        0        0     2069 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_round.py
--rw-r--r--   0        0        0     9600 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_run_lengths.py
--rw-r--r--   0        0        0     3166 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_singletons.py
--rw-r--r--   0        0        0     3450 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_softmax.py
--rw-r--r--   0        0        0     2762 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_sort.py
--rw-r--r--   0        0        0     8351 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_std.py
--rw-r--r--   0        0        0     3116 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_strings_astype.py
--rw-r--r--   0        0        0    10595 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_sum.py
--rw-r--r--   0        0        0     4617 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_to_arrow.py
--rw-r--r--   0        0        0     7829 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_to_arrow_table.py
--rw-r--r--   0        0        0     2342 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_to_backend.py
--rw-r--r--   0        0        0     6202 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_to_buffers.py
--rw-r--r--   0        0        0        0 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_to_categorical.py
--rw-r--r--   0        0        0     1167 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_to_cupy.py
--rw-r--r--   0        0        0    13467 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_to_dataframe.py
--rw-r--r--   0        0        0     6792 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_to_feather.py
--rw-r--r--   0        0        0     1167 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_to_jax.py
--rw-r--r--   0        0        0    11188 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_to_json.py
--rw-r--r--   0        0        0     9890 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_to_layout.py
--rw-r--r--   0        0        0     2730 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_to_list.py
--rw-r--r--   0        0        0     2151 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_to_numpy.py
--rw-r--r--   0        0        0     3524 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_to_packed.py
--rw-r--r--   0        0        0    21056 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_to_parquet.py
--rw-r--r--   0        0        0     4321 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_to_parquet_dataset.py
--rw-r--r--   0        0        0    11618 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_to_parquet_row_groups.py
--rw-r--r--   0        0        0     3019 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_to_rdataframe.py
--rw-r--r--   0        0        0     3493 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_to_regular.py
--rw-r--r--   0        0        0    25148 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_transform.py
--rw-r--r--   0        0        0     4701 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_type.py
--rw-r--r--   0        0        0    11324 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_unflatten.py
--rw-r--r--   0        0        0     2571 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_unzip.py
--rw-r--r--   0        0        0     1188 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_validity_error.py
--rw-r--r--   0        0        0     2707 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_values_astype.py
--rw-r--r--   0        0        0    10073 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_var.py
--rw-r--r--   0        0        0     5113 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_where.py
--rw-r--r--   0        0        0     6051 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_with_field.py
--rw-r--r--   0        0        0     2348 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_with_name.py
--rw-r--r--   0        0        0     1795 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_with_parameter.py
--rw-r--r--   0        0        0     3783 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_without_field.py
--rw-r--r--   0        0        0     1571 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_without_parameters.py
--rw-r--r--   0        0        0     2202 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_zeros_like.py
--rw-r--r--   0        0        0     8832 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/ak_zip.py
--rw-r--r--   0        0        0    12436 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/__init__.py
--rw-r--r--   0        0        0     2163 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_capitalize.py
--rw-r--r--   0        0        0     2423 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_center.py
--rw-r--r--   0        0        0     2483 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_count_substring.py
--rw-r--r--   0        0        0     2555 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_count_substring_regex.py
--rw-r--r--   0        0        0     2397 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_ends_with.py
--rw-r--r--   0        0        0     3011 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_extract_regex.py
--rw-r--r--   0        0        0     2478 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_find_substring.py
--rw-r--r--   0        0        0     2538 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_find_substring_regex.py
--rw-r--r--   0        0        0     3202 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_index_in.py
--rw-r--r--   0        0        0     2141 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_is_alnum.py
--rw-r--r--   0        0        0     2137 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_is_alpha.py
--rw-r--r--   0        0        0     2090 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_is_ascii.py
--rw-r--r--   0        0        0     2147 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_is_decimal.py
--rw-r--r--   0        0        0     2171 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_is_digit.py
--rw-r--r--   0        0        0     2989 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_is_in.py
--rw-r--r--   0        0        0     2135 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_is_lower.py
--rw-r--r--   0        0        0     2213 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_is_numeric.py
--rw-r--r--   0        0        0     2167 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_is_printable.py
--rw-r--r--   0        0        0     2137 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_is_space.py
--rw-r--r--   0        0        0     2373 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_is_title.py
--rw-r--r--   0        0        0     2264 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_is_upper.py
--rw-r--r--   0        0        0     4631 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_join.py
--rw-r--r--   0        0        0     2612 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_join_element_wise.py
--rw-r--r--   0        0        0     2002 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_length.py
--rw-r--r--   0        0        0     2032 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_lower.py
--rw-r--r--   0        0        0     2414 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_lpad.py
--rw-r--r--   0        0        0     2304 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_ltrim.py
--rw-r--r--   0        0        0     2039 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_ltrim_whitespace.py
--rw-r--r--   0        0        0     2571 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_match_like.py
--rw-r--r--   0        0        0     2363 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_match_substring.py
--rw-r--r--   0        0        0     2395 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_match_substring_regex.py
--rw-r--r--   0        0        0     3708 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_repeat.py
--rw-r--r--   0        0        0     2610 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_replace_slice.py
--rw-r--r--   0        0        0     2761 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_replace_substring.py
--rw-r--r--   0        0        0     2829 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_replace_substring_regex.py
--rw-r--r--   0        0        0     2145 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_reverse.py
--rw-r--r--   0        0        0     2415 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_rpad.py
--rw-r--r--   0        0        0     2293 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_rtrim.py
--rw-r--r--   0        0        0     2040 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_rtrim_whitespace.py
--rw-r--r--   0        0        0     2931 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_slice.py
--rw-r--r--   0        0        0     2684 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_split_pattern.py
--rw-r--r--   0        0        0     2820 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_split_pattern_regex.py
--rw-r--r--   0        0        0     3108 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_split_whitespace.py
--rw-r--r--   0        0        0     2427 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_starts_with.py
--rw-r--r--   0        0        0     2142 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_swapcase.py
--rw-r--r--   0        0        0     2266 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_title.py
--rw-r--r--   0        0        0     2883 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_to_categorical.py
--rw-r--r--   0        0        0     2307 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_trim.py
--rw-r--r--   0        0        0     2021 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_trim_whitespace.py
--rw-r--r--   0        0        0     2038 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/operations/str/akstr_upper.py
--rw-r--r--   0        0        0      739 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/types/__init__.py
--rw-r--r--   0        0        0   163323 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/types/_awkward_datashape_parser.py
--rw-r--r--   0        0        0     2340 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/types/arraytype.py
--rw-r--r--   0        0        0     3119 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/types/listtype.py
--rw-r--r--   0        0        0     6316 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/types/numpytype.py
--rw-r--r--   0        0        0     4161 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/types/optiontype.py
--rw-r--r--   0        0        0     9689 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/types/recordtype.py
--rw-r--r--   0        0        0     4052 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/types/regulartype.py
--rw-r--r--   0        0        0     1505 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/types/scalartype.py
--rw-r--r--   0        0        0    10210 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/types/type.py
--rw-r--r--   0        0        0     4210 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/types/uniontype.py
--rw-r--r--   0        0        0     1390 2024-04-01 18:26:47.000000 awkward-2.6.3/src/awkward/types/unknowntype.py
--rw-r--r--   0        0        0       84 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/__init__.py
--rw-r--r--   0        0        0     3427 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0002_minimal_listarray.py
--rw-r--r--   0        0        0      520 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0006_deep_iteration.py
--rw-r--r--   0        0        0     5597 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0008_slices_and_getitem.py
--rw-r--r--   0        0        0    13410 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0011_listarray.py
--rw-r--r--   0        0        0     4494 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0013_error_handling_struct.py
--rw-r--r--   0        0        0    16859 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0014_finish_up_getitem.py
--rw-r--r--   0        0        0     5201 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0018_fromiter_fillable.py
--rw-r--r--   0        0        0     9804 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0019_use_json_library.py
--rw-r--r--   0        0        0    13719 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0020_support_unsigned_indexes.py
--rw-r--r--   0        0        0     6423 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0021_emptyarray.py
--rw-r--r--   0        0        0    10727 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0023_regular_array.py
--rw-r--r--   0        0        0     4922 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0024_use_regular_array.py
--rw-r--r--   0        0        0    25613 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0025_record_array.py
--rw-r--r--   0        0        0     3753 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0028_add_dressed_types.py
--rw-r--r--   0        0        0     5828 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0032_replace_dressedtype.py
--rw-r--r--   0        0        0    12059 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0046_start_indexedarray.py
--rw-r--r--   0        0        0      930 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0049_distinguish_record_and_recordarray_behaviors.py
--rw-r--r--   0        0        0    12247 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0057_introducing_forms.py
--rw-r--r--   0        0        0     5462 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0070_argmin_and_argmax.py
--rw-r--r--   0        0        0     5416 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0072_fillna_operation.py
--rw-r--r--   0        0        0    15726 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0074_argsort_and_sort.py
--rw-r--r--   0        0        0     2868 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0077_zip_operation.py
--rw-r--r--   0        0        0    11966 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0078_argcross_and_cross.py
--rw-r--r--   0        0        0    12156 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0079_argchoose_and_choose.py
--rw-r--r--   0        0        0     7028 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0080_flatpandas_multiindex_rows_and_columns.py
--rw-r--r--   0        0        0     6651 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0084_start_unionarray.py
--rw-r--r--   0        0        0     6583 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0086_nep13_ufunc.py
--rw-r--r--   0        0        0    12209 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0089_numpy_functions.py
--rw-r--r--   0        0        0    46754 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0093_simplify_uniontypes_and_optiontypes.py
--rw-r--r--   0        0        0     6991 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0107_assign_fields_to_records.py
--rw-r--r--   0        0        0    46691 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0111_jagged_and_masked_getitem.py
--rw-r--r--   0        0        0    77548 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0115_generic_reducer_operation.py
--rw-r--r--   0        0        0    35194 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0118_numba_cpointers.py
--rw-r--r--   0        0        0     1123 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0119_numexpr_and_broadcast_arrays.py
--rw-r--r--   0        0        0     1138 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0124_strings_in_numba.py
--rw-r--r--   0        0        0    32146 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0127_tomask_operation.py
--rw-r--r--   0        0        0     3715 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0127b_tomask_operation_numba.py
--rw-r--r--   0        0        0      870 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0138_emptyarray_type.py
--rw-r--r--   0        0        0    17955 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0150_flatten.py
--rw-r--r--   0        0        0     3634 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0163_negative_axis_wrap.py
--rw-r--r--   0        0        0     9811 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0166_0167_0170_random_issues.py
--rw-r--r--   0        0        0     4584 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0173_astype_operation.py
--rw-r--r--   0        0        0    24070 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0184_concatenate_operation.py
--rw-r--r--   0        0        0     2095 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0193_is_none_axis_parameter.py
--rw-r--r--   0        0        0     3384 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0198_tutorial_documentation_1.py
--rw-r--r--   0        0        0     9030 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0222_count_with_axis0.py
--rw-r--r--   0        0        0    75637 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0224_arrow_to_awkward.py
--rw-r--r--   0        0        0      613 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0264_reduce_last_empty.py
--rw-r--r--   0        0        0     3283 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0273_path_for_with_field.py
--rw-r--r--   0        0        0      775 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0286_broadcast_single_value_with_field.py
--rw-r--r--   0        0        0     2237 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0290_bug_fixes_for_hats.py
--rw-r--r--   0        0        0     4838 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0315_integerindex.py
--rw-r--r--   0        0        0     5777 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0331_pandas_indexedarray.py
--rw-r--r--   0        0        0     1289 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0334_fully_broadcastable_where.py
--rw-r--r--   0        0        0      598 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0339_highlevel_sorting_function.py
--rw-r--r--   0        0        0     6789 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0348_form_keys.py
--rw-r--r--   0        0        0     4554 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0355_mixins.py
--rw-r--r--   0        0        0    10428 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0395_complex_type_arrays.py
--rw-r--r--   0        0        0     4966 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0395_fix_numba_indexedarray.py
--rw-r--r--   0        0        0     3244 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0397_arrays_as_constants_in_numba.py
--rw-r--r--   0        0        0     6987 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0401_add_categorical_type_for_arrow_dictionary.py
--rw-r--r--   0        0        0    22496 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0404_array_validity_check.py
--rw-r--r--   0        0        0    14314 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0410_fix_argminmax_positions_for_missing_values.py
--rw-r--r--   0        0        0    17487 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0437_stream_of_many_json_files.py
--rw-r--r--   0        0        0    32953 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0447_preserve_regularness_in_reduce.py
--rw-r--r--   0        0        0    27090 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0449_merge_many_arrays_in_one_pass.py
--rw-r--r--   0        0        0     4091 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0493_zeros_ones_full_like.py
--rw-r--r--   0        0        0     1638 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0496_provide_local_index.py
--rw-r--r--   0        0        0     2091 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0499_getitem_indexedarray_bug.py
--rw-r--r--   0        0        0     1319 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0504_block_ufuncs_for_strings.py
--rw-r--r--   0        0        0     2958 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0511_copy_and_deepcopy.py
--rw-r--r--   0        0        0     9179 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py
--rw-r--r--   0        0        0      397 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0546_fill_none_replacement_value_type.py
--rw-r--r--   0        0        0     1134 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0549_numba_array_asarray.py
--rw-r--r--   0        0        0     4300 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0557_min_max_initial_argument.py
--rw-r--r--   0        0        0      569 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0559_fix_booleans_in_numba.py
--rw-r--r--   0        0        0      668 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0572_numba_array_ndim.py
--rw-r--r--   0        0        0     4933 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0582_propagate_context_in_broadcast_and_apply.py
--rw-r--r--   0        0        0     1131 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0583_implement_unflatten_function.py
--rw-r--r--   0        0        0     3116 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0590_allow_regulararray_size_zero.py
--rw-r--r--   0        0        0     5976 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py
--rw-r--r--   0        0        0      510 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0627_behavior_from_dict_of_arrays.py
--rw-r--r--   0        0        0     8237 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0652_tests_of_complex_numbers.py
--rw-r--r--   0        0        0     2342 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0674_categorical_validation.py
--rw-r--r--   0        0        0      782 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0713_getitem_field_should_simplify_optiontype.py
--rw-r--r--   0        0        0     1274 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py
--rw-r--r--   0        0        0     1087 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0730_unflatten_axis_parameter.py
--rw-r--r--   0        0        0     2601 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0733_run_lengths.py
--rw-r--r--   0        0        0     2159 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0736_implement_argsort_for_strings.py
--rw-r--r--   0        0        0      362 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0758_ak_zip_scallars.py
--rw-r--r--   0        0        0     1154 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0766_prevent_combinations_of_characters.py
--rw-r--r--   0        0        0    25871 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0773_typeparser.py
--rw-r--r--   0        0        0      811 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0788_indexedarray_carrying_recordarray_parameters.py
--rw-r--r--   0        0        0      903 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0794_ak_cartesian_on_empty_array.py
--rw-r--r--   0        0        0     1180 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0803_argsort_fix_type.py
--rw-r--r--   0        0        0     1396 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0806_empty_lists_cartesian_fix.py
--rw-r--r--   0        0        0     7877 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0813_full_like_dtype_arg.py
--rw-r--r--   0        0        0     1693 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0815_broadcast_union_types_to_all_possibilities.py
--rw-r--r--   0        0        0      520 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0819_issue.py
--rw-r--r--   0        0        0      714 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0828_arrow_datatype_null.py
--rw-r--r--   0        0        0    23641 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0835_datetime_type.py
--rw-r--r--   0        0        0      708 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0835_datetime_type_pandas.py
--rw-r--r--   0        0        0     4694 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0835_datetime_type_pyarrow.py
--rw-r--r--   0        0        0      712 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0850_argsort_mask_array.py
--rw-r--r--   0        0        0      481 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0863_is_none_numpy_array.py
--rw-r--r--   0        0        0     1061 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0866_getitem_field_and_flatten_unions.py
--rw-r--r--   0        0        0      961 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0875_arrow_null_type.py
--rw-r--r--   0        0        0      933 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0879_non_primitive_with_field.py
--rw-r--r--   0        0        0      595 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0884_index_and_identifier_refactoring.py
--rw-r--r--   0        0        0     1118 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0889_ptp.py
--rw-r--r--   0        0        0    53387 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0896_content_classes_refactoring.py
--rw-r--r--   0        0        0     1783 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0898_unzip_heterogeneous_records.py
--rw-r--r--   0        0        0      453 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0903_ArrayView_expects_contiguous_NumpyArrays.py
--rw-r--r--   0        0        0      562 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0905_leading_zeros_in_unflatten.py
--rw-r--r--   0        0        0     1080 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0906_arrow_fixed_size_list_type.py
--rw-r--r--   0        0        0      698 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0910_unflatten_counts_relation.py
--rw-r--r--   0        0        0     5293 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0912_packed.py
--rw-r--r--   0        0        0   108025 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0914_types_and_forms.py
--rw-r--r--   0        0        0     1909 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0916_datetime_values_astype.py
--rw-r--r--   0        0        0     5554 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0927_numpy_array_nbytes.py
--rw-r--r--   0        0        0      741 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0930_bug_in_unionarray_purelist_parameter.py
--rw-r--r--   0        0        0     1659 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0945_argsort_sort_nan_array.py
--rw-r--r--   0        0        0    28060 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0958_new_forms_must_accept_old_form_json.py
--rw-r--r--   0        0        0    28316 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0959__getitem_array_implementation.py
--rw-r--r--   0        0        0      683 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0975_mask_multidimensional_numpy_array.py
--rw-r--r--   0        0        0      676 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0979_where_multidimentional_numpy_array.py
--rw-r--r--   0        0        0     5835 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0982_missing_case_in_nonlocal_reducers.py
--rw-r--r--   0        0        0     2008 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0984_ravel.py
--rw-r--r--   0        0        0     1838 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_0992_correct_ptp_unmasking.py
--rw-r--r--   0        0        0     2132 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py
--rw-r--r--   0        0        0      461 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1006_packed_regular_array_zero_size.py
--rw-r--r--   0        0        0      448 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1007_from_buffers_empty_ndarray.py
--rw-r--r--   0        0        0      583 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1017_numpyarray_broadcast.py
--rw-r--r--   0        0        0      817 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1030_mixin_class_name.py
--rw-r--r--   0        0        0    52146 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1031_start_getitem_next.py
--rw-r--r--   0        0        0    18039 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1031b_start_getitem_next_specialized.py
--rw-r--r--   0        0        0     1178 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1049_concatenate_single_array.py
--rw-r--r--   0        0        0     1591 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1055_fill_none_numpy_dimension.py
--rw-r--r--   0        0        0    42282 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1059_localindex.py
--rw-r--r--   0        0        0      583 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1066_to_numpy_masked_structured_array.py
--rw-r--r--   0        0        0      717 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1071_mask_identity_false_should_not_return_option_type.py
--rw-r--r--   0        0        0    27770 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1072_sort.py
--rw-r--r--   0        0        0    44172 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1074_combinations.py
--rw-r--r--   0        0        0     5213 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1075_validityerror.py
--rw-r--r--   0        0        0      305 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1106_argminmax_axis_None_missing_values.py
--rw-r--r--   0        0        0    25563 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1110_type_tracer_1.py
--rw-r--r--   0        0        0     1902 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1116_project_maskedarrays.py
--rw-r--r--   0        0        0    28382 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1125_to_arrow_from_arrow.py
--rw-r--r--   0        0        0     6308 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1132_utility_methods_for_highlevel_functions.py
--rw-r--r--   0        0        0    21130 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1134_from_buffers_to_buffers.py
--rw-r--r--   0        0        0    57354 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1135_rpad_operation.py
--rw-r--r--   0        0        0     4671 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1136_regulararray_zeros_in_shape.py
--rw-r--r--   0        0        0    10535 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1137_num.py
--rw-r--r--   0        0        0    10576 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1142_numbers_to_type.py
--rw-r--r--   0        0        0     2591 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1149_datetime_sort.py
--rw-r--r--   0        0        0      662 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1154_arrow_tables_should_preserve_parameters.py
--rw-r--r--   0        0        0    32589 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1162_ak_from_json_schema.py
--rw-r--r--   0        0        0      798 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1183_bugs_found_by_dask_project_2.py
--rw-r--r--   0        0        0     1318 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1189_fix_singletons_for_non_optional_data.py
--rw-r--r--   0        0        0      583 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1192_iterables_in___array_function__.py
--rw-r--r--   0        0        0      640 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1193_is_none_nested_option.py
--rw-r--r--   0        0        0     2633 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1233_ak_with_name.py
--rw-r--r--   0        0        0    26572 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1240_v2_implementation_of_numba_1.py
--rw-r--r--   0        0        0     1178 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1259_simplify_optiontype.py
--rw-r--r--   0        0        0     1592 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1260_simplify_masked_option_types.py
--rw-r--r--   0        0        0      713 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1271_fix_4D_reducers.py
--rw-r--r--   0        0        0    33099 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1294_to_and_from_parquet.py
--rw-r--r--   0        0        0     1977 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py
--rw-r--r--   0        0        0    62372 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1300_awkward_to_cpp_converter_with_cling.py
--rw-r--r--   0        0        0    39506 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1300b_same_for_numba.py
--rw-r--r--   0        0        0      399 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1305_mixed_awkward_numpy_slicing.py
--rw-r--r--   0        0        0     1734 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1308_zip_after_option.py
--rw-r--r--   0        0        0     1736 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1318_array_function_types.py
--rw-r--r--   0        0        0     1762 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1320_mask_identity_defaults.py
--rw-r--r--   0        0        0      679 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1344_broadcast_arrays_depth_limit.py
--rw-r--r--   0        0        0     6653 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1345_avro_reader.py
--rw-r--r--   0        0        0     4594 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1351_is_tuple.py
--rw-r--r--   0        0        0     8394 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1374_to_rdataframe.py
--rw-r--r--   0        0        0     1787 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1377_ravel_string.py
--rw-r--r--   0        0        0     1500 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1379_reducers_with_axis_None_and_typetracers.py
--rw-r--r--   0        0        0     1416 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1399_from_jax.py
--rw-r--r--   0        0        0     1259 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1399_to_jax.py
--rw-r--r--   0        0        0      329 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1400_with_name_record.py
--rw-r--r--   0        0        0      481 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1403_from_numpy_strings.py
--rw-r--r--   0        0        0     3502 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1405_slicing_untested_cases.py
--rw-r--r--   0        0        0     7211 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1415_behaviour_forwarding.py
--rw-r--r--   0        0        0    18745 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1440_start_v2_to_parquet.py
--rw-r--r--   0        0        0    14434 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1447_jax_autodiff_slices_ufuncs.py
--rw-r--r--   0        0        0     8623 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1449_v2_to_json_from_json_functions.py
--rw-r--r--   0        0        0      694 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1453_write_single_records_to_parquet.py
--rw-r--r--   0        0        0     9860 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1473_from_rdataframe.py
--rw-r--r--   0        0        0    24680 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1477_generator_entry_type_as_rvec.py
--rw-r--r--   0        0        0     3611 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1490_jax_reducers_combinations.py
--rw-r--r--   0        0        0     3937 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1502_getitem_jagged_issue1406.py
--rw-r--r--   0        0        0     1853 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1504_typetracer_like.py
--rw-r--r--   0        0        0     4945 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1508_awkward_from_rdataframe.py
--rw-r--r--   0        0        0     2218 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1511_set_attribute.py
--rw-r--r--   0        0        0      786 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1539_isnone_axis_check_issue1417.py
--rw-r--r--   0        0        0     1602 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1559_fix_ufuncs_records_1439.py
--rw-r--r--   0        0        0     1039 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1565_axis_wrap_if_negative_record.py
--rw-r--r--   0        0        0     1117 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1567_fix_longlong_in_Index.py
--rw-r--r--   0        0        0     3054 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1568_fix_lengths_empty_regular_slices.py
--rw-r--r--   0        0        0      417 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1578_to_arrow_empty_recordarray.py
--rw-r--r--   0        0        0     5943 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1586_concatenate_should_preserve_regulararray.py
--rw-r--r--   0        0        0      337 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1593_empty_slice_list_record.py
--rw-r--r--   0        0        0     7292 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1604_preserve_form_in_concatenate.py
--rw-r--r--   0        0        0     4404 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1607_no_reducers_on_records.py
--rw-r--r--   0        0        0    10067 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1613_generator_tolayout_records.py
--rw-r--r--   0        0        0      759 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1619_from_parquet_empty_field.py
--rw-r--r--   0        0        0     6056 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1620_layout_builders.py
--rw-r--r--   0        0        0     8154 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1625_multiple_columns_from_rdataframe.py
--rw-r--r--   0        0        0      802 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1642_from_iter_of_tuples.py
--rw-r--r--   0        0        0      421 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1644_concatenate_zeros_length.py
--rw-r--r--   0        0        0     4349 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1650_Record_to_list_should_listify_itself.py
--rw-r--r--   0        0        0     1053 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1671_categorical_type.py
--rw-r--r--   0        0        0    11791 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1672_broadcast_parameters.py
--rw-r--r--   0        0        0     4485 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1677_array_builder_in_numba.py
--rw-r--r--   0        0        0      576 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1685_IndexedArray_project_parameters.py
--rw-r--r--   0        0        0      810 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1686_UnionArray_simplified_preserve_parameters.py
--rw-r--r--   0        0        0      994 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1688_pack_categorical.py
--rw-r--r--   0        0        0      557 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1703_fill_none_typetracer.py
--rw-r--r--   0        0        0     1775 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1707_broadcast_parameters_ufunc.py
--rw-r--r--   0        0        0      541 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1709_ak_array_constructor_behavior.py
--rw-r--r--   0        0        0      430 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1735_from_numpy_mask.py
--rw-r--r--   0        0        0      609 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1747_bytemaskedarray_mergemany.py
--rw-r--r--   0        0        0      856 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1753_indexedarray_merge_kernel.py
--rw-r--r--   0        0        0     1509 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1762_jax_behavior_support.py
--rw-r--r--   0        0        0      621 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1764_jax_jacobian.py
--rw-r--r--   0        0        0      994 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1765_add_ioanas_test_of_to_arraylib.py
--rw-r--r--   0        0        0     4822 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1766_record_form_fields.py
--rw-r--r--   0        0        0     2937 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1781_rdataframe_snapshot.py
--rw-r--r--   0        0        0      733 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1784_reduce_leading_sublist.py
--rw-r--r--   0        0        0      599 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1790_reduce_regulararray.py
--rw-r--r--   0        0        0     4223 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1791_reduce_trailing_sublist.py
--rw-r--r--   0        0        0     1059 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1794_run_lengths_empty_sublist.py
--rw-r--r--   0        0        0      439 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1823_fill_none_axis_none.py
--rw-r--r--   0        0        0      513 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1826_ravel_preserve_none.py
--rw-r--r--   0        0        0     1483 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1829_to_from_rdataframe_bool.py
--rw-r--r--   0        0        0      620 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py
--rw-r--r--   0        0        0     1129 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1847_numpy_array_contiguous.py
--rw-r--r--   0        0        0      765 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1850_bytemasked_array_to_bytemaskedarray.py
--rw-r--r--   0        0        0     1672 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1867_pass_behavior_through_combinations.py
--rw-r--r--   0        0        0    17296 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1904_drop_none.py
--rw-r--r--   0        0        0     3591 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1914_improved_axis_to_posaxis.py
--rw-r--r--   0        0        0     4639 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py
--rw-r--r--   0        0        0      953 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1930_unflatten_counts_checks.py
--rw-r--r--   0        0        0      801 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1936_with_field_broadcasting.py
--rw-r--r--   0        0        0      583 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1940_ak_backend.py
--rw-r--r--   0        0        0     1489 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1943_regular_indexing.py
--rw-r--r--   0        0        0      220 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1944_to_numpy_empty_record_array.py
--rw-r--r--   0        0        0     1163 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1960_awkward_from_rdataframe.py
--rw-r--r--   0        0        0     3319 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1961_ak_without_field.py
--rw-r--r--   0        0        0      312 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1978_akRecord_constructor_should_retain_type.py
--rw-r--r--   0        0        0      381 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_1991_missed_a_NumpyArray_raw_call_without_underscore.py
--rw-r--r--   0        0        0      403 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2008_ak_type_layout.py
--rw-r--r--   0        0        0    10254 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2020_reduce_axis_none.py
--rw-r--r--   0        0        0      835 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2021_check_TypeTracerArray_in_ak_where.py
--rw-r--r--   0        0        0      677 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2023_from_rdataframe.py
--rw-r--r--   0        0        0     2938 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py
--rw-r--r--   0        0        0     1251 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2047_ak_transform_regular_to_jagged.py
--rw-r--r--   0        0        0      527 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2051_arraybuilder_behavior_propagation.py
--rw-r--r--   0        0        0     1307 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2055_array_builder_check.py
--rw-r--r--   0        0        0     1691 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2058_merge_numpy_array.py
--rw-r--r--   0        0        0      740 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2064_fill_none_record.py
--rw-r--r--   0        0        0      831 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2067_to_buffers_byteorder.py
--rw-r--r--   0        0        0      806 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2070_to_layout_string.py
--rw-r--r--   0        0        0     1230 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2071_unflatten_non_packed_counts.py
--rw-r--r--   0        0        0      323 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2076_ak_unzip_record.py
--rw-r--r--   0        0        0      577 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2078_array_function_wrap.py
--rw-r--r--   0        0        0      621 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2082_broadcast_zero_size.py
--rw-r--r--   0        0        0     1763 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2085_empty_if_typetracer.py
--rw-r--r--   0        0        0     2614 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2096_ak_scalar_type.py
--rw-r--r--   0        0        0     1009 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2101_pickle_behavior_class.py
--rw-r--r--   0        0        0      551 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2104_numpy_merge_option.py
--rw-r--r--   0        0        0     2748 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2106_pickle_class.py
--rw-r--r--   0        0        0      954 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2108_fill_none_indexed.py
--rw-r--r--   0        0        0     2132 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2115_fix_up_typetracers.py
--rw-r--r--   0        0        0      516 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2120_missing_field_error.py
--rw-r--r--   0        0        0     1066 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2125_type_of_scalar.py
--rw-r--r--   0        0        0     1925 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2150_typetracer_high_level_ufunc.py
--rw-r--r--   0        0        0     1930 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2179_parameter_merging_rules.py
--rw-r--r--   0        0        0      332 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2181_with_name_len.py
--rw-r--r--   0        0        0     2989 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2185_merge_union_of_records.py
--rw-r--r--   0        0        0      560 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py
--rw-r--r--   0        0        0     7333 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2192_union_absorb_indexed.py
--rw-r--r--   0        0        0     6087 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2198_almost_equal.py
--rw-r--r--   0        0        0     1284 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2202_filter_multiple_columns_from_rdataframe.py
--rw-r--r--   0        0        0     1485 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2214_offset_bool_index.py
--rw-r--r--   0        0        0      366 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2219_flatten_empty.py
--rw-r--r--   0        0        0      695 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2226_slice_regulararray_typetracer.py
--rw-r--r--   0        0        0     1760 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2229_getitem_range_slice.py
--rw-r--r--   0        0        0     4035 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2234_from_rdataframe_keep_order.py
--rw-r--r--   0        0        0     4136 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2236_merge_union_of_records_option.py
--rw-r--r--   0        0        0      517 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2240_merge_union_parameters.py
--rw-r--r--   0        0        0     1369 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2240_simplify_merge_as_union.py
--rw-r--r--   0        0        0      544 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2246_slice_not_packed.py
--rw-r--r--   0        0        0      765 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2250_full_like_bool.py
--rw-r--r--   0        0        0     1867 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2258_from_rdataframe_with_arguments.py
--rw-r--r--   0        0        0      524 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2259_run_lengths_typetracer.py
--rw-r--r--   0        0        0      592 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2263_to_packed_list.py
--rw-r--r--   0        0        0      347 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2266_fix_nan_to_num.py
--rw-r--r--   0        0        0      941 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2267_broadcast_fields.py
--rw-r--r--   0        0        0     1368 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2293_unflatten_typetracer.py
--rw-r--r--   0        0        0      438 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2294_view_unknown_scalar.py
--rw-r--r--   0        0        0      752 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2296_duplicate_field.py
--rw-r--r--   0        0        0     2294 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2297_common_backend.py
--rw-r--r--   0        0        0      487 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2304_index_typetracer.py
--rw-r--r--   0        0        0      680 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2305_nep_18_lazy_conversion.py
--rw-r--r--   0        0        0     2895 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2306_cppyy_jit.py
--rw-r--r--   0        0        0     4418 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2319_from_buffers_array.py
--rw-r--r--   0        0        0      753 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2327_array_interface.py
--rw-r--r--   0        0        0     1760 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2329_cartesian_broadcasting_fixes.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2346_broadcast_depth_limit.py
--rw-r--r--   0        0        0    15641 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2349_growablebuffer_in_numba.py
--rw-r--r--   0        0        0      650 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2354_ufunc_same_backend.py
--rw-r--r--   0        0        0      679 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2355_to_backend_record.py
--rw-r--r--   0        0        0     1467 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2361_typetracer_asarray_nd.py
--rw-r--r--   0        0        0      966 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2364_empty_list_of_string.py
--rw-r--r--   0        0        0    37032 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2365_enforce_type.py
--rw-r--r--   0        0        0     2956 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2368_type_is_equal.py
--rw-r--r--   0        0        0     5376 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2373_unzip_touching.py
--rw-r--r--   0        0        0     5984 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2374_cartesian_touching.py
--rw-r--r--   0        0        0     1069 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2385_with_field_empty_record.py
--rw-r--r--   0        0        0      988 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2395_copy_asarray_touch.py
--rw-r--r--   0        0        0      244 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2407_broadcast_no_arrays.py
--rw-r--r--   0        0        0    34537 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2408_layoutbuilder_in_numba.py
--rw-r--r--   0        0        0      885 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2410_string_broadcast.py
--rw-r--r--   0        0        0      847 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2411_cartesian_axis_validation.py
--rw-r--r--   0        0        0      736 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2417_bytemasked_singletons.py
--rw-r--r--   0        0        0      382 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2418_union_broadcast_unknown.py
--rw-r--r--   0        0        0     1595 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2424_almost_equal_union_record.py
--rw-r--r--   0        0        0     1254 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2425_forms_from_type.py
--rw-r--r--   0        0        0      577 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2426_is_equal_to.py
--rw-r--r--   0        0        0      616 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2444_minimal_listarray.py
--rw-r--r--   0        0        0      889 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2471_flatten_string.py
--rw-r--r--   0        0        0     1063 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2484_reduce_starts_empty.py
--rw-r--r--   0        0        0      691 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2487_broadcast_list_offsets.py
--rw-r--r--   0        0        0     1351 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2490_reduce_regulararray_positional.py
--rw-r--r--   0        0        0     1848 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2495_concatenate_typetracer.py
--rw-r--r--   0        0        0     3832 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2501_positional_record_reducer.py
--rw-r--r--   0        0        0      293 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2503_deprecate_to_numpyform.py
--rw-r--r--   0        0        0     4974 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2512_record_array_carry.py
--rw-r--r--   0        0        0      329 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2518_datetime_units_as_parameter.py
--rw-r--r--   0        0        0     5978 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2536_select_columns.py
--rw-r--r--   0        0        0      767 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2548_record_form_fields.py
--rw-r--r--   0        0        0     3661 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2549_list_nominal_type.py
--rw-r--r--   0        0        0      702 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2550_validity_error_recursive.py
--rw-r--r--   0        0        0      470 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2556_jax_tracer_error.py
--rw-r--r--   0        0        0      475 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2560_minimal_listarray.py
--rw-r--r--   0        0        0     1483 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2564_string_broadcast_regular.py
--rw-r--r--   0        0        0      922 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2571_awkward_ListOffsetArray_reduce_local_nextparents_64.py
--rw-r--r--   0        0        0      357 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2591_nan_to_num.py
--rw-r--r--   0        0        0     2459 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2595_transform_termination.py
--rw-r--r--   0        0        0      856 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2603_custom_behaviors_with_jax.py
--rw-r--r--   0        0        0     3565 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2604_read_awkward1_pickles.py
--rw-r--r--   0        0        0    65992 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2616_use_pyarrow_for_strings.py
--rw-r--r--   0        0        0     1993 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2623_optiontype_outside_record_strings.py
--rw-r--r--   0        0        0     5330 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2630_akstr_to_categorical.py
--rw-r--r--   0        0        0      734 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2631_vectorised_to_numpy_strings.py
--rw-r--r--   0        0        0      437 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2632_unflatten_length.py
--rw-r--r--   0        0        0      580 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2634_listarray_pad_none.py
--rw-r--r--   0        0        0      961 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2637_jax_tracer_error.py
--rw-r--r--   0        0        0      874 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2638_mean_and_count_grads.py
--rw-r--r--   0        0        0      657 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2646_from_parquet_highlevel.py
--rw-r--r--   0        0        0     1732 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2649_dlpack_support.py
--rw-r--r--   0        0        0     1424 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2650_arrow_array_highlevel.py
--rw-r--r--   0        0        0      594 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2651_parameter_union.py
--rw-r--r--   0        0        0     1389 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2653_slice_listoffsetarray.py
--rw-r--r--   0        0        0      476 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2654_divmod.py
--rw-r--r--   0        0        0     3772 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2656_unflatten_axis_typetracer.py
--rw-r--r--   0        0        0    24851 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2660_expected_container_keys_from_form.py
--rw-r--r--   0        0        0     1949 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2663_broadcast_tuples.py
--rw-r--r--   0        0        0     1765 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2665_out_of_band_pickle.py
--rw-r--r--   0        0        0     4036 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2671_typetracer_with_report_deprecated_length.py
--rw-r--r--   0        0        0     1723 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2672_touch_data.py
--rw-r--r--   0        0        0      524 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2678_same_backend.py
--rw-r--r--   0        0        0     3104 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2682_custom_pickler.py
--rw-r--r--   0        0        0     1103 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2683_to_and_from_feather.py
--rw-r--r--   0        0        0     1013 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2693_to_buffers_placeholders.py
--rw-r--r--   0        0        0      301 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2710_pickle_unknown_length.py
--rw-r--r--   0        0        0     3973 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2713_from_buffers_allow_noncanonical.py
--rw-r--r--   0        0        0    17061 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2714_from_buffers_placeholders.py
--rw-r--r--   0        0        0     1157 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2718_frombuffer_typetracer.py
--rw-r--r--   0        0        0     1372 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2719_typetracer_buffer_key.py
--rw-r--r--   0        0        0      873 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2724_expected_from_buffers_recursive.py
--rw-r--r--   0        0        0      851 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2727_remove_structure_regular.py
--rw-r--r--   0        0        0     4031 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2754_highlevel_behavior_missing.py
--rw-r--r--   0        0        0     9111 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2757_attrs_metadata.py
--rw-r--r--   0        0        0     1384 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2759_update_class_consistently.py
--rw-r--r--   0        0        0     3649 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2763_to_layout_granularity.py
--rw-r--r--   0        0        0      427 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2765_slice_from_typetracer.py
--rw-r--r--   0        0        0     1573 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2769_argsort_all_none.py
--rw-r--r--   0        0        0     1070 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2770_serialize_and_deserialize_behaviour_for_numba.py
--rw-r--r--   0        0        0      574 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2785_ak_num_typetracer_axis_0.py
--rw-r--r--   0        0        0     1991 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2793_nep_50_gradual_support.py
--rw-r--r--   0        0        0     1744 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2799_numba_ufunc_resolution.py
--rw-r--r--   0        0        0     4607 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2803_string_formatter.py
--rw-r--r--   0        0        0     1347 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2806_attrs_typetracer.py
--rw-r--r--   0        0        0     1160 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2808_dtype_ufunc_bool.py
--rw-r--r--   0        0        0      471 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2815_return_scalar_firsts.py
--rw-r--r--   0        0        0      478 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2816_public_typetracer_api.py
--rw-r--r--   0        0        0      789 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2837_ufunc_attrs_behavior.py
--rw-r--r--   0        0        0      922 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2857_full_like_scalar.py
--rw-r--r--   0        0        0     4080 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2860_enforce_concatenated_form.py
--rw-r--r--   0        0        0      798 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2866_getitem_attrs.py
--rw-r--r--   0        0        0     1382 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2889_test_chunked_array.py
--rw-r--r--   0        0        0     4399 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2898_to_parquet_dataset.py
--rw-r--r--   0        0        0     2989 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2917_real_imag_angle.py
--rw-r--r--   0        0        0      965 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2917_round.py
--rw-r--r--   0        0        0      800 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2918_fix_var_axis_not_minus_one.py
--rw-r--r--   0        0        0     3793 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2928_nested_cartesian_record.py
--rw-r--r--   0        0        0      361 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2934_argmin_argmax_bool.py
--rw-r--r--   0        0        0     5582 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_2968_to_parquet_row_groups.py
--rw-r--r--   0        0        0      470 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_3028_mask_bitmaskedarray.py
--rw-r--r--   0        0        0      466 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_3033_flatten_bitmaskedarray.py
--rw-r--r--   0        0        0      829 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/test_3060_indexoption_to_numpy_record_array.py
--rw-r--r--   0        0        0      124 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/__init__.py
--rw-r--r--   0        0        0      218 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/array_enum_test_data.avro
--rw-r--r--   0        0        0      176 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/array_string_test_data.avro
--rw-r--r--   0        0        0      152 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/array_test_data.avro
--rw-r--r--   0        0        0      440 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/awkward1-bytemaskedarray.pkl
--rw-r--r--   0        0        0      255 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/awkward1-emptyarray.pkl
--rw-r--r--   0        0        0      461 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/awkward1-indexedoptionarray.pkl
--rw-r--r--   0        0        0      468 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/awkward1-listoffsetarray.pkl
--rw-r--r--   0        0        0      288 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/awkward1-numpyarray.pkl
--rw-r--r--   0        0        0      368 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/awkward1-partitioned-numpyarray.pkl
--rw-r--r--   0        0        0      446 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/awkward1-recordarray-tuple.pkl
--rw-r--r--   0        0        0      455 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/awkward1-recordarray.pkl
--rw-r--r--   0        0        0      564 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/awkward1-regulararray.pkl
--rw-r--r--   0        0        0      499 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/awkward1-strings.pkl
--rw-r--r--   0        0        0      736 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/awkward1-unionarray.pkl
--rw-r--r--   0        0        0      325 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/awkward1-unmaskedarray.pkl
--rw-r--r--   0        0        0      115 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/bool_test_data.avro
--rw-r--r--   0        0        0      130 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/bytes_test_data.avro
--rw-r--r--   0        0        0   523374 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/complex-nested.json
--rw-r--r--   0        0        0      158 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/double_test_data.avro
--rw-r--r--   0        0        0      191 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/enum_null_test_data.avro
--rw-r--r--   0        0        0      180 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/enum_test_data.avro
--rw-r--r--   0        0        0      218 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/fixed_test_data.avro
--rw-r--r--   0        0        0      116 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/float_test_data.avro
--rw-r--r--   0        0        0      106 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/int_null_test_data.avro
--rw-r--r--   0        0        0      128 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/int_string_null_test_data.avro
--rw-r--r--   0        0        0       89 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/int_test_data.avro
--rw-r--r--   0        0        0     3035 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/list-depths-records-list.parquet
--rw-r--r--   0        0        0     2871 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/list-depths-records.parquet
--rw-r--r--   0        0        0      497 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/list-depths-simple.parquet
--rw-r--r--   0        0        0     1136 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/list-depths-strings.parquet
--rw-r--r--   0        0        0     1060 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/list-depths.parquet
--rw-r--r--   0        0        0      465 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/list-lengths.parquet
--rw-r--r--   0        0        0      116 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/long_test_data.avro
--rw-r--r--   0        0        0      681 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/nonnullable-depths.parquet
--rw-r--r--   0        0        0       75 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/null_test_data.avro
--rw-r--r--   0        0        0      719 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/nullable-depths.parquet
--rw-r--r--   0        0        0      635 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/nullable-levels.parquet
--rw-r--r--   0        0        0     3050 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/nullable-list-depths-records-list.parquet
--rw-r--r--   0        0        0     2926 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/nullable-list-depths-records.parquet
--rw-r--r--   0        0        0     1179 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/nullable-list-depths-strings.parquet
--rw-r--r--   0        0        0     1101 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/nullable-list-depths.parquet
--rw-r--r--   0        0        0      430 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/nullable-record-primitives-simple.parquet
--rw-r--r--   0        0        0     1181 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/nullable-record-primitives.parquet
--rw-r--r--   0        0        0     1193 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/record-primitives.parquet
--rw-r--r--   0        0        0      326 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/record_0_test_data.avro
--rw-r--r--   0        0        0      368 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/record_1_test_data.avro
--rw-r--r--   0        0        0      263 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/record_null_test_data.avro
--rw-r--r--   0        0        0      423 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/record_test_data.avro
--rw-r--r--   0        0        0      116 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/string_null_test_data.avro
--rw-r--r--   0        0        0      125 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/string_test_data.avro
--rw-r--r--   0        0        0      544 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/test-nan-inf.json
--rw-r--r--   0        0        0      155 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/test-record-array.json
--rw-r--r--   0        0        0      803 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/test-two-arrays.json
--rw-r--r--   0        0        0      535 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/test.json
--rw-r--r--   0        0        0      180 2024-04-01 18:26:47.000000 awkward-2.6.3/tests/samples/zero-record-batches.parquet
--rw-r--r--   0        0        0       84 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda/__init__.py
--rw-r--r--   0        0        0     6875 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda/test_1276_cuda_num.py
--rw-r--r--   0        0        0    13304 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda/test_1276_cuda_transfers.py
--rw-r--r--   0        0        0     1348 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda/test_1276_cupy_interop.py
--rw-r--r--   0        0        0     1808 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda/test_1276_from_cupy.py
--rw-r--r--   0        0        0    42828 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda/test_1300_same_for_numba_cuda.py
--rw-r--r--   0        0        0     1244 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda/test_1381_check_errors.py
--rw-r--r--   0        0        0    11072 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda/test_1809_array_cuda_jit.py
--rw-r--r--   0        0        0    44720 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda/test_2922a_new_cuda_kernels.py
--rw-r--r--   0        0        0    48680 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda/test_2922b_new_cuda_kernels.py
--rw-r--r--   0        0        0      146 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/__init__.py
--rw-r--r--   0        0        0     5009 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_BitMaskedArray_to_ByteMaskedArray.py
--rw-r--r--   0        0        0     4655 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_BitMaskedArray_to_IndexedOptionArray64.py
--rw-r--r--   0        0        0     2772 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_getitem_nextcarry_64.py
--rw-r--r--   0        0        0     3664 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_getitem_nextcarry_outindex_64.py
--rw-r--r--   0        0        0     3190 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_numnull.py
--rw-r--r--   0        0        0    17790 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_overlay_mask8.py
--rw-r--r--   0        0        0      517 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_reduce_next_64.py
--rw-r--r--   0        0        0      537 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.py
--rw-r--r--   0        0        0      548 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.py
--rw-r--r--   0        0        0     3413 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_toIndexedOptionArray64.py
--rw-r--r--   0        0        0    29905 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_Content_getitem_next_missing_jagged_getmaskstartstop.py
--rw-r--r--   0        0        0      510 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_Index_nones_as_index_64.py
--rw-r--r--   0        0        0     2861 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_flatten_nextcarry_64.py
--rw-r--r--   0        0        0    14874 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_flatten_none2empty_64.py
--rw-r--r--   0        0        0     2861 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_getitem_nextcarry_64.py
--rw-r--r--   0        0        0     2437 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_getitem_nextcarry_outindex_64.py
--rw-r--r--   0        0        0      516 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_index_of_nulls.py
--rw-r--r--   0        0        0     3119 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_numnull.py
--rw-r--r--   0        0        0      517 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_numnull_parents.py
--rw-r--r--   0        0        0      520 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_overlay_mask8_to64.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_ranges_carry_next_64.py
--rw-r--r--   0        0        0      516 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_ranges_next_64.py
--rw-r--r--   0        0        0      516 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_reduce_next_64.py
--rw-r--r--   0        0        0      536 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_reduce_next_nonlocal_nextshifts_64.py
--rw-r--r--   0        0        0      547 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_reduce_next_nonlocal_nextshifts_fromshifts_64.py
--rw-r--r--   0        0        0     9865 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_simplify32_to64.py
--rw-r--r--   0        0        0     9865 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_simplify64_to64.py
--rw-r--r--   0        0        0     9910 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_simplifyU32_to64.py
--rw-r--r--   0        0        0     8475 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_validity.py
--rw-r--r--   0        0        0     2861 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_flatten_nextcarry_64.py
--rw-r--r--   0        0        0    14874 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_flatten_none2empty_64.py
--rw-r--r--   0        0        0     2861 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_getitem_nextcarry_64.py
--rw-r--r--   0        0        0     2437 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_getitem_nextcarry_outindex_64.py
--rw-r--r--   0        0        0      516 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_index_of_nulls.py
--rw-r--r--   0        0        0     3119 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_numnull.py
--rw-r--r--   0        0        0      517 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_numnull_parents.py
--rw-r--r--   0        0        0      520 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_overlay_mask8_to64.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_ranges_carry_next_64.py
--rw-r--r--   0        0        0      516 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_ranges_next_64.py
--rw-r--r--   0        0        0      516 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_reduce_next_64.py
--rw-r--r--   0        0        0      536 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_reduce_next_nonlocal_nextshifts_64.py
--rw-r--r--   0        0        0      547 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_reduce_next_nonlocal_nextshifts_fromshifts_64.py
--rw-r--r--   0        0        0     9865 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_simplify32_to64.py
--rw-r--r--   0        0        0     9865 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_simplify64_to64.py
--rw-r--r--   0        0        0     9910 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_simplifyU32_to64.py
--rw-r--r--   0        0        0     8475 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_validity.py
--rw-r--r--   0        0        0     2876 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_flatten_nextcarry_64.py
--rw-r--r--   0        0        0    14949 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_flatten_none2empty_64.py
--rw-r--r--   0        0        0     2876 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_getitem_nextcarry_64.py
--rw-r--r--   0        0        0     2452 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_getitem_nextcarry_outindex_64.py
--rw-r--r--   0        0        0      517 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_index_of_nulls.py
--rw-r--r--   0        0        0     3134 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_numnull.py
--rw-r--r--   0        0        0      518 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_numnull_parents.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_overlay_mask8_to64.py
--rw-r--r--   0        0        0      523 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_ranges_carry_next_64.py
--rw-r--r--   0        0        0      517 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_ranges_next_64.py
--rw-r--r--   0        0        0      517 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_reduce_next_64.py
--rw-r--r--   0        0        0      537 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_reduce_next_nonlocal_nextshifts_64.py
--rw-r--r--   0        0        0      548 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_reduce_next_nonlocal_nextshifts_fromshifts_64.py
--rw-r--r--   0        0        0     9910 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_simplify32_to64.py
--rw-r--r--   0        0        0     9910 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_simplify64_to64.py
--rw-r--r--   0        0        0     9955 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_simplifyU32_to64.py
--rw-r--r--   0        0        0     8550 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_validity.py
--rw-r--r--   0        0        0     2969 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray_fill_to64_count.py
--rw-r--r--   0        0        0     3629 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray_fill_to64_from32.py
--rw-r--r--   0        0        0     3629 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray_fill_to64_from64.py
--rw-r--r--   0        0        0     3644 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray_fill_to64_fromU32.py
--rw-r--r--   0        0        0      517 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray_numnull_unique_64.py
--rw-r--r--   0        0        0      526 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray_reduce_next_fix_offsets_64.py
--rw-r--r--   0        0        0     3373 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedOptionArray_rpad_and_clip_mask_axis1_64.py
--rw-r--r--   0        0        0     1350 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_broadcast_tooffsets_64.py
--rw-r--r--   0        0        0    24052 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_combinations_length_64.py
--rw-r--r--   0        0        0     3899 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_compact_offsets_64.py
--rw-r--r--   0        0        0    17497 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_jagged_descend_64.py
--rw-r--r--   0        0        0     6678 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_jagged_expand_64.py
--rw-r--r--   0        0        0     8008 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_next_array_64.py
--rw-r--r--   0        0        0    46454 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_next_array_advanced_64.py
--rw-r--r--   0        0        0     1427 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_next_at_64.py
--rw-r--r--   0        0        0     3284 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_next_range_counts_64.py
--rw-r--r--   0        0        0      535 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_next_range_spreadadvanced_64.py
--rw-r--r--   0        0        0     2081 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_localindex_64.py
--rw-r--r--   0        0        0     3612 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_min_range.py
--rw-r--r--   0        0        0     3898 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_rpad_and_clip_length_axis1.py
--rw-r--r--   0        0        0     6207 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_rpad_axis1_64.py
--rw-r--r--   0        0        0     2285 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_validity.py
--rw-r--r--   0        0        0     1350 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_broadcast_tooffsets_64.py
--rw-r--r--   0        0        0    24052 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_combinations_length_64.py
--rw-r--r--   0        0        0     3899 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_compact_offsets_64.py
--rw-r--r--   0        0        0    17497 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_jagged_descend_64.py
--rw-r--r--   0        0        0     6678 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_jagged_expand_64.py
--rw-r--r--   0        0        0     8008 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_next_array_64.py
--rw-r--r--   0        0        0    46454 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_next_array_advanced_64.py
--rw-r--r--   0        0        0     1427 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_next_at_64.py
--rw-r--r--   0        0        0     3284 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_next_range_counts_64.py
--rw-r--r--   0        0        0      535 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_next_range_spreadadvanced_64.py
--rw-r--r--   0        0        0     2081 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_localindex_64.py
--rw-r--r--   0        0        0     3612 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_min_range.py
--rw-r--r--   0        0        0     3898 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_rpad_and_clip_length_axis1.py
--rw-r--r--   0        0        0     6207 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_rpad_axis1_64.py
--rw-r--r--   0        0        0     2285 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_validity.py
--rw-r--r--   0        0        0     1360 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_broadcast_tooffsets_64.py
--rw-r--r--   0        0        0    24177 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_combinations_length_64.py
--rw-r--r--   0        0        0     3924 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_compact_offsets_64.py
--rw-r--r--   0        0        0    17622 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_jagged_descend_64.py
--rw-r--r--   0        0        0     6703 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_jagged_expand_64.py
--rw-r--r--   0        0        0     8043 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_next_array_64.py
--rw-r--r--   0        0        0    46669 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_next_array_advanced_64.py
--rw-r--r--   0        0        0     1437 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_next_at_64.py
--rw-r--r--   0        0        0     3299 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_next_range_counts_64.py
--rw-r--r--   0        0        0      536 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_next_range_spreadadvanced_64.py
--rw-r--r--   0        0        0     2090 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_localindex_64.py
--rw-r--r--   0        0        0     3637 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_min_range.py
--rw-r--r--   0        0        0     3923 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_rpad_and_clip_length_axis1.py
--rw-r--r--   0        0        0     6252 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_rpad_axis1_64.py
--rw-r--r--   0        0        0     2310 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_validity.py
--rw-r--r--   0        0        0     5525 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray_fill_to64_from32.py
--rw-r--r--   0        0        0     5525 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray_fill_to64_from64.py
--rw-r--r--   0        0        0     5550 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray_fill_to64_fromU32.py
--rw-r--r--   0        0        0     3908 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray_getitem_jagged_carrylen_64.py
--rw-r--r--   0        0        0      523 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray_getitem_jagged_numvalid_64.py
--rw-r--r--   0        0        0    20350 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray32_flatten_offsets_64.py
--rw-r--r--   0        0        0      532 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray32_reduce_local_nextparents_64.py
--rw-r--r--   0        0        0      527 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray32_rpad_and_clip_axis1_64.py
--rw-r--r--   0        0        0      518 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray32_rpad_axis1_64.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray32_rpad_length_axis1.py
--rw-r--r--   0        0        0     2424 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray32_toRegularArray.py
--rw-r--r--   0        0        0    20350 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray64_flatten_offsets_64.py
--rw-r--r--   0        0        0      532 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray64_reduce_local_nextparents_64.py
--rw-r--r--   0        0        0      527 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray64_rpad_and_clip_axis1_64.py
--rw-r--r--   0        0        0      518 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray64_rpad_axis1_64.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray64_rpad_length_axis1.py
--rw-r--r--   0        0        0     2424 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray64_toRegularArray.py
--rw-r--r--   0        0        0    20425 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArrayU32_flatten_offsets_64.py
--rw-r--r--   0        0        0      533 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArrayU32_reduce_local_nextparents_64.py
--rw-r--r--   0        0        0      528 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArrayU32_rpad_and_clip_axis1_64.py
--rw-r--r--   0        0        0      519 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArrayU32_rpad_axis1_64.py
--rw-r--r--   0        0        0      523 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArrayU32_rpad_length_axis1.py
--rw-r--r--   0        0        0     2439 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArrayU32_toRegularArray.py
--rw-r--r--   0        0        0    20055 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray_drop_none_indexes_32.py
--rw-r--r--   0        0        0    20055 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray_drop_none_indexes_64.py
--rw-r--r--   0        0        0      523 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray_local_preparenext_64.py
--rw-r--r--   0        0        0      542 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray_reduce_nonlocal_maxcount_offsetscopy_64.py
--rw-r--r--   0        0        0      532 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray_reduce_nonlocal_nextstarts_64.py
--rw-r--r--   0        0        0    26500 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_MaskedArray32_getitem_next_jagged_project.py
--rw-r--r--   0        0        0    26500 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_MaskedArray64_getitem_next_jagged_project.py
--rw-r--r--   0        0        0    26575 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_MaskedArrayU32_getitem_next_jagged_project.py
--rw-r--r--   0        0        0      524 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromfloat32.py
--rw-r--r--   0        0        0      524 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromfloat64.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromint16.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromint32.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromint64.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromint8.py
--rw-r--r--   0        0        0      523 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromuint16.py
--rw-r--r--   0        0        0      523 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromuint32.py
--rw-r--r--   0        0        0      523 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromuint64.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromuint8.py
--rw-r--r--   0        0        0      524 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromfloat32.py
--rw-r--r--   0        0        0      524 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromfloat64.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromint16.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromint32.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromint64.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromint8.py
--rw-r--r--   0        0        0      523 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromuint16.py
--rw-r--r--   0        0        0      523 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromuint32.py
--rw-r--r--   0        0        0      523 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromuint64.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromuint8.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromfloat32.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromfloat64.py
--rw-r--r--   0        0        0      520 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromint16.py
--rw-r--r--   0        0        0      520 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromint32.py
--rw-r--r--   0        0        0      520 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromint64.py
--rw-r--r--   0        0        0      519 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromint8.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromuint16.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromuint32.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromuint64.py
--rw-r--r--   0        0        0      520 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromuint8.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromfloat32.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromfloat64.py
--rw-r--r--   0        0        0      520 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromint16.py
--rw-r--r--   0        0        0      520 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromint32.py
--rw-r--r--   0        0        0      520 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromint64.py
--rw-r--r--   0        0        0      519 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromint8.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromuint16.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromuint32.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromuint64.py
--rw-r--r--   0        0        0      520 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromuint8.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromfloat32.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromfloat64.py
--rw-r--r--   0        0        0      520 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromint16.py
--rw-r--r--   0        0        0      520 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromint32.py
--rw-r--r--   0        0        0      520 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromint64.py
--rw-r--r--   0        0        0      519 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromint8.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromuint16.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromuint32.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromuint64.py
--rw-r--r--   0        0        0      520 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromuint8.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromfloat32.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromfloat64.py
--rw-r--r--   0        0        0      519 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromint16.py
--rw-r--r--   0        0        0      519 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromint32.py
--rw-r--r--   0        0        0      519 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromint64.py
--rw-r--r--   0        0        0      518 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromint8.py
--rw-r--r--   0        0        0      520 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromuint16.py
--rw-r--r--   0        0        0      520 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromuint32.py
--rw-r--r--   0        0        0      520 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromuint64.py
--rw-r--r--   0        0        0      519 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromuint8.py
--rw-r--r--   0        0        0      523 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromfloat32.py
--rw-r--r--   0        0        0      523 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromfloat64.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromint16.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromint32.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromint64.py
--rw-r--r--   0        0        0      520 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromint8.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromuint16.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromuint32.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromuint64.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromuint8.py
--rw-r--r--   0        0        0      523 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromfloat32.py
--rw-r--r--   0        0        0      523 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromfloat64.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromint16.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromint32.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromint64.py
--rw-r--r--   0        0        0      520 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromint8.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromuint16.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromuint32.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromuint64.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromuint8.py
--rw-r--r--   0        0        0      523 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromfloat32.py
--rw-r--r--   0        0        0      523 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromfloat64.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromint16.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromint32.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromint64.py
--rw-r--r--   0        0        0      520 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromint8.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromuint16.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromuint32.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromuint64.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromuint8.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromfloat32.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromfloat64.py
--rw-r--r--   0        0        0      520 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromint16.py
--rw-r--r--   0        0        0      520 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromint32.py
--rw-r--r--   0        0        0      520 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromint64.py
--rw-r--r--   0        0        0      519 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromint8.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromuint16.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromuint32.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromuint64.py
--rw-r--r--   0        0        0      520 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromuint8.py
--rw-r--r--   0        0        0      522 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_pad_zero_to_length_uint8.py
--rw-r--r--   0        0        0      521 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_reduce_adjust_starts_64.py
--rw-r--r--   0        0        0      528 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_reduce_adjust_starts_shifts_64.py
--rw-r--r--   0        0        0      528 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_reduce_mask_ByteMaskedArray_64.py
--rw-r--r--   0        0        0    13090 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_carry_64.py
--rw-r--r--   0        0        0    19346 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_jagged_expand_64.py
--rw-r--r--   0        0        0    24330 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_next_array_64.py
--rw-r--r--   0        0        0   125787 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_next_array_advanced_64.py
--rw-r--r--   0        0        0    11737 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_next_array_regularize_64.py
--rw-r--r--   0        0        0     2375 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_next_at_64.py
--rw-r--r--   0        0        0      958 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_next_range_64.py
--rw-r--r--   0        0        0    14446 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_next_range_spreadadvanced_64.py
--rw-r--r--   0        0        0     2371 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_RegularArray_localindex_64.py
--rw-r--r--   0        0        0      527 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_RegularArray_reduce_local_nextparents_64.py
--rw-r--r--   0        0        0      530 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_RegularArray_reduce_nonlocal_preparenext_64.py
--rw-r--r--   0        0        0      897 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_RegularArray_rpad_and_clip_axis1_64.py
--rw-r--r--   0        0        0    13570 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_32_project_64.py
--rw-r--r--   0        0        0   619561 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_32_simplify8_32_to8_64.py
--rw-r--r--   0        0        0   619561 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_32_simplify8_64_to8_64.py
--rw-r--r--   0        0        0   621061 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_32_simplify8_U32_to8_64.py
--rw-r--r--   0        0        0    14770 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_32_simplify_one_to8_64.py
--rw-r--r--   0        0        0    61679 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_32_validity.py
--rw-r--r--   0        0        0    13570 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_64_project_64.py
--rw-r--r--   0        0        0   619561 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_64_simplify8_32_to8_64.py
--rw-r--r--   0        0        0   619561 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_64_simplify8_64_to8_64.py
--rw-r--r--   0        0        0   621061 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_64_simplify8_U32_to8_64.py
--rw-r--r--   0        0        0    14770 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_64_simplify_one_to8_64.py
--rw-r--r--   0        0        0    61679 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_64_validity.py
--rw-r--r--   0        0        0    13615 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_U32_project_64.py
--rw-r--r--   0        0        0   621061 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_U32_simplify8_32_to8_64.py
--rw-r--r--   0        0        0   621061 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_U32_simplify8_64_to8_64.py
--rw-r--r--   0        0        0   622561 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_U32_simplify8_U32_to8_64.py
--rw-r--r--   0        0        0    14815 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_U32_simplify_one_to8_64.py
--rw-r--r--   0        0        0    62054 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_U32_validity.py
--rw-r--r--   0        0        0     3185 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_regular_index_getsize.py
--rw-r--r--   0        0        0      864 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray_fillindex_to64_count.py
--rw-r--r--   0        0        0     3564 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray_fillindex_to64_from32.py
--rw-r--r--   0        0        0     3564 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray_fillindex_to64_from64.py
--rw-r--r--   0        0        0     3579 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray_fillindex_to64_fromU32.py
--rw-r--r--   0        0        0     3199 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray_fillna_from32_to64.py
--rw-r--r--   0        0        0     3199 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray_fillna_from64_to64.py
--rw-r--r--   0        0        0     3214 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray_fillna_fromU32_to64.py
--rw-r--r--   0        0        0      870 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray_filltags_to8_const.py
--rw-r--r--   0        0        0     3650 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray_filltags_to8_from8.py
--rw-r--r--   0        0        0      816 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_index_rpad_and_clip_axis0_64.py
--rw-r--r--   0        0        0     1021 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_index_rpad_and_clip_axis1_64.py
--rw-r--r--   0        0        0      763 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_localindex_64.py
--rw-r--r--   0        0        0    17411 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_missing_repeat_64.py
--rw-r--r--   0        0        0      511 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_argmax_float32_64.py
--rw-r--r--   0        0        0      511 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_argmax_float64_64.py
--rw-r--r--   0        0        0      509 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_argmax_int16_64.py
--rw-r--r--   0        0        0      509 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_argmax_int32_64.py
--rw-r--r--   0        0        0      509 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_argmax_int64_64.py
--rw-r--r--   0        0        0      508 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_argmax_int8_64.py
--rw-r--r--   0        0        0      510 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_argmax_uint16_64.py
--rw-r--r--   0        0        0      510 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_argmax_uint32_64.py
--rw-r--r--   0        0        0      510 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_argmax_uint64_64.py
--rw-r--r--   0        0        0      509 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_argmax_uint8_64.py
--rw-r--r--   0        0        0      511 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_argmin_float32_64.py
--rw-r--r--   0        0        0      511 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_argmin_float64_64.py
--rw-r--r--   0        0        0      509 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_argmin_int16_64.py
--rw-r--r--   0        0        0      509 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_argmin_int32_64.py
--rw-r--r--   0        0        0      509 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_argmin_int64_64.py
--rw-r--r--   0        0        0      508 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_argmin_int8_64.py
--rw-r--r--   0        0        0      510 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_argmin_uint16_64.py
--rw-r--r--   0        0        0      510 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_argmin_uint32_64.py
--rw-r--r--   0        0        0      510 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_argmin_uint64_64.py
--rw-r--r--   0        0        0      509 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_argmin_uint8_64.py
--rw-r--r--   0        0        0      502 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_count_64.py
--rw-r--r--   0        0        0      514 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_bool_64.py
--rw-r--r--   0        0        0      517 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_float32_64.py
--rw-r--r--   0        0        0      517 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_float64_64.py
--rw-r--r--   0        0        0      515 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_int16_64.py
--rw-r--r--   0        0        0      515 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_int32_64.py
--rw-r--r--   0        0        0      515 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_int64_64.py
--rw-r--r--   0        0        0      514 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_int8_64.py
--rw-r--r--   0        0        0      516 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_uint16_64.py
--rw-r--r--   0        0        0      516 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_uint32_64.py
--rw-r--r--   0        0        0      516 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_uint64_64.py
--rw-r--r--   0        0        0      515 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_uint8_64.py
--rw-r--r--   0        0        0      516 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_max_float32_float32_64.py
--rw-r--r--   0        0        0      516 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_max_float64_float64_64.py
--rw-r--r--   0        0        0      512 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_max_int16_int16_64.py
--rw-r--r--   0        0        0      512 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_max_int32_int32_64.py
--rw-r--r--   0        0        0      512 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_max_int64_int64_64.py
--rw-r--r--   0        0        0      510 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_max_int8_int8_64.py
--rw-r--r--   0        0        0      514 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_max_uint16_uint16_64.py
--rw-r--r--   0        0        0      514 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_max_uint32_uint32_64.py
--rw-r--r--   0        0        0      514 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_max_uint64_uint64_64.py
--rw-r--r--   0        0        0      512 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_max_uint8_uint8_64.py
--rw-r--r--   0        0        0      516 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_min_float32_float32_64.py
--rw-r--r--   0        0        0      516 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_min_float64_float64_64.py
--rw-r--r--   0        0        0      512 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_min_int16_int16_64.py
--rw-r--r--   0        0        0      512 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_min_int32_int32_64.py
--rw-r--r--   0        0        0      512 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_min_int64_int64_64.py
--rw-r--r--   0        0        0      510 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_min_int8_int8_64.py
--rw-r--r--   0        0        0      514 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_min_uint16_uint16_64.py
--rw-r--r--   0        0        0      514 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_min_uint32_uint32_64.py
--rw-r--r--   0        0        0      514 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_min_uint64_uint64_64.py
--rw-r--r--   0        0        0      512 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_min_uint8_uint8_64.py
--rw-r--r--   0        0        0      511 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_bool_64.py
--rw-r--r--   0        0        0      514 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_float32_64.py
--rw-r--r--   0        0        0      514 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_float64_64.py
--rw-r--r--   0        0        0      512 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_int16_64.py
--rw-r--r--   0        0        0      512 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_int32_64.py
--rw-r--r--   0        0        0      512 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_int64_64.py
--rw-r--r--   0        0        0      511 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_int8_64.py
--rw-r--r--   0        0        0      513 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_uint16_64.py
--rw-r--r--   0        0        0      513 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_uint32_64.py
--rw-r--r--   0        0        0      513 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_uint64_64.py
--rw-r--r--   0        0        0      512 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_uint8_64.py
--rw-r--r--   0        0        0      510 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_bool_64.py
--rw-r--r--   0        0        0      513 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_float32_64.py
--rw-r--r--   0        0        0      513 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_float64_64.py
--rw-r--r--   0        0        0      511 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_int16_64.py
--rw-r--r--   0        0        0      511 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_int32_64.py
--rw-r--r--   0        0        0      511 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_int64_64.py
--rw-r--r--   0        0        0      510 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_int8_64.py
--rw-r--r--   0        0        0      512 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_uint16_64.py
--rw-r--r--   0        0        0      512 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_uint32_64.py
--rw-r--r--   0        0        0      512 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_uint64_64.py
--rw-r--r--   0        0        0      511 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_uint8_64.py
--rw-r--r--   0        0        0      516 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_float32_float32_64.py
--rw-r--r--   0        0        0      516 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_float64_float64_64.py
--rw-r--r--   0        0        0      511 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_int32_bool_64.py
--rw-r--r--   0        0        0      512 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_int32_int16_64.py
--rw-r--r--   0        0        0      512 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_int32_int32_64.py
--rw-r--r--   0        0        0      511 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_int32_int8_64.py
--rw-r--r--   0        0        0      511 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_int64_bool_64.py
--rw-r--r--   0        0        0      512 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_int64_int16_64.py
--rw-r--r--   0        0        0      512 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_int64_int32_64.py
--rw-r--r--   0        0        0      512 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_int64_int64_64.py
--rw-r--r--   0        0        0      511 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_int64_int8_64.py
--rw-r--r--   0        0        0      514 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint32_uint16_64.py
--rw-r--r--   0        0        0      514 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint32_uint32_64.py
--rw-r--r--   0        0        0      513 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint32_uint8_64.py
--rw-r--r--   0        0        0      514 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint64_uint16_64.py
--rw-r--r--   0        0        0      514 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint64_uint32_64.py
--rw-r--r--   0        0        0      514 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint64_uint64_64.py
--rw-r--r--   0        0        0      513 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint64_uint8_64.py
--rw-r--r--   0        0        0      501 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_sorting_ranges.py
--rw-r--r--   0        0        0      508 2024-04-01 18:26:47.000000 awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_sorting_ranges_length.py
--rw-r--r--   0        0        0     2364 2024-04-01 18:26:47.000000 awkward-2.6.3/.gitignore
--rw-r--r--   0        0        0     1520 2024-04-01 18:26:47.000000 awkward-2.6.3/LICENSE
--rw-r--r--   0        0        0     8928 2024-04-01 18:26:47.000000 awkward-2.6.3/pyproject.toml
--rw-r--r--   0        0        0     6975 2024-04-01 18:26:47.000000 awkward-2.6.3/PKG-INFO
+-rw-r--r--   0        0        0     1889 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/CITATION.cff
+-rw-r--r--   0        0        0    14355 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/CONTRIBUTING.md
+-rw-r--r--   0        0        0    25943 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/README.md
+-rw-r--r--   0        0        0      173 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/juliapkg.json
+-rw-r--r--   0        0        0      393 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/requirements-test-full.txt
+-rw-r--r--   0        0        0      105 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/requirements-test-minimal.txt
+-rw-r--r--   0        0        0     8686 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/_toc.yml
+-rw-r--r--   0        0        0     7735 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/conf.py
+-rw-r--r--   0        0        0      346 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/environment.yml.cog
+-rw-r--r--   0        0        0     3469 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/index.md
+-rw-r--r--   0        0        0    11690 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/prepare_docstrings.py
+-rw-r--r--   0        0        0     4448 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/redirects-user-guide.json
+-rw-r--r--   0        0        0    11440 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/redirects.json
+-rw-r--r--   0        0        0       33 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/requirements-wasm.txt
+-rw-r--r--   0        0        0      571 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/requirements.txt
+-rw-r--r--   0        0        0      825 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/switcher.json
+-rw-r--r--   0        0        0      942 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/_static/css/awkward.css
+-rw-r--r--   0        0        0      355 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/_static/css/try-awkward-array.css
+lrwxr-xr-x   0        0        0        0 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/_static/image/logo-300px-white.png -> ../../../docs-img/logo/logo-300px-white.png
+lrwxr-xr-x   0        0        0        0 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/_static/image/logo-300px.png -> ../../../docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0      469 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/_templates/funding.html
+-rw-r--r--   0        0        0      474 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/_templates/redirect.html
+-rw-r--r--   0        0        0   245975 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/data/y77d-th95.json
+-rw-r--r--   0        0        0     2968 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/getting-started/community-tutorials.md
+-rw-r--r--   0        0        0     4654 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/getting-started/index.md
+-rw-r--r--   0        0        0     3346 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/getting-started/papers-and-talks.md
+-rw-r--r--   0        0        0       93 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/getting-started/try-awkward-array.md
+lrwxr-xr-x   0        0        0        0 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/getting-started/demo/example-reduction-sum.svg -> ../../../docs-img/diagrams/example-reduction-sum.svg
+-rw-r--r--   0        0        0    13128 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/getting-started/demo/what-is-an-awkward-array.ipynb
+lrwxr-xr-x   0        0        0        0 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/image/awkward-1-0-layers.svg -> ../../docs-img/diagrams/awkward-1-0-layers.svg
+lrwxr-xr-x   0        0        0        0 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/image/bikeroutes-scaling.svg -> ../../docs-img/plots/bikeroutes-scaling.svg
+lrwxr-xr-x   0        0        0        0 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/image/desire-path.jpg -> ../../docs-img/photos/desire-path.jpg
+lrwxr-xr-x   0        0        0        0 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/image/example-array.svg -> ../../docs-img/diagrams/example-array.svg
+-rw-r--r--   0        0        0    17067 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/image/example-hierarchy.svg
+lrwxr-xr-x   0        0        0        0 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/image/example-reduction-sum-only.svg -> ../../docs-img/diagrams/example-reduction-sum-only.svg
+lrwxr-xr-x   0        0        0        0 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/image/example-reduction-sum.svg -> ../../docs-img/diagrams/example-reduction-sum.svg
+lrwxr-xr-x   0        0        0        0 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/image/favicon.ico -> ../../docs-img/logo/favicon.ico
+lrwxr-xr-x   0        0        0        0 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/image/github-issues-documentation.png -> ../../docs-img/screenshots/github-issues-documentation.png
+lrwxr-xr-x   0        0        0        0 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/image/how-it-works.svg -> ../../docs-img/diagrams/how-it-works.svg
+lrwxr-xr-x   0        0        0        0 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/image/logo-300px.png -> ../../docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0    24232 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/reference/ak.behavior.md
+-rw-r--r--   0        0        0     1426 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/reference/ak.builder.ArrayBuilder.rst
+-rw-r--r--   0        0        0    64727 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/reference/awkwardforth.rst
+-rw-r--r--   0        0        0      271 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/reference/index.md
+-rw-r--r--   0        0        0     9491 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/reference/toctree.txt
+-rw-r--r--   0        0        0   214211 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/samples/Android.head.log.gz
+-rw-r--r--   0        0        0     8320 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/10-minutes-to-awkward-array.md
+-rw-r--r--   0        0        0      926 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-combinatorics-best-match.md
+-rw-r--r--   0        0        0      930 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-combinatorics-cartesian-combinations.md
+-rw-r--r--   0        0        0      263 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-combinatorics.md
+-rw-r--r--   0        0        0     8335 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-convert-arrow.md
+-rw-r--r--   0        0        0     6323 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-convert-buffers.md
+-rw-r--r--   0        0        0     2455 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-convert-json.md
+-rw-r--r--   0        0        0    13475 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-convert-numpy.md
+-rw-r--r--   0        0        0     7182 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-convert-pandas.md
+-rw-r--r--   0        0        0    18472 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-convert-python.md
+-rw-r--r--   0        0        0     3554 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-convert-rdataframe.md
+-rw-r--r--   0        0        0      271 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-convert.md
+-rw-r--r--   0        0        0    11973 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-create-arraybuilder.md
+-rw-r--r--   0        0        0    36902 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-create-constructors.md
+-rw-r--r--   0        0        0     7383 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-create-lists.md
+-rw-r--r--   0        0        0     7456 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-create-missing.md
+-rw-r--r--   0        0        0    11542 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-create-records.md
+-rw-r--r--   0        0        0     4093 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-create-strings.md
+-rw-r--r--   0        0        0     4364 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-create-unflatten-group.md
+-rw-r--r--   0        0        0      267 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-create.md
+-rw-r--r--   0        0        0      834 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-examine-checking-validity.md
+-rw-r--r--   0        0        0     2919 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-examine-list-fields.md
+-rw-r--r--   0        0        0      848 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-examine-simple-slicing.md
+-rw-r--r--   0        0        0      838 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-examine-single-item.md
+-rw-r--r--   0        0        0     6778 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-examine-type.md
+-rw-r--r--   0        0        0      269 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-examine.md
+-rw-r--r--   0        0        0      844 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-filter-cut-mask.md
+-rw-r--r--   0        0        0     3889 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-filter-masked.md
+-rw-r--r--   0        0        0      840 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-filter-num.md
+-rw-r--r--   0        0        0     7955 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-filter-ragged.md
+-rw-r--r--   0        0        0      265 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-filter.md
+-rw-r--r--   0        0        0      818 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-math-argminmax.md
+-rw-r--r--   0        0        0      822 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-math-broadcasting.md
+-rw-r--r--   0        0        0      828 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-math-gpu.md
+-rw-r--r--   0        0        0      838 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-math-numpy.md
+-rw-r--r--   0        0        0      846 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-math-reducing.md
+-rw-r--r--   0        0        0      870 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-math-statistics.md
+-rw-r--r--   0        0        0      265 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-math.md
+-rw-r--r--   0        0        0     3411 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-restructure-add-fields.md
+-rw-r--r--   0        0        0      842 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-restructure-concatenate.md
+-rw-r--r--   0        0        0    19083 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-restructure-flatten.md
+-rw-r--r--   0        0        0     7568 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-restructure-pad.md
+-rw-r--r--   0        0        0      852 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-restructure-rename-records.md
+-rw-r--r--   0        0        0      832 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-restructure-sort.md
+-rw-r--r--   0        0        0     9624 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-restructure-zip-project.md
+-rw-r--r--   0        0        0      273 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-restructure.md
+-rw-r--r--   0        0        0     2599 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-specialize-differentiate-jax.md
+-rw-r--r--   0        0        0      870 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-specialize-in-numba.md
+-rw-r--r--   0        0        0      838 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-specialize-lorentz.md
+-rw-r--r--   0        0        0      874 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-specialize-override-numpy.md
+-rw-r--r--   0        0        0      870 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-specialize-subclass.md
+-rw-r--r--   0        0        0      277 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-specialize.md
+-rw-r--r--   0        0        0    10650 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-strings-extract-substrings.md
+-rw-r--r--   0        0        0     5030 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-strings-read-binary.md
+-rw-r--r--   0        0        0     5734 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-strings-split-and-join.md
+-rw-r--r--   0        0        0    11694 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-use-header-only-layoutbuilder.md
+-rw-r--r--   0        0        0     7580 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-use-in-cpp-cppyy.ipynb
+-rw-r--r--   0        0        0      277 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-use-in-cpp.md
+-rw-r--r--   0        0        0      900 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-use-in-numba-arraybuilder.md
+-rw-r--r--   0        0        0     9973 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-use-in-numba-cuda.ipynb
+-rw-r--r--   0        0        0      900 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-use-in-numba-features.md
+-rw-r--r--   0        0        0      279 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/how-to-use-in-numba.md
+-rw-r--r--   0        0        0      344 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/index.md
+-rw-r--r--   0        0        0        0 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs/user-guide/requirements.txt
+-rw-r--r--   0        0        0   367587 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/panel-data-analysts.png
+-rw-r--r--   0        0        0   794465 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/panel-data-analysts.svg
+-rw-r--r--   0        0        0   140700 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/panel-developers.png
+-rw-r--r--   0        0        0   328307 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/panel-developers.svg
+-rw-r--r--   0        0        0    73584 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/panel-doxygen.png
+-rw-r--r--   0        0        0    58179 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/panel-sphinx.png
+-rw-r--r--   0        0        0   127063 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/panel-tutorials-alternate.png
+-rw-r--r--   0        0        0   173327 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/panel-tutorials.png
+-rw-r--r--   0        0        0    12541 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/awkward-1-0-layers.pdf
+-rw-r--r--   0        0        0    65246 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/awkward-1-0-layers.png
+-rw-r--r--   0        0        0    41004 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/awkward-1-0-layers.svg
+-rw-r--r--   0        0        0    14946 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/awkward-timeline.pdf
+-rw-r--r--   0        0        0   125180 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/awkward-timeline.png
+-rw-r--r--   0        0        0    70209 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/awkward-timeline.svg
+-rw-r--r--   0        0        0   436595 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/awkward-uproot-timeline-pip-github.png
+-rw-r--r--   0        0        0   426911 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg
+-rw-r--r--   0        0        0   335955 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/awkward-uproot-timeline-pip.png
+-rw-r--r--   0        0        0   325268 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/awkward-uproot-timeline-pip.svg
+-rw-r--r--   0        0        0   129696 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/awkward-uproot-timeline.png
+-rw-r--r--   0        0        0   120554 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/awkward-uproot-timeline.svg
+-rw-r--r--   0        0        0     5208 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/cartoon-broadcasting.png
+-rw-r--r--   0        0        0    25065 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/cartoon-broadcasting.svg
+-rw-r--r--   0        0        0     5754 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/cartoon-cartesian.png
+-rw-r--r--   0        0        0    32616 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/cartoon-cartesian.svg
+-rw-r--r--   0        0        0     9584 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/cartoon-combinations.png
+-rw-r--r--   0        0        0    39524 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/cartoon-combinations.svg
+-rw-r--r--   0        0        0    10808 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/cartoon-schematic.png
+-rw-r--r--   0        0        0    25779 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/cartoon-schematic.svg
+-rw-r--r--   0        0        0    18178 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/example-array.svg
+-rw-r--r--   0        0        0    36024 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/example-hierarchy.png
+-rw-r--r--   0        0        0    17092 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/example-hierarchy.svg
+-rw-r--r--   0        0        0    21120 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/example-reduction-sum-only.svg
+-rw-r--r--   0        0        0    29325 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/example-reduction-sum.svg
+-rw-r--r--   0        0        0    55553 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/example-reduction.png
+-rw-r--r--   0        0        0    21631 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/example-reduction.svg
+-rw-r--r--   0        0        0    10978 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/git-strategy.pdf
+-rw-r--r--   0        0        0    58904 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/git-strategy.png
+-rw-r--r--   0        0        0    28990 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/git-strategy.svg
+-rw-r--r--   0        0        0   113587 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/how-it-works-muons.png
+-rw-r--r--   0        0        0    57471 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/how-it-works-muons.svg
+-rw-r--r--   0        0        0    58475 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/how-it-works.svg
+-rw-r--r--   0        0        0    63989 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/sorting-axis.svg
+-rw-r--r--   0        0        0   124038 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/reducers/all.svg
+-rw-r--r--   0        0        0   128558 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/reducers/any.svg
+-rw-r--r--   0        0        0   134490 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/reducers/argmax.svg
+-rw-r--r--   0        0        0   133192 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/reducers/argmin.svg
+-rw-r--r--   0        0        0   106277 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/reducers/count.svg
+-rw-r--r--   0        0        0   116417 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/reducers/count_nonzero.svg
+-rw-r--r--   0        0        0   111789 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/reducers/max.svg
+-rw-r--r--   0        0        0   109239 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/reducers/min.svg
+-rw-r--r--   0        0        0   124702 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/reducers/product.svg
+-rw-r--r--   0        0        0   108897 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/diagrams/reducers/sum.svg
+-rw-r--r--   0        0        0     8347 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/logo/favicon.ico
+-rw-r--r--   0        0        0     8984 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/logo/logo-300px-white.png
+-rw-r--r--   0        0        0    11964 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0    24707 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/logo/logo-600px.png
+-rw-r--r--   0        0        0    18767 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/logo/logo.svg
+-rw-r--r--   0        0        0    90413 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/photos/desire-path.jpg
+-rw-r--r--   0        0        0    52113 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/plots/awkward-0-popularity.pdf
+-rw-r--r--   0        0        0   146109 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/plots/awkward-0-popularity.png
+-rw-r--r--   0        0        0   147576 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/plots/awkward-0-popularity.svg
+-rw-r--r--   0        0        0    26938 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/plots/bikeroutes-scaling.svg
+-rw-r--r--   0        0        0     8891 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/docs-img/screenshots/github-issues-documentation.png
+-rw-r--r--   0        0        0     1288 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/__init__.py
+-rw-r--r--   0        0        0     1210 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_attrs.py
+-rw-r--r--   0        0        0     5709 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_behavior.py
+-rw-r--r--   0        0        0    36351 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_broadcasting.py
+-rw-r--r--   0        0        0     1293 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_categorical.py
+-rw-r--r--   0        0        0     2849 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_dispatch.py
+-rw-r--r--   0        0        0    13568 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_do.py
+-rw-r--r--   0        0        0    15027 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_errors.py
+-rw-r--r--   0        0        0      370 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_ext.py
+-rw-r--r--   0        0        0     5876 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_kernels.py
+-rw-r--r--   0        0        0    11380 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_layout.py
+-rw-r--r--   0        0        0    10016 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_lookup.py
+-rw-r--r--   0        0        0     8493 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_operators.py
+-rw-r--r--   0        0        0     5023 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_parameters.py
+-rw-r--r--   0        0        0     3746 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_pickle.py
+-rw-r--r--   0        0        0    13901 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_prettyprint.py
+-rw-r--r--   0        0        0    29440 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_reducers.py
+-rw-r--r--   0        0        0     1490 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_regularize.py
+-rw-r--r--   0        0        0     1212 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_singleton.py
+-rw-r--r--   0        0        0    23669 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_slicing.py
+-rw-r--r--   0        0        0      732 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_typetracer.py
+-rw-r--r--   0        0        0     1451 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_typing.py
+-rw-r--r--   0        0        0     2260 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_util.py
+-rw-r--r--   0        0        0      790 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_v2.py
+-rw-r--r--   0        0        0      231 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/builder.py
+-rw-r--r--   0        0        0      922 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/cppyy.py
+-rw-r--r--   0        0        0      260 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/errors.py
+-rw-r--r--   0        0        0      269 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/forth.py
+-rw-r--r--   0        0        0   112732 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/highlevel.py
+-rw-r--r--   0        0        0     9627 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/index.py
+-rw-r--r--   0        0        0     4073 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/jax.py
+-rw-r--r--   0        0        0     8386 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/record.py
+-rw-r--r--   0        0        0     8239 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/typetracer.py
+-rw-r--r--   0        0        0       84 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_backends/__init__.py
+-rw-r--r--   0        0        0     1916 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_backends/backend.py
+-rw-r--r--   0        0        0     1288 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_backends/cupy.py
+-rw-r--r--   0        0        0     4246 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_backends/dispatch.py
+-rw-r--r--   0        0        0     1318 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_backends/jax.py
+-rw-r--r--   0        0        0      973 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_backends/numpy.py
+-rw-r--r--   0        0        0     1454 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_backends/typetracer.py
+-rw-r--r--   0        0        0       84 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/__init__.py
+-rw-r--r--   0        0        0    32644 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/avro.py
+-rw-r--r--   0        0        0    53565 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cling.py
+-rw-r--r--   0        0        0      484 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/dlpack.py
+-rw-r--r--   0        0        0      983 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/hist.py
+-rw-r--r--   0        0        0     4701 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/numexpr.py
+-rw-r--r--   0        0        0    16958 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/numpy.py
+-rw-r--r--   0        0        0    40019 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/pyarrow.py
+-rw-r--r--   0        0        0     8546 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/__init__.py
+-rw-r--r--   0        0        0   284416 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/_kernel_signatures.py
+-rw-r--r--   0        0        0     2333 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu
+-rw-r--r--   0        0        0     4085 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu
+-rw-r--r--   0        0        0     1959 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu
+-rw-r--r--   0        0        0     2259 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu
+-rw-r--r--   0        0        0     1756 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_numnull.cu
+-rw-r--r--   0        0        0      637 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu
+-rw-r--r--   0        0        0     2540 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu
+-rw-r--r--   0        0        0     2474 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu
+-rw-r--r--   0        0        0     2678 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu
+-rw-r--r--   0        0        0      549 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu
+-rw-r--r--   0        0        0     2661 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu
+-rw-r--r--   0        0        0     2114 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_nones_as_index.cu
+-rw-r--r--   0        0        0      590 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill.cu
+-rw-r--r--   0        0        0      502 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill_count.cu
+-rw-r--r--   0        0        0     2353 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu
+-rw-r--r--   0        0        0     3316 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_none2empty.cu
+-rw-r--r--   0        0        0     2371 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu
+-rw-r--r--   0        0        0     2684 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu
+-rw-r--r--   0        0        0     2229 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_index_of_nulls.cu
+-rw-r--r--   0        0        0     1707 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_numnull.cu
+-rw-r--r--   0        0        0     1961 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_numnull_parents.cu
+-rw-r--r--   0        0        0      468 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_numnull_unique_64.cu
+-rw-r--r--   0        0        0      550 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu
+-rw-r--r--   0        0        0     2535 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_ranges_carry_next_64.cu
+-rw-r--r--   0        0        0     2865 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_ranges_next_64.cu
+-rw-r--r--   0        0        0     2433 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu
+-rw-r--r--   0        0        0      580 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu
+-rw-r--r--   0        0        0     2339 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu
+-rw-r--r--   0        0        0     2543 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu
+-rw-r--r--   0        0        0      884 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu
+-rw-r--r--   0        0        0      836 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu
+-rw-r--r--   0        0        0     2005 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu
+-rw-r--r--   0        0        0     3835 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_broadcast_tooffsets.cu
+-rw-r--r--   0        0        0     3234 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_combinations_length.cu
+-rw-r--r--   0        0        0     2434 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu
+-rw-r--r--   0        0        0      715 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_fill.cu
+-rw-r--r--   0        0        0     2006 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_carrylen.cu
+-rw-r--r--   0        0        0     3305 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_descend.cu
+-rw-r--r--   0        0        0     1484 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu
+-rw-r--r--   0        0        0     2810 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_numvalid.cu
+-rw-r--r--   0        0        0     1720 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu
+-rw-r--r--   0        0        0     1663 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array_advanced.cu
+-rw-r--r--   0        0        0      958 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_at.cu
+-rw-r--r--   0        0        0     1815 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_range_counts.cu
+-rw-r--r--   0        0        0      695 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_range_spreadadvanced.cu
+-rw-r--r--   0        0        0      617 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_localindex.cu
+-rw-r--r--   0        0        0     2026 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_min_range.cu
+-rw-r--r--   0        0        0     2067 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_rpad_and_clip_length_axis1.cu
+-rw-r--r--   0        0        0     2712 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_rpad_axis1.cu
+-rw-r--r--   0        0        0     1076 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu
+-rw-r--r--   0        0        0     2525 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_drop_none_indexes.cu
+-rw-r--r--   0        0        0      595 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu
+-rw-r--r--   0        0        0     1106 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_local_preparenext_64.cu
+-rw-r--r--   0        0        0      693 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_local_nextparents_64.cu
+-rw-r--r--   0        0        0     2240 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_nonlocal_maxcount_offsetscopy_64.cu
+-rw-r--r--   0        0        0     2045 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_nonlocal_nextstarts_64.cu
+-rw-r--r--   0        0        0      974 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu
+-rw-r--r--   0        0        0     1525 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu
+-rw-r--r--   0        0        0     2302 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_length_axis1.cu
+-rw-r--r--   0        0        0     1118 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_toRegularArray.cu
+-rw-r--r--   0        0        0     2383 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu
+-rw-r--r--   0        0        0      497 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_fill.cu
+-rw-r--r--   0        0        0     1755 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_pad_zero_to_length.cu
+-rw-r--r--   0        0        0      645 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu
+-rw-r--r--   0        0        0      704 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu
+-rw-r--r--   0        0        0      577 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu
+-rw-r--r--   0        0        0      639 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu
+-rw-r--r--   0        0        0      811 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu
+-rw-r--r--   0        0        0      773 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu
+-rw-r--r--   0        0        0      690 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu
+-rw-r--r--   0        0        0      909 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_regularize.cu
+-rw-r--r--   0        0        0      814 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu
+-rw-r--r--   0        0        0      699 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu
+-rw-r--r--   0        0        0      651 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu
+-rw-r--r--   0        0        0      556 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu
+-rw-r--r--   0        0        0     1946 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_reduce_local_nextparents.cu
+-rw-r--r--   0        0        0     2353 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_reduce_nonlocal_preparenext.cu
+-rw-r--r--   0        0        0      825 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_rpad_and_clip_axis1.cu
+-rw-r--r--   0        0        0      520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillindex.cu
+-rw-r--r--   0        0        0      479 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillindex_count.cu
+-rw-r--r--   0        0        0      503 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillna.cu
+-rw-r--r--   0        0        0      540 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_filltags.cu
+-rw-r--r--   0        0        0      487 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_filltags_const.cu
+-rw-r--r--   0        0        0     2195 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu
+-rw-r--r--   0        0        0      864 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_regular_index_getsize.cu
+-rw-r--r--   0        0        0      893 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_simplify.cu
+-rw-r--r--   0        0        0      709 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_simplify_one.cu
+-rw-r--r--   0        0        0     1221 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu
+-rw-r--r--   0        0        0      652 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis0.cu
+-rw-r--r--   0        0        0      544 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu
+-rw-r--r--   0        0        0      417 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_localindex.cu
+-rw-r--r--   0        0        0      721 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu
+-rw-r--r--   0        0        0     1910 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu
+-rw-r--r--   0        0        0     1819 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu
+-rw-r--r--   0        0        0     2756 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu
+-rw-r--r--   0        0        0     2935 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu
+-rw-r--r--   0        0        0     1830 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu
+-rw-r--r--   0        0        0     1830 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu
+-rw-r--r--   0        0        0     2890 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu
+-rw-r--r--   0        0        0     2670 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu
+-rw-r--r--   0        0        0     2873 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu
+-rw-r--r--   0        0        0     3015 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu
+-rw-r--r--   0        0        0     3015 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu
+-rw-r--r--   0        0        0     2337 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_sorting_ranges.cu
+-rw-r--r--   0        0        0     1873 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_sorting_ranges_length.cu
+-rw-r--r--   0        0        0     4774 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu
+-rw-r--r--   0        0        0     1624 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/header-only/awkward/BuilderOptions.h
+-rw-r--r--   0        0        0    19818 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/header-only/awkward/GrowableBuffer.h
+-rw-r--r--   0        0        0    84571 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/header-only/awkward/LayoutBuilder.h
+-rw-r--r--   0        0        0     9545 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/header-only/awkward/utils.h
+-rw-r--r--   0        0        0      367 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/jax/__init__.py
+-rw-r--r--   0        0        0    11453 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/jax/reducers.py
+-rw-r--r--   0        0        0     5980 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/jax/trees.py
+-rw-r--r--   0        0        0       84 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/numba/__init__.py
+-rw-r--r--   0        0        0    36568 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/numba/arrayview.py
+-rw-r--r--   0        0        0     1264 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/numba/arrayview_cuda.py
+-rw-r--r--   0        0        0    32515 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/numba/builder.py
+-rw-r--r--   0        0        0     9730 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/numba/growablebuffer.py
+-rw-r--r--   0        0        0    52143 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/numba/layout.py
+-rw-r--r--   0        0        0    43392 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/numba/layoutbuilder.py
+-rw-r--r--   0        0        0       84 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/rdataframe/__init__.py
+-rw-r--r--   0        0        0     9411 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/rdataframe/from_rdataframe.py
+-rw-r--r--   0        0        0     9954 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/rdataframe/to_rdataframe.py
+-rw-r--r--   0        0        0     1483 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h
+-rw-r--r--   0        0        0        0 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_meta/__init__.py
+-rw-r--r--   0        0        0     1424 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_meta/bitmaskedmeta.py
+-rw-r--r--   0        0        0     1425 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_meta/bytemaskedmeta.py
+-rw-r--r--   0        0        0      966 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_meta/emptymeta.py
+-rw-r--r--   0        0        0     1412 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_meta/indexedmeta.py
+-rw-r--r--   0        0        0     1463 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_meta/indexedoptionmeta.py
+-rw-r--r--   0        0        0     1824 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_meta/listmeta.py
+-rw-r--r--   0        0        0     1834 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_meta/listoffsetmeta.py
+-rw-r--r--   0        0        0     3760 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_meta/meta.py
+-rw-r--r--   0        0        0     1310 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_meta/numpymeta.py
+-rw-r--r--   0        0        0     4085 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_meta/recordmeta.py
+-rw-r--r--   0        0        0     1945 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_meta/regularmeta.py
+-rw-r--r--   0        0        0     3065 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_meta/unionmeta.py
+-rw-r--r--   0        0        0     1435 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_meta/unmaskedmeta.py
+-rw-r--r--   0        0        0     1350 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_nplikes/__init__.py
+-rw-r--r--   0        0        0     3152 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_nplikes/array_like.py
+-rw-r--r--   0        0        0    23468 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_nplikes/array_module.py
+-rw-r--r--   0        0        0     5706 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_nplikes/cupy.py
+-rw-r--r--   0        0        0     1615 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_nplikes/dispatch.py
+-rw-r--r--   0        0        0     2529 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_nplikes/jax.py
+-rw-r--r--   0        0        0     2086 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_nplikes/numpy.py
+-rw-r--r--   0        0        0    12667 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_nplikes/numpy_like.py
+-rw-r--r--   0        0        0     4553 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_nplikes/placeholder.py
+-rw-r--r--   0        0        0     2402 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_nplikes/shape.py
+-rw-r--r--   0        0        0    60519 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_nplikes/typetracer.py
+-rw-r--r--   0        0        0     2648 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/_nplikes/ufuncs.py
+-rw-r--r--   0        0        0       84 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/behaviors/__init__.py
+-rw-r--r--   0        0        0      186 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/behaviors/categorical.py
+-rw-r--r--   0        0        0     3931 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/behaviors/mixins.py
+-rw-r--r--   0        0        0      250 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/behaviors/string.py
+-rw-r--r--   0        0        0     1018 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/contents/__init__.py
+-rw-r--r--   0        0        0    28854 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/contents/bitmaskedarray.py
+-rw-r--r--   0        0        0    42368 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/contents/bytemaskedarray.py
+-rw-r--r--   0        0        0    43592 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/contents/content.py
+-rw-r--r--   0        0        0    13977 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/contents/emptyarray.py
+-rw-r--r--   0        0        0    43371 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/contents/indexedarray.py
+-rw-r--r--   0        0        0    66378 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/contents/indexedoptionarray.py
+-rw-r--r--   0        0        0    63078 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/contents/listarray.py
+-rw-r--r--   0        0        0    88691 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/contents/listoffsetarray.py
+-rw-r--r--   0        0        0    49445 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/contents/numpyarray.py
+-rw-r--r--   0        0        0    46575 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/contents/recordarray.py
+-rw-r--r--   0        0        0    58528 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/contents/regulararray.py
+-rw-r--r--   0        0        0    60274 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/contents/unionarray.py
+-rw-r--r--   0        0        0    20007 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/contents/unmaskedarray.py
+-rw-r--r--   0        0        0      994 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/forms/__init__.py
+-rw-r--r--   0        0        0     6344 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/forms/bitmaskedform.py
+-rw-r--r--   0        0        0     5562 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/forms/bytemaskedform.py
+-rw-r--r--   0        0        0     3485 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/forms/emptyform.py
+-rw-r--r--   0        0        0    22946 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/forms/form.py
+-rw-r--r--   0        0        0     5940 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/forms/indexedform.py
+-rw-r--r--   0        0        0     5298 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/forms/indexedoptionform.py
+-rw-r--r--   0        0        0     5387 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/forms/listform.py
+-rw-r--r--   0        0        0     4627 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/forms/listoffsetform.py
+-rw-r--r--   0        0        0     8044 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/forms/numpyform.py
+-rw-r--r--   0        0        0     6693 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/forms/recordform.py
+-rw-r--r--   0        0        0     4692 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/forms/regularform.py
+-rw-r--r--   0        0        0     6650 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/forms/unionform.py
+-rw-r--r--   0        0        0     4376 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/forms/unmaskedform.py
+-rw-r--r--   0        0        0     9532 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/numba/__init__.py
+-rw-r--r--   0        0        0    23941 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/numba/layoutbuilder.py
+-rw-r--r--   0        0        0     5243 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/__init__.py
+-rw-r--r--   0        0        0     3391 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_all.py
+-rw-r--r--   0        0        0     8574 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_almost_equal.py
+-rw-r--r--   0        0        0     1902 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_angle.py
+-rw-r--r--   0        0        0     3394 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_any.py
+-rw-r--r--   0        0        0     4426 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_argcartesian.py
+-rw-r--r--   0        0        0     3792 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_argcombinations.py
+-rw-r--r--   0        0        0     5771 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_argmax.py
+-rw-r--r--   0        0        0     5632 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_argmin.py
+-rw-r--r--   0        0        0     3241 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_argsort.py
+-rw-r--r--   0        0        0     1141 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_backend.py
+-rw-r--r--   0        0        0     9915 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_broadcast_arrays.py
+-rw-r--r--   0        0        0     7278 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_broadcast_fields.py
+-rw-r--r--   0        0        0    15811 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_cartesian.py
+-rw-r--r--   0        0        0     1709 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_categories.py
+-rw-r--r--   0        0        0     8091 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_combinations.py
+-rw-r--r--   0        0        0    26808 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_concatenate.py
+-rw-r--r--   0        0        0     2773 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_copy.py
+-rw-r--r--   0        0        0     6533 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_corr.py
+-rw-r--r--   0        0        0     4619 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_count.py
+-rw-r--r--   0        0        0     3418 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_count_nonzero.py
+-rw-r--r--   0        0        0     5733 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_covar.py
+-rw-r--r--   0        0        0     4745 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_drop_none.py
+-rw-r--r--   0        0        0    50491 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_enforce_type.py
+-rw-r--r--   0        0        0     1175 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_fields.py
+-rw-r--r--   0        0        0     4667 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_fill_none.py
+-rw-r--r--   0        0        0     3523 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_firsts.py
+-rw-r--r--   0        0        0     7810 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_flatten.py
+-rw-r--r--   0        0        0     3214 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_from_arrow.py
+-rw-r--r--   0        0        0      785 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_from_arrow_schema.py
+-rw-r--r--   0        0        0     2629 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_from_avro_file.py
+-rw-r--r--   0        0        0    16560 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_from_buffers.py
+-rw-r--r--   0        0        0     1876 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_from_categorical.py
+-rw-r--r--   0        0        0     1591 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_from_cupy.py
+-rw-r--r--   0        0        0     3009 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_from_dlpack.py
+-rw-r--r--   0        0        0     2437 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_from_feather.py
+-rw-r--r--   0        0        0     4080 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_from_iter.py
+-rw-r--r--   0        0        0     1667 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_from_jax.py
+-rw-r--r--   0        0        0    28871 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_from_json.py
+-rw-r--r--   0        0        0     2206 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_from_numpy.py
+-rw-r--r--   0        0        0    11541 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_from_parquet.py
+-rw-r--r--   0        0        0     3163 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_from_rdataframe.py
+-rw-r--r--   0        0        0     3083 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_from_regular.py
+-rw-r--r--   0        0        0     9320 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_full_like.py
+-rw-r--r--   0        0        0     1713 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_imag.py
+-rw-r--r--   0        0        0      951 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_is_categorical.py
+-rw-r--r--   0        0        0     2606 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_is_none.py
+-rw-r--r--   0        0        0      921 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_is_tuple.py
+-rw-r--r--   0        0        0      965 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_is_valid.py
+-rw-r--r--   0        0        0     2640 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_isclose.py
+-rw-r--r--   0        0        0     8525 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_linear_fit.py
+-rw-r--r--   0        0        0     3434 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_local_index.py
+-rw-r--r--   0        0        0     4720 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_mask.py
+-rw-r--r--   0        0        0     6035 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_max.py
+-rw-r--r--   0        0        0     9367 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_mean.py
+-rw-r--r--   0        0        0     3699 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_merge_option_of_records.py
+-rw-r--r--   0        0        0    12416 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_merge_union_of_records.py
+-rw-r--r--   0        0        0     3114 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_metadata_from_parquet.py
+-rw-r--r--   0        0        0     6057 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_min.py
+-rw-r--r--   0        0        0     5248 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_moment.py
+-rw-r--r--   0        0        0     2033 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_nan_to_none.py
+-rw-r--r--   0        0        0     5461 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_nan_to_num.py
+-rw-r--r--   0        0        0     4200 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_num.py
+-rw-r--r--   0        0        0     1992 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_ones_like.py
+-rw-r--r--   0        0        0     4431 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_pad_none.py
+-rw-r--r--   0        0        0     1844 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_parameters.py
+-rw-r--r--   0        0        0     5149 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_prod.py
+-rw-r--r--   0        0        0     4573 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_ptp.py
+-rw-r--r--   0        0        0     2470 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_ravel.py
+-rw-r--r--   0        0        0     1708 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_real.py
+-rw-r--r--   0        0        0     2069 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_round.py
+-rw-r--r--   0        0        0     9600 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_run_lengths.py
+-rw-r--r--   0        0        0     3166 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_singletons.py
+-rw-r--r--   0        0        0     3450 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_softmax.py
+-rw-r--r--   0        0        0     2762 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_sort.py
+-rw-r--r--   0        0        0     8351 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_std.py
+-rw-r--r--   0        0        0     3116 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_strings_astype.py
+-rw-r--r--   0        0        0    10595 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_sum.py
+-rw-r--r--   0        0        0     4617 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_to_arrow.py
+-rw-r--r--   0        0        0     7829 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_to_arrow_table.py
+-rw-r--r--   0        0        0     2342 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_to_backend.py
+-rw-r--r--   0        0        0     6202 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_to_buffers.py
+-rw-r--r--   0        0        0        0 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_to_categorical.py
+-rw-r--r--   0        0        0     1167 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_to_cupy.py
+-rw-r--r--   0        0        0    13467 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_to_dataframe.py
+-rw-r--r--   0        0        0     6792 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_to_feather.py
+-rw-r--r--   0        0        0     1167 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_to_jax.py
+-rw-r--r--   0        0        0    11188 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_to_json.py
+-rw-r--r--   0        0        0     9890 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_to_layout.py
+-rw-r--r--   0        0        0     2730 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_to_list.py
+-rw-r--r--   0        0        0     2151 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_to_numpy.py
+-rw-r--r--   0        0        0     3524 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_to_packed.py
+-rw-r--r--   0        0        0    21056 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_to_parquet.py
+-rw-r--r--   0        0        0     4321 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_to_parquet_dataset.py
+-rw-r--r--   0        0        0    11618 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_to_parquet_row_groups.py
+-rw-r--r--   0        0        0     3019 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_to_rdataframe.py
+-rw-r--r--   0        0        0     3493 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_to_regular.py
+-rw-r--r--   0        0        0    25148 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_transform.py
+-rw-r--r--   0        0        0     4701 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_type.py
+-rw-r--r--   0        0        0    11324 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_unflatten.py
+-rw-r--r--   0        0        0     2571 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_unzip.py
+-rw-r--r--   0        0        0     1188 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_validity_error.py
+-rw-r--r--   0        0        0     2707 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_values_astype.py
+-rw-r--r--   0        0        0    10073 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_var.py
+-rw-r--r--   0        0        0     5113 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_where.py
+-rw-r--r--   0        0        0     6051 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_with_field.py
+-rw-r--r--   0        0        0     2348 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_with_name.py
+-rw-r--r--   0        0        0     1795 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_with_parameter.py
+-rw-r--r--   0        0        0     3783 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_without_field.py
+-rw-r--r--   0        0        0     1571 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_without_parameters.py
+-rw-r--r--   0        0        0     2202 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_zeros_like.py
+-rw-r--r--   0        0        0     8832 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/ak_zip.py
+-rw-r--r--   0        0        0    12436 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/__init__.py
+-rw-r--r--   0        0        0     2163 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_capitalize.py
+-rw-r--r--   0        0        0     2423 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_center.py
+-rw-r--r--   0        0        0     2483 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_count_substring.py
+-rw-r--r--   0        0        0     2555 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_count_substring_regex.py
+-rw-r--r--   0        0        0     2397 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_ends_with.py
+-rw-r--r--   0        0        0     3011 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_extract_regex.py
+-rw-r--r--   0        0        0     2478 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_find_substring.py
+-rw-r--r--   0        0        0     2538 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_find_substring_regex.py
+-rw-r--r--   0        0        0     3202 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_index_in.py
+-rw-r--r--   0        0        0     2141 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_is_alnum.py
+-rw-r--r--   0        0        0     2137 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_is_alpha.py
+-rw-r--r--   0        0        0     2090 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_is_ascii.py
+-rw-r--r--   0        0        0     2147 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_is_decimal.py
+-rw-r--r--   0        0        0     2171 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_is_digit.py
+-rw-r--r--   0        0        0     2989 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_is_in.py
+-rw-r--r--   0        0        0     2135 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_is_lower.py
+-rw-r--r--   0        0        0     2213 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_is_numeric.py
+-rw-r--r--   0        0        0     2167 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_is_printable.py
+-rw-r--r--   0        0        0     2137 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_is_space.py
+-rw-r--r--   0        0        0     2373 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_is_title.py
+-rw-r--r--   0        0        0     2264 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_is_upper.py
+-rw-r--r--   0        0        0     4631 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_join.py
+-rw-r--r--   0        0        0     2612 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_join_element_wise.py
+-rw-r--r--   0        0        0     2002 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_length.py
+-rw-r--r--   0        0        0     2032 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_lower.py
+-rw-r--r--   0        0        0     2414 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_lpad.py
+-rw-r--r--   0        0        0     2304 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_ltrim.py
+-rw-r--r--   0        0        0     2039 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_ltrim_whitespace.py
+-rw-r--r--   0        0        0     2571 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_match_like.py
+-rw-r--r--   0        0        0     2363 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_match_substring.py
+-rw-r--r--   0        0        0     2395 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_match_substring_regex.py
+-rw-r--r--   0        0        0     3708 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_repeat.py
+-rw-r--r--   0        0        0     2610 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_replace_slice.py
+-rw-r--r--   0        0        0     2761 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_replace_substring.py
+-rw-r--r--   0        0        0     2829 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_replace_substring_regex.py
+-rw-r--r--   0        0        0     2145 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_reverse.py
+-rw-r--r--   0        0        0     2415 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_rpad.py
+-rw-r--r--   0        0        0     2293 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_rtrim.py
+-rw-r--r--   0        0        0     2040 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_rtrim_whitespace.py
+-rw-r--r--   0        0        0     2931 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_slice.py
+-rw-r--r--   0        0        0     2684 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_split_pattern.py
+-rw-r--r--   0        0        0     2820 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_split_pattern_regex.py
+-rw-r--r--   0        0        0     3108 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_split_whitespace.py
+-rw-r--r--   0        0        0     2427 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_starts_with.py
+-rw-r--r--   0        0        0     2142 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_swapcase.py
+-rw-r--r--   0        0        0     2266 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_title.py
+-rw-r--r--   0        0        0     2883 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_to_categorical.py
+-rw-r--r--   0        0        0     2307 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_trim.py
+-rw-r--r--   0        0        0     2021 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_trim_whitespace.py
+-rw-r--r--   0        0        0     2038 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/operations/str/akstr_upper.py
+-rw-r--r--   0        0        0      739 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/types/__init__.py
+-rw-r--r--   0        0        0   163323 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/types/_awkward_datashape_parser.py
+-rw-r--r--   0        0        0     2340 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/types/arraytype.py
+-rw-r--r--   0        0        0     3119 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/types/listtype.py
+-rw-r--r--   0        0        0     6316 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/types/numpytype.py
+-rw-r--r--   0        0        0     4161 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/types/optiontype.py
+-rw-r--r--   0        0        0     9689 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/types/recordtype.py
+-rw-r--r--   0        0        0     4052 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/types/regulartype.py
+-rw-r--r--   0        0        0     1505 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/types/scalartype.py
+-rw-r--r--   0        0        0    10210 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/types/type.py
+-rw-r--r--   0        0        0     4210 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/types/uniontype.py
+-rw-r--r--   0        0        0     1390 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/src/awkward/types/unknowntype.py
+-rw-r--r--   0        0        0       84 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/__init__.py
+-rw-r--r--   0        0        0     3427 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0002_minimal_listarray.py
+-rw-r--r--   0        0        0      520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0006_deep_iteration.py
+-rw-r--r--   0        0        0     5597 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0008_slices_and_getitem.py
+-rw-r--r--   0        0        0    13410 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0011_listarray.py
+-rw-r--r--   0        0        0     4494 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0013_error_handling_struct.py
+-rw-r--r--   0        0        0    16859 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0014_finish_up_getitem.py
+-rw-r--r--   0        0        0     5201 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0018_fromiter_fillable.py
+-rw-r--r--   0        0        0     9804 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0019_use_json_library.py
+-rw-r--r--   0        0        0    13719 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0020_support_unsigned_indexes.py
+-rw-r--r--   0        0        0     6423 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0021_emptyarray.py
+-rw-r--r--   0        0        0    10727 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0023_regular_array.py
+-rw-r--r--   0        0        0     4922 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0024_use_regular_array.py
+-rw-r--r--   0        0        0    25613 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0025_record_array.py
+-rw-r--r--   0        0        0     3753 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0028_add_dressed_types.py
+-rw-r--r--   0        0        0     5828 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0032_replace_dressedtype.py
+-rw-r--r--   0        0        0    12059 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0046_start_indexedarray.py
+-rw-r--r--   0        0        0      930 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0049_distinguish_record_and_recordarray_behaviors.py
+-rw-r--r--   0        0        0    12247 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0057_introducing_forms.py
+-rw-r--r--   0        0        0     5462 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0070_argmin_and_argmax.py
+-rw-r--r--   0        0        0     5416 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0072_fillna_operation.py
+-rw-r--r--   0        0        0    15726 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0074_argsort_and_sort.py
+-rw-r--r--   0        0        0     2868 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0077_zip_operation.py
+-rw-r--r--   0        0        0    11966 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0078_argcross_and_cross.py
+-rw-r--r--   0        0        0    12156 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0079_argchoose_and_choose.py
+-rw-r--r--   0        0        0     7028 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0080_flatpandas_multiindex_rows_and_columns.py
+-rw-r--r--   0        0        0     6651 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0084_start_unionarray.py
+-rw-r--r--   0        0        0     6583 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0086_nep13_ufunc.py
+-rw-r--r--   0        0        0    12209 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0089_numpy_functions.py
+-rw-r--r--   0        0        0    46754 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0093_simplify_uniontypes_and_optiontypes.py
+-rw-r--r--   0        0        0     6991 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0107_assign_fields_to_records.py
+-rw-r--r--   0        0        0    46691 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0111_jagged_and_masked_getitem.py
+-rw-r--r--   0        0        0    77548 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0115_generic_reducer_operation.py
+-rw-r--r--   0        0        0    35194 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0118_numba_cpointers.py
+-rw-r--r--   0        0        0     1123 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0119_numexpr_and_broadcast_arrays.py
+-rw-r--r--   0        0        0     1138 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0124_strings_in_numba.py
+-rw-r--r--   0        0        0    32146 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0127_tomask_operation.py
+-rw-r--r--   0        0        0     3715 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0127b_tomask_operation_numba.py
+-rw-r--r--   0        0        0      870 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0138_emptyarray_type.py
+-rw-r--r--   0        0        0    17955 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0150_flatten.py
+-rw-r--r--   0        0        0     3634 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0163_negative_axis_wrap.py
+-rw-r--r--   0        0        0     9811 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0166_0167_0170_random_issues.py
+-rw-r--r--   0        0        0     4584 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0173_astype_operation.py
+-rw-r--r--   0        0        0    24070 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0184_concatenate_operation.py
+-rw-r--r--   0        0        0     2095 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0193_is_none_axis_parameter.py
+-rw-r--r--   0        0        0     3384 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0198_tutorial_documentation_1.py
+-rw-r--r--   0        0        0     9030 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0222_count_with_axis0.py
+-rw-r--r--   0        0        0    75637 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0224_arrow_to_awkward.py
+-rw-r--r--   0        0        0      613 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0264_reduce_last_empty.py
+-rw-r--r--   0        0        0     3283 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0273_path_for_with_field.py
+-rw-r--r--   0        0        0      775 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0286_broadcast_single_value_with_field.py
+-rw-r--r--   0        0        0     2237 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0290_bug_fixes_for_hats.py
+-rw-r--r--   0        0        0     4838 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0315_integerindex.py
+-rw-r--r--   0        0        0     5777 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0331_pandas_indexedarray.py
+-rw-r--r--   0        0        0     1289 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0334_fully_broadcastable_where.py
+-rw-r--r--   0        0        0      598 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0339_highlevel_sorting_function.py
+-rw-r--r--   0        0        0     6789 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0348_form_keys.py
+-rw-r--r--   0        0        0     4554 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0355_mixins.py
+-rw-r--r--   0        0        0    10428 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0395_complex_type_arrays.py
+-rw-r--r--   0        0        0     4966 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0395_fix_numba_indexedarray.py
+-rw-r--r--   0        0        0     3244 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0397_arrays_as_constants_in_numba.py
+-rw-r--r--   0        0        0     6987 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0401_add_categorical_type_for_arrow_dictionary.py
+-rw-r--r--   0        0        0    22496 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0404_array_validity_check.py
+-rw-r--r--   0        0        0    14314 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0410_fix_argminmax_positions_for_missing_values.py
+-rw-r--r--   0        0        0    17487 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0437_stream_of_many_json_files.py
+-rw-r--r--   0        0        0    32953 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0447_preserve_regularness_in_reduce.py
+-rw-r--r--   0        0        0    27090 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0449_merge_many_arrays_in_one_pass.py
+-rw-r--r--   0        0        0     4091 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0493_zeros_ones_full_like.py
+-rw-r--r--   0        0        0     1638 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0496_provide_local_index.py
+-rw-r--r--   0        0        0     2091 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0499_getitem_indexedarray_bug.py
+-rw-r--r--   0        0        0     1319 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0504_block_ufuncs_for_strings.py
+-rw-r--r--   0        0        0     2958 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0511_copy_and_deepcopy.py
+-rw-r--r--   0        0        0     9179 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py
+-rw-r--r--   0        0        0      397 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0546_fill_none_replacement_value_type.py
+-rw-r--r--   0        0        0     1134 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0549_numba_array_asarray.py
+-rw-r--r--   0        0        0     4300 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0557_min_max_initial_argument.py
+-rw-r--r--   0        0        0      569 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0559_fix_booleans_in_numba.py
+-rw-r--r--   0        0        0      668 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0572_numba_array_ndim.py
+-rw-r--r--   0        0        0     4933 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0582_propagate_context_in_broadcast_and_apply.py
+-rw-r--r--   0        0        0     1131 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0583_implement_unflatten_function.py
+-rw-r--r--   0        0        0     3116 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0590_allow_regulararray_size_zero.py
+-rw-r--r--   0        0        0     5976 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py
+-rw-r--r--   0        0        0      510 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0627_behavior_from_dict_of_arrays.py
+-rw-r--r--   0        0        0     8237 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0652_tests_of_complex_numbers.py
+-rw-r--r--   0        0        0     2342 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0674_categorical_validation.py
+-rw-r--r--   0        0        0      782 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0713_getitem_field_should_simplify_optiontype.py
+-rw-r--r--   0        0        0     1274 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py
+-rw-r--r--   0        0        0     1087 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0730_unflatten_axis_parameter.py
+-rw-r--r--   0        0        0     2601 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0733_run_lengths.py
+-rw-r--r--   0        0        0     2159 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0736_implement_argsort_for_strings.py
+-rw-r--r--   0        0        0      362 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0758_ak_zip_scallars.py
+-rw-r--r--   0        0        0     1154 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0766_prevent_combinations_of_characters.py
+-rw-r--r--   0        0        0    25871 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0773_typeparser.py
+-rw-r--r--   0        0        0      811 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0788_indexedarray_carrying_recordarray_parameters.py
+-rw-r--r--   0        0        0      903 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0794_ak_cartesian_on_empty_array.py
+-rw-r--r--   0        0        0     1180 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0803_argsort_fix_type.py
+-rw-r--r--   0        0        0     1396 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0806_empty_lists_cartesian_fix.py
+-rw-r--r--   0        0        0     6343 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0813_full_like_dtype_arg.py
+-rw-r--r--   0        0        0     1693 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0815_broadcast_union_types_to_all_possibilities.py
+-rw-r--r--   0        0        0      520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0819_issue.py
+-rw-r--r--   0        0        0      714 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0828_arrow_datatype_null.py
+-rw-r--r--   0        0        0    23641 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0835_datetime_type.py
+-rw-r--r--   0        0        0      708 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0835_datetime_type_pandas.py
+-rw-r--r--   0        0        0     4694 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0835_datetime_type_pyarrow.py
+-rw-r--r--   0        0        0      712 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0850_argsort_mask_array.py
+-rw-r--r--   0        0        0      481 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0863_is_none_numpy_array.py
+-rw-r--r--   0        0        0     1061 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0866_getitem_field_and_flatten_unions.py
+-rw-r--r--   0        0        0      961 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0875_arrow_null_type.py
+-rw-r--r--   0        0        0      933 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0879_non_primitive_with_field.py
+-rw-r--r--   0        0        0      595 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0884_index_and_identifier_refactoring.py
+-rw-r--r--   0        0        0     1118 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0889_ptp.py
+-rw-r--r--   0        0        0    53387 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0896_content_classes_refactoring.py
+-rw-r--r--   0        0        0     1783 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0898_unzip_heterogeneous_records.py
+-rw-r--r--   0        0        0      453 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0903_ArrayView_expects_contiguous_NumpyArrays.py
+-rw-r--r--   0        0        0      562 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0905_leading_zeros_in_unflatten.py
+-rw-r--r--   0        0        0     1080 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0906_arrow_fixed_size_list_type.py
+-rw-r--r--   0        0        0      698 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0910_unflatten_counts_relation.py
+-rw-r--r--   0        0        0     5293 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0912_packed.py
+-rw-r--r--   0        0        0   108025 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0914_types_and_forms.py
+-rw-r--r--   0        0        0     1909 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0916_datetime_values_astype.py
+-rw-r--r--   0        0        0     5554 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0927_numpy_array_nbytes.py
+-rw-r--r--   0        0        0      741 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0930_bug_in_unionarray_purelist_parameter.py
+-rw-r--r--   0        0        0     1659 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0945_argsort_sort_nan_array.py
+-rw-r--r--   0        0        0    28060 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0958_new_forms_must_accept_old_form_json.py
+-rw-r--r--   0        0        0    28316 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0959__getitem_array_implementation.py
+-rw-r--r--   0        0        0      683 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0975_mask_multidimensional_numpy_array.py
+-rw-r--r--   0        0        0      676 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0979_where_multidimentional_numpy_array.py
+-rw-r--r--   0        0        0     5835 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0982_missing_case_in_nonlocal_reducers.py
+-rw-r--r--   0        0        0     2008 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0984_ravel.py
+-rw-r--r--   0        0        0     1838 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_0992_correct_ptp_unmasking.py
+-rw-r--r--   0        0        0     2132 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py
+-rw-r--r--   0        0        0      461 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1006_packed_regular_array_zero_size.py
+-rw-r--r--   0        0        0      448 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1007_from_buffers_empty_ndarray.py
+-rw-r--r--   0        0        0      583 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1017_numpyarray_broadcast.py
+-rw-r--r--   0        0        0      817 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1030_mixin_class_name.py
+-rw-r--r--   0        0        0    52146 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1031_start_getitem_next.py
+-rw-r--r--   0        0        0    18039 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1031b_start_getitem_next_specialized.py
+-rw-r--r--   0        0        0     1178 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1049_concatenate_single_array.py
+-rw-r--r--   0        0        0     1591 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1055_fill_none_numpy_dimension.py
+-rw-r--r--   0        0        0    42282 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1059_localindex.py
+-rw-r--r--   0        0        0      583 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1066_to_numpy_masked_structured_array.py
+-rw-r--r--   0        0        0      717 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1071_mask_identity_false_should_not_return_option_type.py
+-rw-r--r--   0        0        0    27770 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1072_sort.py
+-rw-r--r--   0        0        0    44172 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1074_combinations.py
+-rw-r--r--   0        0        0     5213 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1075_validityerror.py
+-rw-r--r--   0        0        0      305 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1106_argminmax_axis_None_missing_values.py
+-rw-r--r--   0        0        0    25563 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1110_type_tracer_1.py
+-rw-r--r--   0        0        0     1902 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1116_project_maskedarrays.py
+-rw-r--r--   0        0        0    28382 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1125_to_arrow_from_arrow.py
+-rw-r--r--   0        0        0     6308 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1132_utility_methods_for_highlevel_functions.py
+-rw-r--r--   0        0        0    21130 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1134_from_buffers_to_buffers.py
+-rw-r--r--   0        0        0    57354 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1135_rpad_operation.py
+-rw-r--r--   0        0        0     4671 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1136_regulararray_zeros_in_shape.py
+-rw-r--r--   0        0        0    10519 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1137_num.py
+-rw-r--r--   0        0        0    10576 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1142_numbers_to_type.py
+-rw-r--r--   0        0        0     2591 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1149_datetime_sort.py
+-rw-r--r--   0        0        0      662 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1154_arrow_tables_should_preserve_parameters.py
+-rw-r--r--   0        0        0    32589 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1162_ak_from_json_schema.py
+-rw-r--r--   0        0        0      798 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1183_bugs_found_by_dask_project_2.py
+-rw-r--r--   0        0        0     1318 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1189_fix_singletons_for_non_optional_data.py
+-rw-r--r--   0        0        0      583 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1192_iterables_in___array_function__.py
+-rw-r--r--   0        0        0      640 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1193_is_none_nested_option.py
+-rw-r--r--   0        0        0     2633 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1233_ak_with_name.py
+-rw-r--r--   0        0        0    26572 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1240_v2_implementation_of_numba_1.py
+-rw-r--r--   0        0        0     1178 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1259_simplify_optiontype.py
+-rw-r--r--   0        0        0     1592 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1260_simplify_masked_option_types.py
+-rw-r--r--   0        0        0      713 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1271_fix_4D_reducers.py
+-rw-r--r--   0        0        0    33099 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1294_to_and_from_parquet.py
+-rw-r--r--   0        0        0     1977 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py
+-rw-r--r--   0        0        0    62372 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1300_awkward_to_cpp_converter_with_cling.py
+-rw-r--r--   0        0        0    39506 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1300b_same_for_numba.py
+-rw-r--r--   0        0        0      399 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1305_mixed_awkward_numpy_slicing.py
+-rw-r--r--   0        0        0     1734 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1308_zip_after_option.py
+-rw-r--r--   0        0        0     1736 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1318_array_function_types.py
+-rw-r--r--   0        0        0     1762 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1320_mask_identity_defaults.py
+-rw-r--r--   0        0        0      679 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1344_broadcast_arrays_depth_limit.py
+-rw-r--r--   0        0        0     6653 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1345_avro_reader.py
+-rw-r--r--   0        0        0     4594 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1351_is_tuple.py
+-rw-r--r--   0        0        0     8394 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1374_to_rdataframe.py
+-rw-r--r--   0        0        0     1787 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1377_ravel_string.py
+-rw-r--r--   0        0        0     1500 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1379_reducers_with_axis_None_and_typetracers.py
+-rw-r--r--   0        0        0     1416 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1399_from_jax.py
+-rw-r--r--   0        0        0     1259 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1399_to_jax.py
+-rw-r--r--   0        0        0      329 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1400_with_name_record.py
+-rw-r--r--   0        0        0      481 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1403_from_numpy_strings.py
+-rw-r--r--   0        0        0     3502 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1405_slicing_untested_cases.py
+-rw-r--r--   0        0        0     7211 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1415_behaviour_forwarding.py
+-rw-r--r--   0        0        0    18745 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1440_start_v2_to_parquet.py
+-rw-r--r--   0        0        0    14434 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1447_jax_autodiff_slices_ufuncs.py
+-rw-r--r--   0        0        0     8623 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1449_v2_to_json_from_json_functions.py
+-rw-r--r--   0        0        0      694 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1453_write_single_records_to_parquet.py
+-rw-r--r--   0        0        0     9860 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1473_from_rdataframe.py
+-rw-r--r--   0        0        0    24680 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1477_generator_entry_type_as_rvec.py
+-rw-r--r--   0        0        0     3611 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1490_jax_reducers_combinations.py
+-rw-r--r--   0        0        0     3937 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1502_getitem_jagged_issue1406.py
+-rw-r--r--   0        0        0     1853 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1504_typetracer_like.py
+-rw-r--r--   0        0        0     4945 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1508_awkward_from_rdataframe.py
+-rw-r--r--   0        0        0     2218 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1511_set_attribute.py
+-rw-r--r--   0        0        0      786 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1539_isnone_axis_check_issue1417.py
+-rw-r--r--   0        0        0     1602 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1559_fix_ufuncs_records_1439.py
+-rw-r--r--   0        0        0     1039 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1565_axis_wrap_if_negative_record.py
+-rw-r--r--   0        0        0     1117 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1567_fix_longlong_in_Index.py
+-rw-r--r--   0        0        0     3054 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1568_fix_lengths_empty_regular_slices.py
+-rw-r--r--   0        0        0      417 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1578_to_arrow_empty_recordarray.py
+-rw-r--r--   0        0        0     5943 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1586_concatenate_should_preserve_regulararray.py
+-rw-r--r--   0        0        0      337 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1593_empty_slice_list_record.py
+-rw-r--r--   0        0        0     7292 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1604_preserve_form_in_concatenate.py
+-rw-r--r--   0        0        0     4404 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1607_no_reducers_on_records.py
+-rw-r--r--   0        0        0    10067 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1613_generator_tolayout_records.py
+-rw-r--r--   0        0        0      759 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1619_from_parquet_empty_field.py
+-rw-r--r--   0        0        0     6056 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1620_layout_builders.py
+-rw-r--r--   0        0        0     8154 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1625_multiple_columns_from_rdataframe.py
+-rw-r--r--   0        0        0      802 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1642_from_iter_of_tuples.py
+-rw-r--r--   0        0        0      421 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1644_concatenate_zeros_length.py
+-rw-r--r--   0        0        0     4349 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1650_Record_to_list_should_listify_itself.py
+-rw-r--r--   0        0        0     1053 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1671_categorical_type.py
+-rw-r--r--   0        0        0    11791 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1672_broadcast_parameters.py
+-rw-r--r--   0        0        0     4485 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1677_array_builder_in_numba.py
+-rw-r--r--   0        0        0      576 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1685_IndexedArray_project_parameters.py
+-rw-r--r--   0        0        0      810 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1686_UnionArray_simplified_preserve_parameters.py
+-rw-r--r--   0        0        0      994 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1688_pack_categorical.py
+-rw-r--r--   0        0        0      557 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1703_fill_none_typetracer.py
+-rw-r--r--   0        0        0     1775 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1707_broadcast_parameters_ufunc.py
+-rw-r--r--   0        0        0      541 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1709_ak_array_constructor_behavior.py
+-rw-r--r--   0        0        0      430 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1735_from_numpy_mask.py
+-rw-r--r--   0        0        0      609 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1747_bytemaskedarray_mergemany.py
+-rw-r--r--   0        0        0      856 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1753_indexedarray_merge_kernel.py
+-rw-r--r--   0        0        0     1509 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1762_jax_behavior_support.py
+-rw-r--r--   0        0        0      621 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1764_jax_jacobian.py
+-rw-r--r--   0        0        0      994 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1765_add_ioanas_test_of_to_arraylib.py
+-rw-r--r--   0        0        0     4822 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1766_record_form_fields.py
+-rw-r--r--   0        0        0     2937 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1781_rdataframe_snapshot.py
+-rw-r--r--   0        0        0      733 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1784_reduce_leading_sublist.py
+-rw-r--r--   0        0        0      599 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1790_reduce_regulararray.py
+-rw-r--r--   0        0        0     4223 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1791_reduce_trailing_sublist.py
+-rw-r--r--   0        0        0     1059 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1794_run_lengths_empty_sublist.py
+-rw-r--r--   0        0        0      439 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1823_fill_none_axis_none.py
+-rw-r--r--   0        0        0      513 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1826_ravel_preserve_none.py
+-rw-r--r--   0        0        0     1483 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1829_to_from_rdataframe_bool.py
+-rw-r--r--   0        0        0      620 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py
+-rw-r--r--   0        0        0     1129 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1847_numpy_array_contiguous.py
+-rw-r--r--   0        0        0      765 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1850_bytemasked_array_to_bytemaskedarray.py
+-rw-r--r--   0        0        0     1672 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1867_pass_behavior_through_combinations.py
+-rw-r--r--   0        0        0    17271 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1904_drop_none.py
+-rw-r--r--   0        0        0     3585 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1914_improved_axis_to_posaxis.py
+-rw-r--r--   0        0        0     4639 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py
+-rw-r--r--   0        0        0      953 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1930_unflatten_counts_checks.py
+-rw-r--r--   0        0        0      801 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1936_with_field_broadcasting.py
+-rw-r--r--   0        0        0      583 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1940_ak_backend.py
+-rw-r--r--   0        0        0     1489 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1943_regular_indexing.py
+-rw-r--r--   0        0        0      220 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1944_to_numpy_empty_record_array.py
+-rw-r--r--   0        0        0     1163 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1960_awkward_from_rdataframe.py
+-rw-r--r--   0        0        0     3319 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1961_ak_without_field.py
+-rw-r--r--   0        0        0      312 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1978_akRecord_constructor_should_retain_type.py
+-rw-r--r--   0        0        0      381 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_1991_missed_a_NumpyArray_raw_call_without_underscore.py
+-rw-r--r--   0        0        0      403 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2008_ak_type_layout.py
+-rw-r--r--   0        0        0    10254 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2020_reduce_axis_none.py
+-rw-r--r--   0        0        0      835 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2021_check_TypeTracerArray_in_ak_where.py
+-rw-r--r--   0        0        0      677 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2023_from_rdataframe.py
+-rw-r--r--   0        0        0     2938 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py
+-rw-r--r--   0        0        0     1251 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2047_ak_transform_regular_to_jagged.py
+-rw-r--r--   0        0        0      527 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2051_arraybuilder_behavior_propagation.py
+-rw-r--r--   0        0        0     1307 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2055_array_builder_check.py
+-rw-r--r--   0        0        0     1691 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2058_merge_numpy_array.py
+-rw-r--r--   0        0        0      740 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2064_fill_none_record.py
+-rw-r--r--   0        0        0      831 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2067_to_buffers_byteorder.py
+-rw-r--r--   0        0        0      806 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2070_to_layout_string.py
+-rw-r--r--   0        0        0     1230 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2071_unflatten_non_packed_counts.py
+-rw-r--r--   0        0        0      323 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2076_ak_unzip_record.py
+-rw-r--r--   0        0        0      577 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2078_array_function_wrap.py
+-rw-r--r--   0        0        0      621 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2082_broadcast_zero_size.py
+-rw-r--r--   0        0        0     1763 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2085_empty_if_typetracer.py
+-rw-r--r--   0        0        0     2614 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2096_ak_scalar_type.py
+-rw-r--r--   0        0        0     1009 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2101_pickle_behavior_class.py
+-rw-r--r--   0        0        0      551 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2104_numpy_merge_option.py
+-rw-r--r--   0        0        0     2748 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2106_pickle_class.py
+-rw-r--r--   0        0        0      954 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2108_fill_none_indexed.py
+-rw-r--r--   0        0        0     2132 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2115_fix_up_typetracers.py
+-rw-r--r--   0        0        0      516 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2120_missing_field_error.py
+-rw-r--r--   0        0        0     1066 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2125_type_of_scalar.py
+-rw-r--r--   0        0        0     1925 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2150_typetracer_high_level_ufunc.py
+-rw-r--r--   0        0        0     1930 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2179_parameter_merging_rules.py
+-rw-r--r--   0        0        0      332 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2181_with_name_len.py
+-rw-r--r--   0        0        0     2989 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2185_merge_union_of_records.py
+-rw-r--r--   0        0        0      560 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py
+-rw-r--r--   0        0        0     7333 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2192_union_absorb_indexed.py
+-rw-r--r--   0        0        0     6087 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2198_almost_equal.py
+-rw-r--r--   0        0        0     1284 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2202_filter_multiple_columns_from_rdataframe.py
+-rw-r--r--   0        0        0     1485 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2214_offset_bool_index.py
+-rw-r--r--   0        0        0      366 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2219_flatten_empty.py
+-rw-r--r--   0        0        0      695 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2226_slice_regulararray_typetracer.py
+-rw-r--r--   0        0        0     1760 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2229_getitem_range_slice.py
+-rw-r--r--   0        0        0     4035 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2234_from_rdataframe_keep_order.py
+-rw-r--r--   0        0        0     4136 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2236_merge_union_of_records_option.py
+-rw-r--r--   0        0        0      517 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2240_merge_union_parameters.py
+-rw-r--r--   0        0        0     1369 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2240_simplify_merge_as_union.py
+-rw-r--r--   0        0        0      544 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2246_slice_not_packed.py
+-rw-r--r--   0        0        0      765 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2250_full_like_bool.py
+-rw-r--r--   0        0        0     1867 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2258_from_rdataframe_with_arguments.py
+-rw-r--r--   0        0        0      524 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2259_run_lengths_typetracer.py
+-rw-r--r--   0        0        0      592 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2263_to_packed_list.py
+-rw-r--r--   0        0        0      347 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2266_fix_nan_to_num.py
+-rw-r--r--   0        0        0      941 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2267_broadcast_fields.py
+-rw-r--r--   0        0        0     1368 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2293_unflatten_typetracer.py
+-rw-r--r--   0        0        0      438 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2294_view_unknown_scalar.py
+-rw-r--r--   0        0        0      752 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2296_duplicate_field.py
+-rw-r--r--   0        0        0     2294 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2297_common_backend.py
+-rw-r--r--   0        0        0      487 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2304_index_typetracer.py
+-rw-r--r--   0        0        0      680 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2305_nep_18_lazy_conversion.py
+-rw-r--r--   0        0        0     2895 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2306_cppyy_jit.py
+-rw-r--r--   0        0        0     4418 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2319_from_buffers_array.py
+-rw-r--r--   0        0        0      753 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2327_array_interface.py
+-rw-r--r--   0        0        0     1760 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2329_cartesian_broadcasting_fixes.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2346_broadcast_depth_limit.py
+-rw-r--r--   0        0        0    15641 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2349_growablebuffer_in_numba.py
+-rw-r--r--   0        0        0      650 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2354_ufunc_same_backend.py
+-rw-r--r--   0        0        0      679 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2355_to_backend_record.py
+-rw-r--r--   0        0        0     1467 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2361_typetracer_asarray_nd.py
+-rw-r--r--   0        0        0      966 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2364_empty_list_of_string.py
+-rw-r--r--   0        0        0    37032 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2365_enforce_type.py
+-rw-r--r--   0        0        0     2956 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2368_type_is_equal.py
+-rw-r--r--   0        0        0     5376 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2373_unzip_touching.py
+-rw-r--r--   0        0        0     5984 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2374_cartesian_touching.py
+-rw-r--r--   0        0        0     1069 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2385_with_field_empty_record.py
+-rw-r--r--   0        0        0      988 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2395_copy_asarray_touch.py
+-rw-r--r--   0        0        0      244 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2407_broadcast_no_arrays.py
+-rw-r--r--   0        0        0    34537 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2408_layoutbuilder_in_numba.py
+-rw-r--r--   0        0        0      885 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2410_string_broadcast.py
+-rw-r--r--   0        0        0      832 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2411_cartesian_axis_validation.py
+-rw-r--r--   0        0        0      736 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2417_bytemasked_singletons.py
+-rw-r--r--   0        0        0      382 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2418_union_broadcast_unknown.py
+-rw-r--r--   0        0        0     1595 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2424_almost_equal_union_record.py
+-rw-r--r--   0        0        0     1254 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2425_forms_from_type.py
+-rw-r--r--   0        0        0      577 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2426_is_equal_to.py
+-rw-r--r--   0        0        0      616 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2444_minimal_listarray.py
+-rw-r--r--   0        0        0      889 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2471_flatten_string.py
+-rw-r--r--   0        0        0     1063 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2484_reduce_starts_empty.py
+-rw-r--r--   0        0        0      691 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2487_broadcast_list_offsets.py
+-rw-r--r--   0        0        0     1351 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2490_reduce_regulararray_positional.py
+-rw-r--r--   0        0        0     1848 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2495_concatenate_typetracer.py
+-rw-r--r--   0        0        0     3832 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2501_positional_record_reducer.py
+-rw-r--r--   0        0        0      293 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2503_deprecate_to_numpyform.py
+-rw-r--r--   0        0        0     4974 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2512_record_array_carry.py
+-rw-r--r--   0        0        0      329 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2518_datetime_units_as_parameter.py
+-rw-r--r--   0        0        0     5978 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2536_select_columns.py
+-rw-r--r--   0        0        0      767 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2548_record_form_fields.py
+-rw-r--r--   0        0        0     3661 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2549_list_nominal_type.py
+-rw-r--r--   0        0        0      702 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2550_validity_error_recursive.py
+-rw-r--r--   0        0        0      470 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2556_jax_tracer_error.py
+-rw-r--r--   0        0        0      475 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2560_minimal_listarray.py
+-rw-r--r--   0        0        0     1483 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2564_string_broadcast_regular.py
+-rw-r--r--   0        0        0      922 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2571_awkward_ListOffsetArray_reduce_local_nextparents_64.py
+-rw-r--r--   0        0        0      357 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2591_nan_to_num.py
+-rw-r--r--   0        0        0     2459 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2595_transform_termination.py
+-rw-r--r--   0        0        0      856 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2603_custom_behaviors_with_jax.py
+-rw-r--r--   0        0        0     3565 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2604_read_awkward1_pickles.py
+-rw-r--r--   0        0        0    65992 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2616_use_pyarrow_for_strings.py
+-rw-r--r--   0        0        0     1993 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2623_optiontype_outside_record_strings.py
+-rw-r--r--   0        0        0     5330 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2630_akstr_to_categorical.py
+-rw-r--r--   0        0        0      734 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2631_vectorised_to_numpy_strings.py
+-rw-r--r--   0        0        0      437 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2632_unflatten_length.py
+-rw-r--r--   0        0        0      580 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2634_listarray_pad_none.py
+-rw-r--r--   0        0        0      961 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2637_jax_tracer_error.py
+-rw-r--r--   0        0        0      874 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2638_mean_and_count_grads.py
+-rw-r--r--   0        0        0      657 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2646_from_parquet_highlevel.py
+-rw-r--r--   0        0        0     1732 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2649_dlpack_support.py
+-rw-r--r--   0        0        0     1424 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2650_arrow_array_highlevel.py
+-rw-r--r--   0        0        0      594 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2651_parameter_union.py
+-rw-r--r--   0        0        0     1389 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2653_slice_listoffsetarray.py
+-rw-r--r--   0        0        0      476 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2654_divmod.py
+-rw-r--r--   0        0        0     3772 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2656_unflatten_axis_typetracer.py
+-rw-r--r--   0        0        0    24851 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2660_expected_container_keys_from_form.py
+-rw-r--r--   0        0        0     1949 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2663_broadcast_tuples.py
+-rw-r--r--   0        0        0     1765 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2665_out_of_band_pickle.py
+-rw-r--r--   0        0        0     4036 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2671_typetracer_with_report_deprecated_length.py
+-rw-r--r--   0        0        0     1723 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2672_touch_data.py
+-rw-r--r--   0        0        0      524 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2678_same_backend.py
+-rw-r--r--   0        0        0     3104 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2682_custom_pickler.py
+-rw-r--r--   0        0        0     1103 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2683_to_and_from_feather.py
+-rw-r--r--   0        0        0     1013 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2693_to_buffers_placeholders.py
+-rw-r--r--   0        0        0      301 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2710_pickle_unknown_length.py
+-rw-r--r--   0        0        0     3973 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2713_from_buffers_allow_noncanonical.py
+-rw-r--r--   0        0        0    17061 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2714_from_buffers_placeholders.py
+-rw-r--r--   0        0        0     1157 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2718_frombuffer_typetracer.py
+-rw-r--r--   0        0        0     1372 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2719_typetracer_buffer_key.py
+-rw-r--r--   0        0        0      873 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2724_expected_from_buffers_recursive.py
+-rw-r--r--   0        0        0      851 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2727_remove_structure_regular.py
+-rw-r--r--   0        0        0     4031 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2754_highlevel_behavior_missing.py
+-rw-r--r--   0        0        0     9111 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2757_attrs_metadata.py
+-rw-r--r--   0        0        0     1384 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2759_update_class_consistently.py
+-rw-r--r--   0        0        0     3649 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2763_to_layout_granularity.py
+-rw-r--r--   0        0        0      427 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2765_slice_from_typetracer.py
+-rw-r--r--   0        0        0     1573 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2769_argsort_all_none.py
+-rw-r--r--   0        0        0     1070 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2770_serialize_and_deserialize_behaviour_for_numba.py
+-rw-r--r--   0        0        0      574 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2785_ak_num_typetracer_axis_0.py
+-rw-r--r--   0        0        0     1776 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2793_nep_50_gradual_support.py
+-rw-r--r--   0        0        0     1744 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2799_numba_ufunc_resolution.py
+-rw-r--r--   0        0        0     4607 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2803_string_formatter.py
+-rw-r--r--   0        0        0     1347 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2806_attrs_typetracer.py
+-rw-r--r--   0        0        0     1160 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2808_dtype_ufunc_bool.py
+-rw-r--r--   0        0        0      471 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2815_return_scalar_firsts.py
+-rw-r--r--   0        0        0      478 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2816_public_typetracer_api.py
+-rw-r--r--   0        0        0      789 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2837_ufunc_attrs_behavior.py
+-rw-r--r--   0        0        0      922 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2857_full_like_scalar.py
+-rw-r--r--   0        0        0     4080 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2860_enforce_concatenated_form.py
+-rw-r--r--   0        0        0      798 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2866_getitem_attrs.py
+-rw-r--r--   0        0        0     1382 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2889_test_chunked_array.py
+-rw-r--r--   0        0        0     4399 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2898_to_parquet_dataset.py
+-rw-r--r--   0        0        0     2989 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2917_real_imag_angle.py
+-rw-r--r--   0        0        0      965 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2917_round.py
+-rw-r--r--   0        0        0      800 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2918_fix_var_axis_not_minus_one.py
+-rw-r--r--   0        0        0     3793 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2928_nested_cartesian_record.py
+-rw-r--r--   0        0        0      361 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2934_argmin_argmax_bool.py
+-rw-r--r--   0        0        0     5582 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_2968_to_parquet_row_groups.py
+-rw-r--r--   0        0        0      470 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_3028_mask_bitmaskedarray.py
+-rw-r--r--   0        0        0      466 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/test_3033_flatten_bitmaskedarray.py
+-rw-r--r--   0        0        0      124 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/__init__.py
+-rw-r--r--   0        0        0      218 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/array_enum_test_data.avro
+-rw-r--r--   0        0        0      176 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/array_string_test_data.avro
+-rw-r--r--   0        0        0      152 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/array_test_data.avro
+-rw-r--r--   0        0        0      440 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/awkward1-bytemaskedarray.pkl
+-rw-r--r--   0        0        0      255 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/awkward1-emptyarray.pkl
+-rw-r--r--   0        0        0      461 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/awkward1-indexedoptionarray.pkl
+-rw-r--r--   0        0        0      468 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/awkward1-listoffsetarray.pkl
+-rw-r--r--   0        0        0      288 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/awkward1-numpyarray.pkl
+-rw-r--r--   0        0        0      368 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/awkward1-partitioned-numpyarray.pkl
+-rw-r--r--   0        0        0      446 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/awkward1-recordarray-tuple.pkl
+-rw-r--r--   0        0        0      455 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/awkward1-recordarray.pkl
+-rw-r--r--   0        0        0      564 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/awkward1-regulararray.pkl
+-rw-r--r--   0        0        0      499 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/awkward1-strings.pkl
+-rw-r--r--   0        0        0      736 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/awkward1-unionarray.pkl
+-rw-r--r--   0        0        0      325 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/awkward1-unmaskedarray.pkl
+-rw-r--r--   0        0        0      115 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/bool_test_data.avro
+-rw-r--r--   0        0        0      130 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/bytes_test_data.avro
+-rw-r--r--   0        0        0   523374 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/complex-nested.json
+-rw-r--r--   0        0        0      158 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/double_test_data.avro
+-rw-r--r--   0        0        0      191 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/enum_null_test_data.avro
+-rw-r--r--   0        0        0      180 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/enum_test_data.avro
+-rw-r--r--   0        0        0      218 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/fixed_test_data.avro
+-rw-r--r--   0        0        0      116 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/float_test_data.avro
+-rw-r--r--   0        0        0      106 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/int_null_test_data.avro
+-rw-r--r--   0        0        0      128 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/int_string_null_test_data.avro
+-rw-r--r--   0        0        0       89 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/int_test_data.avro
+-rw-r--r--   0        0        0     3035 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/list-depths-records-list.parquet
+-rw-r--r--   0        0        0     2871 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/list-depths-records.parquet
+-rw-r--r--   0        0        0      497 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/list-depths-simple.parquet
+-rw-r--r--   0        0        0     1136 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/list-depths-strings.parquet
+-rw-r--r--   0        0        0     1060 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/list-depths.parquet
+-rw-r--r--   0        0        0      465 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/list-lengths.parquet
+-rw-r--r--   0        0        0      116 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/long_test_data.avro
+-rw-r--r--   0        0        0      681 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/nonnullable-depths.parquet
+-rw-r--r--   0        0        0       75 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/null_test_data.avro
+-rw-r--r--   0        0        0      719 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/nullable-depths.parquet
+-rw-r--r--   0        0        0      635 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/nullable-levels.parquet
+-rw-r--r--   0        0        0     3050 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/nullable-list-depths-records-list.parquet
+-rw-r--r--   0        0        0     2926 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/nullable-list-depths-records.parquet
+-rw-r--r--   0        0        0     1179 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/nullable-list-depths-strings.parquet
+-rw-r--r--   0        0        0     1101 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/nullable-list-depths.parquet
+-rw-r--r--   0        0        0      430 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/nullable-record-primitives-simple.parquet
+-rw-r--r--   0        0        0     1181 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/nullable-record-primitives.parquet
+-rw-r--r--   0        0        0     1193 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/record-primitives.parquet
+-rw-r--r--   0        0        0      326 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/record_0_test_data.avro
+-rw-r--r--   0        0        0      368 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/record_1_test_data.avro
+-rw-r--r--   0        0        0      263 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/record_null_test_data.avro
+-rw-r--r--   0        0        0      423 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/record_test_data.avro
+-rw-r--r--   0        0        0      116 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/string_null_test_data.avro
+-rw-r--r--   0        0        0      125 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/string_test_data.avro
+-rw-r--r--   0        0        0      544 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/test-nan-inf.json
+-rw-r--r--   0        0        0      155 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/test-record-array.json
+-rw-r--r--   0        0        0      803 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/test-two-arrays.json
+-rw-r--r--   0        0        0      535 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/test.json
+-rw-r--r--   0        0        0      180 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests/samples/zero-record-batches.parquet
+-rw-r--r--   0        0        0       84 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda/__init__.py
+-rw-r--r--   0        0        0     6909 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda/test_1276_cuda_num.py
+-rw-r--r--   0        0        0    13304 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda/test_1276_cuda_transfers.py
+-rw-r--r--   0        0        0     1348 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda/test_1276_cupy_interop.py
+-rw-r--r--   0        0        0     1808 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda/test_1276_from_cupy.py
+-rw-r--r--   0        0        0    42828 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda/test_1300_same_for_numba_cuda.py
+-rw-r--r--   0        0        0     1244 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda/test_1381_check_errors.py
+-rw-r--r--   0        0        0    11072 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda/test_1809_array_cuda_jit.py
+-rw-r--r--   0        0        0      146 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/__init__.py
+-rw-r--r--   0        0        0     5009 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_BitMaskedArray_to_ByteMaskedArray.py
+-rw-r--r--   0        0        0     4655 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_BitMaskedArray_to_IndexedOptionArray64.py
+-rw-r--r--   0        0        0     2772 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_getitem_nextcarry_64.py
+-rw-r--r--   0        0        0     3664 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_getitem_nextcarry_outindex_64.py
+-rw-r--r--   0        0        0     3190 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_numnull.py
+-rw-r--r--   0        0        0    17790 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_overlay_mask8.py
+-rw-r--r--   0        0        0      517 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_reduce_next_64.py
+-rw-r--r--   0        0        0      537 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.py
+-rw-r--r--   0        0        0      548 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.py
+-rw-r--r--   0        0        0     3413 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_toIndexedOptionArray64.py
+-rw-r--r--   0        0        0    29905 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_Content_getitem_next_missing_jagged_getmaskstartstop.py
+-rw-r--r--   0        0        0      510 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_Index_nones_as_index_64.py
+-rw-r--r--   0        0        0     2861 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_flatten_nextcarry_64.py
+-rw-r--r--   0        0        0    14874 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_flatten_none2empty_64.py
+-rw-r--r--   0        0        0     2861 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_getitem_nextcarry_64.py
+-rw-r--r--   0        0        0     2437 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_getitem_nextcarry_outindex_64.py
+-rw-r--r--   0        0        0      516 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_index_of_nulls.py
+-rw-r--r--   0        0        0     3119 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_numnull.py
+-rw-r--r--   0        0        0      517 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_numnull_parents.py
+-rw-r--r--   0        0        0      520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_overlay_mask8_to64.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_ranges_carry_next_64.py
+-rw-r--r--   0        0        0      516 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_ranges_next_64.py
+-rw-r--r--   0        0        0      516 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_reduce_next_64.py
+-rw-r--r--   0        0        0      536 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_reduce_next_nonlocal_nextshifts_64.py
+-rw-r--r--   0        0        0      547 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_reduce_next_nonlocal_nextshifts_fromshifts_64.py
+-rw-r--r--   0        0        0     9865 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_simplify32_to64.py
+-rw-r--r--   0        0        0     9865 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_simplify64_to64.py
+-rw-r--r--   0        0        0     9910 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_simplifyU32_to64.py
+-rw-r--r--   0        0        0     8475 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_validity.py
+-rw-r--r--   0        0        0     2861 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_flatten_nextcarry_64.py
+-rw-r--r--   0        0        0    14874 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_flatten_none2empty_64.py
+-rw-r--r--   0        0        0     2861 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_getitem_nextcarry_64.py
+-rw-r--r--   0        0        0     2437 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_getitem_nextcarry_outindex_64.py
+-rw-r--r--   0        0        0      516 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_index_of_nulls.py
+-rw-r--r--   0        0        0     3119 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_numnull.py
+-rw-r--r--   0        0        0      517 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_numnull_parents.py
+-rw-r--r--   0        0        0      520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_overlay_mask8_to64.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_ranges_carry_next_64.py
+-rw-r--r--   0        0        0      516 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_ranges_next_64.py
+-rw-r--r--   0        0        0      516 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_reduce_next_64.py
+-rw-r--r--   0        0        0      536 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_reduce_next_nonlocal_nextshifts_64.py
+-rw-r--r--   0        0        0      547 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_reduce_next_nonlocal_nextshifts_fromshifts_64.py
+-rw-r--r--   0        0        0     9865 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_simplify32_to64.py
+-rw-r--r--   0        0        0     9865 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_simplify64_to64.py
+-rw-r--r--   0        0        0     9910 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_simplifyU32_to64.py
+-rw-r--r--   0        0        0     8475 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_validity.py
+-rw-r--r--   0        0        0     2876 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_flatten_nextcarry_64.py
+-rw-r--r--   0        0        0    14949 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_flatten_none2empty_64.py
+-rw-r--r--   0        0        0     2876 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_getitem_nextcarry_64.py
+-rw-r--r--   0        0        0     2452 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_getitem_nextcarry_outindex_64.py
+-rw-r--r--   0        0        0      517 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_index_of_nulls.py
+-rw-r--r--   0        0        0     3134 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_numnull.py
+-rw-r--r--   0        0        0      518 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_numnull_parents.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_overlay_mask8_to64.py
+-rw-r--r--   0        0        0      523 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_ranges_carry_next_64.py
+-rw-r--r--   0        0        0      517 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_ranges_next_64.py
+-rw-r--r--   0        0        0      517 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_reduce_next_64.py
+-rw-r--r--   0        0        0      537 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_reduce_next_nonlocal_nextshifts_64.py
+-rw-r--r--   0        0        0      548 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_reduce_next_nonlocal_nextshifts_fromshifts_64.py
+-rw-r--r--   0        0        0     9910 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_simplify32_to64.py
+-rw-r--r--   0        0        0     9910 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_simplify64_to64.py
+-rw-r--r--   0        0        0     9955 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_simplifyU32_to64.py
+-rw-r--r--   0        0        0     8550 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_validity.py
+-rw-r--r--   0        0        0     2969 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray_fill_to64_count.py
+-rw-r--r--   0        0        0     3629 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray_fill_to64_from32.py
+-rw-r--r--   0        0        0     3629 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray_fill_to64_from64.py
+-rw-r--r--   0        0        0     3644 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray_fill_to64_fromU32.py
+-rw-r--r--   0        0        0      517 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray_numnull_unique_64.py
+-rw-r--r--   0        0        0      526 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray_reduce_next_fix_offsets_64.py
+-rw-r--r--   0        0        0     3373 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedOptionArray_rpad_and_clip_mask_axis1_64.py
+-rw-r--r--   0        0        0     1350 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_broadcast_tooffsets_64.py
+-rw-r--r--   0        0        0    24052 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_combinations_length_64.py
+-rw-r--r--   0        0        0     3899 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_compact_offsets_64.py
+-rw-r--r--   0        0        0    17497 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_jagged_descend_64.py
+-rw-r--r--   0        0        0     6678 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_jagged_expand_64.py
+-rw-r--r--   0        0        0     8008 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_next_array_64.py
+-rw-r--r--   0        0        0    46454 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_next_array_advanced_64.py
+-rw-r--r--   0        0        0     1427 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_next_at_64.py
+-rw-r--r--   0        0        0     3284 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_next_range_counts_64.py
+-rw-r--r--   0        0        0      535 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_next_range_spreadadvanced_64.py
+-rw-r--r--   0        0        0     2081 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_localindex_64.py
+-rw-r--r--   0        0        0     3612 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_min_range.py
+-rw-r--r--   0        0        0     3898 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_rpad_and_clip_length_axis1.py
+-rw-r--r--   0        0        0     6207 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_rpad_axis1_64.py
+-rw-r--r--   0        0        0     2285 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_validity.py
+-rw-r--r--   0        0        0     1350 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_broadcast_tooffsets_64.py
+-rw-r--r--   0        0        0    24052 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_combinations_length_64.py
+-rw-r--r--   0        0        0     3899 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_compact_offsets_64.py
+-rw-r--r--   0        0        0    17497 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_jagged_descend_64.py
+-rw-r--r--   0        0        0     6678 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_jagged_expand_64.py
+-rw-r--r--   0        0        0     8008 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_next_array_64.py
+-rw-r--r--   0        0        0    46454 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_next_array_advanced_64.py
+-rw-r--r--   0        0        0     1427 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_next_at_64.py
+-rw-r--r--   0        0        0     3284 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_next_range_counts_64.py
+-rw-r--r--   0        0        0      535 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_next_range_spreadadvanced_64.py
+-rw-r--r--   0        0        0     2081 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_localindex_64.py
+-rw-r--r--   0        0        0     3612 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_min_range.py
+-rw-r--r--   0        0        0     3898 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_rpad_and_clip_length_axis1.py
+-rw-r--r--   0        0        0     6207 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_rpad_axis1_64.py
+-rw-r--r--   0        0        0     2285 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_validity.py
+-rw-r--r--   0        0        0     1360 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_broadcast_tooffsets_64.py
+-rw-r--r--   0        0        0    24177 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_combinations_length_64.py
+-rw-r--r--   0        0        0     3924 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_compact_offsets_64.py
+-rw-r--r--   0        0        0    17622 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_jagged_descend_64.py
+-rw-r--r--   0        0        0     6703 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_jagged_expand_64.py
+-rw-r--r--   0        0        0     8043 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_next_array_64.py
+-rw-r--r--   0        0        0    46669 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_next_array_advanced_64.py
+-rw-r--r--   0        0        0     1437 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_next_at_64.py
+-rw-r--r--   0        0        0     3299 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_next_range_counts_64.py
+-rw-r--r--   0        0        0      536 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_next_range_spreadadvanced_64.py
+-rw-r--r--   0        0        0     2090 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_localindex_64.py
+-rw-r--r--   0        0        0     3637 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_min_range.py
+-rw-r--r--   0        0        0     3923 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_rpad_and_clip_length_axis1.py
+-rw-r--r--   0        0        0     6252 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_rpad_axis1_64.py
+-rw-r--r--   0        0        0     2310 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_validity.py
+-rw-r--r--   0        0        0     5525 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray_fill_to64_from32.py
+-rw-r--r--   0        0        0     5525 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray_fill_to64_from64.py
+-rw-r--r--   0        0        0     5550 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray_fill_to64_fromU32.py
+-rw-r--r--   0        0        0     3908 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray_getitem_jagged_carrylen_64.py
+-rw-r--r--   0        0        0      523 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray_getitem_jagged_numvalid_64.py
+-rw-r--r--   0        0        0    20350 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray32_flatten_offsets_64.py
+-rw-r--r--   0        0        0      532 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray32_reduce_local_nextparents_64.py
+-rw-r--r--   0        0        0      527 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray32_rpad_and_clip_axis1_64.py
+-rw-r--r--   0        0        0      518 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray32_rpad_axis1_64.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray32_rpad_length_axis1.py
+-rw-r--r--   0        0        0     2424 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray32_toRegularArray.py
+-rw-r--r--   0        0        0    20350 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray64_flatten_offsets_64.py
+-rw-r--r--   0        0        0      532 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray64_reduce_local_nextparents_64.py
+-rw-r--r--   0        0        0      527 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray64_rpad_and_clip_axis1_64.py
+-rw-r--r--   0        0        0      518 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray64_rpad_axis1_64.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray64_rpad_length_axis1.py
+-rw-r--r--   0        0        0     2424 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray64_toRegularArray.py
+-rw-r--r--   0        0        0    20425 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArrayU32_flatten_offsets_64.py
+-rw-r--r--   0        0        0      533 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArrayU32_reduce_local_nextparents_64.py
+-rw-r--r--   0        0        0      528 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArrayU32_rpad_and_clip_axis1_64.py
+-rw-r--r--   0        0        0      519 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArrayU32_rpad_axis1_64.py
+-rw-r--r--   0        0        0      523 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArrayU32_rpad_length_axis1.py
+-rw-r--r--   0        0        0     2439 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArrayU32_toRegularArray.py
+-rw-r--r--   0        0        0    20055 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray_drop_none_indexes_32.py
+-rw-r--r--   0        0        0    20055 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray_drop_none_indexes_64.py
+-rw-r--r--   0        0        0      523 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray_local_preparenext_64.py
+-rw-r--r--   0        0        0      542 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray_reduce_nonlocal_maxcount_offsetscopy_64.py
+-rw-r--r--   0        0        0      532 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray_reduce_nonlocal_nextstarts_64.py
+-rw-r--r--   0        0        0    26500 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_MaskedArray32_getitem_next_jagged_project.py
+-rw-r--r--   0        0        0    26500 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_MaskedArray64_getitem_next_jagged_project.py
+-rw-r--r--   0        0        0    26575 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_MaskedArrayU32_getitem_next_jagged_project.py
+-rw-r--r--   0        0        0      524 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromfloat32.py
+-rw-r--r--   0        0        0      524 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromfloat64.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromint16.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromint32.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromint64.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromint8.py
+-rw-r--r--   0        0        0      523 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromuint16.py
+-rw-r--r--   0        0        0      523 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromuint32.py
+-rw-r--r--   0        0        0      523 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromuint64.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromuint8.py
+-rw-r--r--   0        0        0      524 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromfloat32.py
+-rw-r--r--   0        0        0      524 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromfloat64.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromint16.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromint32.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromint64.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromint8.py
+-rw-r--r--   0        0        0      523 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromuint16.py
+-rw-r--r--   0        0        0      523 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromuint32.py
+-rw-r--r--   0        0        0      523 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromuint64.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromuint8.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromfloat32.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromfloat64.py
+-rw-r--r--   0        0        0      520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromint16.py
+-rw-r--r--   0        0        0      520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromint32.py
+-rw-r--r--   0        0        0      520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromint64.py
+-rw-r--r--   0        0        0      519 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromint8.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromuint16.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromuint32.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromuint64.py
+-rw-r--r--   0        0        0      520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromuint8.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromfloat32.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromfloat64.py
+-rw-r--r--   0        0        0      520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromint16.py
+-rw-r--r--   0        0        0      520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromint32.py
+-rw-r--r--   0        0        0      520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromint64.py
+-rw-r--r--   0        0        0      519 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromint8.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromuint16.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromuint32.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromuint64.py
+-rw-r--r--   0        0        0      520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromuint8.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromfloat32.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromfloat64.py
+-rw-r--r--   0        0        0      520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromint16.py
+-rw-r--r--   0        0        0      520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromint32.py
+-rw-r--r--   0        0        0      520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromint64.py
+-rw-r--r--   0        0        0      519 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromint8.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromuint16.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromuint32.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromuint64.py
+-rw-r--r--   0        0        0      520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromuint8.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromfloat32.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromfloat64.py
+-rw-r--r--   0        0        0      519 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromint16.py
+-rw-r--r--   0        0        0      519 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromint32.py
+-rw-r--r--   0        0        0      519 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromint64.py
+-rw-r--r--   0        0        0      518 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromint8.py
+-rw-r--r--   0        0        0      520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromuint16.py
+-rw-r--r--   0        0        0      520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromuint32.py
+-rw-r--r--   0        0        0      520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromuint64.py
+-rw-r--r--   0        0        0      519 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromuint8.py
+-rw-r--r--   0        0        0      523 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromfloat32.py
+-rw-r--r--   0        0        0      523 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromfloat64.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromint16.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromint32.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromint64.py
+-rw-r--r--   0        0        0      520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromint8.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromuint16.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromuint32.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromuint64.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromuint8.py
+-rw-r--r--   0        0        0      523 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromfloat32.py
+-rw-r--r--   0        0        0      523 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromfloat64.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromint16.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromint32.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromint64.py
+-rw-r--r--   0        0        0      520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromint8.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromuint16.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromuint32.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromuint64.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromuint8.py
+-rw-r--r--   0        0        0      523 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromfloat32.py
+-rw-r--r--   0        0        0      523 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromfloat64.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromint16.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromint32.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromint64.py
+-rw-r--r--   0        0        0      520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromint8.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromuint16.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromuint32.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromuint64.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromuint8.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromfloat32.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromfloat64.py
+-rw-r--r--   0        0        0      520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromint16.py
+-rw-r--r--   0        0        0      520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromint32.py
+-rw-r--r--   0        0        0      520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromint64.py
+-rw-r--r--   0        0        0      519 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromint8.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromuint16.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromuint32.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromuint64.py
+-rw-r--r--   0        0        0      520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromuint8.py
+-rw-r--r--   0        0        0      522 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_pad_zero_to_length_uint8.py
+-rw-r--r--   0        0        0      521 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_reduce_adjust_starts_64.py
+-rw-r--r--   0        0        0      528 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_reduce_adjust_starts_shifts_64.py
+-rw-r--r--   0        0        0      528 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_reduce_mask_ByteMaskedArray_64.py
+-rw-r--r--   0        0        0    13090 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_carry_64.py
+-rw-r--r--   0        0        0    19346 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_jagged_expand_64.py
+-rw-r--r--   0        0        0    24330 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_next_array_64.py
+-rw-r--r--   0        0        0   125787 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_next_array_advanced_64.py
+-rw-r--r--   0        0        0    11737 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_next_array_regularize_64.py
+-rw-r--r--   0        0        0     2375 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_next_at_64.py
+-rw-r--r--   0        0        0      958 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_next_range_64.py
+-rw-r--r--   0        0        0    14446 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_next_range_spreadadvanced_64.py
+-rw-r--r--   0        0        0     2371 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_RegularArray_localindex_64.py
+-rw-r--r--   0        0        0      527 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_RegularArray_reduce_local_nextparents_64.py
+-rw-r--r--   0        0        0      530 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_RegularArray_reduce_nonlocal_preparenext_64.py
+-rw-r--r--   0        0        0      897 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_RegularArray_rpad_and_clip_axis1_64.py
+-rw-r--r--   0        0        0    13570 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_32_project_64.py
+-rw-r--r--   0        0        0   619561 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_32_simplify8_32_to8_64.py
+-rw-r--r--   0        0        0   619561 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_32_simplify8_64_to8_64.py
+-rw-r--r--   0        0        0   621061 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_32_simplify8_U32_to8_64.py
+-rw-r--r--   0        0        0    14770 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_32_simplify_one_to8_64.py
+-rw-r--r--   0        0        0    61679 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_32_validity.py
+-rw-r--r--   0        0        0    13570 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_64_project_64.py
+-rw-r--r--   0        0        0   619561 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_64_simplify8_32_to8_64.py
+-rw-r--r--   0        0        0   619561 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_64_simplify8_64_to8_64.py
+-rw-r--r--   0        0        0   621061 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_64_simplify8_U32_to8_64.py
+-rw-r--r--   0        0        0    14770 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_64_simplify_one_to8_64.py
+-rw-r--r--   0        0        0    61679 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_64_validity.py
+-rw-r--r--   0        0        0    13615 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_U32_project_64.py
+-rw-r--r--   0        0        0   621061 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_U32_simplify8_32_to8_64.py
+-rw-r--r--   0        0        0   621061 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_U32_simplify8_64_to8_64.py
+-rw-r--r--   0        0        0   622561 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_U32_simplify8_U32_to8_64.py
+-rw-r--r--   0        0        0    14815 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_U32_simplify_one_to8_64.py
+-rw-r--r--   0        0        0    62054 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_U32_validity.py
+-rw-r--r--   0        0        0     3185 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_regular_index_getsize.py
+-rw-r--r--   0        0        0      864 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray_fillindex_to64_count.py
+-rw-r--r--   0        0        0     3564 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray_fillindex_to64_from32.py
+-rw-r--r--   0        0        0     3564 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray_fillindex_to64_from64.py
+-rw-r--r--   0        0        0     3579 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray_fillindex_to64_fromU32.py
+-rw-r--r--   0        0        0     3199 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray_fillna_from32_to64.py
+-rw-r--r--   0        0        0     3199 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray_fillna_from64_to64.py
+-rw-r--r--   0        0        0     3214 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray_fillna_fromU32_to64.py
+-rw-r--r--   0        0        0      870 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray_filltags_to8_const.py
+-rw-r--r--   0        0        0     3650 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray_filltags_to8_from8.py
+-rw-r--r--   0        0        0      816 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_index_rpad_and_clip_axis0_64.py
+-rw-r--r--   0        0        0     1021 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_index_rpad_and_clip_axis1_64.py
+-rw-r--r--   0        0        0      763 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_localindex_64.py
+-rw-r--r--   0        0        0    17411 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_missing_repeat_64.py
+-rw-r--r--   0        0        0      511 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_argmax_float32_64.py
+-rw-r--r--   0        0        0      511 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_argmax_float64_64.py
+-rw-r--r--   0        0        0      509 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_argmax_int16_64.py
+-rw-r--r--   0        0        0      509 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_argmax_int32_64.py
+-rw-r--r--   0        0        0      509 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_argmax_int64_64.py
+-rw-r--r--   0        0        0      508 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_argmax_int8_64.py
+-rw-r--r--   0        0        0      510 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_argmax_uint16_64.py
+-rw-r--r--   0        0        0      510 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_argmax_uint32_64.py
+-rw-r--r--   0        0        0      510 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_argmax_uint64_64.py
+-rw-r--r--   0        0        0      509 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_argmax_uint8_64.py
+-rw-r--r--   0        0        0      511 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_argmin_float32_64.py
+-rw-r--r--   0        0        0      511 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_argmin_float64_64.py
+-rw-r--r--   0        0        0      509 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_argmin_int16_64.py
+-rw-r--r--   0        0        0      509 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_argmin_int32_64.py
+-rw-r--r--   0        0        0      509 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_argmin_int64_64.py
+-rw-r--r--   0        0        0      508 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_argmin_int8_64.py
+-rw-r--r--   0        0        0      510 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_argmin_uint16_64.py
+-rw-r--r--   0        0        0      510 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_argmin_uint32_64.py
+-rw-r--r--   0        0        0      510 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_argmin_uint64_64.py
+-rw-r--r--   0        0        0      509 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_argmin_uint8_64.py
+-rw-r--r--   0        0        0      502 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_count_64.py
+-rw-r--r--   0        0        0      514 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_bool_64.py
+-rw-r--r--   0        0        0      517 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_float32_64.py
+-rw-r--r--   0        0        0      517 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_float64_64.py
+-rw-r--r--   0        0        0      515 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_int16_64.py
+-rw-r--r--   0        0        0      515 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_int32_64.py
+-rw-r--r--   0        0        0      515 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_int64_64.py
+-rw-r--r--   0        0        0      514 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_int8_64.py
+-rw-r--r--   0        0        0      516 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_uint16_64.py
+-rw-r--r--   0        0        0      516 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_uint32_64.py
+-rw-r--r--   0        0        0      516 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_uint64_64.py
+-rw-r--r--   0        0        0      515 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_uint8_64.py
+-rw-r--r--   0        0        0      516 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_max_float32_float32_64.py
+-rw-r--r--   0        0        0      516 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_max_float64_float64_64.py
+-rw-r--r--   0        0        0      512 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_max_int16_int16_64.py
+-rw-r--r--   0        0        0      512 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_max_int32_int32_64.py
+-rw-r--r--   0        0        0      512 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_max_int64_int64_64.py
+-rw-r--r--   0        0        0      510 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_max_int8_int8_64.py
+-rw-r--r--   0        0        0      514 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_max_uint16_uint16_64.py
+-rw-r--r--   0        0        0      514 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_max_uint32_uint32_64.py
+-rw-r--r--   0        0        0      514 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_max_uint64_uint64_64.py
+-rw-r--r--   0        0        0      512 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_max_uint8_uint8_64.py
+-rw-r--r--   0        0        0      516 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_min_float32_float32_64.py
+-rw-r--r--   0        0        0      516 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_min_float64_float64_64.py
+-rw-r--r--   0        0        0      512 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_min_int16_int16_64.py
+-rw-r--r--   0        0        0      512 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_min_int32_int32_64.py
+-rw-r--r--   0        0        0      512 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_min_int64_int64_64.py
+-rw-r--r--   0        0        0      510 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_min_int8_int8_64.py
+-rw-r--r--   0        0        0      514 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_min_uint16_uint16_64.py
+-rw-r--r--   0        0        0      514 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_min_uint32_uint32_64.py
+-rw-r--r--   0        0        0      514 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_min_uint64_uint64_64.py
+-rw-r--r--   0        0        0      512 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_min_uint8_uint8_64.py
+-rw-r--r--   0        0        0      511 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_bool_64.py
+-rw-r--r--   0        0        0      514 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_float32_64.py
+-rw-r--r--   0        0        0      514 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_float64_64.py
+-rw-r--r--   0        0        0      512 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_int16_64.py
+-rw-r--r--   0        0        0      512 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_int32_64.py
+-rw-r--r--   0        0        0      512 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_int64_64.py
+-rw-r--r--   0        0        0      511 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_int8_64.py
+-rw-r--r--   0        0        0      513 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_uint16_64.py
+-rw-r--r--   0        0        0      513 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_uint32_64.py
+-rw-r--r--   0        0        0      513 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_uint64_64.py
+-rw-r--r--   0        0        0      512 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_uint8_64.py
+-rw-r--r--   0        0        0      510 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_bool_64.py
+-rw-r--r--   0        0        0      513 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_float32_64.py
+-rw-r--r--   0        0        0      513 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_float64_64.py
+-rw-r--r--   0        0        0      511 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_int16_64.py
+-rw-r--r--   0        0        0      511 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_int32_64.py
+-rw-r--r--   0        0        0      511 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_int64_64.py
+-rw-r--r--   0        0        0      510 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_int8_64.py
+-rw-r--r--   0        0        0      512 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_uint16_64.py
+-rw-r--r--   0        0        0      512 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_uint32_64.py
+-rw-r--r--   0        0        0      512 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_uint64_64.py
+-rw-r--r--   0        0        0      511 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_uint8_64.py
+-rw-r--r--   0        0        0      516 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_float32_float32_64.py
+-rw-r--r--   0        0        0      516 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_float64_float64_64.py
+-rw-r--r--   0        0        0      511 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_int32_bool_64.py
+-rw-r--r--   0        0        0      512 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_int32_int16_64.py
+-rw-r--r--   0        0        0      512 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_int32_int32_64.py
+-rw-r--r--   0        0        0      511 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_int32_int8_64.py
+-rw-r--r--   0        0        0      511 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_int64_bool_64.py
+-rw-r--r--   0        0        0      512 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_int64_int16_64.py
+-rw-r--r--   0        0        0      512 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_int64_int32_64.py
+-rw-r--r--   0        0        0      512 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_int64_int64_64.py
+-rw-r--r--   0        0        0      511 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_int64_int8_64.py
+-rw-r--r--   0        0        0      514 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint32_uint16_64.py
+-rw-r--r--   0        0        0      514 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint32_uint32_64.py
+-rw-r--r--   0        0        0      513 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint32_uint8_64.py
+-rw-r--r--   0        0        0      514 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint64_uint16_64.py
+-rw-r--r--   0        0        0      514 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint64_uint32_64.py
+-rw-r--r--   0        0        0      514 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint64_uint64_64.py
+-rw-r--r--   0        0        0      513 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint64_uint8_64.py
+-rw-r--r--   0        0        0      501 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_sorting_ranges.py
+-rw-r--r--   0        0        0      508 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_sorting_ranges_length.py
+-rw-r--r--   0        0        0     2364 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/.gitignore
+-rw-r--r--   0        0        0     1520 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/LICENSE
+-rw-r--r--   0        0        0     8936 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/pyproject.toml
+-rw-r--r--   0        0        0     6983 2024-03-21 23:08:24.000000 awkward-2.6.3rc2/PKG-INFO
```

### Comparing `awkward-2.6.3/CITATION.cff` & `awkward-2.6.3rc2/CITATION.cff`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/CONTRIBUTING.md` & `awkward-2.6.3rc2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/README.md` & `awkward-2.6.3rc2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -219,15 +219,14 @@
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://www.mloning.com/"><img src="https://avatars.githubusercontent.com/u/21020482?v=4?s=100" width="100px;" alt="Markus Löning"/><br /><sub><b>Markus Löning</b></sub></a><br /><a href="https://github.com/scikit-hep/awkward/commits?author=mloning" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/kkothari2001"><img src="https://avatars.githubusercontent.com/u/53650538?v=4?s=100" width="100px;" alt="Kush Kothari"/><br /><sub><b>Kush Kothari</b></sub></a><br /><a href="https://github.com/scikit-hep/awkward/commits?author=kkothari2001" title="Code">💻</a> <a href="https://github.com/scikit-hep/awkward/commits?author=kkothari2001" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/jrueb"><img src="https://avatars.githubusercontent.com/u/30041073?v=4?s=100" width="100px;" alt="Jonas Rübenach"/><br /><sub><b>Jonas Rübenach</b></sub></a><br /><a href="https://github.com/scikit-hep/awkward/commits?author=jrueb" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://blog.jling.dev"><img src="https://avatars.githubusercontent.com/u/5306213?v=4?s=100" width="100px;" alt="Jerry Ling"/><br /><sub><b>Jerry Ling</b></sub></a><br /><a href="https://github.com/scikit-hep/awkward/commits?author=Moelf" title="Documentation">📖</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/lobis"><img src="https://avatars.githubusercontent.com/u/35803280?v=4?s=100" width="100px;" alt="Luis Antonio Obis Aparicio"/><br /><sub><b>Luis Antonio Obis Aparicio</b></sub></a><br /><a href="https://github.com/scikit-hep/awkward/commits?author=lobis" title="Code">💻</a></td>
-      <td align="center" valign="top" width="14.28%"><a href="https://github.com/tcawlfield"><img src="https://avatars.githubusercontent.com/u/4094385?v=4?s=100" width="100px;" alt="Topher Cawlfield"/><br /><sub><b>Topher Cawlfield</b></sub></a><br /><a href="https://github.com/scikit-hep/awkward/commits?author=tcawlfield" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `awkward-2.6.3/docs/_toc.yml` & `awkward-2.6.3rc2/docs/_toc.yml`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/conf.py` & `awkward-2.6.3rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/index.md` & `awkward-2.6.3rc2/docs/index.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/prepare_docstrings.py` & `awkward-2.6.3rc2/docs/prepare_docstrings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/redirects-user-guide.json` & `awkward-2.6.3rc2/docs/redirects-user-guide.json`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/redirects.json` & `awkward-2.6.3rc2/docs/redirects.json`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/requirements.txt` & `awkward-2.6.3rc2/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/switcher.json` & `awkward-2.6.3rc2/docs/switcher.json`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/_static/css/awkward.css` & `awkward-2.6.3rc2/docs/_static/css/awkward.css`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/data/y77d-th95.json` & `awkward-2.6.3rc2/docs/data/y77d-th95.json`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/getting-started/community-tutorials.md` & `awkward-2.6.3rc2/docs/getting-started/community-tutorials.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/getting-started/index.md` & `awkward-2.6.3rc2/docs/getting-started/index.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/getting-started/papers-and-talks.md` & `awkward-2.6.3rc2/docs/getting-started/papers-and-talks.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/getting-started/demo/what-is-an-awkward-array.ipynb` & `awkward-2.6.3rc2/docs/getting-started/demo/what-is-an-awkward-array.ipynb`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/image/example-hierarchy.svg` & `awkward-2.6.3rc2/docs/image/example-hierarchy.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/reference/ak.behavior.md` & `awkward-2.6.3rc2/docs/reference/ak.behavior.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/reference/ak.builder.ArrayBuilder.rst` & `awkward-2.6.3rc2/docs/reference/ak.builder.ArrayBuilder.rst`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/reference/awkwardforth.rst` & `awkward-2.6.3rc2/docs/reference/awkwardforth.rst`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/reference/toctree.txt` & `awkward-2.6.3rc2/docs/reference/toctree.txt`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/samples/Android.head.log.gz` & `awkward-2.6.3rc2/docs/samples/Android.head.log.gz`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/10-minutes-to-awkward-array.md` & `awkward-2.6.3rc2/docs/user-guide/10-minutes-to-awkward-array.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-combinatorics-best-match.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-combinatorics-best-match.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-combinatorics-cartesian-combinations.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-combinatorics-cartesian-combinations.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-convert-arrow.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-convert-arrow.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-convert-buffers.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-convert-buffers.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-convert-json.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-convert-json.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-convert-numpy.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-convert-numpy.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-convert-pandas.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-convert-pandas.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-convert-python.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-convert-python.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-convert-rdataframe.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-convert-rdataframe.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-create-arraybuilder.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-create-arraybuilder.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-create-constructors.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-create-constructors.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-create-lists.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-create-lists.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-create-missing.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-create-missing.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-create-records.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-create-records.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-create-strings.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-create-strings.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-create-unflatten-group.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-create-unflatten-group.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-examine-checking-validity.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-examine-checking-validity.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-examine-list-fields.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-examine-list-fields.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-examine-simple-slicing.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-examine-simple-slicing.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-examine-single-item.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-examine-single-item.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-examine-type.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-examine-type.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-filter-cut-mask.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-filter-cut-mask.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-filter-masked.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-filter-masked.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-filter-num.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-filter-num.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-filter-ragged.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-filter-ragged.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-math-argminmax.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-math-argminmax.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-math-broadcasting.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-math-broadcasting.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-math-gpu.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-math-gpu.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-math-numpy.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-math-numpy.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-math-reducing.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-math-reducing.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-math-statistics.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-math-statistics.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-restructure-add-fields.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-restructure-add-fields.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-restructure-concatenate.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-restructure-concatenate.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-restructure-flatten.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-restructure-flatten.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-restructure-pad.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-restructure-pad.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-restructure-rename-records.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-restructure-rename-records.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-restructure-sort.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-restructure-sort.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-restructure-zip-project.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-restructure-zip-project.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-specialize-differentiate-jax.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-specialize-differentiate-jax.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-specialize-in-numba.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-specialize-in-numba.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-specialize-lorentz.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-specialize-lorentz.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-specialize-override-numpy.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-specialize-override-numpy.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-specialize-subclass.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-specialize-subclass.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-strings-extract-substrings.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-strings-extract-substrings.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-strings-read-binary.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-strings-read-binary.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-strings-split-and-join.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-strings-split-and-join.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-use-header-only-layoutbuilder.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-use-header-only-layoutbuilder.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-use-in-cpp-cppyy.ipynb` & `awkward-2.6.3rc2/docs/user-guide/how-to-use-in-cpp-cppyy.ipynb`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-use-in-numba-arraybuilder.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-use-in-numba-arraybuilder.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-use-in-numba-cuda.ipynb` & `awkward-2.6.3rc2/docs/user-guide/how-to-use-in-numba-cuda.ipynb`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs/user-guide/how-to-use-in-numba-features.md` & `awkward-2.6.3rc2/docs/user-guide/how-to-use-in-numba-features.md`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/panel-data-analysts.png` & `awkward-2.6.3rc2/docs-img/panel-data-analysts.png`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/panel-data-analysts.svg` & `awkward-2.6.3rc2/docs-img/panel-data-analysts.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/panel-developers.png` & `awkward-2.6.3rc2/docs-img/panel-developers.png`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/panel-developers.svg` & `awkward-2.6.3rc2/docs-img/panel-developers.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/panel-doxygen.png` & `awkward-2.6.3rc2/docs-img/panel-doxygen.png`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/panel-sphinx.png` & `awkward-2.6.3rc2/docs-img/panel-sphinx.png`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/panel-tutorials-alternate.png` & `awkward-2.6.3rc2/docs-img/panel-tutorials-alternate.png`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/panel-tutorials.png` & `awkward-2.6.3rc2/docs-img/panel-tutorials.png`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/awkward-1-0-layers.pdf` & `awkward-2.6.3rc2/docs-img/diagrams/awkward-1-0-layers.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/awkward-1-0-layers.png` & `awkward-2.6.3rc2/docs-img/diagrams/awkward-1-0-layers.png`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/awkward-1-0-layers.svg` & `awkward-2.6.3rc2/docs-img/diagrams/awkward-1-0-layers.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/awkward-timeline.pdf` & `awkward-2.6.3rc2/docs-img/diagrams/awkward-timeline.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/awkward-timeline.png` & `awkward-2.6.3rc2/docs-img/diagrams/awkward-timeline.png`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/awkward-timeline.svg` & `awkward-2.6.3rc2/docs-img/diagrams/awkward-timeline.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/awkward-uproot-timeline-pip-github.png` & `awkward-2.6.3rc2/docs-img/diagrams/awkward-uproot-timeline-pip-github.png`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg` & `awkward-2.6.3rc2/docs-img/diagrams/awkward-uproot-timeline-pip-github.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/awkward-uproot-timeline-pip.png` & `awkward-2.6.3rc2/docs-img/diagrams/awkward-uproot-timeline-pip.png`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/awkward-uproot-timeline-pip.svg` & `awkward-2.6.3rc2/docs-img/diagrams/awkward-uproot-timeline-pip.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/awkward-uproot-timeline.png` & `awkward-2.6.3rc2/docs-img/diagrams/awkward-uproot-timeline.png`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/awkward-uproot-timeline.svg` & `awkward-2.6.3rc2/docs-img/diagrams/awkward-uproot-timeline.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/cartoon-broadcasting.png` & `awkward-2.6.3rc2/docs-img/diagrams/cartoon-broadcasting.png`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/cartoon-broadcasting.svg` & `awkward-2.6.3rc2/docs-img/diagrams/cartoon-broadcasting.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/cartoon-cartesian.png` & `awkward-2.6.3rc2/docs-img/diagrams/cartoon-cartesian.png`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/cartoon-cartesian.svg` & `awkward-2.6.3rc2/docs-img/diagrams/cartoon-cartesian.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/cartoon-combinations.png` & `awkward-2.6.3rc2/docs-img/diagrams/cartoon-combinations.png`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/cartoon-combinations.svg` & `awkward-2.6.3rc2/docs-img/diagrams/cartoon-combinations.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/cartoon-schematic.png` & `awkward-2.6.3rc2/docs-img/diagrams/cartoon-schematic.png`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/cartoon-schematic.svg` & `awkward-2.6.3rc2/docs-img/diagrams/cartoon-schematic.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/example-array.svg` & `awkward-2.6.3rc2/docs-img/diagrams/example-array.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/example-hierarchy.png` & `awkward-2.6.3rc2/docs-img/diagrams/example-hierarchy.png`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/example-hierarchy.svg` & `awkward-2.6.3rc2/docs-img/diagrams/example-hierarchy.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/example-reduction-sum-only.svg` & `awkward-2.6.3rc2/docs-img/diagrams/example-reduction-sum-only.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/example-reduction-sum.svg` & `awkward-2.6.3rc2/docs-img/diagrams/example-reduction-sum.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/example-reduction.png` & `awkward-2.6.3rc2/docs-img/diagrams/example-reduction.png`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/example-reduction.svg` & `awkward-2.6.3rc2/docs-img/diagrams/example-reduction.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/git-strategy.pdf` & `awkward-2.6.3rc2/docs-img/diagrams/git-strategy.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/git-strategy.png` & `awkward-2.6.3rc2/docs-img/diagrams/git-strategy.png`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/git-strategy.svg` & `awkward-2.6.3rc2/docs-img/diagrams/git-strategy.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/how-it-works-muons.png` & `awkward-2.6.3rc2/docs-img/diagrams/how-it-works-muons.png`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/how-it-works-muons.svg` & `awkward-2.6.3rc2/docs-img/diagrams/how-it-works-muons.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/how-it-works.svg` & `awkward-2.6.3rc2/docs-img/diagrams/how-it-works.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/sorting-axis.svg` & `awkward-2.6.3rc2/docs-img/diagrams/sorting-axis.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/reducers/all.svg` & `awkward-2.6.3rc2/docs-img/diagrams/reducers/all.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/reducers/any.svg` & `awkward-2.6.3rc2/docs-img/diagrams/reducers/any.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/reducers/argmax.svg` & `awkward-2.6.3rc2/docs-img/diagrams/reducers/argmax.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/reducers/argmin.svg` & `awkward-2.6.3rc2/docs-img/diagrams/reducers/argmin.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/reducers/count.svg` & `awkward-2.6.3rc2/docs-img/diagrams/reducers/count.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/reducers/count_nonzero.svg` & `awkward-2.6.3rc2/docs-img/diagrams/reducers/count_nonzero.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/reducers/max.svg` & `awkward-2.6.3rc2/docs-img/diagrams/reducers/max.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/reducers/min.svg` & `awkward-2.6.3rc2/docs-img/diagrams/reducers/min.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/reducers/product.svg` & `awkward-2.6.3rc2/docs-img/diagrams/reducers/product.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/diagrams/reducers/sum.svg` & `awkward-2.6.3rc2/docs-img/diagrams/reducers/sum.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/logo/favicon.ico` & `awkward-2.6.3rc2/docs-img/logo/favicon.ico`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/logo/logo-300px-white.png` & `awkward-2.6.3rc2/docs-img/logo/logo-300px-white.png`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/logo/logo-300px.png` & `awkward-2.6.3rc2/docs-img/logo/logo-300px.png`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/logo/logo-600px.png` & `awkward-2.6.3rc2/docs-img/logo/logo-600px.png`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/logo/logo.svg` & `awkward-2.6.3rc2/docs-img/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/photos/desire-path.jpg` & `awkward-2.6.3rc2/docs-img/photos/desire-path.jpg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/plots/awkward-0-popularity.pdf` & `awkward-2.6.3rc2/docs-img/plots/awkward-0-popularity.pdf`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/plots/awkward-0-popularity.png` & `awkward-2.6.3rc2/docs-img/plots/awkward-0-popularity.png`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/plots/awkward-0-popularity.svg` & `awkward-2.6.3rc2/docs-img/plots/awkward-0-popularity.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/plots/bikeroutes-scaling.svg` & `awkward-2.6.3rc2/docs-img/plots/bikeroutes-scaling.svg`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/docs-img/screenshots/github-issues-documentation.png` & `awkward-2.6.3rc2/docs-img/screenshots/github-issues-documentation.png`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/__init__.py` & `awkward-2.6.3rc2/src/awkward/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_attrs.py` & `awkward-2.6.3rc2/src/awkward/_attrs.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_behavior.py` & `awkward-2.6.3rc2/src/awkward/_behavior.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_broadcasting.py` & `awkward-2.6.3rc2/src/awkward/_broadcasting.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_categorical.py` & `awkward-2.6.3rc2/src/awkward/_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_dispatch.py` & `awkward-2.6.3rc2/src/awkward/_dispatch.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_do.py` & `awkward-2.6.3rc2/src/awkward/_do.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_errors.py` & `awkward-2.6.3rc2/src/awkward/_errors.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_kernels.py` & `awkward-2.6.3rc2/src/awkward/_kernels.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_layout.py` & `awkward-2.6.3rc2/src/awkward/_layout.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_lookup.py` & `awkward-2.6.3rc2/src/awkward/_lookup.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_operators.py` & `awkward-2.6.3rc2/src/awkward/_operators.py`

 * *Files 8% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 """
 
 from __future__ import annotations
 
-import numpy as np
+from numpy.core import umath as um
 
 
 def _disables_array_ufunc(obj):
     """True when __array_ufunc__ is set to None."""
     try:
         return obj.__array_ufunc__ is None
     except AttributeError:
@@ -175,43 +175,43 @@
     .. versionadded:: 1.13
     """
 
     # Like np.ndarray, this mixin class implements "Option 1" from the ufunc
     # overrides NEP.
 
     # comparisons don't have reflected and in-place versions
-    __lt__ = _binary_method(np.less, "lt")
-    __le__ = _binary_method(np.less_equal, "le")
-    __eq__ = _binary_method(np.equal, "eq")
-    __ne__ = _binary_method(np.not_equal, "ne")
-    __gt__ = _binary_method(np.greater, "gt")
-    __ge__ = _binary_method(np.greater_equal, "ge")
+    __lt__ = _binary_method(um.less, "lt")
+    __le__ = _binary_method(um.less_equal, "le")
+    __eq__ = _binary_method(um.equal, "eq")
+    __ne__ = _binary_method(um.not_equal, "ne")
+    __gt__ = _binary_method(um.greater, "gt")
+    __ge__ = _binary_method(um.greater_equal, "ge")
 
     # numeric methods
-    __add__, __radd__, __iadd__ = _numeric_methods(np.add, "add")
-    __sub__, __rsub__, __isub__ = _numeric_methods(np.subtract, "sub")
-    __mul__, __rmul__, __imul__ = _numeric_methods(np.multiply, "mul")
-    __matmul__, __rmatmul__, __imatmul__ = _numeric_methods(np.matmul, "matmul")
+    __add__, __radd__, __iadd__ = _numeric_methods(um.add, "add")
+    __sub__, __rsub__, __isub__ = _numeric_methods(um.subtract, "sub")
+    __mul__, __rmul__, __imul__ = _numeric_methods(um.multiply, "mul")
+    __matmul__, __rmatmul__, __imatmul__ = _numeric_methods(um.matmul, "matmul")
     # Python 3 does not use __div__, __rdiv__, or __idiv__
     __truediv__, __rtruediv__, __itruediv__ = _numeric_methods(
-        np.true_divide, "truediv"
+        um.true_divide, "truediv"
     )
     __floordiv__, __rfloordiv__, __ifloordiv__ = _numeric_methods(
-        np.floor_divide, "floordiv"
+        um.floor_divide, "floordiv"
     )
-    __mod__, __rmod__, __imod__ = _numeric_methods(np.remainder, "mod")
-    __divmod__ = _binary_method(np.divmod, "divmod")
-    __rdivmod__ = _reflected_binary_method(np.divmod, "divmod")
+    __mod__, __rmod__, __imod__ = _numeric_methods(um.remainder, "mod")
+    __divmod__ = _binary_method(um.divmod, "divmod")
+    __rdivmod__ = _reflected_binary_method(um.divmod, "divmod")
     # __idivmod__ does not exist
     # TODO: handle the optional third argument for __pow__?
-    __pow__, __rpow__, __ipow__ = _numeric_methods(np.power, "pow")
-    __lshift__, __rlshift__, __ilshift__ = _numeric_methods(np.left_shift, "lshift")
-    __rshift__, __rrshift__, __irshift__ = _numeric_methods(np.right_shift, "rshift")
-    __and__, __rand__, __iand__ = _numeric_methods(np.bitwise_and, "and")
-    __xor__, __rxor__, __ixor__ = _numeric_methods(np.bitwise_xor, "xor")
-    __or__, __ror__, __ior__ = _numeric_methods(np.bitwise_or, "or")
+    __pow__, __rpow__, __ipow__ = _numeric_methods(um.power, "pow")
+    __lshift__, __rlshift__, __ilshift__ = _numeric_methods(um.left_shift, "lshift")
+    __rshift__, __rrshift__, __irshift__ = _numeric_methods(um.right_shift, "rshift")
+    __and__, __rand__, __iand__ = _numeric_methods(um.bitwise_and, "and")
+    __xor__, __rxor__, __ixor__ = _numeric_methods(um.bitwise_xor, "xor")
+    __or__, __ror__, __ior__ = _numeric_methods(um.bitwise_or, "or")
 
     # unary methods
-    __neg__ = _unary_method(np.negative, "neg")
-    __pos__ = _unary_method(np.positive, "pos")
-    __abs__ = _unary_method(np.absolute, "abs")
-    __invert__ = _unary_method(np.invert, "invert")
+    __neg__ = _unary_method(um.negative, "neg")
+    __pos__ = _unary_method(um.positive, "pos")
+    __abs__ = _unary_method(um.absolute, "abs")
+    __invert__ = _unary_method(um.invert, "invert")
```

### Comparing `awkward-2.6.3/src/awkward/_parameters.py` & `awkward-2.6.3rc2/src/awkward/_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_pickle.py` & `awkward-2.6.3rc2/src/awkward/_pickle.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_prettyprint.py` & `awkward-2.6.3rc2/src/awkward/_prettyprint.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_reducers.py` & `awkward-2.6.3rc2/src/awkward/_reducers.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,23 +58,21 @@
         elif dtype == np.complex128:
             return np.dtype(np.float64)
         elif dtype == np.complex64:
             return np.dtype(np.float32)
         else:
             return dtype
 
-    _use32 = (ak._util.win or ak._util.bits32) and not ak._util.numpy2
-
     @classmethod
     def _promote_integer_rank(cls, given_dtype: DTypeLike) -> DTypeLike:
         if given_dtype in (np.bool_, np.int8, np.int16, np.int32):
-            return np.int32 if cls._use32 else np.int64
+            return np.int32 if ak._util.win or ak._util.bits32 else np.int64
 
         elif given_dtype in (np.uint8, np.uint16, np.uint32):
-            return np.uint32 if cls._use32 else np.uint64
+            return np.uint32 if ak._util.win or ak._util.bits32 else np.uint64
 
         else:
             return given_dtype
 
 
 def apply_positional_corrections(
     reduced: ak.contents.NumpyArray,
```

### Comparing `awkward-2.6.3/src/awkward/_regularize.py` & `awkward-2.6.3rc2/src/awkward/_regularize.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_singleton.py` & `awkward-2.6.3rc2/src/awkward/_singleton.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_slicing.py` & `awkward-2.6.3rc2/src/awkward/_slicing.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_typetracer.py` & `awkward-2.6.3rc2/src/awkward/_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_typing.py` & `awkward-2.6.3rc2/src/awkward/_typing.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_util.py` & `awkward-2.6.3rc2/src/awkward/_util.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,23 +4,18 @@
 
 import base64
 import os
 import struct
 import sys
 from collections.abc import Collection
 
-import numpy as np  # noqa: TID251
-import packaging.version
-
 from awkward._typing import TypeVar
 
 win = os.name == "nt"
 bits32 = struct.calcsize("P") * 8 == 32
-numpy2 = packaging.version.parse(np.__version__) >= packaging.version.Version("2.0.0b1")
-
 
 # matches include/awkward/common.h
 kMaxInt8 = 127  # 2**7  - 1
 kMaxUInt8 = 255  # 2**8  - 1
 kMaxInt32 = 2147483647  # 2**31 - 1
 kMaxUInt32 = 4294967295  # 2**32 - 1
 kMaxInt64 = 9223372036854775806  # 2**63 - 2: see below
```

### Comparing `awkward-2.6.3/src/awkward/_v2.py` & `awkward-2.6.3rc2/src/awkward/_v2.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/cppyy.py` & `awkward-2.6.3rc2/src/awkward/cppyy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/highlevel.py` & `awkward-2.6.3rc2/src/awkward/highlevel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/index.py` & `awkward-2.6.3rc2/src/awkward/index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/jax.py` & `awkward-2.6.3rc2/src/awkward/jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/record.py` & `awkward-2.6.3rc2/src/awkward/record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/typetracer.py` & `awkward-2.6.3rc2/src/awkward/typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_backends/backend.py` & `awkward-2.6.3rc2/src/awkward/_backends/backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_backends/cupy.py` & `awkward-2.6.3rc2/src/awkward/_backends/cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_backends/dispatch.py` & `awkward-2.6.3rc2/src/awkward/_backends/dispatch.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_backends/jax.py` & `awkward-2.6.3rc2/src/awkward/_backends/jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_backends/numpy.py` & `awkward-2.6.3rc2/src/awkward/_backends/numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_backends/typetracer.py` & `awkward-2.6.3rc2/src/awkward/_backends/typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/avro.py` & `awkward-2.6.3rc2/src/awkward/_connect/avro.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cling.py` & `awkward-2.6.3rc2/src/awkward/_connect/cling.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/hist.py` & `awkward-2.6.3rc2/src/awkward/_connect/hist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/numexpr.py` & `awkward-2.6.3rc2/src/awkward/_connect/numexpr.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/numpy.py` & `awkward-2.6.3rc2/src/awkward/_connect/numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/pyarrow.py` & `awkward-2.6.3rc2/src/awkward/_connect/pyarrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/__init__.py` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/_kernel_signatures.py` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/_kernel_signatures.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-kernel-signatures.py
 #
 # This step is normally run explicitly before generating a package
```

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_ByteMaskedArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_BitMaskedArray_to_IndexedOptionArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_getitem_nextcarry_outindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_numnull.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_numnull.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_overlay_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ByteMaskedArray_toIndexedOptionArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_Content_getitem_next_missing_jagged_getmaskstartstop.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_nones_as_index.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_Index_nones_as_index.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_fill.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_nextcarry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_none2empty.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_flatten_none2empty.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_getitem_nextcarry_outindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_index_of_nulls.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_index_of_nulls.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_numnull.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_numnull.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_numnull_parents.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_numnull_parents.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_overlay_mask.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_ranges_carry_next_64.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_ranges_carry_next_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_ranges_next_64.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_ranges_next_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_fix_offsets_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_simplify.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedArray_validity.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_IndexedOptionArray_rpad_and_clip_mask_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_broadcast_tooffsets.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_broadcast_tooffsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_combinations_length.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_combinations_length.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_compact_offsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_fill.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_fill.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_carrylen.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_carrylen.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_descend.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_descend.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_expand.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_numvalid.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_jagged_numvalid.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array_advanced.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_array_advanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_at.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_at.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_range_counts.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_range_counts.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_range_spreadadvanced.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_getitem_next_range_spreadadvanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_localindex.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_localindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_min_range.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_min_range.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_rpad_and_clip_length_axis1.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_rpad_and_clip_length_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_rpad_axis1.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_rpad_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListArray_validity.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_drop_none_indexes.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_drop_none_indexes.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_flatten_offsets.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_local_preparenext_64.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_local_preparenext_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_local_nextparents_64.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_local_nextparents_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_nonlocal_maxcount_offsetscopy_64.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_nonlocal_maxcount_offsetscopy_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_nonlocal_nextstarts_64.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_reduce_nonlocal_nextstarts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_and_clip_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_length_axis1.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_rpad_length_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_toRegularArray.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_ListOffsetArray_toRegularArray.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_MaskedArray_getitem_next_jagged_project.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_pad_zero_to_length.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_pad_zero_to_length.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_adjust_starts_shifts_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_NumpyArray_reduce_mask_ByteMaskedArray_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_carry.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_jagged_expand.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_advanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_regularize.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_array_regularize.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_at.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_getitem_next_range_spreadadvanced.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_localindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_reduce_local_nextparents.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_reduce_local_nextparents.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_reduce_nonlocal_preparenext.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_reduce_nonlocal_preparenext.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_rpad_and_clip_axis1.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_RegularArray_rpad_and_clip_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillindex.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_fillindex.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_filltags.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_filltags.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_project.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_regular_index_getsize.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_regular_index_getsize.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_simplify.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_simplify.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_simplify_one.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_simplify_one.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_UnionArray_validity.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis0.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis0.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_index_rpad_and_clip_axis1.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_missing_repeat.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmax.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_argmin.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_count_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_countnonzero.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_max.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_min.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_prod_bool.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_bool.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int32_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_reduce_sum_int64_bool_64.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_sorting_ranges.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_sorting_ranges.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/awkward_sorting_ranges_length.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/awkward_sorting_ranges_length.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu` & `awkward-2.6.3rc2/src/awkward/_connect/cuda/cuda_kernels/cuda_common.cu`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/header-only/awkward/BuilderOptions.h` & `awkward-2.6.3rc2/src/awkward/_connect/header-only/awkward/BuilderOptions.h`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/header-only/awkward/GrowableBuffer.h` & `awkward-2.6.3rc2/src/awkward/_connect/header-only/awkward/GrowableBuffer.h`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/header-only/awkward/LayoutBuilder.h` & `awkward-2.6.3rc2/src/awkward/_connect/header-only/awkward/LayoutBuilder.h`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/header-only/awkward/utils.h` & `awkward-2.6.3rc2/src/awkward/_connect/header-only/awkward/utils.h`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/jax/reducers.py` & `awkward-2.6.3rc2/src/awkward/_connect/jax/reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/jax/trees.py` & `awkward-2.6.3rc2/src/awkward/_connect/jax/trees.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/numba/arrayview.py` & `awkward-2.6.3rc2/src/awkward/_connect/numba/arrayview.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/numba/arrayview_cuda.py` & `awkward-2.6.3rc2/src/awkward/_connect/numba/arrayview_cuda.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/numba/builder.py` & `awkward-2.6.3rc2/src/awkward/_connect/numba/builder.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/numba/growablebuffer.py` & `awkward-2.6.3rc2/src/awkward/_connect/numba/growablebuffer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/numba/layout.py` & `awkward-2.6.3rc2/src/awkward/_connect/numba/layout.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/numba/layoutbuilder.py` & `awkward-2.6.3rc2/src/awkward/_connect/numba/layoutbuilder.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/rdataframe/from_rdataframe.py` & `awkward-2.6.3rc2/src/awkward/_connect/rdataframe/from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/rdataframe/to_rdataframe.py` & `awkward-2.6.3rc2/src/awkward/_connect/rdataframe/to_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h` & `awkward-2.6.3rc2/src/awkward/_connect/rdataframe/include/rdataframe/jagged_builders.h`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_meta/bitmaskedmeta.py` & `awkward-2.6.3rc2/src/awkward/_meta/bitmaskedmeta.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_meta/bytemaskedmeta.py` & `awkward-2.6.3rc2/src/awkward/_meta/bytemaskedmeta.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_meta/emptymeta.py` & `awkward-2.6.3rc2/src/awkward/_meta/emptymeta.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_meta/indexedmeta.py` & `awkward-2.6.3rc2/src/awkward/_meta/indexedmeta.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_meta/indexedoptionmeta.py` & `awkward-2.6.3rc2/src/awkward/_meta/indexedoptionmeta.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_meta/listmeta.py` & `awkward-2.6.3rc2/src/awkward/_meta/listmeta.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_meta/listoffsetmeta.py` & `awkward-2.6.3rc2/src/awkward/_meta/listoffsetmeta.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_meta/meta.py` & `awkward-2.6.3rc2/src/awkward/_meta/meta.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_meta/numpymeta.py` & `awkward-2.6.3rc2/src/awkward/_meta/numpymeta.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_meta/recordmeta.py` & `awkward-2.6.3rc2/src/awkward/_meta/recordmeta.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_meta/regularmeta.py` & `awkward-2.6.3rc2/src/awkward/_meta/regularmeta.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_meta/unionmeta.py` & `awkward-2.6.3rc2/src/awkward/_meta/unionmeta.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_meta/unmaskedmeta.py` & `awkward-2.6.3rc2/src/awkward/_meta/unmaskedmeta.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_nplikes/__init__.py` & `awkward-2.6.3rc2/src/awkward/_nplikes/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_nplikes/array_like.py` & `awkward-2.6.3rc2/src/awkward/_nplikes/array_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_nplikes/array_module.py` & `awkward-2.6.3rc2/src/awkward/_nplikes/array_module.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_nplikes/cupy.py` & `awkward-2.6.3rc2/src/awkward/_nplikes/cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_nplikes/dispatch.py` & `awkward-2.6.3rc2/src/awkward/_nplikes/dispatch.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_nplikes/jax.py` & `awkward-2.6.3rc2/src/awkward/_nplikes/jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_nplikes/numpy.py` & `awkward-2.6.3rc2/src/awkward/_nplikes/numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_nplikes/numpy_like.py` & `awkward-2.6.3rc2/src/awkward/_nplikes/numpy_like.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     DType,
     Literal,
     NamedTuple,
     Protocol,
     TypeAlias,
     TypeVar,
 )
-from awkward.errors import AxisError
 
 if TYPE_CHECKING:
     from numpy.typing import DTypeLike
 
     from awkward._nplikes.placeholder import PlaceholderArray
 
 
@@ -80,15 +79,15 @@
     nan = numpy.nan
     inf = numpy.inf
 
     nat = numpy.datetime64("NaT")
     datetime_data = staticmethod(numpy.datetime_data)
     issubdtype = staticmethod(numpy.issubdtype)
 
-    AxisError = AxisError
+    AxisError = numpy.AxisError
 
 
 if hasattr(numpy, "float16"):
     NumpyMetadata.float16 = numpy.float16  # type: ignore[attr-defined]
 
 if hasattr(numpy, "float128"):
     NumpyMetadata.float128 = numpy.float128  # type: ignore[attr-defined]
```

### Comparing `awkward-2.6.3/src/awkward/_nplikes/placeholder.py` & `awkward-2.6.3rc2/src/awkward/_nplikes/placeholder.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_nplikes/shape.py` & `awkward-2.6.3rc2/src/awkward/_nplikes/shape.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_nplikes/typetracer.py` & `awkward-2.6.3rc2/src/awkward/_nplikes/typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/_nplikes/ufuncs.py` & `awkward-2.6.3rc2/src/awkward/_nplikes/ufuncs.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/behaviors/mixins.py` & `awkward-2.6.3rc2/src/awkward/behaviors/mixins.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/contents/__init__.py` & `awkward-2.6.3rc2/src/awkward/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/contents/bitmaskedarray.py` & `awkward-2.6.3rc2/src/awkward/contents/bitmaskedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/contents/bytemaskedarray.py` & `awkward-2.6.3rc2/src/awkward/contents/bytemaskedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/contents/content.py` & `awkward-2.6.3rc2/src/awkward/contents/content.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/contents/emptyarray.py` & `awkward-2.6.3rc2/src/awkward/contents/emptyarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/contents/indexedarray.py` & `awkward-2.6.3rc2/src/awkward/contents/indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/contents/indexedoptionarray.py` & `awkward-2.6.3rc2/src/awkward/contents/indexedoptionarray.py`

 * *Files 2% similar despite different names*

```diff
@@ -1590,23 +1590,34 @@
                 if isinstance(content, nplike.ma.MaskedArray):
                     mask1 = index_nplike.ma.getmaskarray(content)
                     mask = index_nplike.asarray(mask, copy=True)
                     mask[index_nplike.logical_not(mask0)] |= mask1
 
                 data[index_nplike.logical_not(mask0)] = content
 
-                if content.dtype.names is not None:
-                    missing_data = tuple(
-                        create_missing_data(each_dtype, backend)
-                        for each_dtype, _ in content.dtype.fields.values()
-                    )
+                if np.issubdtype(content.dtype, np.bool_):
+                    data[mask0] = False
+                elif np.issubdtype(content.dtype, np.floating):
+                    data[mask0] = np.nan
+                elif np.issubdtype(content.dtype, np.complexfloating):
+                    data[mask0] = np.nan + np.nan * 1j
+                elif np.issubdtype(content.dtype, np.integer):
+                    data[mask0] = np.iinfo(content.dtype).max
+                elif np.issubdtype(content.dtype.type, np.datetime64) or np.issubdtype(
+                    content.dtype.type, np.timedelta64
+                ):
+                    data[mask0] = nplike.asarray(
+                        [np.iinfo(np.int64).max], dtype=content.dtype
+                    )[0]
+                elif np.issubdtype(content.dtype, np.str_):
+                    data[mask0] = ""
+                elif np.issubdtype(content.dtype, np.bytes_):
+                    data[mask0] = b""
                 else:
-                    missing_data = create_missing_data(content.dtype, backend)
-
-                data[mask0] = missing_data
+                    raise AssertionError(f"unrecognized dtype: {content.dtype}")
 
                 return nplike.ma.MaskedArray(data, mask)
             else:
                 raise ValueError(
                     "Content.to_nplike cannot convert 'None' values to "
                     "np.ma.MaskedArray unless the "
                     "'allow_missing' parameter is set to True"
@@ -1760,34 +1771,7 @@
         return (
             self._is_equal_to_generic(other, all_parameters)
             and self._index.is_equal_to(other.index, index_dtype, numpyarray)
             and self._content._is_equal_to(
                 other.content, index_dtype, numpyarray, all_parameters
             )
         )
-
-
-def create_missing_data(dtype, backend):
-    """Create missing data based on the input dtype
-
-    Missing data are represented differently based on the Numpy array
-    dtype, this function returns the proper missing data representation
-    given the input dtype
-    """
-    if np.issubdtype(dtype, np.bool_):
-        return False
-    elif np.issubdtype(dtype, np.floating):
-        return np.nan
-    elif np.issubdtype(dtype, np.complexfloating):
-        return np.nan + np.nan * 1j
-    elif np.issubdtype(dtype, np.integer):
-        return np.iinfo(dtype).max
-    elif np.issubdtype(dtype.type, np.datetime64) or np.issubdtype(
-        dtype.type, np.timedelta64
-    ):
-        return backend.nplike.asarray([np.iinfo(np.int64).max], dtype=dtype)[0]
-    elif np.issubdtype(dtype, np.str_):
-        return ""
-    elif np.issubdtype(dtype, np.bytes_):
-        return b""
-    else:
-        raise AssertionError(f"unrecognized dtype: {dtype}")
```

### Comparing `awkward-2.6.3/src/awkward/contents/listarray.py` & `awkward-2.6.3rc2/src/awkward/contents/listarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/contents/listoffsetarray.py` & `awkward-2.6.3rc2/src/awkward/contents/listoffsetarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/contents/numpyarray.py` & `awkward-2.6.3rc2/src/awkward/contents/numpyarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/contents/recordarray.py` & `awkward-2.6.3rc2/src/awkward/contents/recordarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/contents/regulararray.py` & `awkward-2.6.3rc2/src/awkward/contents/regulararray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/contents/unionarray.py` & `awkward-2.6.3rc2/src/awkward/contents/unionarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/contents/unmaskedarray.py` & `awkward-2.6.3rc2/src/awkward/contents/unmaskedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/forms/__init__.py` & `awkward-2.6.3rc2/src/awkward/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/forms/bitmaskedform.py` & `awkward-2.6.3rc2/src/awkward/forms/bitmaskedform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/forms/bytemaskedform.py` & `awkward-2.6.3rc2/src/awkward/forms/bytemaskedform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/forms/emptyform.py` & `awkward-2.6.3rc2/src/awkward/forms/emptyform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/forms/form.py` & `awkward-2.6.3rc2/src/awkward/forms/form.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/forms/indexedform.py` & `awkward-2.6.3rc2/src/awkward/forms/indexedform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/forms/indexedoptionform.py` & `awkward-2.6.3rc2/src/awkward/forms/indexedoptionform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/forms/listform.py` & `awkward-2.6.3rc2/src/awkward/forms/listform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/forms/listoffsetform.py` & `awkward-2.6.3rc2/src/awkward/forms/listoffsetform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/forms/numpyform.py` & `awkward-2.6.3rc2/src/awkward/forms/numpyform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/forms/recordform.py` & `awkward-2.6.3rc2/src/awkward/forms/recordform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/forms/regularform.py` & `awkward-2.6.3rc2/src/awkward/forms/regularform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/forms/unionform.py` & `awkward-2.6.3rc2/src/awkward/forms/unionform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/forms/unmaskedform.py` & `awkward-2.6.3rc2/src/awkward/forms/unmaskedform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/numba/__init__.py` & `awkward-2.6.3rc2/src/awkward/numba/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/numba/layoutbuilder.py` & `awkward-2.6.3rc2/src/awkward/numba/layoutbuilder.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/__init__.py` & `awkward-2.6.3rc2/src/awkward/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_all.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_all.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_almost_equal.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_almost_equal.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_angle.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_angle.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_any.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_any.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_argcartesian.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_argcartesian.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_argcombinations.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_argcombinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_argmax.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_argmax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_argmin.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_argmin.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_argsort.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_argsort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_backend.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_broadcast_arrays.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_broadcast_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_broadcast_fields.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_broadcast_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_cartesian.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_cartesian.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_categories.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_categories.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_combinations.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_concatenate.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_concatenate.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_copy.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_copy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_corr.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_corr.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_count.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_count.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_count_nonzero.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_count_nonzero.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_covar.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_covar.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_drop_none.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_drop_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_enforce_type.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_enforce_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_fields.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_fill_none.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_fill_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_firsts.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_firsts.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_flatten.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_flatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_from_arrow.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_from_arrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_from_arrow_schema.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_from_arrow_schema.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_from_avro_file.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_from_avro_file.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_from_buffers.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_from_buffers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_from_categorical.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_from_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_from_cupy.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_from_cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_from_dlpack.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_from_dlpack.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_from_feather.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_from_feather.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_from_iter.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_from_iter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_from_jax.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_from_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_from_json.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_from_json.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_from_numpy.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_from_numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_from_parquet.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_from_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_from_rdataframe.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_from_regular.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_from_regular.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_full_like.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_full_like.py`

 * *Files 7% similar despite different names*

```diff
@@ -154,65 +154,70 @@
             if dtype is not None and including_unknown:
                 return layout.to_NumpyArray(dtype=dtype)
             else:
                 return None
 
         elif layout.parameter("__array__") in {"bytestring", "string"}:
             stringlike_type = layout.parameter("__array__")
-            charlike_type = "byte" if stringlike_type == "bytestring" else "char"
-
             if fill_value is _ZEROS:
-                # special case because output lists will all have length zero,
-                # rather than b"0" or "0" or something
                 asbytes = nplike.frombuffer(b"", dtype=np.uint8)
                 result = ak.contents.ListArray(
                     ak.index.Index64(
                         index_nplike.zeros(layout.length, dtype=np.int64),
                         nplike=index_nplike,
                     ),
                     ak.index.Index64(
                         index_nplike.zeros(layout.length, dtype=np.int64),
                         nplike=index_nplike,
                     ),
                     ak.contents.NumpyArray(
                         asbytes,
-                        parameters={"__array__": charlike_type},
+                        parameters={
+                            "__array__": "byte"
+                            if stringlike_type == "bytestring"
+                            else "char"
+                        },
                     ),
                     parameters={"__array__": stringlike_type},
                 )
 
-            else:
-                # NumPy 2.x converts "0" and b"0" (ASCII codec 48) to True (because it's not codec 0)
-                # NumPy 1.x converts them to False because it parses bytestrings and strings
-                # both versions of NumPy parse bytestrings and strings when converting to anything other than booleans
-                numpy2_behavior = nplike.astype(nplike.asarray(["0"]), dtype=np.bool_)[
-                    0
-                ]
-                if dtype == np.dtype(np.bool_) and numpy2_behavior:
-                    asbytes = b"\1" if fill_value else b"\0"
-                elif isinstance(fill_value, bytes):
+            elif stringlike_type == "bytestring":
+                if isinstance(fill_value, bytes):
                     asbytes = fill_value
                 else:
                     asbytes = str(fill_value).encode("utf-8", "surrogateescape")
-
                 asbytes = nplike.frombuffer(asbytes, dtype=np.uint8)
+
                 result = ak.contents.ListArray(
                     ak.index.Index64(
                         index_nplike.zeros(layout.length, dtype=np.int64),
                         nplike=index_nplike,
                     ),
                     ak.index.Index64(
                         index_nplike.full(layout.length, len(asbytes), dtype=np.int64)
                     ),
-                    ak.contents.NumpyArray(
-                        asbytes, parameters={"__array__": charlike_type}
-                    ),
-                    parameters={"__array__": stringlike_type},
+                    ak.contents.NumpyArray(asbytes, parameters={"__array__": "byte"}),
+                    parameters={"__array__": "bytestring"},
                 )
 
+            else:
+                assert stringlike_type == "string"
+                asstr = str(fill_value).encode("utf-8", "surrogateescape")
+                asbytes = nplike.frombuffer(asstr, dtype=np.uint8)
+                result = ak.contents.ListArray(
+                    ak.index.Index64(
+                        index_nplike.zeros(layout.length, dtype=np.int64),
+                        nplike=index_nplike,
+                    ),
+                    ak.index.Index64(
+                        index_nplike.full(layout.length, len(asbytes), dtype=np.int64)
+                    ),
+                    ak.contents.NumpyArray(asbytes, parameters={"__array__": "char"}),
+                    parameters={"__array__": "string"},
+                )
             if dtype is not None:
                 # Interpret strings as numeric/bool types
                 result = ak.operations.strings_astype(
                     result, dtype, highlevel=False, behavior=behavior
                 )
                 # Convert dtype
                 result = ak.operations.values_astype(
```

### Comparing `awkward-2.6.3/src/awkward/operations/ak_imag.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_imag.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_is_categorical.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_is_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_is_none.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_is_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_is_tuple.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_is_tuple.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_is_valid.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_is_valid.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_isclose.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_isclose.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_linear_fit.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_linear_fit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_local_index.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_local_index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_mask.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_mask.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_max.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_max.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_mean.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_mean.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_merge_option_of_records.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_merge_option_of_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_merge_union_of_records.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_merge_union_of_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_metadata_from_parquet.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_metadata_from_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_min.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_min.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_moment.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_moment.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_nan_to_none.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_nan_to_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_nan_to_num.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_nan_to_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_num.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_num.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_ones_like.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_ones_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_pad_none.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_pad_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_parameters.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_prod.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_prod.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_ptp.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_ptp.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_ravel.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_ravel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_real.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_real.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_round.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_round.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_run_lengths.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_run_lengths.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_singletons.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_singletons.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_softmax.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_softmax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_sort.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_std.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_std.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_strings_astype.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_strings_astype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_sum.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_sum.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_to_arrow.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_to_arrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_to_arrow_table.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_to_arrow_table.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_to_backend.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_to_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_to_buffers.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_to_buffers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_to_cupy.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_to_cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_to_dataframe.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_to_dataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_to_feather.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_to_feather.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_to_jax.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_to_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_to_json.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_to_json.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_to_layout.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_to_layout.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_to_list.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_to_list.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_to_numpy.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_to_numpy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_to_packed.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_to_packed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_to_parquet.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_to_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_to_parquet_dataset.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_to_parquet_dataset.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_to_parquet_row_groups.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_to_parquet_row_groups.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_to_rdataframe.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_to_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_to_regular.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_to_regular.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_transform.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_transform.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_type.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_unflatten.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_unflatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_unzip.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_unzip.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_validity_error.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_validity_error.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_values_astype.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_values_astype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_var.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_var.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_where.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_where.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_with_field.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_with_name.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_with_name.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_with_parameter.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_with_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_without_field.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_without_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_without_parameters.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_without_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_zeros_like.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_zeros_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/ak_zip.py` & `awkward-2.6.3rc2/src/awkward/operations/ak_zip.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/__init__.py` & `awkward-2.6.3rc2/src/awkward/operations/str/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_capitalize.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_capitalize.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_center.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_center.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_count_substring.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_count_substring.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_count_substring_regex.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_count_substring_regex.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_ends_with.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_ends_with.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_extract_regex.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_extract_regex.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_find_substring.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_find_substring.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_find_substring_regex.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_find_substring_regex.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_index_in.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_index_in.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_is_alnum.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_is_alnum.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_is_alpha.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_is_alpha.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_is_ascii.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_is_ascii.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_is_decimal.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_is_decimal.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_is_digit.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_is_digit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_is_in.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_is_in.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_is_lower.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_is_lower.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_is_numeric.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_is_numeric.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_is_printable.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_is_printable.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_is_space.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_is_space.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_is_title.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_is_title.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_is_upper.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_is_upper.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_join.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_join.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_join_element_wise.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_join_element_wise.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_length.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_length.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_lower.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_lower.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_lpad.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_lpad.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_ltrim.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_ltrim.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_ltrim_whitespace.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_ltrim_whitespace.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_match_like.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_match_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_match_substring.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_match_substring.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_match_substring_regex.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_match_substring_regex.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_repeat.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_repeat.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_replace_slice.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_replace_slice.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_replace_substring.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_replace_substring.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_replace_substring_regex.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_replace_substring_regex.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_reverse.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_reverse.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_rpad.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_rpad.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_rtrim.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_rtrim.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_rtrim_whitespace.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_rtrim_whitespace.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_slice.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_slice.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_split_pattern.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_split_pattern.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_split_pattern_regex.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_split_pattern_regex.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_split_whitespace.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_split_whitespace.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_starts_with.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_starts_with.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_swapcase.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_swapcase.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_title.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_title.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_to_categorical.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_to_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_trim.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_trim.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_trim_whitespace.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_trim_whitespace.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/operations/str/akstr_upper.py` & `awkward-2.6.3rc2/src/awkward/operations/str/akstr_upper.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/types/__init__.py` & `awkward-2.6.3rc2/src/awkward/types/__init__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/types/_awkward_datashape_parser.py` & `awkward-2.6.3rc2/src/awkward/types/_awkward_datashape_parser.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/types/arraytype.py` & `awkward-2.6.3rc2/src/awkward/types/arraytype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/types/listtype.py` & `awkward-2.6.3rc2/src/awkward/types/listtype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/types/numpytype.py` & `awkward-2.6.3rc2/src/awkward/types/numpytype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/types/optiontype.py` & `awkward-2.6.3rc2/src/awkward/types/optiontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/types/recordtype.py` & `awkward-2.6.3rc2/src/awkward/types/recordtype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/types/regulartype.py` & `awkward-2.6.3rc2/src/awkward/types/regulartype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/types/scalartype.py` & `awkward-2.6.3rc2/src/awkward/types/scalartype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/types/type.py` & `awkward-2.6.3rc2/src/awkward/types/type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/types/uniontype.py` & `awkward-2.6.3rc2/src/awkward/types/uniontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/src/awkward/types/unknowntype.py` & `awkward-2.6.3rc2/src/awkward/types/unknowntype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0002_minimal_listarray.py` & `awkward-2.6.3rc2/tests/test_0002_minimal_listarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0006_deep_iteration.py` & `awkward-2.6.3rc2/tests/test_0006_deep_iteration.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0008_slices_and_getitem.py` & `awkward-2.6.3rc2/tests/test_0008_slices_and_getitem.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0011_listarray.py` & `awkward-2.6.3rc2/tests/test_0011_listarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0013_error_handling_struct.py` & `awkward-2.6.3rc2/tests/test_0013_error_handling_struct.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0014_finish_up_getitem.py` & `awkward-2.6.3rc2/tests/test_0014_finish_up_getitem.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0018_fromiter_fillable.py` & `awkward-2.6.3rc2/tests/test_0018_fromiter_fillable.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0019_use_json_library.py` & `awkward-2.6.3rc2/tests/test_0019_use_json_library.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0020_support_unsigned_indexes.py` & `awkward-2.6.3rc2/tests/test_0020_support_unsigned_indexes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0021_emptyarray.py` & `awkward-2.6.3rc2/tests/test_0021_emptyarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0023_regular_array.py` & `awkward-2.6.3rc2/tests/test_0023_regular_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0024_use_regular_array.py` & `awkward-2.6.3rc2/tests/test_0024_use_regular_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0025_record_array.py` & `awkward-2.6.3rc2/tests/test_0025_record_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0028_add_dressed_types.py` & `awkward-2.6.3rc2/tests/test_0028_add_dressed_types.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0032_replace_dressedtype.py` & `awkward-2.6.3rc2/tests/test_0032_replace_dressedtype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0046_start_indexedarray.py` & `awkward-2.6.3rc2/tests/test_0046_start_indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0049_distinguish_record_and_recordarray_behaviors.py` & `awkward-2.6.3rc2/tests/test_0049_distinguish_record_and_recordarray_behaviors.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0057_introducing_forms.py` & `awkward-2.6.3rc2/tests/test_0057_introducing_forms.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0070_argmin_and_argmax.py` & `awkward-2.6.3rc2/tests/test_0070_argmin_and_argmax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0072_fillna_operation.py` & `awkward-2.6.3rc2/tests/test_0072_fillna_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0074_argsort_and_sort.py` & `awkward-2.6.3rc2/tests/test_0074_argsort_and_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0077_zip_operation.py` & `awkward-2.6.3rc2/tests/test_0077_zip_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0078_argcross_and_cross.py` & `awkward-2.6.3rc2/tests/test_0078_argcross_and_cross.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0079_argchoose_and_choose.py` & `awkward-2.6.3rc2/tests/test_0079_argchoose_and_choose.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0080_flatpandas_multiindex_rows_and_columns.py` & `awkward-2.6.3rc2/tests/test_0080_flatpandas_multiindex_rows_and_columns.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0084_start_unionarray.py` & `awkward-2.6.3rc2/tests/test_0084_start_unionarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0086_nep13_ufunc.py` & `awkward-2.6.3rc2/tests/test_0086_nep13_ufunc.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0089_numpy_functions.py` & `awkward-2.6.3rc2/tests/test_0089_numpy_functions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0093_simplify_uniontypes_and_optiontypes.py` & `awkward-2.6.3rc2/tests/test_0093_simplify_uniontypes_and_optiontypes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0107_assign_fields_to_records.py` & `awkward-2.6.3rc2/tests/test_0107_assign_fields_to_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0111_jagged_and_masked_getitem.py` & `awkward-2.6.3rc2/tests/test_0111_jagged_and_masked_getitem.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0115_generic_reducer_operation.py` & `awkward-2.6.3rc2/tests/test_0115_generic_reducer_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0118_numba_cpointers.py` & `awkward-2.6.3rc2/tests/test_0118_numba_cpointers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0119_numexpr_and_broadcast_arrays.py` & `awkward-2.6.3rc2/tests/test_0119_numexpr_and_broadcast_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0124_strings_in_numba.py` & `awkward-2.6.3rc2/tests/test_0124_strings_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0127_tomask_operation.py` & `awkward-2.6.3rc2/tests/test_0127_tomask_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0127b_tomask_operation_numba.py` & `awkward-2.6.3rc2/tests/test_0127b_tomask_operation_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0138_emptyarray_type.py` & `awkward-2.6.3rc2/tests/test_0138_emptyarray_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0150_flatten.py` & `awkward-2.6.3rc2/tests/test_0150_flatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0163_negative_axis_wrap.py` & `awkward-2.6.3rc2/tests/test_0163_negative_axis_wrap.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0166_0167_0170_random_issues.py` & `awkward-2.6.3rc2/tests/test_0166_0167_0170_random_issues.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0173_astype_operation.py` & `awkward-2.6.3rc2/tests/test_0173_astype_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0184_concatenate_operation.py` & `awkward-2.6.3rc2/tests/test_0184_concatenate_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0193_is_none_axis_parameter.py` & `awkward-2.6.3rc2/tests/test_0193_is_none_axis_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0198_tutorial_documentation_1.py` & `awkward-2.6.3rc2/tests/test_0198_tutorial_documentation_1.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0222_count_with_axis0.py` & `awkward-2.6.3rc2/tests/test_0222_count_with_axis0.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0224_arrow_to_awkward.py` & `awkward-2.6.3rc2/tests/test_0224_arrow_to_awkward.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0264_reduce_last_empty.py` & `awkward-2.6.3rc2/tests/test_0264_reduce_last_empty.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0273_path_for_with_field.py` & `awkward-2.6.3rc2/tests/test_0273_path_for_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0286_broadcast_single_value_with_field.py` & `awkward-2.6.3rc2/tests/test_0286_broadcast_single_value_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0290_bug_fixes_for_hats.py` & `awkward-2.6.3rc2/tests/test_0290_bug_fixes_for_hats.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0315_integerindex.py` & `awkward-2.6.3rc2/tests/test_0315_integerindex.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0331_pandas_indexedarray.py` & `awkward-2.6.3rc2/tests/test_0331_pandas_indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0334_fully_broadcastable_where.py` & `awkward-2.6.3rc2/tests/test_0334_fully_broadcastable_where.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0339_highlevel_sorting_function.py` & `awkward-2.6.3rc2/tests/test_0339_highlevel_sorting_function.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0348_form_keys.py` & `awkward-2.6.3rc2/tests/test_0348_form_keys.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0355_mixins.py` & `awkward-2.6.3rc2/tests/test_0355_mixins.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0395_complex_type_arrays.py` & `awkward-2.6.3rc2/tests/test_0395_complex_type_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0395_fix_numba_indexedarray.py` & `awkward-2.6.3rc2/tests/test_0395_fix_numba_indexedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0397_arrays_as_constants_in_numba.py` & `awkward-2.6.3rc2/tests/test_0397_arrays_as_constants_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0401_add_categorical_type_for_arrow_dictionary.py` & `awkward-2.6.3rc2/tests/test_0401_add_categorical_type_for_arrow_dictionary.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0404_array_validity_check.py` & `awkward-2.6.3rc2/tests/test_0404_array_validity_check.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0410_fix_argminmax_positions_for_missing_values.py` & `awkward-2.6.3rc2/tests/test_0410_fix_argminmax_positions_for_missing_values.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0437_stream_of_many_json_files.py` & `awkward-2.6.3rc2/tests/test_0437_stream_of_many_json_files.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0447_preserve_regularness_in_reduce.py` & `awkward-2.6.3rc2/tests/test_0447_preserve_regularness_in_reduce.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0449_merge_many_arrays_in_one_pass.py` & `awkward-2.6.3rc2/tests/test_0449_merge_many_arrays_in_one_pass.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0493_zeros_ones_full_like.py` & `awkward-2.6.3rc2/tests/test_0493_zeros_ones_full_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0496_provide_local_index.py` & `awkward-2.6.3rc2/tests/test_0496_provide_local_index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0499_getitem_indexedarray_bug.py` & `awkward-2.6.3rc2/tests/test_0499_getitem_indexedarray_bug.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0504_block_ufuncs_for_strings.py` & `awkward-2.6.3rc2/tests/test_0504_block_ufuncs_for_strings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0511_copy_and_deepcopy.py` & `awkward-2.6.3rc2/tests/test_0511_copy_and_deepcopy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py` & `awkward-2.6.3rc2/tests/test_0527_fix_unionarray_ufuncs_and_parameters_in_merging.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0549_numba_array_asarray.py` & `awkward-2.6.3rc2/tests/test_0549_numba_array_asarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0557_min_max_initial_argument.py` & `awkward-2.6.3rc2/tests/test_0557_min_max_initial_argument.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0559_fix_booleans_in_numba.py` & `awkward-2.6.3rc2/tests/test_0559_fix_booleans_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0572_numba_array_ndim.py` & `awkward-2.6.3rc2/tests/test_0572_numba_array_ndim.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0582_propagate_context_in_broadcast_and_apply.py` & `awkward-2.6.3rc2/tests/test_0582_propagate_context_in_broadcast_and_apply.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0583_implement_unflatten_function.py` & `awkward-2.6.3rc2/tests/test_0583_implement_unflatten_function.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0590_allow_regulararray_size_zero.py` & `awkward-2.6.3rc2/tests/test_0590_allow_regulararray_size_zero.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py` & `awkward-2.6.3rc2/tests/test_0593_preserve_nullability_in_arrow_and_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0652_tests_of_complex_numbers.py` & `awkward-2.6.3rc2/tests/test_0652_tests_of_complex_numbers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0674_categorical_validation.py` & `awkward-2.6.3rc2/tests/test_0674_categorical_validation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0713_getitem_field_should_simplify_optiontype.py` & `awkward-2.6.3rc2/tests/test_0713_getitem_field_should_simplify_optiontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py` & `awkward-2.6.3rc2/tests/test_0723_ensure_that_jagged_slice_fits_array_length.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0730_unflatten_axis_parameter.py` & `awkward-2.6.3rc2/tests/test_0730_unflatten_axis_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0733_run_lengths.py` & `awkward-2.6.3rc2/tests/test_0733_run_lengths.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0736_implement_argsort_for_strings.py` & `awkward-2.6.3rc2/tests/test_0736_implement_argsort_for_strings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0766_prevent_combinations_of_characters.py` & `awkward-2.6.3rc2/tests/test_0766_prevent_combinations_of_characters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0773_typeparser.py` & `awkward-2.6.3rc2/tests/test_0773_typeparser.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0788_indexedarray_carrying_recordarray_parameters.py` & `awkward-2.6.3rc2/tests/test_0788_indexedarray_carrying_recordarray_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0794_ak_cartesian_on_empty_array.py` & `awkward-2.6.3rc2/tests/test_0794_ak_cartesian_on_empty_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0803_argsort_fix_type.py` & `awkward-2.6.3rc2/tests/test_0803_argsort_fix_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0806_empty_lists_cartesian_fix.py` & `awkward-2.6.3rc2/tests/test_0806_empty_lists_cartesian_fix.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0813_full_like_dtype_arg.py` & `awkward-2.6.3rc2/tests/test_0813_full_like_dtype_arg.py`

 * *Files 13% similar despite different names*

```diff
@@ -140,63 +140,7 @@
     bool_type = ak.operations.ones_like(array, dtype=bool)
     assert int_type64.to_list() == float_type.to_list()
     assert int_type64.to_list() == bool_type.to_list()
     assert_array_type(int_type32, np.int32)
     assert_array_type(int_type64, np.int64)
     assert_array_type(float_type, float)
     assert_array_type(bool_type, np.bool_)
-
-
-def test_numpy2_changes():
-    numpy2_behavior = np.asarray(["0"]).astype(np.bool_)[0]
-
-    if numpy2_behavior:
-        assert ak.full_like([[True, False], [], [True]], b"0").to_list() == [
-            [True, True],
-            [],
-            [True],
-        ]
-        assert ak.full_like([[True, False], [], [True]], "0").to_list() == [
-            [True, True],
-            [],
-            [True],
-        ]
-
-    else:
-        assert ak.full_like([[True, False], [], [True]], b"0").to_list() == [
-            [False, False],
-            [],
-            [False],
-        ]
-        assert ak.full_like([[True, False], [], [True]], "0").to_list() == [
-            [False, False],
-            [],
-            [False],
-        ]
-
-    assert ak.full_like(
-        [["one", "two"], [], ["three"]], 0, dtype=np.bool_
-    ).to_list() == [[False, False], [], [False]]
-    assert ak.full_like(
-        [[b"one", b"two"], [], [b"three"]], 0, dtype=np.bool_
-    ).to_list() == [[False, False], [], [False]]
-
-    assert ak.full_like([["one", "two"], [], ["three"]], "0").to_list() == [
-        ["0", "0"],
-        [],
-        ["0"],
-    ]
-    assert ak.full_like([["one", "two"], [], ["three"]], b"0").to_list() == [
-        ["0", "0"],
-        [],
-        ["0"],
-    ]
-    assert ak.full_like([[b"one", b"two"], [], [b"three"]], "0").to_list() == [
-        [b"0", b"0"],
-        [],
-        [b"0"],
-    ]
-    assert ak.full_like([[b"one", b"two"], [], [b"three"]], b"0").to_list() == [
-        [b"0", b"0"],
-        [],
-        [b"0"],
-    ]
```

### Comparing `awkward-2.6.3/tests/test_0815_broadcast_union_types_to_all_possibilities.py` & `awkward-2.6.3rc2/tests/test_0815_broadcast_union_types_to_all_possibilities.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0819_issue.py` & `awkward-2.6.3rc2/tests/test_0819_issue.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0828_arrow_datatype_null.py` & `awkward-2.6.3rc2/tests/test_0828_arrow_datatype_null.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0835_datetime_type.py` & `awkward-2.6.3rc2/tests/test_0835_datetime_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0835_datetime_type_pandas.py` & `awkward-2.6.3rc2/tests/test_0835_datetime_type_pandas.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0835_datetime_type_pyarrow.py` & `awkward-2.6.3rc2/tests/test_0835_datetime_type_pyarrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0850_argsort_mask_array.py` & `awkward-2.6.3rc2/tests/test_0850_argsort_mask_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0866_getitem_field_and_flatten_unions.py` & `awkward-2.6.3rc2/tests/test_0866_getitem_field_and_flatten_unions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0875_arrow_null_type.py` & `awkward-2.6.3rc2/tests/test_0875_arrow_null_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0879_non_primitive_with_field.py` & `awkward-2.6.3rc2/tests/test_0879_non_primitive_with_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0884_index_and_identifier_refactoring.py` & `awkward-2.6.3rc2/tests/test_0884_index_and_identifier_refactoring.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0889_ptp.py` & `awkward-2.6.3rc2/tests/test_0889_ptp.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0896_content_classes_refactoring.py` & `awkward-2.6.3rc2/tests/test_0896_content_classes_refactoring.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0898_unzip_heterogeneous_records.py` & `awkward-2.6.3rc2/tests/test_0898_unzip_heterogeneous_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0905_leading_zeros_in_unflatten.py` & `awkward-2.6.3rc2/tests/test_0905_leading_zeros_in_unflatten.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0906_arrow_fixed_size_list_type.py` & `awkward-2.6.3rc2/tests/test_0906_arrow_fixed_size_list_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0910_unflatten_counts_relation.py` & `awkward-2.6.3rc2/tests/test_0910_unflatten_counts_relation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0912_packed.py` & `awkward-2.6.3rc2/tests/test_0912_packed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0914_types_and_forms.py` & `awkward-2.6.3rc2/tests/test_0914_types_and_forms.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0916_datetime_values_astype.py` & `awkward-2.6.3rc2/tests/test_0916_datetime_values_astype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0927_numpy_array_nbytes.py` & `awkward-2.6.3rc2/tests/test_0927_numpy_array_nbytes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0930_bug_in_unionarray_purelist_parameter.py` & `awkward-2.6.3rc2/tests/test_0930_bug_in_unionarray_purelist_parameter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0945_argsort_sort_nan_array.py` & `awkward-2.6.3rc2/tests/test_0945_argsort_sort_nan_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0958_new_forms_must_accept_old_form_json.py` & `awkward-2.6.3rc2/tests/test_0958_new_forms_must_accept_old_form_json.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0959__getitem_array_implementation.py` & `awkward-2.6.3rc2/tests/test_0959__getitem_array_implementation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0975_mask_multidimensional_numpy_array.py` & `awkward-2.6.3rc2/tests/test_0975_mask_multidimensional_numpy_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0979_where_multidimentional_numpy_array.py` & `awkward-2.6.3rc2/tests/test_0979_where_multidimentional_numpy_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0982_missing_case_in_nonlocal_reducers.py` & `awkward-2.6.3rc2/tests/test_0982_missing_case_in_nonlocal_reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0984_ravel.py` & `awkward-2.6.3rc2/tests/test_0984_ravel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_0992_correct_ptp_unmasking.py` & `awkward-2.6.3rc2/tests/test_0992_correct_ptp_unmasking.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py` & `awkward-2.6.3rc2/tests/test_1000_fixes_argmax_for_ListOffsetArray_with_nonzero_start.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1017_numpyarray_broadcast.py` & `awkward-2.6.3rc2/tests/test_1017_numpyarray_broadcast.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1030_mixin_class_name.py` & `awkward-2.6.3rc2/tests/test_1030_mixin_class_name.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1031_start_getitem_next.py` & `awkward-2.6.3rc2/tests/test_1031_start_getitem_next.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1031b_start_getitem_next_specialized.py` & `awkward-2.6.3rc2/tests/test_1031b_start_getitem_next_specialized.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1049_concatenate_single_array.py` & `awkward-2.6.3rc2/tests/test_1049_concatenate_single_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1055_fill_none_numpy_dimension.py` & `awkward-2.6.3rc2/tests/test_1055_fill_none_numpy_dimension.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1059_localindex.py` & `awkward-2.6.3rc2/tests/test_1059_localindex.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1066_to_numpy_masked_structured_array.py` & `awkward-2.6.3rc2/tests/test_1066_to_numpy_masked_structured_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1071_mask_identity_false_should_not_return_option_type.py` & `awkward-2.6.3rc2/tests/test_1071_mask_identity_false_should_not_return_option_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1072_sort.py` & `awkward-2.6.3rc2/tests/test_1072_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1074_combinations.py` & `awkward-2.6.3rc2/tests/test_1074_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1075_validityerror.py` & `awkward-2.6.3rc2/tests/test_1075_validityerror.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1110_type_tracer_1.py` & `awkward-2.6.3rc2/tests/test_1110_type_tracer_1.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1116_project_maskedarrays.py` & `awkward-2.6.3rc2/tests/test_1116_project_maskedarrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1125_to_arrow_from_arrow.py` & `awkward-2.6.3rc2/tests/test_1125_to_arrow_from_arrow.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1132_utility_methods_for_highlevel_functions.py` & `awkward-2.6.3rc2/tests/test_1132_utility_methods_for_highlevel_functions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1134_from_buffers_to_buffers.py` & `awkward-2.6.3rc2/tests/test_1134_from_buffers_to_buffers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1135_rpad_operation.py` & `awkward-2.6.3rc2/tests/test_1135_rpad_operation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1136_regulararray_zeros_in_shape.py` & `awkward-2.6.3rc2/tests/test_1136_regulararray_zeros_in_shape.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1137_num.py` & `awkward-2.6.3rc2/tests/test_1137_num.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from __future__ import annotations
 
 import numpy as np
 import pytest
 
 import awkward as ak
-from awkward.errors import AxisError
 
 to_list = ak.operations.to_list
 
 
 def test_bytemaskedarray_num():
     content = ak.operations.from_iter(
         [
@@ -40,30 +39,30 @@
     assert to_list(ak.num(array, axis=-1)) == [[3, 0, 2], [], None, None, [0, 3]]
 
 
 def test_emptyarray():
     array = ak.contents.EmptyArray()
     assert to_list(ak.num(array, 0)) == 0
     assert to_list(ak.num(array, -1)) == 0
-    with pytest.raises(AxisError) as err:
+    with pytest.raises(np.AxisError) as err:
         ak.num(array, 1)
     assert "axis=1 exceeds the depth" in str(err.value)
 
 
 def test_numpyarray():
     array = ak.contents.NumpyArray(np.arange(2 * 3 * 5 * 7).reshape(2, 3, 5, 7))
 
     assert ak.num(array, 0) == 2
     assert to_list(ak.num(array, 1)) == [3, 3]
     assert to_list(ak.num(array, axis=2)) == [[5, 5, 5], [5, 5, 5]]
     assert to_list(ak.num(array, 3)) == [
         [[7, 7, 7, 7, 7], [7, 7, 7, 7, 7], [7, 7, 7, 7, 7]],
         [[7, 7, 7, 7, 7], [7, 7, 7, 7, 7], [7, 7, 7, 7, 7]],
     ]
-    with pytest.raises(AxisError) as err:
+    with pytest.raises(np.AxisError) as err:
         ak.num(array, 4)
     assert "axis=4 exceeds the depth" in str(err.value)
 
 
 def test_regulararray():
     array = ak.contents.NumpyArray(
         np.arange(2 * 3 * 5 * 7).reshape(2, 3, 5, 7)
@@ -72,15 +71,15 @@
     assert ak.num(array, 0) == 2
     assert to_list(ak.num(array, 1)) == [3, 3]
     assert to_list(ak.num(array, 2)) == [[5, 5, 5], [5, 5, 5]]
     assert to_list(ak.num(array, 3)) == [
         [[7, 7, 7, 7, 7], [7, 7, 7, 7, 7], [7, 7, 7, 7, 7]],
         [[7, 7, 7, 7, 7], [7, 7, 7, 7, 7], [7, 7, 7, 7, 7]],
     ]
-    with pytest.raises(AxisError) as err:
+    with pytest.raises(np.AxisError) as err:
         ak.num(array, 4)
     assert "axis=4 exceeds the depth" in str(err.value)
 
     empty = ak.contents.RegularArray(
         ak.highlevel.Array([[1, 2, 3], [], [4, 5]]).layout, 0, zeros_length=0
     )
 
@@ -109,15 +108,15 @@
     assert to_list(ak.num(array, 1)) == [3, 0, 2]
     assert to_list(ak.num(array, 2)) == [[3, 3, 3], [], [3, 3]]
     assert to_list(ak.num(array, 3)) == [
         [[2, 2, 2], [2, 2, 2], [2, 2, 2]],
         [],
         [[2, 2, 2], [2, 2, 2]],
     ]
-    with pytest.raises(AxisError) as err:
+    with pytest.raises(np.AxisError) as err:
         ak.num(array, 4)
     assert "axis=4 exceeds the depth" in str(err.value)
 
 
 def test_listoffsetarray():
     content = ak.contents.NumpyArray(np.arange(2 * 3 * 5).reshape(5, 3, 2))
     offsets = ak.index.Index64(np.array([0, 3, 3, 5], dtype=np.int64))
@@ -137,15 +136,15 @@
     assert to_list(ak.num(array, 1)) == [3, 0, 2]
     assert to_list(ak.num(array, 2)) == [[3, 3, 3], [], [3, 3]]
     assert to_list(ak.num(array, 3)) == [
         [[2, 2, 2], [2, 2, 2], [2, 2, 2]],
         [],
         [[2, 2, 2], [2, 2, 2]],
     ]
-    with pytest.raises(AxisError) as err:
+    with pytest.raises(np.AxisError) as err:
         ak.num(array, 4)
     assert "axis=4 exceeds the depth" in str(err.value)
 
 
 def test_indexedarray():
     content = ak.contents.NumpyArray(np.arange(2 * 3 * 5).reshape(5, 3, 2))
     offsets = ak.index.Index64(np.array([0, 3, 3, 5], dtype=np.int64))
@@ -170,15 +169,15 @@
     assert to_list(ak.num(array, 3)) == [
         [[2, 2, 2], [2, 2, 2]],
         [[2, 2, 2], [2, 2, 2]],
         [],
         [[2, 2, 2], [2, 2, 2], [2, 2, 2]],
     ]
 
-    with pytest.raises(AxisError) as err:
+    with pytest.raises(np.AxisError) as err:
         ak.num(array, 4)
     assert "axis=4 exceeds the depth" in str(err.value)
 
 
 def test_indexedoptionarray():
     content = ak.contents.NumpyArray(np.arange(2 * 3 * 5).reshape(5, 3, 2))
     offsets = ak.index.Index64(np.array([0, 3, 3, 5], dtype=np.int64))
@@ -207,15 +206,15 @@
         None,
         [[2, 2, 2], [2, 2, 2]],
         [],
         None,
         [[2, 2, 2], [2, 2, 2], [2, 2, 2]],
     ]
 
-    with pytest.raises(AxisError) as err:
+    with pytest.raises(np.AxisError) as err:
         ak.num(array, 4)
     assert "axis=4 exceeds the depth" in str(err.value)
 
 
 def test_recordarray():
     array = ak.operations.from_iter(
         [
```

### Comparing `awkward-2.6.3/tests/test_1142_numbers_to_type.py` & `awkward-2.6.3rc2/tests/test_1142_numbers_to_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1149_datetime_sort.py` & `awkward-2.6.3rc2/tests/test_1149_datetime_sort.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1154_arrow_tables_should_preserve_parameters.py` & `awkward-2.6.3rc2/tests/test_1154_arrow_tables_should_preserve_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1162_ak_from_json_schema.py` & `awkward-2.6.3rc2/tests/test_1162_ak_from_json_schema.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1183_bugs_found_by_dask_project_2.py` & `awkward-2.6.3rc2/tests/test_1183_bugs_found_by_dask_project_2.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1189_fix_singletons_for_non_optional_data.py` & `awkward-2.6.3rc2/tests/test_1189_fix_singletons_for_non_optional_data.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1192_iterables_in___array_function__.py` & `awkward-2.6.3rc2/tests/test_1192_iterables_in___array_function__.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1193_is_none_nested_option.py` & `awkward-2.6.3rc2/tests/test_1193_is_none_nested_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1233_ak_with_name.py` & `awkward-2.6.3rc2/tests/test_1233_ak_with_name.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1240_v2_implementation_of_numba_1.py` & `awkward-2.6.3rc2/tests/test_1240_v2_implementation_of_numba_1.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1259_simplify_optiontype.py` & `awkward-2.6.3rc2/tests/test_1259_simplify_optiontype.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1260_simplify_masked_option_types.py` & `awkward-2.6.3rc2/tests/test_1260_simplify_masked_option_types.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1271_fix_4D_reducers.py` & `awkward-2.6.3rc2/tests/test_1271_fix_4D_reducers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1294_to_and_from_parquet.py` & `awkward-2.6.3rc2/tests/test_1294_to_and_from_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py` & `awkward-2.6.3rc2/tests/test_1298_allow_nan_to_num_arguments_to_be_arrays.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1300_awkward_to_cpp_converter_with_cling.py` & `awkward-2.6.3rc2/tests/test_1300_awkward_to_cpp_converter_with_cling.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1300b_same_for_numba.py` & `awkward-2.6.3rc2/tests/test_1300b_same_for_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1308_zip_after_option.py` & `awkward-2.6.3rc2/tests/test_1308_zip_after_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1318_array_function_types.py` & `awkward-2.6.3rc2/tests/test_1318_array_function_types.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1320_mask_identity_defaults.py` & `awkward-2.6.3rc2/tests/test_1320_mask_identity_defaults.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1344_broadcast_arrays_depth_limit.py` & `awkward-2.6.3rc2/tests/test_1344_broadcast_arrays_depth_limit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1345_avro_reader.py` & `awkward-2.6.3rc2/tests/test_1345_avro_reader.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1351_is_tuple.py` & `awkward-2.6.3rc2/tests/test_1351_is_tuple.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1374_to_rdataframe.py` & `awkward-2.6.3rc2/tests/test_1374_to_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1377_ravel_string.py` & `awkward-2.6.3rc2/tests/test_1377_ravel_string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1379_reducers_with_axis_None_and_typetracers.py` & `awkward-2.6.3rc2/tests/test_1379_reducers_with_axis_None_and_typetracers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1399_from_jax.py` & `awkward-2.6.3rc2/tests/test_1399_from_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1399_to_jax.py` & `awkward-2.6.3rc2/tests/test_1399_to_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1405_slicing_untested_cases.py` & `awkward-2.6.3rc2/tests/test_1405_slicing_untested_cases.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1415_behaviour_forwarding.py` & `awkward-2.6.3rc2/tests/test_1415_behaviour_forwarding.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1440_start_v2_to_parquet.py` & `awkward-2.6.3rc2/tests/test_1440_start_v2_to_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1447_jax_autodiff_slices_ufuncs.py` & `awkward-2.6.3rc2/tests/test_1447_jax_autodiff_slices_ufuncs.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1449_v2_to_json_from_json_functions.py` & `awkward-2.6.3rc2/tests/test_1449_v2_to_json_from_json_functions.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1453_write_single_records_to_parquet.py` & `awkward-2.6.3rc2/tests/test_1453_write_single_records_to_parquet.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1473_from_rdataframe.py` & `awkward-2.6.3rc2/tests/test_1473_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1477_generator_entry_type_as_rvec.py` & `awkward-2.6.3rc2/tests/test_1477_generator_entry_type_as_rvec.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1490_jax_reducers_combinations.py` & `awkward-2.6.3rc2/tests/test_1490_jax_reducers_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1502_getitem_jagged_issue1406.py` & `awkward-2.6.3rc2/tests/test_1502_getitem_jagged_issue1406.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1504_typetracer_like.py` & `awkward-2.6.3rc2/tests/test_1504_typetracer_like.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1508_awkward_from_rdataframe.py` & `awkward-2.6.3rc2/tests/test_1508_awkward_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1511_set_attribute.py` & `awkward-2.6.3rc2/tests/test_1511_set_attribute.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1539_isnone_axis_check_issue1417.py` & `awkward-2.6.3rc2/tests/test_1539_isnone_axis_check_issue1417.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1559_fix_ufuncs_records_1439.py` & `awkward-2.6.3rc2/tests/test_1559_fix_ufuncs_records_1439.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1565_axis_wrap_if_negative_record.py` & `awkward-2.6.3rc2/tests/test_1565_axis_wrap_if_negative_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1567_fix_longlong_in_Index.py` & `awkward-2.6.3rc2/tests/test_1567_fix_longlong_in_Index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1568_fix_lengths_empty_regular_slices.py` & `awkward-2.6.3rc2/tests/test_1568_fix_lengths_empty_regular_slices.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1586_concatenate_should_preserve_regulararray.py` & `awkward-2.6.3rc2/tests/test_1586_concatenate_should_preserve_regulararray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1604_preserve_form_in_concatenate.py` & `awkward-2.6.3rc2/tests/test_1604_preserve_form_in_concatenate.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1607_no_reducers_on_records.py` & `awkward-2.6.3rc2/tests/test_1607_no_reducers_on_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1613_generator_tolayout_records.py` & `awkward-2.6.3rc2/tests/test_1613_generator_tolayout_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1619_from_parquet_empty_field.py` & `awkward-2.6.3rc2/tests/test_1619_from_parquet_empty_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1620_layout_builders.py` & `awkward-2.6.3rc2/tests/test_1620_layout_builders.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1625_multiple_columns_from_rdataframe.py` & `awkward-2.6.3rc2/tests/test_1625_multiple_columns_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1642_from_iter_of_tuples.py` & `awkward-2.6.3rc2/tests/test_1642_from_iter_of_tuples.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1650_Record_to_list_should_listify_itself.py` & `awkward-2.6.3rc2/tests/test_1650_Record_to_list_should_listify_itself.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1671_categorical_type.py` & `awkward-2.6.3rc2/tests/test_1671_categorical_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1672_broadcast_parameters.py` & `awkward-2.6.3rc2/tests/test_1672_broadcast_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1677_array_builder_in_numba.py` & `awkward-2.6.3rc2/tests/test_1677_array_builder_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1685_IndexedArray_project_parameters.py` & `awkward-2.6.3rc2/tests/test_1685_IndexedArray_project_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1686_UnionArray_simplified_preserve_parameters.py` & `awkward-2.6.3rc2/tests/test_1686_UnionArray_simplified_preserve_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1688_pack_categorical.py` & `awkward-2.6.3rc2/tests/test_1688_pack_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1703_fill_none_typetracer.py` & `awkward-2.6.3rc2/tests/test_1703_fill_none_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1707_broadcast_parameters_ufunc.py` & `awkward-2.6.3rc2/tests/test_1707_broadcast_parameters_ufunc.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1709_ak_array_constructor_behavior.py` & `awkward-2.6.3rc2/tests/test_1709_ak_array_constructor_behavior.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1747_bytemaskedarray_mergemany.py` & `awkward-2.6.3rc2/tests/test_1747_bytemaskedarray_mergemany.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1753_indexedarray_merge_kernel.py` & `awkward-2.6.3rc2/tests/test_1753_indexedarray_merge_kernel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1762_jax_behavior_support.py` & `awkward-2.6.3rc2/tests/test_1762_jax_behavior_support.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1764_jax_jacobian.py` & `awkward-2.6.3rc2/tests/test_1764_jax_jacobian.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1765_add_ioanas_test_of_to_arraylib.py` & `awkward-2.6.3rc2/tests/test_1765_add_ioanas_test_of_to_arraylib.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1766_record_form_fields.py` & `awkward-2.6.3rc2/tests/test_1766_record_form_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1781_rdataframe_snapshot.py` & `awkward-2.6.3rc2/tests/test_1781_rdataframe_snapshot.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1784_reduce_leading_sublist.py` & `awkward-2.6.3rc2/tests/test_1784_reduce_leading_sublist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1790_reduce_regulararray.py` & `awkward-2.6.3rc2/tests/test_1790_reduce_regulararray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1791_reduce_trailing_sublist.py` & `awkward-2.6.3rc2/tests/test_1791_reduce_trailing_sublist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1794_run_lengths_empty_sublist.py` & `awkward-2.6.3rc2/tests/test_1794_run_lengths_empty_sublist.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1826_ravel_preserve_none.py` & `awkward-2.6.3rc2/tests/test_1826_ravel_preserve_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1829_to_from_rdataframe_bool.py` & `awkward-2.6.3rc2/tests/test_1829_to_from_rdataframe_bool.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py` & `awkward-2.6.3rc2/tests/test_1840_ak_type_to_handle_ndarray_dtype_and_nptypes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1847_numpy_array_contiguous.py` & `awkward-2.6.3rc2/tests/test_1847_numpy_array_contiguous.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1850_bytemasked_array_to_bytemaskedarray.py` & `awkward-2.6.3rc2/tests/test_1850_bytemasked_array_to_bytemaskedarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1867_pass_behavior_through_combinations.py` & `awkward-2.6.3rc2/tests/test_1867_pass_behavior_through_combinations.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1904_drop_none.py` & `awkward-2.6.3rc2/tests/test_1904_drop_none.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 from __future__ import annotations
 
 import numpy as np
 import pytest
 
 import awkward as ak
-from awkward.errors import AxisError
 
 to_list = ak.operations.to_list
 
 
 def test_from_iter():
     a = ak.Array([[1], [2, None]])
     assert to_list(ak.drop_none(a)) == [[1], [2]]
@@ -425,18 +424,18 @@
     assert isinstance(ak.drop_none(ak.Array([1, 2, 3]), highlevel=True), ak.Array)
     assert isinstance(
         ak.drop_none(ak.Array([1, 2, 3]), highlevel=False), ak.contents.Content
     )
 
 
 def test_incorect_axis():
-    with pytest.raises(AxisError):
+    with pytest.raises(np.AxisError):
         ak.drop_none(ak.Array([[[None]]]), axis=4)
 
-    with pytest.raises(AxisError):
+    with pytest.raises(np.AxisError):
         ak.drop_none(ak.Array([1, 2, None]), axis=2)
 
 
 def test_RecordArray():
     a = ak.Array(
         [
             [{"x": [1], "y": [[2]]}],
@@ -543,15 +542,15 @@
     ]
 
     assert ak.is_none(array, axis=-2).tolist() == [
         None,
         [None, {"x": False, "y": [False]}],
         [{"x": False, "y": [True]}, {"x": False, "y": [False]}],
     ]
-    with pytest.raises(AxisError):
+    with pytest.raises(np.AxisError):
         ak.drop_none(array, axis=-2).tolist()
 
     array2 = ak.Array(
         [
             None,
             [None, {"x": [1], "y": [[2]]}],
             [{"x": None, "y": [None]}, {"x": [None], "y": [[None]]}],
@@ -564,9 +563,9 @@
     ]
 
     assert ak.is_none(array2, axis=-2).tolist() == [
         None,
         [None, {"x": False, "y": [False]}],
         [{"x": True, "y": [True]}, {"x": False, "y": [False]}],
     ]
-    with pytest.raises(AxisError):
+    with pytest.raises(np.AxisError):
         ak.drop_none(array2, axis=-2).tolist()
```

### Comparing `awkward-2.6.3/tests/test_1914_improved_axis_to_posaxis.py` & `awkward-2.6.3rc2/tests/test_1914_improved_axis_to_posaxis.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward/blob/main/LICENSE
 
 from __future__ import annotations
 
+import numpy as np
 import pytest
 
 import awkward as ak
-from awkward.errors import AxisError
 
 
 def test_is_none():
     array = ak.Array(
         [
             None,
             [None],
@@ -41,15 +41,15 @@
         [None],
         [{"x": None, "y": None}],
         [{"x": [True], "y": [True]}],
         [{"x": [False], "y": [False]}],
         [{"x": [False], "y": [False]}],
     ]
 
-    with pytest.raises(AxisError):
+    with pytest.raises(np.AxisError):
         ak.is_none(array, axis=3)
 
     assert ak.is_none(array, axis=-1).tolist() == [
         None,
         [None],
         [{"x": None, "y": None}],
         [{"x": [True], "y": [None]}],
@@ -61,15 +61,15 @@
         [None],
         [{"x": True, "y": None}],
         [{"x": False, "y": [True]}],
         [{"x": False, "y": [False]}],
         [{"x": False, "y": [False]}],
     ]
 
-    with pytest.raises(AxisError):
+    with pytest.raises(np.AxisError):
         ak.is_none(array, axis=-3)
 
 
 def test_singletons():
     array = ak.Array(
         [
             None,
@@ -104,15 +104,15 @@
         [None],
         [{"x": None, "y": None}],
         [{"x": [[]], "y": [[]]}],
         [{"x": [[1]], "y": [[[None]]]}],
         [{"x": [[2]], "y": [[[1, 2, 3]]]}],
     ]
 
-    with pytest.raises(AxisError):
+    with pytest.raises(np.AxisError):
         ak.singletons(array, axis=3)
 
     assert ak.singletons(array, axis=-1).tolist() == [
         None,
         [None],
         [{"x": None, "y": None}],
         [{"x": [[]], "y": [None]}],
@@ -125,15 +125,15 @@
         [None],
         [{"x": [], "y": None}],
         [{"x": [[None]], "y": [[]]}],
         [{"x": [[1]], "y": [[[None]]]}],
         [{"x": [[2]], "y": [[[1, 2, 3]]]}],
     ]
 
-    with pytest.raises(AxisError):
+    with pytest.raises(np.AxisError):
         ak.singletons(array, axis=-3)
 
 
 def test_is_none_union():
     left = ak.Array([[[{"x": 1, "y": None}]]])
     right = ak.Array([[[{"a": 1, "b": None}]]])
```

### Comparing `awkward-2.6.3/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py` & `awkward-2.6.3rc2/tests/test_1928_replace_simplify_method_with_classmethod_constructor.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1930_unflatten_counts_checks.py` & `awkward-2.6.3rc2/tests/test_1930_unflatten_counts_checks.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1936_with_field_broadcasting.py` & `awkward-2.6.3rc2/tests/test_1936_with_field_broadcasting.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1940_ak_backend.py` & `awkward-2.6.3rc2/tests/test_1940_ak_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1943_regular_indexing.py` & `awkward-2.6.3rc2/tests/test_1943_regular_indexing.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1960_awkward_from_rdataframe.py` & `awkward-2.6.3rc2/tests/test_1960_awkward_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_1961_ak_without_field.py` & `awkward-2.6.3rc2/tests/test_1961_ak_without_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2020_reduce_axis_none.py` & `awkward-2.6.3rc2/tests/test_2020_reduce_axis_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2021_check_TypeTracerArray_in_ak_where.py` & `awkward-2.6.3rc2/tests/test_2021_check_TypeTracerArray_in_ak_where.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2023_from_rdataframe.py` & `awkward-2.6.3rc2/tests/test_2023_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py` & `awkward-2.6.3rc2/tests/test_2027_add_data_touch_reporting_to_TypeTracerArray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2047_ak_transform_regular_to_jagged.py` & `awkward-2.6.3rc2/tests/test_2047_ak_transform_regular_to_jagged.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2051_arraybuilder_behavior_propagation.py` & `awkward-2.6.3rc2/tests/test_2051_arraybuilder_behavior_propagation.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2055_array_builder_check.py` & `awkward-2.6.3rc2/tests/test_2055_array_builder_check.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2058_merge_numpy_array.py` & `awkward-2.6.3rc2/tests/test_2058_merge_numpy_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2064_fill_none_record.py` & `awkward-2.6.3rc2/tests/test_2064_fill_none_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2067_to_buffers_byteorder.py` & `awkward-2.6.3rc2/tests/test_2067_to_buffers_byteorder.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2070_to_layout_string.py` & `awkward-2.6.3rc2/tests/test_2070_to_layout_string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2071_unflatten_non_packed_counts.py` & `awkward-2.6.3rc2/tests/test_2071_unflatten_non_packed_counts.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2078_array_function_wrap.py` & `awkward-2.6.3rc2/tests/test_2078_array_function_wrap.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2082_broadcast_zero_size.py` & `awkward-2.6.3rc2/tests/test_2082_broadcast_zero_size.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2085_empty_if_typetracer.py` & `awkward-2.6.3rc2/tests/test_2085_empty_if_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2096_ak_scalar_type.py` & `awkward-2.6.3rc2/tests/test_2096_ak_scalar_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2101_pickle_behavior_class.py` & `awkward-2.6.3rc2/tests/test_2101_pickle_behavior_class.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2104_numpy_merge_option.py` & `awkward-2.6.3rc2/tests/test_2104_numpy_merge_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2106_pickle_class.py` & `awkward-2.6.3rc2/tests/test_2106_pickle_class.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2108_fill_none_indexed.py` & `awkward-2.6.3rc2/tests/test_2108_fill_none_indexed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2115_fix_up_typetracers.py` & `awkward-2.6.3rc2/tests/test_2115_fix_up_typetracers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2120_missing_field_error.py` & `awkward-2.6.3rc2/tests/test_2120_missing_field_error.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2125_type_of_scalar.py` & `awkward-2.6.3rc2/tests/test_2125_type_of_scalar.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2150_typetracer_high_level_ufunc.py` & `awkward-2.6.3rc2/tests/test_2150_typetracer_high_level_ufunc.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2179_parameter_merging_rules.py` & `awkward-2.6.3rc2/tests/test_2179_parameter_merging_rules.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2185_merge_union_of_records.py` & `awkward-2.6.3rc2/tests/test_2185_merge_union_of_records.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py` & `awkward-2.6.3rc2/tests/test_2188_values_astype_turns_EmptyArray_into_NumpyArray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2192_union_absorb_indexed.py` & `awkward-2.6.3rc2/tests/test_2192_union_absorb_indexed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2198_almost_equal.py` & `awkward-2.6.3rc2/tests/test_2198_almost_equal.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2202_filter_multiple_columns_from_rdataframe.py` & `awkward-2.6.3rc2/tests/test_2202_filter_multiple_columns_from_rdataframe.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2214_offset_bool_index.py` & `awkward-2.6.3rc2/tests/test_2214_offset_bool_index.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2226_slice_regulararray_typetracer.py` & `awkward-2.6.3rc2/tests/test_2226_slice_regulararray_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2229_getitem_range_slice.py` & `awkward-2.6.3rc2/tests/test_2229_getitem_range_slice.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2234_from_rdataframe_keep_order.py` & `awkward-2.6.3rc2/tests/test_2234_from_rdataframe_keep_order.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2236_merge_union_of_records_option.py` & `awkward-2.6.3rc2/tests/test_2236_merge_union_of_records_option.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2240_merge_union_parameters.py` & `awkward-2.6.3rc2/tests/test_2240_merge_union_parameters.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2240_simplify_merge_as_union.py` & `awkward-2.6.3rc2/tests/test_2240_simplify_merge_as_union.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2246_slice_not_packed.py` & `awkward-2.6.3rc2/tests/test_2246_slice_not_packed.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2250_full_like_bool.py` & `awkward-2.6.3rc2/tests/test_2250_full_like_bool.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2258_from_rdataframe_with_arguments.py` & `awkward-2.6.3rc2/tests/test_2258_from_rdataframe_with_arguments.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2259_run_lengths_typetracer.py` & `awkward-2.6.3rc2/tests/test_2259_run_lengths_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2263_to_packed_list.py` & `awkward-2.6.3rc2/tests/test_2263_to_packed_list.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2267_broadcast_fields.py` & `awkward-2.6.3rc2/tests/test_2267_broadcast_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2293_unflatten_typetracer.py` & `awkward-2.6.3rc2/tests/test_2293_unflatten_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2296_duplicate_field.py` & `awkward-2.6.3rc2/tests/test_2296_duplicate_field.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2297_common_backend.py` & `awkward-2.6.3rc2/tests/test_2297_common_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2305_nep_18_lazy_conversion.py` & `awkward-2.6.3rc2/tests/test_2305_nep_18_lazy_conversion.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2306_cppyy_jit.py` & `awkward-2.6.3rc2/tests/test_2306_cppyy_jit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2319_from_buffers_array.py` & `awkward-2.6.3rc2/tests/test_2319_from_buffers_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2327_array_interface.py` & `awkward-2.6.3rc2/tests/test_2327_array_interface.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2329_cartesian_broadcasting_fixes.py` & `awkward-2.6.3rc2/tests/test_2329_cartesian_broadcasting_fixes.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2346_broadcast_depth_limit.py` & `awkward-2.6.3rc2/tests/test_2346_broadcast_depth_limit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2349_growablebuffer_in_numba.py` & `awkward-2.6.3rc2/tests/test_2349_growablebuffer_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2354_ufunc_same_backend.py` & `awkward-2.6.3rc2/tests/test_2354_ufunc_same_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2355_to_backend_record.py` & `awkward-2.6.3rc2/tests/test_2355_to_backend_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2361_typetracer_asarray_nd.py` & `awkward-2.6.3rc2/tests/test_2361_typetracer_asarray_nd.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2364_empty_list_of_string.py` & `awkward-2.6.3rc2/tests/test_2364_empty_list_of_string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2365_enforce_type.py` & `awkward-2.6.3rc2/tests/test_2365_enforce_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2368_type_is_equal.py` & `awkward-2.6.3rc2/tests/test_2368_type_is_equal.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2373_unzip_touching.py` & `awkward-2.6.3rc2/tests/test_2373_unzip_touching.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2374_cartesian_touching.py` & `awkward-2.6.3rc2/tests/test_2374_cartesian_touching.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2385_with_field_empty_record.py` & `awkward-2.6.3rc2/tests/test_2385_with_field_empty_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2395_copy_asarray_touch.py` & `awkward-2.6.3rc2/tests/test_2395_copy_asarray_touch.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2408_layoutbuilder_in_numba.py` & `awkward-2.6.3rc2/tests/test_2408_layoutbuilder_in_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2410_string_broadcast.py` & `awkward-2.6.3rc2/tests/test_2410_string_broadcast.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2411_cartesian_axis_validation.py` & `awkward-2.6.3rc2/tests/test_2411_cartesian_axis_validation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/awkward/blob/main/LICENSE
 
 from __future__ import annotations
 
+import numpy as np
 import pytest
 
 import awkward as ak
-from awkward.errors import AxisError
 
 
 def test_simple():
     left = ak.Array([1, 2, 3])
     right = ak.Array([["lambda", "sigma", "eta", "phi"], ["delta"]])
     pair = ak.cartesian([left, right], axis=0)
     assert pair.ndim == 1
@@ -22,9 +22,9 @@
         (3, ["delta"]),
     ]
 
 
 def test_out_of_bounds():
     left = ak.Array([1, 2, 3])
     right = ak.Array([["lambda", "sigma", "eta", "phi"], ["delta"]])
-    with pytest.raises(AxisError):
+    with pytest.raises(np.AxisError):
         ak.cartesian([left, right], axis=2)
```

### Comparing `awkward-2.6.3/tests/test_2417_bytemasked_singletons.py` & `awkward-2.6.3rc2/tests/test_2417_bytemasked_singletons.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2424_almost_equal_union_record.py` & `awkward-2.6.3rc2/tests/test_2424_almost_equal_union_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2425_forms_from_type.py` & `awkward-2.6.3rc2/tests/test_2425_forms_from_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2426_is_equal_to.py` & `awkward-2.6.3rc2/tests/test_2426_is_equal_to.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2444_minimal_listarray.py` & `awkward-2.6.3rc2/tests/test_2444_minimal_listarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2471_flatten_string.py` & `awkward-2.6.3rc2/tests/test_2471_flatten_string.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2484_reduce_starts_empty.py` & `awkward-2.6.3rc2/tests/test_2484_reduce_starts_empty.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2487_broadcast_list_offsets.py` & `awkward-2.6.3rc2/tests/test_2487_broadcast_list_offsets.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2490_reduce_regulararray_positional.py` & `awkward-2.6.3rc2/tests/test_2490_reduce_regulararray_positional.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2495_concatenate_typetracer.py` & `awkward-2.6.3rc2/tests/test_2495_concatenate_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2501_positional_record_reducer.py` & `awkward-2.6.3rc2/tests/test_2501_positional_record_reducer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2512_record_array_carry.py` & `awkward-2.6.3rc2/tests/test_2512_record_array_carry.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2536_select_columns.py` & `awkward-2.6.3rc2/tests/test_2536_select_columns.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2548_record_form_fields.py` & `awkward-2.6.3rc2/tests/test_2548_record_form_fields.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2549_list_nominal_type.py` & `awkward-2.6.3rc2/tests/test_2549_list_nominal_type.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2550_validity_error_recursive.py` & `awkward-2.6.3rc2/tests/test_2550_validity_error_recursive.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2564_string_broadcast_regular.py` & `awkward-2.6.3rc2/tests/test_2564_string_broadcast_regular.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2571_awkward_ListOffsetArray_reduce_local_nextparents_64.py` & `awkward-2.6.3rc2/tests/test_2571_awkward_ListOffsetArray_reduce_local_nextparents_64.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2595_transform_termination.py` & `awkward-2.6.3rc2/tests/test_2595_transform_termination.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2603_custom_behaviors_with_jax.py` & `awkward-2.6.3rc2/tests/test_2603_custom_behaviors_with_jax.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2604_read_awkward1_pickles.py` & `awkward-2.6.3rc2/tests/test_2604_read_awkward1_pickles.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2616_use_pyarrow_for_strings.py` & `awkward-2.6.3rc2/tests/test_2616_use_pyarrow_for_strings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2623_optiontype_outside_record_strings.py` & `awkward-2.6.3rc2/tests/test_2623_optiontype_outside_record_strings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2630_akstr_to_categorical.py` & `awkward-2.6.3rc2/tests/test_2630_akstr_to_categorical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2631_vectorised_to_numpy_strings.py` & `awkward-2.6.3rc2/tests/test_2631_vectorised_to_numpy_strings.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2634_listarray_pad_none.py` & `awkward-2.6.3rc2/tests/test_2634_listarray_pad_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2637_jax_tracer_error.py` & `awkward-2.6.3rc2/tests/test_2637_jax_tracer_error.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2638_mean_and_count_grads.py` & `awkward-2.6.3rc2/tests/test_2638_mean_and_count_grads.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2646_from_parquet_highlevel.py` & `awkward-2.6.3rc2/tests/test_2646_from_parquet_highlevel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2649_dlpack_support.py` & `awkward-2.6.3rc2/tests/test_2649_dlpack_support.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2650_arrow_array_highlevel.py` & `awkward-2.6.3rc2/tests/test_2650_arrow_array_highlevel.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2651_parameter_union.py` & `awkward-2.6.3rc2/tests/test_2651_parameter_union.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2653_slice_listoffsetarray.py` & `awkward-2.6.3rc2/tests/test_2653_slice_listoffsetarray.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2656_unflatten_axis_typetracer.py` & `awkward-2.6.3rc2/tests/test_2656_unflatten_axis_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2660_expected_container_keys_from_form.py` & `awkward-2.6.3rc2/tests/test_2660_expected_container_keys_from_form.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2663_broadcast_tuples.py` & `awkward-2.6.3rc2/tests/test_2663_broadcast_tuples.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2665_out_of_band_pickle.py` & `awkward-2.6.3rc2/tests/test_2665_out_of_band_pickle.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2671_typetracer_with_report_deprecated_length.py` & `awkward-2.6.3rc2/tests/test_2671_typetracer_with_report_deprecated_length.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2672_touch_data.py` & `awkward-2.6.3rc2/tests/test_2672_touch_data.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2678_same_backend.py` & `awkward-2.6.3rc2/tests/test_2678_same_backend.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2682_custom_pickler.py` & `awkward-2.6.3rc2/tests/test_2682_custom_pickler.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2683_to_and_from_feather.py` & `awkward-2.6.3rc2/tests/test_2683_to_and_from_feather.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2693_to_buffers_placeholders.py` & `awkward-2.6.3rc2/tests/test_2693_to_buffers_placeholders.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2713_from_buffers_allow_noncanonical.py` & `awkward-2.6.3rc2/tests/test_2713_from_buffers_allow_noncanonical.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2714_from_buffers_placeholders.py` & `awkward-2.6.3rc2/tests/test_2714_from_buffers_placeholders.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2718_frombuffer_typetracer.py` & `awkward-2.6.3rc2/tests/test_2718_frombuffer_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2719_typetracer_buffer_key.py` & `awkward-2.6.3rc2/tests/test_2719_typetracer_buffer_key.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2724_expected_from_buffers_recursive.py` & `awkward-2.6.3rc2/tests/test_2724_expected_from_buffers_recursive.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2727_remove_structure_regular.py` & `awkward-2.6.3rc2/tests/test_2727_remove_structure_regular.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2754_highlevel_behavior_missing.py` & `awkward-2.6.3rc2/tests/test_2754_highlevel_behavior_missing.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2757_attrs_metadata.py` & `awkward-2.6.3rc2/tests/test_2757_attrs_metadata.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2759_update_class_consistently.py` & `awkward-2.6.3rc2/tests/test_2759_update_class_consistently.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2763_to_layout_granularity.py` & `awkward-2.6.3rc2/tests/test_2763_to_layout_granularity.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2769_argsort_all_none.py` & `awkward-2.6.3rc2/tests/test_2769_argsort_all_none.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2770_serialize_and_deserialize_behaviour_for_numba.py` & `awkward-2.6.3rc2/tests/test_2770_serialize_and_deserialize_behaviour_for_numba.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2785_ak_num_typetracer_axis_0.py` & `awkward-2.6.3rc2/tests/test_2785_ak_num_typetracer_axis_0.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2793_nep_50_gradual_support.py` & `awkward-2.6.3rc2/tests/test_2793_nep_50_gradual_support.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,37 +9,31 @@
 import pytest
 
 import awkward as ak
 
 NUMPY_HAS_NEP_50 = packaging.version.parse(np.__version__) >= packaging.version.Version(
     "1.24.0"
 )
-NUMPY_2 = packaging.version.parse(np.__version__) >= packaging.version.Version(
-    "2.0.0b1"
-)
 
 
 @pytest.mark.skipif(not NUMPY_HAS_NEP_50, reason="NEP-50 requires NumPy >= 1.24.0")
 @pytest.mark.parametrize("backend", ["cpu", "typetracer"])
 def test_with_nep_50(backend):
     array = ak.to_backend(np.arange(255, dtype=np.uint8), backend)
     assert array.layout.dtype == np.dtype(np.uint8)
 
     typed_scalar = np.uint64(0)
     assert (array + typed_scalar).layout.dtype == np.dtype(np.uint64)
 
     # With NEP-50, we can ask NumPy to use value-less type resolution
-    if NUMPY_2 and backend == "cpu":
-        warn_context = pytest.raises(OverflowError)
-    else:
-        warn_context = (
-            pytest.warns(DeprecationWarning, match="out-of-bound Python integers")
-            if backend == "cpu"
-            else contextlib.nullcontext()
-        )
+    warn_context = (
+        pytest.warns(DeprecationWarning, match="out-of-bound Python integers")
+        if backend == "cpu"
+        else contextlib.nullcontext()
+    )
     with warn_context:
         untyped_scalar = 512
         assert (array + untyped_scalar).layout.dtype == np.dtype(np.uint8)
 
 
 @pytest.mark.skipif(NUMPY_HAS_NEP_50, reason="NumPy >= 1.24.0 has NEP-50 support")
 @pytest.mark.parametrize("backend", ["cpu", "typetracer"])
```

### Comparing `awkward-2.6.3/tests/test_2799_numba_ufunc_resolution.py` & `awkward-2.6.3rc2/tests/test_2799_numba_ufunc_resolution.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2803_string_formatter.py` & `awkward-2.6.3rc2/tests/test_2803_string_formatter.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2806_attrs_typetracer.py` & `awkward-2.6.3rc2/tests/test_2806_attrs_typetracer.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2808_dtype_ufunc_bool.py` & `awkward-2.6.3rc2/tests/test_2808_dtype_ufunc_bool.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2837_ufunc_attrs_behavior.py` & `awkward-2.6.3rc2/tests/test_2837_ufunc_attrs_behavior.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2857_full_like_scalar.py` & `awkward-2.6.3rc2/tests/test_2857_full_like_scalar.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2860_enforce_concatenated_form.py` & `awkward-2.6.3rc2/tests/test_2860_enforce_concatenated_form.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2866_getitem_attrs.py` & `awkward-2.6.3rc2/tests/test_2866_getitem_attrs.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2889_test_chunked_array.py` & `awkward-2.6.3rc2/tests/test_2889_test_chunked_array.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2898_to_parquet_dataset.py` & `awkward-2.6.3rc2/tests/test_2898_to_parquet_dataset.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2917_real_imag_angle.py` & `awkward-2.6.3rc2/tests/test_2917_real_imag_angle.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2917_round.py` & `awkward-2.6.3rc2/tests/test_2917_round.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2918_fix_var_axis_not_minus_one.py` & `awkward-2.6.3rc2/tests/test_2918_fix_var_axis_not_minus_one.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2928_nested_cartesian_record.py` & `awkward-2.6.3rc2/tests/test_2928_nested_cartesian_record.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/test_2968_to_parquet_row_groups.py` & `awkward-2.6.3rc2/tests/test_2968_to_parquet_row_groups.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/samples/awkward1-regulararray.pkl` & `awkward-2.6.3rc2/tests/samples/awkward1-regulararray.pkl`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/samples/awkward1-unionarray.pkl` & `awkward-2.6.3rc2/tests/samples/awkward1-unionarray.pkl`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/samples/complex-nested.json` & `awkward-2.6.3rc2/tests/samples/complex-nested.json`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/samples/list-depths-records-list.parquet` & `awkward-2.6.3rc2/tests/samples/list-depths-records-list.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/samples/list-depths-records.parquet` & `awkward-2.6.3rc2/tests/samples/list-depths-records.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/samples/list-depths-strings.parquet` & `awkward-2.6.3rc2/tests/samples/list-depths-strings.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/samples/list-depths.parquet` & `awkward-2.6.3rc2/tests/samples/list-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/samples/nonnullable-depths.parquet` & `awkward-2.6.3rc2/tests/samples/nonnullable-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/samples/nullable-depths.parquet` & `awkward-2.6.3rc2/tests/samples/nullable-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/samples/nullable-levels.parquet` & `awkward-2.6.3rc2/tests/samples/nullable-levels.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/samples/nullable-list-depths-records-list.parquet` & `awkward-2.6.3rc2/tests/samples/nullable-list-depths-records-list.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/samples/nullable-list-depths-records.parquet` & `awkward-2.6.3rc2/tests/samples/nullable-list-depths-records.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/samples/nullable-list-depths-strings.parquet` & `awkward-2.6.3rc2/tests/samples/nullable-list-depths-strings.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/samples/nullable-list-depths.parquet` & `awkward-2.6.3rc2/tests/samples/nullable-list-depths.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/samples/nullable-record-primitives.parquet` & `awkward-2.6.3rc2/tests/samples/nullable-record-primitives.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/samples/record-primitives.parquet` & `awkward-2.6.3rc2/tests/samples/record-primitives.parquet`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/samples/test-nan-inf.json` & `awkward-2.6.3rc2/tests/samples/test-nan-inf.json`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/samples/test-two-arrays.json` & `awkward-2.6.3rc2/tests/samples/test-two-arrays.json`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests/samples/test.json` & `awkward-2.6.3rc2/tests/samples/test.json`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests-cuda/test_1276_cuda_num.py` & `awkward-2.6.3rc2/tests-cuda/test_1276_cuda_num.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,15 +128,15 @@
     )
 
     cuda_recordarray = ak.to_backend(recordarray, "cuda")
 
     assert ak.num(cuda_recordarray, 0) == ak.num(recordarray, 0)
 
     content0 = ak.Array([[1.1, 2.2, 3.3], [], [4.4, 5.5]]).layout
-    content1 = ak.Array(
+    content = ak.Array(
         ["one", "two", "three", "four", "five", "six", "seven", "eight", "nine"]
     ).layout
     tags = ak.index.Index8(np.array([1, 1, 0, 0, 1, 0, 1, 1], dtype=np.int8))
     index = ak.index.Index32(np.array([0, 1, 0, 1, 2, 2, 4, 3], dtype=np.int32))
     unionarray = ak.Array(
         ak.contents.unionarray.UnionArray(tags, index, [content0, content1])
     )
@@ -189,8 +189,9 @@
                         3.8,
                     ]
                 )
             ),
         )
     )
     cuda_ioa = ak.to_backend(ioa, "cuda")
+    ak.to_backend(cuda_ioa, "cpu")
     assert ak.num(cuda_ioa, 0) == ak.num(ioa, 0)
```

### Comparing `awkward-2.6.3/tests-cuda/test_1276_cuda_transfers.py` & `awkward-2.6.3rc2/tests-cuda/test_1276_cuda_transfers.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests-cuda/test_1276_cupy_interop.py` & `awkward-2.6.3rc2/tests-cuda/test_1276_cupy_interop.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests-cuda/test_1276_from_cupy.py` & `awkward-2.6.3rc2/tests-cuda/test_1276_from_cupy.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests-cuda/test_1300_same_for_numba_cuda.py` & `awkward-2.6.3rc2/tests-cuda/test_1300_same_for_numba_cuda.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests-cuda/test_1381_check_errors.py` & `awkward-2.6.3rc2/tests-cuda/test_1381_check_errors.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests-cuda/test_1809_array_cuda_jit.py` & `awkward-2.6.3rc2/tests-cuda/test_1809_array_cuda_jit.py`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_BitMaskedArray_to_ByteMaskedArray.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_BitMaskedArray_to_ByteMaskedArray.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_BitMaskedArray_to_IndexedOptionArray64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_BitMaskedArray_to_IndexedOptionArray64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_getitem_nextcarry_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_getitem_nextcarry_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_getitem_nextcarry_outindex_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_getitem_nextcarry_outindex_64.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_numnull.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_numnull.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_overlay_mask8.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_overlay_mask8.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_reduce_next_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_int16_64.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_ByteMaskedArray_reduce_next_64_1():
+def test_cudaawkward_reduce_prod_bool_int16_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64_1():
+def test_cudaawkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_fromshifts_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_fromshifts_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_reduce_next_nonlocal_nextshifts_fromshifts_64.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_fromshifts_64_1():
+def test_cudaawkward_IndexedArrayU32_reduce_next_nonlocal_nextshifts_fromshifts_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_toIndexedOptionArray64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_toIndexedOptionArray64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_Content_getitem_next_missing_jagged_getmaskstartstop.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_Content_getitem_next_missing_jagged_getmaskstartstop.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_flatten_nextcarry_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_flatten_nextcarry_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_flatten_none2empty_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_flatten_none2empty_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_getitem_nextcarry_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_getitem_nextcarry_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_getitem_nextcarry_outindex_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_getitem_nextcarry_outindex_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_index_of_nulls.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_index_of_nulls.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_numnull.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_numnull.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -13,75 +13,75 @@
 
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
-def test_cudaawkward_IndexedArray32_numnull_1():
+def test_cudaawkward_IndexedArrayU32_numnull_1():
     numnull = cupy.array([123], dtype=cupy.int64)
-    fromindex = cupy.array([1, 0, 0, 1, 1, 1, 0, 0, 1, 0, 1, 0, 1, 1], dtype=cupy.int32)
+    fromindex = cupy.array([1, 0, 0, 1, 1, 1, 0, 0, 1, 0, 1, 0, 1, 1], dtype=cupy.uint32)
     lenindex = 3
-    funcC = cupy_backend['awkward_IndexedArray_numnull', cupy.int64, cupy.int32]
+    funcC = cupy_backend['awkward_IndexedArray_numnull', cupy.int64, cupy.uint32]
     funcC(numnull, fromindex, lenindex)
 
     try:
         ak_cu.synchronize_cuda()
     except:
         pytest.fail("This test case shouldn't have raised an error")
     pytest_numnull = [0]
     assert cupy.array_equal(numnull[:len(pytest_numnull)], cupy.array(pytest_numnull))
 
-def test_cudaawkward_IndexedArray32_numnull_2():
+def test_cudaawkward_IndexedArrayU32_numnull_2():
     numnull = cupy.array([123], dtype=cupy.int64)
-    fromindex = cupy.array([1, 2, 2, 3, 0, 2, 0, 2, 1, 1], dtype=cupy.int32)
+    fromindex = cupy.array([1, 2, 2, 3, 0, 2, 0, 2, 1, 1], dtype=cupy.uint32)
     lenindex = 3
-    funcC = cupy_backend['awkward_IndexedArray_numnull', cupy.int64, cupy.int32]
+    funcC = cupy_backend['awkward_IndexedArray_numnull', cupy.int64, cupy.uint32]
     funcC(numnull, fromindex, lenindex)
 
     try:
         ak_cu.synchronize_cuda()
     except:
         pytest.fail("This test case shouldn't have raised an error")
     pytest_numnull = [0]
     assert cupy.array_equal(numnull[:len(pytest_numnull)], cupy.array(pytest_numnull))
 
-def test_cudaawkward_IndexedArray32_numnull_3():
+def test_cudaawkward_IndexedArrayU32_numnull_3():
     numnull = cupy.array([123], dtype=cupy.int64)
-    fromindex = cupy.array([1, 3, 0, 3, 5, 2, 0, 2, 1, 1], dtype=cupy.int32)
+    fromindex = cupy.array([1, 3, 0, 3, 5, 2, 0, 2, 1, 1], dtype=cupy.uint32)
     lenindex = 3
-    funcC = cupy_backend['awkward_IndexedArray_numnull', cupy.int64, cupy.int32]
+    funcC = cupy_backend['awkward_IndexedArray_numnull', cupy.int64, cupy.uint32]
     funcC(numnull, fromindex, lenindex)
 
     try:
         ak_cu.synchronize_cuda()
     except:
         pytest.fail("This test case shouldn't have raised an error")
     pytest_numnull = [0]
     assert cupy.array_equal(numnull[:len(pytest_numnull)], cupy.array(pytest_numnull))
 
-def test_cudaawkward_IndexedArray32_numnull_4():
+def test_cudaawkward_IndexedArrayU32_numnull_4():
     numnull = cupy.array([123], dtype=cupy.int64)
-    fromindex = cupy.array([1, 4, 2, 3, 1, 2, 3, 1, 4, 3, 2, 1, 3, 2, 4, 5, 1, 2, 3, 4, 5], dtype=cupy.int32)
+    fromindex = cupy.array([1, 4, 2, 3, 1, 2, 3, 1, 4, 3, 2, 1, 3, 2, 4, 5, 1, 2, 3, 4, 5], dtype=cupy.uint32)
     lenindex = 3
-    funcC = cupy_backend['awkward_IndexedArray_numnull', cupy.int64, cupy.int32]
+    funcC = cupy_backend['awkward_IndexedArray_numnull', cupy.int64, cupy.uint32]
     funcC(numnull, fromindex, lenindex)
 
     try:
         ak_cu.synchronize_cuda()
     except:
         pytest.fail("This test case shouldn't have raised an error")
     pytest_numnull = [0]
     assert cupy.array_equal(numnull[:len(pytest_numnull)], cupy.array(pytest_numnull))
 
-def test_cudaawkward_IndexedArray32_numnull_5():
+def test_cudaawkward_IndexedArrayU32_numnull_5():
     numnull = cupy.array([123], dtype=cupy.int64)
-    fromindex = cupy.array([0, 0, 0, 0, 0, 0, 0, 0, 0, 0], dtype=cupy.int32)
+    fromindex = cupy.array([0, 0, 0, 0, 0, 0, 0, 0, 0, 0], dtype=cupy.uint32)
     lenindex = 3
-    funcC = cupy_backend['awkward_IndexedArray_numnull', cupy.int64, cupy.int32]
+    funcC = cupy_backend['awkward_IndexedArray_numnull', cupy.int64, cupy.uint32]
     funcC(numnull, fromindex, lenindex)
 
     try:
         ak_cu.synchronize_cuda()
     except:
         pytest.fail("This test case shouldn't have raised an error")
     pytest_numnull = [0]
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_numnull_parents.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_numnull_parents.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_overlay_mask8_to64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_overlay_mask8_to64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_IndexedArray32_overlay_mask8_to64_1():
+def test_cudaawkward_IndexedArray64_overlay_mask8_to64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_ranges_carry_next_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_ranges_carry_next_64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_ranges_next_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_ranges_next_64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_reduce_next_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_uint64_64.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_IndexedArray32_reduce_next_64_1():
+def test_cudaawkward_reduce_sum_bool_uint64_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_reduce_next_nonlocal_nextshifts_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_reduce_next_nonlocal_nextshifts_64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_reduce_next_nonlocal_nextshifts_fromshifts_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_reduce_next_nonlocal_nextshifts_64.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_IndexedArray32_reduce_next_nonlocal_nextshifts_fromshifts_64_1():
+def test_cudaawkward_IndexedArray64_reduce_next_nonlocal_nextshifts_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_simplify32_to64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_simplify32_to64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_simplify64_to64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_simplify64_to64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_simplifyU32_to64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_simplifyU32_to64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray32_validity.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_validity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_flatten_nextcarry_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_flatten_nextcarry_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_flatten_none2empty_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_flatten_none2empty_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_getitem_nextcarry_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_getitem_nextcarry_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_getitem_nextcarry_outindex_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_getitem_nextcarry_outindex_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_index_of_nulls.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_index_of_nulls.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_numnull.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_numnull.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_numnull_parents.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_numnull_parents.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_overlay_mask8_to64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_ranges_next_64.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_IndexedArray64_overlay_mask8_to64_1():
+def test_cudaawkward_IndexedArray64_ranges_next_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_ranges_carry_next_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_ranges_carry_next_64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_ranges_next_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_ranges_next_64.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_IndexedArray64_ranges_next_64_1():
+def test_cudaawkward_IndexedArrayU32_ranges_next_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_reduce_next_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_reduce_next_64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_reduce_next_nonlocal_nextshifts_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_reduce_next_nonlocal_nextshifts_64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_IndexedArray64_reduce_next_nonlocal_nextshifts_64_1():
+def test_cudaawkward_IndexedArrayU32_reduce_next_nonlocal_nextshifts_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_reduce_next_nonlocal_nextshifts_fromshifts_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_reduce_next_nonlocal_nextshifts_fromshifts_64.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_IndexedArray64_reduce_next_nonlocal_nextshifts_fromshifts_64_1():
+def test_cudaawkward_IndexedArray32_reduce_next_nonlocal_nextshifts_fromshifts_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_simplify32_to64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_simplify32_to64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_simplify64_to64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_simplify64_to64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_simplifyU32_to64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_simplifyU32_to64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray64_validity.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_validity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_flatten_nextcarry_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_flatten_nextcarry_64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_flatten_none2empty_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_flatten_none2empty_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_getitem_nextcarry_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_getitem_nextcarry_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_getitem_nextcarry_outindex_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_getitem_nextcarry_outindex_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_index_of_nulls.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromint8.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_IndexedArrayU32_index_of_nulls_1():
+def test_cudaawkward_NumpyArray_fill_toint8_fromint8_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_numnull.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_numnull.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -13,75 +13,75 @@
 
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
-def test_cudaawkward_IndexedArrayU32_numnull_1():
+def test_cudaawkward_IndexedArray32_numnull_1():
     numnull = cupy.array([123], dtype=cupy.int64)
-    fromindex = cupy.array([1, 0, 0, 1, 1, 1, 0, 0, 1, 0, 1, 0, 1, 1], dtype=cupy.uint32)
+    fromindex = cupy.array([1, 0, 0, 1, 1, 1, 0, 0, 1, 0, 1, 0, 1, 1], dtype=cupy.int32)
     lenindex = 3
-    funcC = cupy_backend['awkward_IndexedArray_numnull', cupy.int64, cupy.uint32]
+    funcC = cupy_backend['awkward_IndexedArray_numnull', cupy.int64, cupy.int32]
     funcC(numnull, fromindex, lenindex)
 
     try:
         ak_cu.synchronize_cuda()
     except:
         pytest.fail("This test case shouldn't have raised an error")
     pytest_numnull = [0]
     assert cupy.array_equal(numnull[:len(pytest_numnull)], cupy.array(pytest_numnull))
 
-def test_cudaawkward_IndexedArrayU32_numnull_2():
+def test_cudaawkward_IndexedArray32_numnull_2():
     numnull = cupy.array([123], dtype=cupy.int64)
-    fromindex = cupy.array([1, 2, 2, 3, 0, 2, 0, 2, 1, 1], dtype=cupy.uint32)
+    fromindex = cupy.array([1, 2, 2, 3, 0, 2, 0, 2, 1, 1], dtype=cupy.int32)
     lenindex = 3
-    funcC = cupy_backend['awkward_IndexedArray_numnull', cupy.int64, cupy.uint32]
+    funcC = cupy_backend['awkward_IndexedArray_numnull', cupy.int64, cupy.int32]
     funcC(numnull, fromindex, lenindex)
 
     try:
         ak_cu.synchronize_cuda()
     except:
         pytest.fail("This test case shouldn't have raised an error")
     pytest_numnull = [0]
     assert cupy.array_equal(numnull[:len(pytest_numnull)], cupy.array(pytest_numnull))
 
-def test_cudaawkward_IndexedArrayU32_numnull_3():
+def test_cudaawkward_IndexedArray32_numnull_3():
     numnull = cupy.array([123], dtype=cupy.int64)
-    fromindex = cupy.array([1, 3, 0, 3, 5, 2, 0, 2, 1, 1], dtype=cupy.uint32)
+    fromindex = cupy.array([1, 3, 0, 3, 5, 2, 0, 2, 1, 1], dtype=cupy.int32)
     lenindex = 3
-    funcC = cupy_backend['awkward_IndexedArray_numnull', cupy.int64, cupy.uint32]
+    funcC = cupy_backend['awkward_IndexedArray_numnull', cupy.int64, cupy.int32]
     funcC(numnull, fromindex, lenindex)
 
     try:
         ak_cu.synchronize_cuda()
     except:
         pytest.fail("This test case shouldn't have raised an error")
     pytest_numnull = [0]
     assert cupy.array_equal(numnull[:len(pytest_numnull)], cupy.array(pytest_numnull))
 
-def test_cudaawkward_IndexedArrayU32_numnull_4():
+def test_cudaawkward_IndexedArray32_numnull_4():
     numnull = cupy.array([123], dtype=cupy.int64)
-    fromindex = cupy.array([1, 4, 2, 3, 1, 2, 3, 1, 4, 3, 2, 1, 3, 2, 4, 5, 1, 2, 3, 4, 5], dtype=cupy.uint32)
+    fromindex = cupy.array([1, 4, 2, 3, 1, 2, 3, 1, 4, 3, 2, 1, 3, 2, 4, 5, 1, 2, 3, 4, 5], dtype=cupy.int32)
     lenindex = 3
-    funcC = cupy_backend['awkward_IndexedArray_numnull', cupy.int64, cupy.uint32]
+    funcC = cupy_backend['awkward_IndexedArray_numnull', cupy.int64, cupy.int32]
     funcC(numnull, fromindex, lenindex)
 
     try:
         ak_cu.synchronize_cuda()
     except:
         pytest.fail("This test case shouldn't have raised an error")
     pytest_numnull = [0]
     assert cupy.array_equal(numnull[:len(pytest_numnull)], cupy.array(pytest_numnull))
 
-def test_cudaawkward_IndexedArrayU32_numnull_5():
+def test_cudaawkward_IndexedArray32_numnull_5():
     numnull = cupy.array([123], dtype=cupy.int64)
-    fromindex = cupy.array([0, 0, 0, 0, 0, 0, 0, 0, 0, 0], dtype=cupy.uint32)
+    fromindex = cupy.array([0, 0, 0, 0, 0, 0, 0, 0, 0, 0], dtype=cupy.int32)
     lenindex = 3
-    funcC = cupy_backend['awkward_IndexedArray_numnull', cupy.int64, cupy.uint32]
+    funcC = cupy_backend['awkward_IndexedArray_numnull', cupy.int64, cupy.int32]
     funcC(numnull, fromindex, lenindex)
 
     try:
         ak_cu.synchronize_cuda()
     except:
         pytest.fail("This test case shouldn't have raised an error")
     pytest_numnull = [0]
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_numnull_parents.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromint8.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_IndexedArrayU32_numnull_parents_1():
+def test_cudaawkward_NumpyArray_fill_tofloat64_fromint8_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_overlay_mask8_to64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_overlay_mask8_to64.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_ranges_carry_next_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_ranges_carry_next_64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_ranges_next_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_numnull_parents.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_IndexedArrayU32_ranges_next_64_1():
+def test_cudaawkward_IndexedArrayU32_numnull_parents_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_reduce_next_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_reduce_next_64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_reduce_next_nonlocal_nextshifts_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray32_reduce_local_nextparents_64.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_IndexedArrayU32_reduce_next_nonlocal_nextshifts_64_1():
+def test_cudaawkward_ListOffsetArray32_reduce_local_nextparents_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_reduce_next_nonlocal_nextshifts_fromshifts_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_RegularArray_reduce_nonlocal_preparenext_64.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_IndexedArrayU32_reduce_next_nonlocal_nextshifts_fromshifts_64_1():
+def test_cudaawkward_RegularArray_reduce_nonlocal_preparenext_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_simplify32_to64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_simplify32_to64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_simplify64_to64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_simplify64_to64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_simplifyU32_to64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_simplifyU32_to64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_validity.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArrayU32_validity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray_fill_to64_count.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray_fill_to64_count.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray_fill_to64_from32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray_fill_to64_from32.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray_fill_to64_from64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray_fill_to64_from64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray_fill_to64_fromU32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray_fill_to64_fromU32.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray_numnull_unique_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromfloat64.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_IndexedArray_numnull_unique_64_1():
+def test_cudaawkward_NumpyArray_fill_toint8_fromfloat64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedArray_reduce_next_fix_offsets_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_int32_64.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_IndexedArray_reduce_next_fix_offsets_64_1():
+def test_cudaawkward_reduce_prod_bool_int32_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_IndexedOptionArray_rpad_and_clip_mask_axis1_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedOptionArray_rpad_and_clip_mask_axis1_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_broadcast_tooffsets_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_broadcast_tooffsets_64.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -13,25 +13,25 @@
 
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
-def test_cudaawkward_ListArray32_broadcast_tooffsets_64_1():
+def test_cudaawkward_ListArrayU32_broadcast_tooffsets_64_1():
     tocarry = cupy.array([123], dtype=cupy.int64)
     fromoffsets = cupy.array([2, 3, 3, 4, 5, 5, 5, 5, 5, 6, 7, 8, 10, 11], dtype=cupy.int64)
     offsetslength = 3
-    fromstarts = cupy.array([2, 0, 2, 1, 2, 1, 2, 1, 2, 1, 2, 1], dtype=cupy.int32)
-    fromstops = cupy.array([3, 2, 4, 5, 3, 4, 2, 5, 3, 4, 6, 11], dtype=cupy.int32)
+    fromstarts = cupy.array([2, 0, 2, 1, 2, 1, 2, 1, 2, 1, 2, 1], dtype=cupy.uint32)
+    fromstops = cupy.array([3, 2, 4, 5, 3, 4, 2, 5, 3, 4, 6, 11], dtype=cupy.uint32)
     lencontent = 3
-    funcC = cupy_backend['awkward_ListArray_broadcast_tooffsets', cupy.int64, cupy.int64, cupy.int32, cupy.int32]
+    funcC = cupy_backend['awkward_ListArray_broadcast_tooffsets', cupy.int64, cupy.int64, cupy.uint32, cupy.uint32]
 
-def test_cudaawkward_ListArray32_broadcast_tooffsets_64_2():
+def test_cudaawkward_ListArrayU32_broadcast_tooffsets_64_2():
     tocarry = cupy.array([123], dtype=cupy.int64)
     fromoffsets = cupy.array([2, 3, 3, 4, 5, 5, 5, 5, 5, 6, 7, 8, 10, 11], dtype=cupy.int64)
     offsetslength = 3
-    fromstarts = cupy.array([0, 0, 0, 0, 0, 0, 0, 0], dtype=cupy.int32)
-    fromstops = cupy.array([1, 1, 1, 1, 1, 1, 1, 1], dtype=cupy.int32)
+    fromstarts = cupy.array([0, 0, 0, 0, 0, 0, 0, 0], dtype=cupy.uint32)
+    fromstops = cupy.array([1, 1, 1, 1, 1, 1, 1, 1], dtype=cupy.uint32)
     lencontent = 6
-    funcC = cupy_backend['awkward_ListArray_broadcast_tooffsets', cupy.int64, cupy.int64, cupy.int32, cupy.int32]
+    funcC = cupy_backend['awkward_ListArray_broadcast_tooffsets', cupy.int64, cupy.int64, cupy.uint32, cupy.uint32]
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_combinations_length_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_combinations_length_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_compact_offsets_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_compact_offsets_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_jagged_descend_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_jagged_descend_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_jagged_expand_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_jagged_expand_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_next_array_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_next_array_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_next_array_advanced_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_next_array_advanced_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_next_at_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_next_at_64.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_next_range_counts_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_next_range_counts_64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_next_range_spreadadvanced_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_getitem_next_range_spreadadvanced_64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_localindex_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_localindex_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_min_range.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_min_range.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_rpad_and_clip_length_axis1.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_rpad_and_clip_length_axis1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_rpad_axis1_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_rpad_axis1_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray32_validity.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_validity.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_broadcast_tooffsets_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_broadcast_tooffsets_64.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_combinations_length_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_combinations_length_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_compact_offsets_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_compact_offsets_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_jagged_descend_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_jagged_descend_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_jagged_expand_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_jagged_expand_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_next_array_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_next_array_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_next_array_advanced_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_next_array_advanced_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_next_at_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_next_at_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_next_range_counts_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_next_range_counts_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_next_range_spreadadvanced_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_getitem_next_range_spreadadvanced_64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_localindex_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_localindex_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_min_range.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_min_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_rpad_and_clip_length_axis1.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_rpad_and_clip_length_axis1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_rpad_axis1_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_rpad_axis1_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray64_validity.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray64_validity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_broadcast_tooffsets_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray32_broadcast_tooffsets_64.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -13,25 +13,25 @@
 
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
-def test_cudaawkward_ListArrayU32_broadcast_tooffsets_64_1():
+def test_cudaawkward_ListArray32_broadcast_tooffsets_64_1():
     tocarry = cupy.array([123], dtype=cupy.int64)
     fromoffsets = cupy.array([2, 3, 3, 4, 5, 5, 5, 5, 5, 6, 7, 8, 10, 11], dtype=cupy.int64)
     offsetslength = 3
-    fromstarts = cupy.array([2, 0, 2, 1, 2, 1, 2, 1, 2, 1, 2, 1], dtype=cupy.uint32)
-    fromstops = cupy.array([3, 2, 4, 5, 3, 4, 2, 5, 3, 4, 6, 11], dtype=cupy.uint32)
+    fromstarts = cupy.array([2, 0, 2, 1, 2, 1, 2, 1, 2, 1, 2, 1], dtype=cupy.int32)
+    fromstops = cupy.array([3, 2, 4, 5, 3, 4, 2, 5, 3, 4, 6, 11], dtype=cupy.int32)
     lencontent = 3
-    funcC = cupy_backend['awkward_ListArray_broadcast_tooffsets', cupy.int64, cupy.int64, cupy.uint32, cupy.uint32]
+    funcC = cupy_backend['awkward_ListArray_broadcast_tooffsets', cupy.int64, cupy.int64, cupy.int32, cupy.int32]
 
-def test_cudaawkward_ListArrayU32_broadcast_tooffsets_64_2():
+def test_cudaawkward_ListArray32_broadcast_tooffsets_64_2():
     tocarry = cupy.array([123], dtype=cupy.int64)
     fromoffsets = cupy.array([2, 3, 3, 4, 5, 5, 5, 5, 5, 6, 7, 8, 10, 11], dtype=cupy.int64)
     offsetslength = 3
-    fromstarts = cupy.array([0, 0, 0, 0, 0, 0, 0, 0], dtype=cupy.uint32)
-    fromstops = cupy.array([1, 1, 1, 1, 1, 1, 1, 1], dtype=cupy.uint32)
+    fromstarts = cupy.array([0, 0, 0, 0, 0, 0, 0, 0], dtype=cupy.int32)
+    fromstops = cupy.array([1, 1, 1, 1, 1, 1, 1, 1], dtype=cupy.int32)
     lencontent = 6
-    funcC = cupy_backend['awkward_ListArray_broadcast_tooffsets', cupy.int64, cupy.int64, cupy.uint32, cupy.uint32]
+    funcC = cupy_backend['awkward_ListArray_broadcast_tooffsets', cupy.int64, cupy.int64, cupy.int32, cupy.int32]
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_combinations_length_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_combinations_length_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_compact_offsets_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_compact_offsets_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_jagged_descend_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_jagged_descend_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_jagged_expand_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_jagged_expand_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_next_array_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_next_array_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_next_array_advanced_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_next_array_advanced_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_next_at_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_next_at_64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_next_range_counts_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_next_range_counts_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_next_range_spreadadvanced_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_getitem_next_range_spreadadvanced_64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_localindex_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_localindex_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_min_range.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_min_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_rpad_and_clip_length_axis1.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_rpad_and_clip_length_axis1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_rpad_axis1_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_rpad_axis1_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArrayU32_validity.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArrayU32_validity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray_fill_to64_from32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray_fill_to64_from32.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray_fill_to64_from64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray_fill_to64_from64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray_fill_to64_fromU32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray_fill_to64_fromU32.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray_getitem_jagged_carrylen_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray_getitem_jagged_carrylen_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListArray_getitem_jagged_numvalid_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListArray_getitem_jagged_numvalid_64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray32_flatten_offsets_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray32_flatten_offsets_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray32_reduce_local_nextparents_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArrayU32_reduce_local_nextparents_64.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_ListOffsetArray32_reduce_local_nextparents_64_1():
+def test_cudaawkward_ListOffsetArrayU32_reduce_local_nextparents_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray32_rpad_and_clip_axis1_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray64_rpad_and_clip_axis1_64.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_ListOffsetArray32_rpad_and_clip_axis1_64_1():
+def test_cudaawkward_ListOffsetArray64_rpad_and_clip_axis1_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray32_rpad_axis1_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray32_rpad_axis1_64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray32_rpad_length_axis1.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArrayU32_rpad_length_axis1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_ListOffsetArray32_rpad_length_axis1_1():
+def test_cudaawkward_ListOffsetArrayU32_rpad_length_axis1_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray32_toRegularArray.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray32_toRegularArray.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray64_flatten_offsets_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray64_flatten_offsets_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray64_reduce_local_nextparents_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray64_reduce_local_nextparents_64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray64_rpad_and_clip_axis1_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromfloat64.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_ListOffsetArray64_rpad_and_clip_axis1_64_1():
+def test_cudaawkward_NumpyArray_fill_touint32_fromfloat64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray64_rpad_axis1_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray64_rpad_axis1_64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray64_rpad_length_axis1.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromuint64.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_ListOffsetArray64_rpad_length_axis1_1():
+def test_cudaawkward_NumpyArray_fill_tofloat32_fromuint64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray64_toRegularArray.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray64_toRegularArray.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArrayU32_flatten_offsets_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArrayU32_flatten_offsets_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArrayU32_reduce_local_nextparents_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromuint64.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_ListOffsetArrayU32_reduce_local_nextparents_64_1():
+def test_cudaawkward_NumpyArray_fill_touint64_fromuint64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArrayU32_rpad_and_clip_axis1_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArrayU32_rpad_and_clip_axis1_64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArrayU32_rpad_axis1_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArrayU32_rpad_axis1_64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArrayU32_rpad_length_axis1.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray64_rpad_length_axis1.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_ListOffsetArrayU32_rpad_length_axis1_1():
+def test_cudaawkward_ListOffsetArray64_rpad_length_axis1_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArrayU32_toRegularArray.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArrayU32_toRegularArray.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray_drop_none_indexes_32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray_drop_none_indexes_32.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray_drop_none_indexes_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray_drop_none_indexes_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray_local_preparenext_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromuint64.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_ListOffsetArray_local_preparenext_64_1():
+def test_cudaawkward_NumpyArray_fill_tofloat64_fromuint64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray_reduce_nonlocal_maxcount_offsetscopy_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_max_int16_int16_64.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_ListOffsetArray_reduce_nonlocal_maxcount_offsetscopy_64_1():
+def test_cudaawkward_reduce_max_int16_int16_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_ListOffsetArray_reduce_nonlocal_nextstarts_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray_reduce_nonlocal_nextstarts_64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_MaskedArray32_getitem_next_jagged_project.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_MaskedArray32_getitem_next_jagged_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_MaskedArray64_getitem_next_jagged_project.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_MaskedArray64_getitem_next_jagged_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_MaskedArrayU32_getitem_next_jagged_project.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_MaskedArrayU32_getitem_next_jagged_project.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromfloat32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromfloat32.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromfloat64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromfloat64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromint16.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromint32.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_tofloat32_fromint16_1():
+def test_cudaawkward_NumpyArray_fill_tofloat32_fromint32_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromint32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromint8.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_tofloat32_fromint32_1():
+def test_cudaawkward_NumpyArray_fill_tofloat32_fromint8_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromint64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromint64.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromint8.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromfloat32.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_tofloat32_fromint8_1():
+def test_cudaawkward_NumpyArray_fill_toint16_fromfloat32_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromuint16.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromuint8.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_tofloat32_fromuint16_1():
+def test_cudaawkward_NumpyArray_fill_tofloat32_fromuint8_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromuint32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromuint32.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromuint64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromuint32.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_tofloat32_fromuint64_1():
+def test_cudaawkward_NumpyArray_fill_toint32_fromuint32_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromuint8.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromuint8.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_tofloat32_fromuint8_1():
+def test_cudaawkward_NumpyArray_fill_toint16_fromuint8_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromfloat32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromfloat32.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromfloat64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromfloat64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_tofloat64_fromfloat64_1():
+def test_cudaawkward_NumpyArray_fill_toint16_fromfloat64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromint16.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromint16.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromint32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromfloat64.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_tofloat64_fromint32_1():
+def test_cudaawkward_NumpyArray_fill_tofloat64_fromfloat64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromint64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromint64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromint8.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromint8.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_tofloat64_fromint8_1():
+def test_cudaawkward_NumpyArray_fill_touint16_fromint8_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromuint16.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromuint16.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromuint32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromuint32.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_tofloat64_fromuint32_1():
+def test_cudaawkward_NumpyArray_fill_touint16_fromuint32_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromuint64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromuint8.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_tofloat64_fromuint64_1():
+def test_cudaawkward_NumpyArray_fill_toint64_fromuint8_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromuint8.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromint32.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_tofloat64_fromuint8_1():
+def test_cudaawkward_NumpyArray_fill_tofloat64_fromint32_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromfloat32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromfloat32.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_toint16_fromfloat32_1():
+def test_cudaawkward_NumpyArray_fill_touint16_fromfloat32_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromfloat64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromfloat64.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_toint16_fromfloat64_1():
+def test_cudaawkward_NumpyArray_fill_touint16_fromfloat64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromint16.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromuint16.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_toint16_fromint16_1():
+def test_cudaawkward_NumpyArray_fill_toint16_fromuint16_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromint32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromint16.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_toint16_fromint32_1():
+def test_cudaawkward_NumpyArray_fill_touint16_fromint16_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromint64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromint64.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromint8.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromint8.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_toint16_fromint8_1():
+def test_cudaawkward_NumpyArray_fill_touint64_fromint8_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromuint16.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromuint16.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_toint16_fromuint16_1():
+def test_cudaawkward_NumpyArray_fill_touint16_fromuint16_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromuint32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromuint32.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_toint16_fromuint32_1():
+def test_cudaawkward_NumpyArray_fill_touint64_fromuint32_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromuint64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromuint32.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_toint16_fromuint64_1():
+def test_cudaawkward_NumpyArray_fill_toint16_fromuint32_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromuint8.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromuint8.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_toint16_fromuint8_1():
+def test_cudaawkward_NumpyArray_fill_toint8_fromuint8_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromfloat32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromfloat32.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_toint32_fromfloat32_1():
+def test_cudaawkward_NumpyArray_fill_touint32_fromfloat32_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromfloat64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromfloat64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromint16.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromint16.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromint32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromint32.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromint64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromint64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromint8.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromint8.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromuint16.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromuint16.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromuint32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromuint32.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_toint32_fromuint32_1():
+def test_cudaawkward_NumpyArray_fill_toint8_fromuint32_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromuint64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromuint64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromuint8.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromuint8.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromfloat32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromfloat32.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_toint64_fromfloat32_1():
+def test_cudaawkward_NumpyArray_fill_touint64_fromfloat32_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromfloat64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromfloat64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromint16.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromint16.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_toint64_fromint16_1():
+def test_cudaawkward_NumpyArray_fill_touint64_fromint16_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromint32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromuint16.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_toint64_fromint32_1():
+def test_cudaawkward_NumpyArray_fill_touint64_fromuint16_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromint64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromint64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromint8.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromfloat64.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_toint64_fromint8_1():
+def test_cudaawkward_NumpyArray_fill_touint64_fromfloat64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromuint16.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromuint16.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_toint64_fromuint16_1():
+def test_cudaawkward_NumpyArray_fill_touint8_fromuint16_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromuint32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromuint16.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_toint64_fromuint32_1():
+def test_cudaawkward_NumpyArray_fill_touint32_fromuint16_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromuint64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromuint32.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_toint64_fromuint64_1():
+def test_cudaawkward_NumpyArray_fill_toint64_fromuint32_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromuint8.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromuint16.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_toint64_fromuint8_1():
+def test_cudaawkward_NumpyArray_fill_toint64_fromuint16_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromfloat32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromfloat32.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_toint8_fromfloat32_1():
+def test_cudaawkward_NumpyArray_fill_touint8_fromfloat32_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromfloat64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromfloat32.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_toint8_fromfloat64_1():
+def test_cudaawkward_NumpyArray_fill_toint8_fromfloat32_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromint16.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromint8.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_toint8_fromint16_1():
+def test_cudaawkward_NumpyArray_fill_toint16_fromint8_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromint32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromint32.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_toint8_fromint32_1():
+def test_cudaawkward_NumpyArray_fill_toint64_fromint32_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromint64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromint64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromint8.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromint8.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_toint8_fromint8_1():
+def test_cudaawkward_NumpyArray_fill_touint8_fromint8_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromuint16.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromuint16.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromuint32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromuint32.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_toint8_fromuint32_1():
+def test_cudaawkward_NumpyArray_fill_touint8_fromuint32_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromuint64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromuint64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromuint8.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromuint8.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_toint8_fromuint8_1():
+def test_cudaawkward_NumpyArray_fill_touint8_fromuint8_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromfloat32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromfloat64.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint16_fromfloat32_1():
+def test_cudaawkward_NumpyArray_fill_touint8_fromfloat64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromfloat64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromint16.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint16_fromfloat64_1():
+def test_cudaawkward_NumpyArray_fill_touint32_fromint16_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromint16.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromuint16.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint16_fromint16_1():
+def test_cudaawkward_NumpyArray_fill_tofloat32_fromuint16_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromint32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromuint8.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint16_fromint32_1():
+def test_cudaawkward_NumpyArray_fill_tofloat64_fromuint8_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromint64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromint32.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint16_fromint64_1():
+def test_cudaawkward_NumpyArray_fill_touint16_fromint32_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromint8.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromint8.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint16_fromint8_1():
+def test_cudaawkward_NumpyArray_fill_touint32_fromint8_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromuint16.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromuint8.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint16_fromuint16_1():
+def test_cudaawkward_NumpyArray_fill_touint16_fromuint8_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromuint32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromuint64.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint16_fromuint32_1():
+def test_cudaawkward_NumpyArray_fill_touint16_fromuint64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromuint64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromuint64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint16_fromuint64_1():
+def test_cudaawkward_NumpyArray_fill_touint8_fromuint64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromuint8.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromuint8.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint16_fromuint8_1():
+def test_cudaawkward_NumpyArray_fill_touint64_fromuint8_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromfloat32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint32_fromfloat32.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint32_fromfloat32_1():
+def test_cudaawkward_NumpyArray_fill_toint32_fromfloat32_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromfloat64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromint32.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint32_fromfloat64_1():
+def test_cudaawkward_NumpyArray_fill_touint32_fromint32_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromint16.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromint64.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint32_fromint16_1():
+def test_cudaawkward_NumpyArray_fill_touint32_fromint64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromint32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromuint8.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint32_fromint32_1():
+def test_cudaawkward_NumpyArray_fill_touint32_fromuint8_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromint64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromint64.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint32_fromint64_1():
+def test_cudaawkward_NumpyArray_fill_touint64_fromint64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromint8.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromint32.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint32_fromint8_1():
+def test_cudaawkward_NumpyArray_fill_touint64_fromint32_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromuint16.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromuint64.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint32_fromuint16_1():
+def test_cudaawkward_NumpyArray_fill_toint16_fromuint64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromuint32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromint64.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint32_fromuint32_1():
+def test_cudaawkward_NumpyArray_fill_touint8_fromint64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromuint64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint16_fromint64.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint32_fromuint64_1():
+def test_cudaawkward_NumpyArray_fill_touint16_fromint64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromuint8.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromint8.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint32_fromuint8_1():
+def test_cudaawkward_NumpyArray_fill_toint64_fromint8_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromfloat32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromfloat32.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint64_fromfloat32_1():
+def test_cudaawkward_NumpyArray_fill_toint64_fromfloat32_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromfloat64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromint16.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint64_fromfloat64_1():
+def test_cudaawkward_NumpyArray_fill_toint64_fromint16_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromint16.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat64_fromuint32.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint64_fromint16_1():
+def test_cudaawkward_NumpyArray_fill_tofloat64_fromuint32_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromint32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_max_uint32_uint32_64.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint64_fromint32_1():
+def test_cudaawkward_reduce_max_uint32_uint32_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromint64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_tofloat32_fromint16.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint64_fromint64_1():
+def test_cudaawkward_NumpyArray_fill_tofloat32_fromint16_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromuint64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray32_rpad_length_axis1.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint64_fromuint64_1():
+def test_cudaawkward_ListOffsetArray32_rpad_length_axis1_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint64_fromuint8.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray32_rpad_and_clip_axis1_64.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint64_fromuint8_1():
+def test_cudaawkward_ListOffsetArray32_rpad_and_clip_axis1_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromfloat32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_overlay_mask8_to64.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint8_fromfloat32_1():
+def test_cudaawkward_IndexedArray32_overlay_mask8_to64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromfloat64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_float32_64.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint8_fromfloat64_1():
+def test_cudaawkward_reduce_sum_bool_float32_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromint16.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromint16.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromint32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromuint32.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint8_fromint32_1():
+def test_cudaawkward_NumpyArray_fill_touint32_fromuint32_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromint64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_max_uint16_uint16_64.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint8_fromint64_1():
+def test_cudaawkward_reduce_max_uint16_uint16_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromint8.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint16_fromint16.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint8_fromint8_1():
+def test_cudaawkward_NumpyArray_fill_toint16_fromint16_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromuint16.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint32_fromuint64.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint8_fromuint16_1():
+def test_cudaawkward_NumpyArray_fill_touint32_fromuint64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromuint32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint8_fromint32.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint8_fromuint32_1():
+def test_cudaawkward_NumpyArray_fill_toint8_fromint32_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromuint64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_min_int16_int16_64.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint8_fromuint64_1():
+def test_cudaawkward_reduce_min_int16_int16_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_touint8_fromuint8.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_float64_64.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_fill_touint8_fromuint8_1():
+def test_cudaawkward_reduce_sum_bool_float64_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_pad_zero_to_length_uint8.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_pad_zero_to_length_uint8.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_reduce_adjust_starts_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_reduce_adjust_starts_64.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_reduce_adjust_starts_shifts_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray32_reduce_next_64.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_reduce_adjust_starts_shifts_64_1():
+def test_cudaawkward_IndexedArray32_reduce_next_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_NumpyArray_reduce_mask_ByteMaskedArray_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_reduce_next_64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_NumpyArray_reduce_mask_ByteMaskedArray_64_1():
+def test_cudaawkward_ByteMaskedArray_reduce_next_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_carry_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_carry_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_jagged_expand_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_jagged_expand_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_next_array_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_next_array_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_next_array_advanced_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_next_array_advanced_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_next_array_regularize_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_next_array_regularize_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_next_at_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_next_at_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_next_range_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_next_range_64.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_next_range_spreadadvanced_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_RegularArray_getitem_next_range_spreadadvanced_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_RegularArray_localindex_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_RegularArray_localindex_64.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_RegularArray_reduce_local_nextparents_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_RegularArray_reduce_local_nextparents_64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_RegularArray_reduce_nonlocal_preparenext_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ListOffsetArray_reduce_nonlocal_maxcount_offsetscopy_64.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_RegularArray_reduce_nonlocal_preparenext_64_1():
+def test_cudaawkward_ListOffsetArray_reduce_nonlocal_maxcount_offsetscopy_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_RegularArray_rpad_and_clip_axis1_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_RegularArray_rpad_and_clip_axis1_64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_32_project_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_32_project_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_32_simplify8_32_to8_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_32_simplify8_32_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_32_simplify8_64_to8_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_32_simplify8_64_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_32_simplify8_U32_to8_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_32_simplify8_U32_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_32_simplify_one_to8_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_32_simplify_one_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_32_validity.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_32_validity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_64_project_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_64_project_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_64_simplify8_32_to8_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_64_simplify8_32_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_64_simplify8_64_to8_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_64_simplify8_64_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_64_simplify8_U32_to8_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_64_simplify8_U32_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_64_simplify_one_to8_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_64_simplify_one_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_64_validity.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_64_validity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_U32_project_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_U32_project_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_U32_simplify8_32_to8_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_U32_simplify8_32_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_U32_simplify8_64_to8_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_U32_simplify8_64_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_U32_simplify8_U32_to8_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_U32_simplify8_U32_to8_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_U32_simplify_one_to8_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_U32_simplify_one_to8_64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_U32_validity.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_U32_validity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray8_regular_index_getsize.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray8_regular_index_getsize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray_fillindex_to64_count.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray_fillindex_to64_count.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray_fillindex_to64_from32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray_fillindex_to64_from32.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray_fillindex_to64_from64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray_fillindex_to64_from64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray_fillindex_to64_fromU32.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray_fillindex_to64_fromU32.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray_fillna_from32_to64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray_fillna_from32_to64.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray_fillna_from64_to64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray_fillna_from64_to64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray_fillna_fromU32_to64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray_fillna_fromU32_to64.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray_filltags_to8_const.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray_filltags_to8_const.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_UnionArray_filltags_to8_from8.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_UnionArray_filltags_to8_from8.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_index_rpad_and_clip_axis0_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_index_rpad_and_clip_axis0_64.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_index_rpad_and_clip_axis1_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_index_rpad_and_clip_axis1_64.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_localindex_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_localindex_64.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_missing_repeat_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_missing_repeat_64.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_bool_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_float64_64.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_countnonzero_bool_64_1():
+def test_cudaawkward_reduce_countnonzero_float64_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_float32_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_uint16_64.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_countnonzero_float32_64_1():
+def test_cudaawkward_reduce_countnonzero_uint16_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_float64_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_min_float64_float64_64.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_countnonzero_float64_64_1():
+def test_cudaawkward_reduce_min_float64_float64_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_int16_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_int16_64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_int32_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_int32_64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_int64_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_int64_64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_int8_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_int8_64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_uint16_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_min_uint16_uint16_64.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_countnonzero_uint16_64_1():
+def test_cudaawkward_reduce_min_uint16_uint16_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_uint32_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_min_int32_int32_64.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_countnonzero_uint32_64_1():
+def test_cudaawkward_reduce_min_int32_int32_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_uint64_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_min_uint64_uint64_64.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_countnonzero_uint64_64_1():
+def test_cudaawkward_reduce_min_uint64_uint64_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_uint8_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_uint16_64.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_countnonzero_uint8_64_1():
+def test_cudaawkward_reduce_sum_bool_uint16_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_max_float32_float32_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_reduce_mask_ByteMaskedArray_64.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_max_float32_float32_64_1():
+def test_cudaawkward_NumpyArray_reduce_mask_ByteMaskedArray_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_max_float64_float64_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray_reduce_next_fix_offsets_64.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_max_float64_float64_64_1():
+def test_cudaawkward_IndexedArray_reduce_next_fix_offsets_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_max_int16_int16_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_NumpyArray_fill_toint64_fromuint64.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_max_int16_int16_64_1():
+def test_cudaawkward_NumpyArray_fill_toint64_fromuint64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_max_int32_int32_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_max_int32_int32_64.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_max_int64_int64_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_max_int64_int64_64.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_max_uint64_uint64_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_max_uint64_uint64_64.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_max_uint8_uint8_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_max_uint8_uint8_64.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_min_float64_float64_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_float64_float64_64.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_min_float64_float64_64_1():
+def test_cudaawkward_reduce_sum_float64_float64_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_min_int16_int16_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_min_int64_int64_64.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_min_int16_int16_64_1():
+def test_cudaawkward_reduce_min_int64_int64_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_min_int32_int32_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_min_int32_int32_64_1():
+def test_cudaawkward_ByteMaskedArray_reduce_next_nonlocal_nextshifts_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_min_int64_int64_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_IndexedArray64_reduce_next_nonlocal_nextshifts_fromshifts_64.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_min_int64_int64_64_1():
+def test_cudaawkward_IndexedArray64_reduce_next_nonlocal_nextshifts_fromshifts_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_min_uint16_uint16_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint32_uint16_64.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_min_uint16_uint16_64_1():
+def test_cudaawkward_reduce_sum_uint32_uint16_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_min_uint64_uint64_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint64_uint32_64.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_min_uint64_uint64_64_1():
+def test_cudaawkward_reduce_sum_uint64_uint32_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_min_uint8_uint8_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_min_uint8_uint8_64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_float32_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_float32_64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_float64_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_float64_64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_int16_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_uint16_64.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_prod_bool_int16_64_1():
+def test_cudaawkward_reduce_prod_bool_uint16_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_int32_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_uint32_64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_prod_bool_int32_64_1():
+def test_cudaawkward_reduce_prod_bool_uint32_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_int64_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_int64_64.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_uint16_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_uint8_64.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_prod_bool_uint16_64_1():
+def test_cudaawkward_reduce_prod_bool_uint8_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_uint32_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_uint64_64.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_prod_bool_uint32_64_1():
+def test_cudaawkward_reduce_prod_bool_uint64_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_uint64_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_uint32_64.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_prod_bool_uint64_64_1():
+def test_cudaawkward_reduce_sum_bool_uint32_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_prod_bool_uint8_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_bool_64.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_prod_bool_uint8_64_1():
+def test_cudaawkward_reduce_countnonzero_bool_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_float32_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_float32_float32_64.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_sum_bool_float32_64_1():
+def test_cudaawkward_reduce_sum_float32_float32_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_float64_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_float32_64.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_sum_bool_float64_64_1():
+def test_cudaawkward_reduce_countnonzero_float32_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_uint16_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_int32_int16_64.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_sum_bool_uint16_64_1():
+def test_cudaawkward_reduce_sum_int32_int16_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_uint32_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_int32_int32_64.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_sum_bool_uint32_64_1():
+def test_cudaawkward_reduce_sum_int32_int32_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_bool_uint64_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_int64_int64_64.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_sum_bool_uint64_64_1():
+def test_cudaawkward_reduce_sum_int64_int64_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_float64_float64_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_min_float32_float32_64.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_sum_float64_float64_64_1():
+def test_cudaawkward_reduce_min_float32_float32_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_int32_int16_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_int64_int32_64.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_sum_int32_int16_64_1():
+def test_cudaawkward_reduce_sum_int64_int32_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_int32_int32_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_max_float32_float32_64.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_sum_int32_int32_64_1():
+def test_cudaawkward_reduce_max_float32_float32_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_int64_int16_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_int64_int16_64.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_int64_int32_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_uint32_64.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_sum_int64_int32_64_1():
+def test_cudaawkward_reduce_countnonzero_uint32_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_int64_int64_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint64_uint64_64.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_sum_int64_int64_64_1():
+def test_cudaawkward_reduce_sum_uint64_uint64_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint32_uint16_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint64_uint16_64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_sum_uint32_uint16_64_1():
+def test_cudaawkward_reduce_sum_uint64_uint16_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint32_uint32_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint32_uint32_64.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint32_uint8_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint32_uint8_64.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint64_uint16_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint64_uint8_64.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_sum_uint64_uint16_64_1():
+def test_cudaawkward_reduce_sum_uint64_uint8_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint64_uint32_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_min_uint32_uint32_64.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_sum_uint64_uint32_64_1():
+def test_cudaawkward_reduce_min_uint32_uint32_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint64_uint64_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_uint64_64.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_sum_uint64_uint64_64_1():
+def test_cudaawkward_reduce_countnonzero_uint64_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/tests-cuda-kernels/test_cudaawkward_reduce_sum_uint64_uint8_64.py` & `awkward-2.6.3rc2/tests-cuda-kernels/test_cudaawkward_reduce_countnonzero_uint8_64.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# AUTO GENERATED ON 2024-04-01 AT 18:26:47
+# AUTO GENERATED ON 2024-03-21 AT 23:08:24
 # DO NOT EDIT BY HAND!
 #
 # To regenerate file, run
 #
 #     python dev/generate-tests.py
 #
 
@@ -14,9 +14,9 @@
 import awkward as ak
 import awkward._connect.cuda as ak_cu
 from awkward._backends.cupy import CupyBackend
 
 cupy_backend = CupyBackend.instance()
 
 @pytest.mark.skip(reason='Unable to generate any tests for kernel')
-def test_cudaawkward_reduce_sum_uint64_uint8_64_1():
+def test_cudaawkward_reduce_countnonzero_uint8_64_1():
     raise NotImplementedError('Unable to generate any tests for kernel')
```

### Comparing `awkward-2.6.3/.gitignore` & `awkward-2.6.3rc2/.gitignore`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/LICENSE` & `awkward-2.6.3rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `awkward-2.6.3/pyproject.toml` & `awkward-2.6.3rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "hatchling>=1.10.0",
     "hatch-fancy-pypi-readme"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "awkward"
-version = "2.6.3"
+version = "2.6.3rc2"
 description = "Manipulate JSON-like data with NumPy-like idioms."
 license = { text = "BSD-3-Clause" }
 requires-python = ">=3.8"
 authors = [
     { name = "Jim Pivarski", email = "pivarski@princeton.edu" },
 ]
 classifiers = [
@@ -36,17 +36,17 @@
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Software Development",
     "Topic :: Utilities",
 ]
 dependencies = [
-    "awkward_cpp==32",
+    "awkward_cpp==31",
     "importlib_metadata>=4.13.0;python_version < \"3.12\"",
-    "numpy>=1.18.0",
+    "numpy>=1.18.0,<2.0",
     "packaging",
     "typing_extensions>=4.1.0; python_version < \"3.11\"",
     "fsspec>=2022.11.0"
 ]
 dynamic = [
     "readme"
 ]
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
 [build-system] requires = [ "hatchling>=1.10.0", "hatch-fancy-pypi-readme" ]
-build-backend = "hatchling.build" [project] name = "awkward" version = "2.6.3"
-description = "Manipulate JSON-like data with NumPy-like idioms." license =
-{ text = "BSD-3-Clause" } requires-python = ">=3.8" authors = [ { name = "Jim
-Pivarski", email = "pivarski@princeton.edu" }, ] classifiers = [ "Development
-Status :: 5 - Production/Stable", "Intended Audience :: Developers", "Intended
-Audience :: Information Technology", "Intended Audience :: Science/Research",
-"License :: OSI Approved :: BSD License", "Operating System :: MacOS :: MacOS
-X", "Operating System :: Microsoft :: Windows", "Operating System :: POSIX ::
-Linux", "Operating System :: Unix", "Programming Language :: Python",
-"Programming Language :: Python :: 3 :: Only", "Programming Language :: Python
-:: 3", "Programming Language :: Python :: 3.8", "Programming Language :: Python
-:: 3.9", "Programming Language :: Python :: 3.10", "Programming Language ::
-Python :: 3.11", "Programming Language :: Python :: 3.12", "Topic ::
-Scientific/Engineering", "Topic :: Scientific/Engineering :: Information
-Analysis", "Topic :: Scientific/Engineering :: Mathematics", "Topic ::
-Scientific/Engineering :: Physics", "Topic :: Software Development", "Topic ::
-Utilities", ] dependencies = [ "awkward_cpp==32",
-"importlib_metadata>=4.13.0;python_version < \"3.12\"", "numpy>=1.18.0",
+build-backend = "hatchling.build" [project] name = "awkward" version =
+"2.6.3rc2" description = "Manipulate JSON-like data with NumPy-like idioms."
+license = { text = "BSD-3-Clause" } requires-python = ">=3.8" authors = [
+{ name = "Jim Pivarski", email = "pivarski@princeton.edu" }, ] classifiers =
+[ "Development Status :: 5 - Production/Stable", "Intended Audience ::
+Developers", "Intended Audience :: Information Technology", "Intended Audience
+:: Science/Research", "License :: OSI Approved :: BSD License", "Operating
+System :: MacOS :: MacOS X", "Operating System :: Microsoft :: Windows",
+"Operating System :: POSIX :: Linux", "Operating System :: Unix", "Programming
+Language :: Python", "Programming Language :: Python :: 3 :: Only",
+"Programming Language :: Python :: 3", "Programming Language :: Python :: 3.8",
+"Programming Language :: Python :: 3.9", "Programming Language :: Python ::
+3.10", "Programming Language :: Python :: 3.11", "Programming Language ::
+Python :: 3.12", "Topic :: Scientific/Engineering", "Topic :: Scientific/
+Engineering :: Information Analysis", "Topic :: Scientific/Engineering ::
+Mathematics", "Topic :: Scientific/Engineering :: Physics", "Topic :: Software
+Development", "Topic :: Utilities", ] dependencies = [ "awkward_cpp==31",
+"importlib_metadata>=4.13.0;python_version < \"3.12\"", "numpy>=1.18.0,<2.0",
 "packaging", "typing_extensions>=4.1.0; python_version < \"3.11\"",
 "fsspec>=2022.11.0" ] dynamic = [ "readme" ] [project.entry-
 points.numba_extensions] init = "awkward.numba:_register" [project.urls] "Bug
 Tracker" = "https://github.com/scikit-hep/awkward-1.0/issues" "Chat" = "https:/
 /gitter.im/Scikit-HEP/awkward-array" "Discussions" = "https://github.com/
 scikit-hep/awkward-1.0/discussions" "Documentation" = "https://awkward-
 array.org" "Homepage" = "https://github.com/scikit-hep/awkward-1.0" "Releases"
```

### Comparing `awkward-2.6.3/PKG-INFO` & `awkward-2.6.3rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: awkward
-Version: 2.6.3
+Version: 2.6.3rc2
 Summary: Manipulate JSON-like data with NumPy-like idioms.
 Project-URL: Bug Tracker, https://github.com/scikit-hep/awkward-1.0/issues
 Project-URL: Chat, https://gitter.im/Scikit-HEP/awkward-array
 Project-URL: Discussions, https://github.com/scikit-hep/awkward-1.0/discussions
 Project-URL: Documentation, https://awkward-array.org
 Project-URL: Homepage, https://github.com/scikit-hep/awkward-1.0
 Project-URL: Releases, https://github.com/scikit-hep/awkward-1.0/releases
@@ -32,18 +32,18 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Software Development
 Classifier: Topic :: Utilities
 Requires-Python: >=3.8
-Requires-Dist: awkward-cpp==32
+Requires-Dist: awkward-cpp==31
 Requires-Dist: fsspec>=2022.11.0
 Requires-Dist: importlib-metadata>=4.13.0; python_version < '3.12'
-Requires-Dist: numpy>=1.18.0
+Requires-Dist: numpy<2.0,>=1.18.0
 Requires-Dist: packaging
 Requires-Dist: typing-extensions>=4.1.0; python_version < '3.11'
 Description-Content-Type: text/markdown
 
 <a href="https://github.com/scikit-hep/awkward-1.0">
     <img src="https://github.com/scikit-hep/awkward-1.0/raw/main/docs-img/logo/logo-300px.png">
 </a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: awkward Version: 2.6.3 Summary: Manipulate JSON-
+Metadata-Version: 2.3 Name: awkward Version: 2.6.3rc2 Summary: Manipulate JSON-
 like data with NumPy-like idioms. Project-URL: Bug Tracker, https://github.com/
 scikit-hep/awkward-1.0/issues Project-URL: Chat, https://gitter.im/Scikit-HEP/
 awkward-array Project-URL: Discussions, https://github.com/scikit-hep/awkward-
 1.0/discussions Project-URL: Documentation, https://awkward-array.org Project-
 URL: Homepage, https://github.com/scikit-hep/awkward-1.0 Project-URL: Releases,
 https://github.com/scikit-hep/awkward-1.0/releases Project-URL: Source Code,
 https://github.com/scikit-hep/awkward-1.0 Author-email: Jim Pivarski
@@ -18,27 +18,27 @@
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Scientific/Engineering Classifier: Topic :: Scientific/Engineering ::
 Information Analysis Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics Classifier: Topic ::
 Software Development Classifier: Topic :: Utilities Requires-Python: >=3.8
-Requires-Dist: awkward-cpp==32 Requires-Dist: fsspec>=2022.11.0 Requires-Dist:
+Requires-Dist: awkward-cpp==31 Requires-Dist: fsspec>=2022.11.0 Requires-Dist:
 importlib-metadata>=4.13.0; python_version < '3.12' Requires-Dist:
-numpy>=1.18.0 Requires-Dist: packaging Requires-Dist: typing-extensions>=4.1.0;
-python_version < '3.11' Description-Content-Type: text/markdown _[_h_t_t_p_s_:_/_/
-_g_i_t_h_u_b_._c_o_m_/_s_c_i_k_i_t_-_h_e_p_/_a_w_k_w_a_r_d_-_1_._0_/_r_a_w_/_m_a_i_n_/_d_o_c_s_-_i_m_g_/_l_o_g_o_/_l_o_g_o_-_3_0_0_p_x_._p_n_g_][![PyPI
-version](https://badge.fury.io/py/awkward.svg)](https://pypi.org/project/
-awkward) [![Conda-Forge](https://img.shields.io/conda/vn/conda-forge/awkward)]
-(https://github.com/conda-forge/awkward-feedstock) [![Python 3.8â3.12](https:
-//img.shields.io/badge/python-3.8%E2%80%923.12-blue)](https://www.python.org)
-[![BSD-3 Clause License](https://img.shields.io/badge/license-BSD%203--Clause-
-blue.svg)](https://opensource.org/licenses/BSD-3-Clause) [![Build Test](https:/
-/github.com/scikit-hep/awkward/actions/workflows/test.yml/
-badge.svg?branch=main)](https://github.com/scikit-hep/awkward/actions/
+numpy<2.0,>=1.18.0 Requires-Dist: packaging Requires-Dist: typing-
+extensions>=4.1.0; python_version < '3.11' Description-Content-Type: text/
+markdown _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_s_c_i_k_i_t_-_h_e_p_/_a_w_k_w_a_r_d_-_1_._0_/_r_a_w_/_m_a_i_n_/_d_o_c_s_-_i_m_g_/_l_o_g_o_/
+_l_o_g_o_-_3_0_0_p_x_._p_n_g_][![PyPI version](https://badge.fury.io/py/awkward.svg)](https://
+pypi.org/project/awkward) [![Conda-Forge](https://img.shields.io/conda/vn/
+conda-forge/awkward)](https://github.com/conda-forge/awkward-feedstock) [!
+[Python 3.8â3.12](https://img.shields.io/badge/python-3.8%E2%80%923.12-blue)]
+(https://www.python.org) [![BSD-3 Clause License](https://img.shields.io/badge/
+license-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-
+Clause) [![Build Test](https://github.com/scikit-hep/awkward/actions/workflows/
+test.yml/badge.svg?branch=main)](https://github.com/scikit-hep/awkward/actions/
 workflows/test.yml) [![Scikit-HEP](https://scikit-hep.org/assets/images/Scikit-
 -HEP-Project-blue.svg)](https://scikit-hep.org/) [![NSF-1836650](https://
 img.shields.io/badge/NSF-1836650-blue.svg)](https://nsf.gov/awardsearch/
 showAward?AWD_ID=1836650) [![DOI](https://zenodo.org/badge/DOI/10.5281/
 zenodo.4341376.svg)](https://doi.org/10.5281/zenodo.4341376) [![Documentation]
 (https://img.shields.io/badge/docs-online-success)](https://awkward-array.org/
 ) [![Gitter](https://img.shields.io/badge/chat-online-success)](https://
```

