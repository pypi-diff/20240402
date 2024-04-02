# Comparing `tmp/schemaorg_lite-0.1.7.tar.gz` & `tmp/schemaorg_lite-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schemaorg_lite-0.1.7.tar", last modified: Mon Feb 19 14:19:14 2024, max compression
+gzip compressed data, was "schemaorg_lite-0.1.8.tar", last modified: Tue Apr  2 10:37:49 2024, max compression
```

## Comparing `schemaorg_lite-0.1.7.tar` & `schemaorg_lite-0.1.8.tar`

### file list

```diff
@@ -1,253 +1,253 @@
--rw-r--r--   0        0        0     1518 2023-11-06 10:34:52.313204 schemaorg_lite-0.1.7/LICENSE
--rw-r--r--   0        0        0      549 2023-11-06 14:14:41.344426 schemaorg_lite-0.1.7/README.md
--rw-r--r--   0        0        0     2447 2024-02-19 14:19:14.963167 schemaorg_lite-0.1.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-13 08:01:43.682908 schemaorg_lite-0.1.7/schemaorg_lite/__init__.py
--rw-r--r--   0        0        0     2880 2024-02-04 20:25:18.335170 schemaorg_lite-0.1.7/schemaorg_lite/data/__init__.py
--rw-r--r--   0        0        0     1172 2023-11-06 13:42:05.342534 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/attic/attic.ttl
--rw-r--r--   0        0        0    14554 2023-11-06 13:42:05.338823 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/auto/auto.ttl
--rw-r--r--   0        0        0     8237 2023-11-06 13:42:05.327404 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/bib/bsdo-1.0.ttl
--rw-r--r--   0        0        0     1876 2023-11-06 13:42:05.343728 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/bib/bsdo-atlas-examples.txt
--rw-r--r--   0        0        0     7041 2023-11-06 13:42:05.343211 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/bib/bsdo-audiobook-examples.txt
--rw-r--r--   0        0        0     2487 2023-11-06 13:42:05.343890 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/bib/bsdo-chapter-examples.txt
--rw-r--r--   0        0        0     6615 2023-11-06 13:42:05.328999 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/bib/bsdo-collection-examples.txt
--rw-r--r--   0        0        0     1832 2023-11-06 13:42:05.328293 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/bib/bsdo-newspaper-examples.txt
--rw-r--r--   0        0        0     1829 2023-11-06 13:42:05.355053 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/bib/bsdo-thesis-examples.txt
--rw-r--r--   0        0        0     4831 2023-11-06 13:42:05.342706 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/bib/bsdo-translation-examples.txt
--rw-r--r--   0        0        0     6635 2023-11-06 13:42:05.344253 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/bib/comics-examples.txt
--rw-r--r--   0        0        0     6381 2023-11-06 13:42:05.321520 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/health-lifesci/MedicalScholarlyArticle-examples.txt
--rw-r--r--   0        0        0    11809 2023-11-06 10:46:38.741032 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/health-lifesci/drug-example.txt
--rw-r--r--   0        0        0   111217 2023-11-06 13:42:05.322642 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/health-lifesci/med-health-core.ttl
--rw-r--r--   0        0        0    12612 2023-11-06 13:42:05.321202 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/health-lifesci/medicalCondition-examples.txt
--rw-r--r--   0        0        0     4078 2023-11-06 13:42:05.342871 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/health-lifesci/medicalGuideline-examples.txt
--rw-r--r--   0        0        0     3511 2023-11-06 13:42:05.356629 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/health-lifesci/medicalWebpage-examples.txt
--rw-r--r--   0        0        0     6389 2023-11-06 13:42:05.344371 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/health-lifesci/physical-activity-and-exercise.ttl
--rwxr-xr-x   0        0        0     3106 2023-11-06 10:46:38.748851 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/meta/meta.jsonld.someday.txt
--rw-r--r--   0        0        0     2391 2023-11-06 13:42:05.320084 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/meta/meta.ttl
--rw-r--r--   0        0        0     1042 2023-11-06 13:42:05.316356 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1045-examples.txt
--rw-r--r--   0        0        0     1203 2023-11-06 13:42:05.353481 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1045.ttl
--rw-r--r--   0        0        0      519 2023-11-06 13:42:05.354431 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1050-examples.txt
--rw-r--r--   0        0        0      682 2023-11-06 13:42:05.322960 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1050.ttl
--rw-r--r--   0        0        0     4269 2023-11-06 13:42:05.318097 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1062-examples.txt
--rw-r--r--   0        0        0     8850 2023-11-06 13:42:05.326560 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1062.ttl
--rw-r--r--   0        0        0      844 2023-11-06 13:42:05.339439 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1083.ttl
--rw-r--r--   0        0        0    15347 2023-11-06 13:42:05.354911 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1156-examples.txt
--rw-r--r--   0        0        0    15890 2023-11-06 13:42:05.326211 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1156.ttl
--rw-r--r--   0        0        0     2234 2023-11-06 13:42:05.358069 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1244.ttl
--rw-r--r--   0        0        0    14580 2023-11-06 13:42:02.072298 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1253-examples.txt
--rw-r--r--   0        0        0    12976 2023-11-06 13:42:05.327958 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1253.ttl
--rw-r--r--   0        0        0     5290 2023-11-06 13:42:05.321474 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1375.ttl
--rw-r--r--   0        0        0     1328 2023-11-06 13:42:05.328523 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1389-examples.txt
--rw-r--r--   0        0        0     1176 2023-11-06 13:42:05.339778 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1397.ttl
--rw-r--r--   0        0        0     1476 2023-11-06 13:42:05.343369 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1401.ttl
--rw-r--r--   0        0        0      692 2023-11-06 13:42:05.353269 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1423-examples.txt
--rw-r--r--   0        0        0     1209 2023-11-06 13:42:05.326763 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1423.ttl
--rw-r--r--   0        0        0     2939 2023-11-06 13:42:05.340119 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1425.ttl
--rw-r--r--   0        0        0     1493 2023-11-06 13:42:05.313904 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1448.ttl
--rw-r--r--   0        0        0     3997 2023-11-06 13:42:05.339151 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1457-examples.txt
--rw-r--r--   0        0        0     5564 2023-11-06 13:42:05.316564 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1457.ttl
--rw-r--r--   0        0        0      562 2023-11-06 13:42:05.358267 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1495.ttl
--rw-r--r--   0        0        0     1908 2023-11-06 13:42:05.344691 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1525-examples.txt
--rw-r--r--   0        0        0    12233 2023-11-06 13:42:05.321331 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1525.ttl
--rw-r--r--   0        0        0      572 2023-11-06 13:42:05.352900 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1559.ttl
--rw-r--r--   0        0        0      639 2023-11-06 13:42:05.341259 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1576.ttl
--rw-r--r--   0        0        0     1422 2023-11-06 13:42:05.315869 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1589.ttl
--rw-r--r--   0        0        0      595 2023-11-06 13:42:05.353938 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1591.ttl
--rw-r--r--   0        0        0      694 2023-11-06 13:42:05.343006 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1624.ttl
--rw-r--r--   0        0        0      364 2023-11-06 13:42:05.337920 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1670-examples.txt
--rw-r--r--   0        0        0      808 2023-11-06 13:42:05.320239 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1672.ttl
--rw-r--r--   0        0        0     2659 2023-11-06 10:46:38.758865 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1688.ttl
--rw-r--r--   0        0        0      988 2023-11-06 13:42:05.340717 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1689-examples.txt
--rw-r--r--   0        0        0     2996 2023-11-06 13:42:05.316153 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1698-examples.txt
--rw-r--r--   0        0        0     1120 2023-11-06 13:42:05.321054 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1741-examples.txt
--rw-r--r--   0        0        0     1914 2023-11-06 13:42:05.353785 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1755.ttl
--rw-r--r--   0        0        0    15754 2023-11-06 13:42:05.324146 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1758-examples.txt
--rw-r--r--   0        0        0     2262 2023-11-06 13:42:05.318249 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1758.ttl
--rw-r--r--   0        0        0     3022 2023-11-06 13:42:05.341675 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1759-examples.txt
--rw-r--r--   0        0        0      966 2023-11-06 13:42:05.341357 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1759.ttl
--rw-r--r--   0        0        0    10049 2023-11-06 13:42:05.322368 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1779-examples.txt
--rw-r--r--   0        0        0     3566 2023-11-06 13:42:05.317411 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1779.ttl
--rw-r--r--   0        0        0     4041 2023-11-06 13:42:05.318687 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1797.ttl
--rw-r--r--   0        0        0    47423 2023-11-06 13:42:05.317564 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1810-examples.txt
--rw-r--r--   0        0        0     3927 2023-11-06 13:42:05.358562 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1810.ttl
--rw-r--r--   0        0        0      738 2023-11-06 13:42:05.341619 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1816.ttl
--rw-r--r--   0        0        0     2112 2023-11-06 13:42:05.337288 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1828.ttl
--rw-r--r--   0        0        0     3219 2023-11-06 13:42:05.340996 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1842-examples.txt
--rw-r--r--   0        0        0     3572 2023-11-06 13:42:05.343821 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1842.ttl
--rw-r--r--   0        0        0     1732 2023-11-06 13:42:05.342691 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1886.ttl
--rw-r--r--   0        0        0      763 2023-11-06 13:42:05.344063 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1909.ttl
--rw-r--r--   0        0        0     1038 2023-11-06 13:42:05.315715 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1950-examples.txt
--rw-r--r--   0        0        0     1006 2023-11-06 13:42:05.343131 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1950.ttl
--rw-r--r--   0        0        0      453 2023-11-06 13:42:05.341105 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1951.ttl
--rw-r--r--   0        0        0      568 2023-11-06 13:42:05.338485 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1976.ttl
--rw-r--r--   0        0        0      406 2023-11-06 13:42:05.315010 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2021-examples.txt
--rw-r--r--   0        0        0      942 2023-11-06 13:42:05.342141 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2021.ttl
--rw-r--r--   0        0        0      459 2023-11-06 13:42:05.324981 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2083-examples.txt
--rw-r--r--   0        0        0      784 2023-11-06 13:42:05.324262 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2083.ttl
--rw-r--r--   0        0        0      390 2023-11-06 13:42:05.321874 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2085-examples.txt
--rw-r--r--   0        0        0      737 2023-11-06 13:42:05.320393 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2085.ttl
--rw-r--r--   0        0        0      860 2023-11-06 13:42:05.338655 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2108-examples.txt
--rw-r--r--   0        0        0     1722 2023-11-06 13:42:05.317044 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2108.ttl
--rw-r--r--   0        0        0      287 2023-11-06 13:42:05.341469 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2109-examples.txt
--rw-r--r--   0        0        0     1094 2023-11-06 13:42:05.342853 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2109.ttl
--rw-r--r--   0        0        0      666 2023-11-06 13:42:05.316010 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2110.ttl
--rw-r--r--   0        0        0      994 2023-11-06 13:42:05.344097 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2111.ttl
--rw-r--r--   0        0        0      638 2023-11-06 13:42:05.345408 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2126.ttl
--rw-r--r--   0        0        0     1113 2023-11-06 13:42:05.322253 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2140.ttl
--rw-r--r--   0        0        0     1608 2023-11-06 13:42:05.345472 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2173-examples.txt
--rw-r--r--   0        0        0      953 2023-11-06 13:42:05.317201 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2173.ttl
--rw-r--r--   0        0        0     1626 2023-11-06 13:42:05.321989 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2192-examples.txt
--rw-r--r--   0        0        0      587 2023-11-06 13:42:05.356318 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2192.ttl
--rw-r--r--   0        0        0      622 2023-11-06 13:42:05.343556 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2242.ttl
--rw-r--r--   0        0        0     1099 2023-11-06 13:42:05.322492 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2244.ttl
--rw-r--r--   0        0        0     3792 2023-11-06 13:42:05.345147 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2288.ttl
--rw-r--r--   0        0        0     3406 2023-11-06 13:42:05.314604 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2289-examples.txt
--rw-r--r--   0        0        0     5153 2023-11-06 13:42:05.354571 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2289.ttl
--rw-r--r--   0        0        0       28 2023-11-06 13:42:05.340865 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2291.ttl
--rw-r--r--   0        0        0      708 2023-11-06 13:42:05.328686 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2294-examples.txt
--rw-r--r--   0        0        0      757 2023-11-06 13:42:05.344870 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2296-examples.txt
--rw-r--r--   0        0        0      644 2023-11-06 13:42:05.345683 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2296.ttl
--rw-r--r--   0        0        0      775 2023-11-06 13:42:05.341948 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2300.ttl
--rw-r--r--   0        0        0     1402 2023-11-06 13:42:05.343389 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2311.ttl
--rw-r--r--   0        0        0      663 2023-11-06 13:42:05.328132 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2329.ttl
--rw-r--r--   0        0        0      454 2023-11-06 13:42:05.355839 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2341.ttl
--rw-r--r--   0        0        0     1824 2023-11-06 13:42:05.344841 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2348.ttl
--rw-r--r--   0        0        0      993 2023-11-06 13:42:05.341935 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2358.ttl
--rw-r--r--   0        0        0     2527 2023-11-06 13:42:05.315571 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2366-examples.txt
--rw-r--r--   0        0        0     8264 2023-11-06 13:42:05.339605 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2373.ttl
--rw-r--r--   0        0        0    11319 2023-11-06 10:46:38.774343 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2374.ttl
--rw-r--r--   0        0        0    15957 2023-11-06 13:42:05.357537 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2381.ttl
--rw-r--r--   0        0        0      423 2023-11-06 13:42:05.339949 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2382.ttl
--rw-r--r--   0        0        0     1021 2023-11-06 13:42:05.343256 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2384-examples.txt
--rw-r--r--   0        0        0     2153 2023-11-06 13:42:05.328847 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2384.ttl
--rw-r--r--   0        0        0      677 2023-11-06 13:42:05.319746 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2394.ttl
--rw-r--r--   0        0        0     1683 2023-11-06 13:42:05.357396 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2396-examples.txt
--rw-r--r--   0        0        0      962 2023-11-06 13:42:05.358416 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2396.ttl
--rw-r--r--   0        0        0    12842 2023-11-06 13:42:05.357289 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2405-examples.txt
--rw-r--r--   0        0        0     1668 2023-11-06 13:42:05.324511 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2405.ttl
--rw-r--r--   0        0        0      683 2023-11-06 13:42:05.337540 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2418.ttl
--rw-r--r--   0        0        0      658 2023-11-06 13:42:05.344538 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2419-examples.txt
--rw-r--r--   0        0        0     4491 2023-11-06 13:42:05.342998 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2419.ttl
--rw-r--r--   0        0        0      410 2023-11-06 13:42:05.322220 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2420.ttl
--rw-r--r--   0        0        0     1307 2023-11-06 13:42:05.338226 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2421-examples.txt
--rw-r--r--   0        0        0      456 2023-11-06 13:42:05.340402 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2421.ttl
--rw-r--r--   0        0        0     1093 2023-11-06 13:42:05.326085 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2427.ttl
--rw-r--r--   0        0        0     1587 2023-11-06 13:42:05.344727 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2450-examples.txt
--rw-r--r--   0        0        0    18210 2023-11-06 10:46:38.778535 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2450.ttl
--rw-r--r--   0        0        0     1795 2023-11-06 13:42:05.357156 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2454.ttl
--rw-r--r--   0        0        0     1136 2023-11-06 13:42:05.327425 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2460.ttl
--rw-r--r--   0        0        0     2179 2023-11-06 13:42:05.321828 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2469.ttl
--rw-r--r--   0        0        0     3064 2023-11-06 13:42:05.354773 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2482-examples.txt
--rw-r--r--   0        0        0      817 2023-11-06 13:42:05.315139 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2483.ttl
--rw-r--r--   0        0        0      510 2023-11-06 13:42:05.316769 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2486.ttl
--rw-r--r--   0        0        0     3601 2023-11-06 13:42:05.314163 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2490-examples.txt
--rw-r--r--   0        0        0     9452 2023-11-06 13:42:05.324470 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2490.ttl
--rw-r--r--   0        0        0      510 2023-11-06 13:42:05.317783 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2493.ttl
--rw-r--r--   0        0        0      427 2023-11-06 13:42:05.323567 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2496.ttl
--rw-r--r--   0        0        0      576 2023-11-06 13:42:05.344414 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2500.ttl
--rw-r--r--   0        0        0    12914 2023-11-06 13:42:05.323260 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2506.ttl
--rw-r--r--   0        0        0     1342 2023-11-06 10:46:38.781728 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2514-examples.txt
--rw-r--r--   0        0        0      893 2023-11-06 13:42:05.345260 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2514.ttl
--rw-r--r--   0        0        0     7820 2023-11-06 13:42:05.319446 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2521.ttl
--rw-r--r--   0        0        0      536 2023-11-06 13:42:05.322652 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2526.ttl
--rw-r--r--   0        0        0     1360 2023-11-06 13:42:05.337741 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2534-examples.txt
--rw-r--r--   0        0        0     3813 2023-11-06 13:42:05.318496 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2534.ttl
--rw-r--r--   0        0        0      713 2023-11-06 10:46:38.783666 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2543-examples.txt
--rw-r--r--   0        0        0    14774 2023-11-06 13:42:05.320548 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2543.ttl
--rw-r--r--   0        0        0     1297 2023-11-06 10:46:38.784230 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2564-examples.txt
--rw-r--r--   0        0        0    13020 2023-11-06 10:46:38.784549 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2564.ttl
--rw-r--r--   0        0        0      672 2023-11-06 10:46:38.784766 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2599-examples.txt
--rw-r--r--   0        0        0      753 2023-11-06 13:42:05.341399 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2599.ttl
--rw-r--r--   0        0        0      680 2023-11-06 13:42:05.345117 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2605.ttl
--rw-r--r--   0        0        0      524 2023-11-06 13:42:05.327108 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2611.ttl
--rw-r--r--   0        0        0      730 2023-11-06 13:42:05.323743 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2636.ttl
--rw-r--r--   0        0        0      605 2023-11-06 13:42:05.357845 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2646.ttl
--rw-r--r--   0        0        0     1035 2023-11-06 13:42:05.319297 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2659.ttl
--rw-r--r--   0        0        0      694 2023-11-06 13:42:05.323413 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2665.ttl
--rw-r--r--   0        0        0     7938 2023-11-06 13:42:05.327278 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2670.ttl
--rw-r--r--   0        0        0      710 2023-11-06 13:42:05.321673 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2681-examples.txt
--rw-r--r--   0        0        0     1569 2023-11-06 10:46:38.787254 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2681.ttl
--rw-r--r--   0        0        0     4148 2023-11-06 13:42:05.340563 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2689.ttl
--rw-r--r--   0        0        0      861 2023-11-06 13:42:05.320838 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-271-examples.txt
--rw-r--r--   0        0        0     1199 2023-11-06 13:42:05.323109 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-271.ttl
--rw-r--r--   0        0        0     2400 2023-11-06 13:42:05.319599 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2712.ttl
--rw-r--r--   0        0        0      571 2023-11-06 13:42:01.900042 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2722-example.txt
--rw-r--r--   0        0        0      684 2023-11-06 10:46:38.788677 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2722.ttl
--rw-r--r--   0        0        0      912 2023-11-06 10:46:38.788974 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2740-examples.txt
--rw-r--r--   0        0        0     1422 2023-11-06 13:42:05.321206 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2740.ttl
--rw-r--r--   0        0        0      578 2023-11-06 13:42:05.318834 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-276.ttl
--rw-r--r--   0        0        0     3011 2023-11-06 13:42:05.325145 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2766.ttl
--rw-r--r--   0        0        0     2574 2023-11-06 13:42:05.343585 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2811-examples.txt
--rw-r--r--   0        0        0    23963 2023-11-06 13:42:05.323957 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2811.ttl
--rw-r--r--   0        0        0     1023 2023-11-06 13:42:05.324633 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2832-examples.txt
--rw-r--r--   0        0        0     2098 2023-11-06 13:42:05.341140 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2832.ttl
--rw-r--r--   0        0        0      743 2023-11-06 10:46:38.790957 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2858.ttl
--rw-r--r--   0        0        0      836 2023-11-06 13:42:05.356799 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2862-examples.txt
--rw-r--r--   0        0        0    15866 2023-11-06 10:46:38.791501 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2862.ttl
--rw-r--r--   0        0        0      669 2023-11-06 10:46:38.791785 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2877.ttl
--rw-r--r--   0        0        0      966 2023-11-06 10:46:38.792017 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2907.ttl
--rw-r--r--   0        0        0      784 2023-11-06 10:46:38.792247 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2912.ttl
--rw-r--r--   0        0        0      843 2023-11-06 13:42:05.355381 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2915.ttl
--rw-r--r--   0        0        0      712 2023-11-06 10:46:38.792674 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2927.ttl
--rw-r--r--   0        0        0     4841 2023-11-06 13:42:05.318987 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2989.ttl
--rw-r--r--   0        0        0      676 2023-11-06 13:42:05.321008 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-3001.ttl
--rw-r--r--   0        0        0     1005 2023-11-06 13:42:05.356012 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-3028-examples.txt
--rw-r--r--   0        0        0     1004 2023-11-06 13:42:05.317942 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-3028.ttl
--rw-r--r--   0        0        0      557 2023-11-06 13:42:05.326637 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-3052.ttl
--rw-r--r--   0        0        0     2441 2023-11-06 13:42:05.341692 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-3057.ttl
--rw-r--r--   0        0        0     1924 2023-11-06 13:42:05.323165 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-3058.ttl
--rw-r--r--   0        0        0     1176 2023-11-06 13:42:05.323905 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-3123.ttl
--rw-r--r--   0        0        0     1529 2023-11-06 13:42:05.321373 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-3134.ttl
--rw-r--r--   0        0        0      875 2023-11-06 13:42:05.338987 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-3135-examples.txt
--rw-r--r--   0        0        0      793 2023-11-06 13:42:05.323402 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-3135.ttl
--rw-r--r--   0        0        0     2025 2023-11-06 10:46:38.795388 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-3281.ttl
--rw-r--r--   0        0        0     2650 2023-11-06 10:46:38.795644 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-3392.ttl
--rw-r--r--   0        0        0     5408 2023-11-06 13:42:05.345282 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-373-examples.txt
--rw-r--r--   0        0        0     1660 2023-11-06 13:42:05.338056 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-373.ttl
--rw-r--r--   0        0        0     5951 2023-11-06 13:42:05.354064 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-383-examples.txt
--rw-r--r--   0        0        0     5360 2023-11-06 13:42:05.322490 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-383.ttl
--rw-r--r--   0        0        0     1615 2023-11-06 13:42:05.324115 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-447-examples.txt
--rw-r--r--   0        0        0     1624 2023-11-06 13:42:05.357020 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-447.ttl
--rwxr-xr-x   0        0        0    10722 2023-11-06 10:46:38.797783 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-894-examples.txt
--rw-r--r--   0        0        0     3868 2023-11-06 10:46:38.798003 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-894.ttl
--rw-r--r--   0        0        0      767 2023-11-06 13:42:05.355578 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-987.ttl
--rw-r--r--   0        0        0     1065 2023-11-06 10:46:38.798363 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-991.ttl
--rw-r--r--   0        0        0      250 2023-11-06 13:42:05.319937 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-template-examples.txt
--rwxr-xr-x   0        0        0      141 2023-11-06 10:46:38.798731 schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/pending-header.jsonld
--rw-r--r--   0        0        0   405369 2023-11-06 13:42:05.326933 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/httpequivs.ttl
--rw-r--r--   0        0        0  2625391 2023-11-06 13:42:05.321987 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schema-all.html
--rw-r--r--   0        0        0  1029634 2023-11-06 13:42:05.342384 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-examples.txt
--rw-r--r--   0        0        0   468380 2023-11-06 13:42:01.901455 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-http-properties.csv
--rw-r--r--   0        0        0  2211808 2023-11-06 13:42:02.025395 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-http-types.csv
--rw-r--r--   0        0        0  1406234 2023-11-06 13:42:05.327149 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-http.jsonld
--rw-r--r--   0        0        0  2518956 2023-11-06 13:42:05.345003 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-http.nq
--rw-r--r--   0        0        0  2107181 2023-11-06 13:42:05.315422 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-http.nt
--rw-r--r--   0        0        0  1394942 2023-11-06 13:42:02.008497 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-http.rdf
--rw-r--r--   0        0        0  1004249 2023-11-06 13:42:05.342383 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-http.ttl
--rw-r--r--   0        0        0   474975 2023-11-06 13:42:01.905995 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-https-properties.csv
--rw-r--r--   0        0        0  2273830 2023-11-06 13:42:02.073767 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-https-types.csv
--rw-r--r--   0        0        0  1407818 2023-11-06 13:42:05.322827 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-https.jsonld
--rw-r--r--   0        0        0  2566202 2023-11-06 13:42:05.319144 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-https.nq
--rw-r--r--   0        0        0  2137956 2023-11-06 13:42:05.327609 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-https.nt
--rw-r--r--   0        0        0  1404711 2023-11-06 13:42:02.099856 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-https.rdf
--rw-r--r--   0        0        0  1005833 2023-11-06 13:42:05.354231 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-https.ttl
--rw-r--r--   0        0        0   466682 2023-11-06 13:42:01.973265 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-http-properties.csv
--rw-r--r--   0        0        0  2208772 2023-11-06 13:42:02.024129 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-http-types.csv
--rw-r--r--   0        0        0  1399270 2023-11-06 13:42:05.315300 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-http.jsonld
--rw-r--r--   0        0        0  2506415 2023-11-06 13:42:05.321736 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-http.nq
--rw-r--r--   0        0        0  2096690 2023-11-06 13:42:05.353650 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-http.nt
--rw-r--r--   0        0        0  1388192 2023-11-06 13:42:01.895548 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-http.rdf
--rw-r--r--   0        0        0   999323 2023-11-06 13:42:05.345556 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-http.ttl
--rw-r--r--   0        0        0   473251 2023-11-06 13:42:01.862291 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-https-properties.csv
--rw-r--r--   0        0        0  2270736 2023-11-06 13:42:01.886658 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-https-types.csv
--rw-r--r--   0        0        0  1400842 2023-11-06 13:42:05.314349 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-https.jsonld
--rw-r--r--   0        0        0  2553413 2023-11-06 13:42:05.327262 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-https.nq
--rw-r--r--   0        0        0  2127299 2023-11-06 13:42:05.321606 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-https.nt
--rw-r--r--   0        0        0  1397919 2023-11-06 13:42:01.905826 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-https.rdf
--rw-r--r--   0        0        0  1000895 2023-11-06 13:42:05.344554 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-https.ttl
--rw-r--r--   0        0        0   349440 2023-11-06 13:42:05.314785 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-shapes.shacl
--rw-r--r--   0        0        0   959610 2023-11-06 10:46:40.492031 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-shapes.shexj
--rw-r--r--   0        0        0    58873 2023-11-06 13:42:05.327756 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-subclasses.shacl
--rw-r--r--   0        0        0  1924602 2023-11-06 13:42:01.963437 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg.owl
--rw-r--r--   0        0        0   173045 2023-11-06 10:46:40.500005 schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorgcontext.jsonld
--rw-r--r--   0        0        0     4392 2024-02-04 20:25:18.308812 schemaorg_lite-0.1.7/schemaorg_lite/main.py
--rw-r--r--   0        0        0     1560 1970-01-01 00:00:00.000000 schemaorg_lite-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1518 2023-11-06 10:34:52.313204 schemaorg_lite-0.1.8/LICENSE
+-rw-r--r--   0        0        0      549 2023-11-06 14:14:41.344426 schemaorg_lite-0.1.8/README.md
+-rw-r--r--   0        0        0     2490 2024-04-02 10:37:49.342322 schemaorg_lite-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-13 08:01:43.682908 schemaorg_lite-0.1.8/schemaorg_lite/__init__.py
+-rw-r--r--   0        0        0     2880 2024-02-04 20:25:18.335170 schemaorg_lite-0.1.8/schemaorg_lite/data/__init__.py
+-rw-r--r--   0        0        0     1172 2023-11-06 13:42:05.342534 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/attic/attic.ttl
+-rw-r--r--   0        0        0    14554 2023-11-06 13:42:05.338823 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/auto/auto.ttl
+-rw-r--r--   0        0        0     8237 2023-11-06 13:42:05.327404 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/bib/bsdo-1.0.ttl
+-rw-r--r--   0        0        0     1876 2023-11-06 13:42:05.343728 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/bib/bsdo-atlas-examples.txt
+-rw-r--r--   0        0        0     7041 2023-11-06 13:42:05.343211 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/bib/bsdo-audiobook-examples.txt
+-rw-r--r--   0        0        0     2487 2023-11-06 13:42:05.343890 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/bib/bsdo-chapter-examples.txt
+-rw-r--r--   0        0        0     6615 2023-11-06 13:42:05.328999 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/bib/bsdo-collection-examples.txt
+-rw-r--r--   0        0        0     1832 2023-11-06 13:42:05.328293 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/bib/bsdo-newspaper-examples.txt
+-rw-r--r--   0        0        0     1829 2023-11-06 13:42:05.355053 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/bib/bsdo-thesis-examples.txt
+-rw-r--r--   0        0        0     4831 2023-11-06 13:42:05.342706 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/bib/bsdo-translation-examples.txt
+-rw-r--r--   0        0        0     6635 2023-11-06 13:42:05.344253 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/bib/comics-examples.txt
+-rw-r--r--   0        0        0     6381 2023-11-06 13:42:05.321520 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/health-lifesci/MedicalScholarlyArticle-examples.txt
+-rw-r--r--   0        0        0    11809 2023-11-06 10:46:38.741032 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/health-lifesci/drug-example.txt
+-rw-r--r--   0        0        0   111217 2023-11-06 13:42:05.322642 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/health-lifesci/med-health-core.ttl
+-rw-r--r--   0        0        0    12612 2023-11-06 13:42:05.321202 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/health-lifesci/medicalCondition-examples.txt
+-rw-r--r--   0        0        0     4078 2023-11-06 13:42:05.342871 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/health-lifesci/medicalGuideline-examples.txt
+-rw-r--r--   0        0        0     3511 2023-11-06 13:42:05.356629 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/health-lifesci/medicalWebpage-examples.txt
+-rw-r--r--   0        0        0     6389 2023-11-06 13:42:05.344371 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/health-lifesci/physical-activity-and-exercise.ttl
+-rwxr-xr-x   0        0        0     3106 2023-11-06 10:46:38.748851 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/meta/meta.jsonld.someday.txt
+-rw-r--r--   0        0        0     2391 2023-11-06 13:42:05.320084 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/meta/meta.ttl
+-rw-r--r--   0        0        0     1042 2023-11-06 13:42:05.316356 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1045-examples.txt
+-rw-r--r--   0        0        0     1203 2023-11-06 13:42:05.353481 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1045.ttl
+-rw-r--r--   0        0        0      519 2023-11-06 13:42:05.354431 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1050-examples.txt
+-rw-r--r--   0        0        0      682 2023-11-06 13:42:05.322960 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1050.ttl
+-rw-r--r--   0        0        0     4269 2023-11-06 13:42:05.318097 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1062-examples.txt
+-rw-r--r--   0        0        0     8850 2023-11-06 13:42:05.326560 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1062.ttl
+-rw-r--r--   0        0        0      844 2023-11-06 13:42:05.339439 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1083.ttl
+-rw-r--r--   0        0        0    15347 2023-11-06 13:42:05.354911 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1156-examples.txt
+-rw-r--r--   0        0        0    15890 2023-11-06 13:42:05.326211 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1156.ttl
+-rw-r--r--   0        0        0     2234 2023-11-06 13:42:05.358069 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1244.ttl
+-rw-r--r--   0        0        0    14580 2023-11-06 13:42:02.072298 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1253-examples.txt
+-rw-r--r--   0        0        0    12976 2023-11-06 13:42:05.327958 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1253.ttl
+-rw-r--r--   0        0        0     5290 2023-11-06 13:42:05.321474 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1375.ttl
+-rw-r--r--   0        0        0     1328 2023-11-06 13:42:05.328523 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1389-examples.txt
+-rw-r--r--   0        0        0     1176 2023-11-06 13:42:05.339778 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1397.ttl
+-rw-r--r--   0        0        0     1476 2023-11-06 13:42:05.343369 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1401.ttl
+-rw-r--r--   0        0        0      692 2023-11-06 13:42:05.353269 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1423-examples.txt
+-rw-r--r--   0        0        0     1209 2023-11-06 13:42:05.326763 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1423.ttl
+-rw-r--r--   0        0        0     2939 2023-11-06 13:42:05.340119 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1425.ttl
+-rw-r--r--   0        0        0     1493 2023-11-06 13:42:05.313904 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1448.ttl
+-rw-r--r--   0        0        0     3997 2023-11-06 13:42:05.339151 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1457-examples.txt
+-rw-r--r--   0        0        0     5564 2023-11-06 13:42:05.316564 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1457.ttl
+-rw-r--r--   0        0        0      562 2023-11-06 13:42:05.358267 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1495.ttl
+-rw-r--r--   0        0        0     1908 2023-11-06 13:42:05.344691 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1525-examples.txt
+-rw-r--r--   0        0        0    12233 2023-11-06 13:42:05.321331 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1525.ttl
+-rw-r--r--   0        0        0      572 2023-11-06 13:42:05.352900 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1559.ttl
+-rw-r--r--   0        0        0      639 2023-11-06 13:42:05.341259 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1576.ttl
+-rw-r--r--   0        0        0     1422 2023-11-06 13:42:05.315869 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1589.ttl
+-rw-r--r--   0        0        0      595 2023-11-06 13:42:05.353938 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1591.ttl
+-rw-r--r--   0        0        0      694 2023-11-06 13:42:05.343006 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1624.ttl
+-rw-r--r--   0        0        0      364 2023-11-06 13:42:05.337920 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1670-examples.txt
+-rw-r--r--   0        0        0      808 2023-11-06 13:42:05.320239 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1672.ttl
+-rw-r--r--   0        0        0     2659 2023-11-06 10:46:38.758865 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1688.ttl
+-rw-r--r--   0        0        0      988 2023-11-06 13:42:05.340717 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1689-examples.txt
+-rw-r--r--   0        0        0     2996 2023-11-06 13:42:05.316153 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1698-examples.txt
+-rw-r--r--   0        0        0     1120 2023-11-06 13:42:05.321054 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1741-examples.txt
+-rw-r--r--   0        0        0     1914 2023-11-06 13:42:05.353785 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1755.ttl
+-rw-r--r--   0        0        0    15754 2023-11-06 13:42:05.324146 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1758-examples.txt
+-rw-r--r--   0        0        0     2262 2023-11-06 13:42:05.318249 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1758.ttl
+-rw-r--r--   0        0        0     3022 2023-11-06 13:42:05.341675 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1759-examples.txt
+-rw-r--r--   0        0        0      966 2023-11-06 13:42:05.341357 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1759.ttl
+-rw-r--r--   0        0        0    10049 2023-11-06 13:42:05.322368 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1779-examples.txt
+-rw-r--r--   0        0        0     3566 2023-11-06 13:42:05.317411 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1779.ttl
+-rw-r--r--   0        0        0     4041 2023-11-06 13:42:05.318687 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1797.ttl
+-rw-r--r--   0        0        0    47423 2023-11-06 13:42:05.317564 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1810-examples.txt
+-rw-r--r--   0        0        0     3927 2023-11-06 13:42:05.358562 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1810.ttl
+-rw-r--r--   0        0        0      738 2023-11-06 13:42:05.341619 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1816.ttl
+-rw-r--r--   0        0        0     2112 2023-11-06 13:42:05.337288 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1828.ttl
+-rw-r--r--   0        0        0     3219 2023-11-06 13:42:05.340996 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1842-examples.txt
+-rw-r--r--   0        0        0     3572 2023-11-06 13:42:05.343821 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1842.ttl
+-rw-r--r--   0        0        0     1732 2023-11-06 13:42:05.342691 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1886.ttl
+-rw-r--r--   0        0        0      763 2023-11-06 13:42:05.344063 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1909.ttl
+-rw-r--r--   0        0        0     1038 2023-11-06 13:42:05.315715 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1950-examples.txt
+-rw-r--r--   0        0        0     1006 2023-11-06 13:42:05.343131 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1950.ttl
+-rw-r--r--   0        0        0      453 2023-11-06 13:42:05.341105 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1951.ttl
+-rw-r--r--   0        0        0      568 2023-11-06 13:42:05.338485 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1976.ttl
+-rw-r--r--   0        0        0      406 2023-11-06 13:42:05.315010 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2021-examples.txt
+-rw-r--r--   0        0        0      942 2023-11-06 13:42:05.342141 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2021.ttl
+-rw-r--r--   0        0        0      459 2023-11-06 13:42:05.324981 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2083-examples.txt
+-rw-r--r--   0        0        0      784 2023-11-06 13:42:05.324262 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2083.ttl
+-rw-r--r--   0        0        0      390 2023-11-06 13:42:05.321874 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2085-examples.txt
+-rw-r--r--   0        0        0      737 2023-11-06 13:42:05.320393 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2085.ttl
+-rw-r--r--   0        0        0      860 2023-11-06 13:42:05.338655 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2108-examples.txt
+-rw-r--r--   0        0        0     1722 2023-11-06 13:42:05.317044 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2108.ttl
+-rw-r--r--   0        0        0      287 2023-11-06 13:42:05.341469 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2109-examples.txt
+-rw-r--r--   0        0        0     1094 2023-11-06 13:42:05.342853 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2109.ttl
+-rw-r--r--   0        0        0      666 2023-11-06 13:42:05.316010 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2110.ttl
+-rw-r--r--   0        0        0      994 2023-11-06 13:42:05.344097 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2111.ttl
+-rw-r--r--   0        0        0      638 2023-11-06 13:42:05.345408 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2126.ttl
+-rw-r--r--   0        0        0     1113 2023-11-06 13:42:05.322253 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2140.ttl
+-rw-r--r--   0        0        0     1608 2023-11-06 13:42:05.345472 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2173-examples.txt
+-rw-r--r--   0        0        0      953 2023-11-06 13:42:05.317201 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2173.ttl
+-rw-r--r--   0        0        0     1626 2023-11-06 13:42:05.321989 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2192-examples.txt
+-rw-r--r--   0        0        0      587 2023-11-06 13:42:05.356318 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2192.ttl
+-rw-r--r--   0        0        0      622 2023-11-06 13:42:05.343556 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2242.ttl
+-rw-r--r--   0        0        0     1099 2023-11-06 13:42:05.322492 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2244.ttl
+-rw-r--r--   0        0        0     3792 2023-11-06 13:42:05.345147 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2288.ttl
+-rw-r--r--   0        0        0     3406 2023-11-06 13:42:05.314604 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2289-examples.txt
+-rw-r--r--   0        0        0     5153 2023-11-06 13:42:05.354571 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2289.ttl
+-rw-r--r--   0        0        0       28 2023-11-06 13:42:05.340865 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2291.ttl
+-rw-r--r--   0        0        0      708 2023-11-06 13:42:05.328686 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2294-examples.txt
+-rw-r--r--   0        0        0      757 2023-11-06 13:42:05.344870 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2296-examples.txt
+-rw-r--r--   0        0        0      644 2023-11-06 13:42:05.345683 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2296.ttl
+-rw-r--r--   0        0        0      775 2023-11-06 13:42:05.341948 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2300.ttl
+-rw-r--r--   0        0        0     1402 2023-11-06 13:42:05.343389 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2311.ttl
+-rw-r--r--   0        0        0      663 2023-11-06 13:42:05.328132 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2329.ttl
+-rw-r--r--   0        0        0      454 2023-11-06 13:42:05.355839 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2341.ttl
+-rw-r--r--   0        0        0     1824 2023-11-06 13:42:05.344841 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2348.ttl
+-rw-r--r--   0        0        0      993 2023-11-06 13:42:05.341935 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2358.ttl
+-rw-r--r--   0        0        0     2527 2023-11-06 13:42:05.315571 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2366-examples.txt
+-rw-r--r--   0        0        0     8264 2023-11-06 13:42:05.339605 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2373.ttl
+-rw-r--r--   0        0        0    11319 2023-11-06 10:46:38.774343 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2374.ttl
+-rw-r--r--   0        0        0    15957 2023-11-06 13:42:05.357537 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2381.ttl
+-rw-r--r--   0        0        0      423 2023-11-06 13:42:05.339949 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2382.ttl
+-rw-r--r--   0        0        0     1021 2023-11-06 13:42:05.343256 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2384-examples.txt
+-rw-r--r--   0        0        0     2153 2023-11-06 13:42:05.328847 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2384.ttl
+-rw-r--r--   0        0        0      677 2023-11-06 13:42:05.319746 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2394.ttl
+-rw-r--r--   0        0        0     1683 2023-11-06 13:42:05.357396 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2396-examples.txt
+-rw-r--r--   0        0        0      962 2023-11-06 13:42:05.358416 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2396.ttl
+-rw-r--r--   0        0        0    12842 2023-11-06 13:42:05.357289 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2405-examples.txt
+-rw-r--r--   0        0        0     1668 2023-11-06 13:42:05.324511 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2405.ttl
+-rw-r--r--   0        0        0      683 2023-11-06 13:42:05.337540 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2418.ttl
+-rw-r--r--   0        0        0      658 2023-11-06 13:42:05.344538 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2419-examples.txt
+-rw-r--r--   0        0        0     4491 2023-11-06 13:42:05.342998 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2419.ttl
+-rw-r--r--   0        0        0      410 2023-11-06 13:42:05.322220 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2420.ttl
+-rw-r--r--   0        0        0     1307 2023-11-06 13:42:05.338226 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2421-examples.txt
+-rw-r--r--   0        0        0      456 2023-11-06 13:42:05.340402 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2421.ttl
+-rw-r--r--   0        0        0     1093 2023-11-06 13:42:05.326085 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2427.ttl
+-rw-r--r--   0        0        0     1587 2023-11-06 13:42:05.344727 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2450-examples.txt
+-rw-r--r--   0        0        0    18210 2023-11-06 10:46:38.778535 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2450.ttl
+-rw-r--r--   0        0        0     1795 2023-11-06 13:42:05.357156 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2454.ttl
+-rw-r--r--   0        0        0     1136 2023-11-06 13:42:05.327425 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2460.ttl
+-rw-r--r--   0        0        0     2179 2023-11-06 13:42:05.321828 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2469.ttl
+-rw-r--r--   0        0        0     3064 2023-11-06 13:42:05.354773 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2482-examples.txt
+-rw-r--r--   0        0        0      817 2023-11-06 13:42:05.315139 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2483.ttl
+-rw-r--r--   0        0        0      510 2023-11-06 13:42:05.316769 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2486.ttl
+-rw-r--r--   0        0        0     3601 2023-11-06 13:42:05.314163 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2490-examples.txt
+-rw-r--r--   0        0        0     9452 2023-11-06 13:42:05.324470 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2490.ttl
+-rw-r--r--   0        0        0      510 2023-11-06 13:42:05.317783 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2493.ttl
+-rw-r--r--   0        0        0      427 2023-11-06 13:42:05.323567 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2496.ttl
+-rw-r--r--   0        0        0      576 2023-11-06 13:42:05.344414 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2500.ttl
+-rw-r--r--   0        0        0    12914 2023-11-06 13:42:05.323260 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2506.ttl
+-rw-r--r--   0        0        0     1342 2023-11-06 10:46:38.781728 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2514-examples.txt
+-rw-r--r--   0        0        0      893 2023-11-06 13:42:05.345260 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2514.ttl
+-rw-r--r--   0        0        0     7820 2023-11-06 13:42:05.319446 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2521.ttl
+-rw-r--r--   0        0        0      536 2023-11-06 13:42:05.322652 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2526.ttl
+-rw-r--r--   0        0        0     1360 2023-11-06 13:42:05.337741 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2534-examples.txt
+-rw-r--r--   0        0        0     3813 2023-11-06 13:42:05.318496 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2534.ttl
+-rw-r--r--   0        0        0      713 2023-11-06 10:46:38.783666 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2543-examples.txt
+-rw-r--r--   0        0        0    14774 2023-11-06 13:42:05.320548 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2543.ttl
+-rw-r--r--   0        0        0     1297 2023-11-06 10:46:38.784230 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2564-examples.txt
+-rw-r--r--   0        0        0    13020 2023-11-06 10:46:38.784549 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2564.ttl
+-rw-r--r--   0        0        0      672 2023-11-06 10:46:38.784766 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2599-examples.txt
+-rw-r--r--   0        0        0      753 2023-11-06 13:42:05.341399 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2599.ttl
+-rw-r--r--   0        0        0      680 2023-11-06 13:42:05.345117 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2605.ttl
+-rw-r--r--   0        0        0      524 2023-11-06 13:42:05.327108 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2611.ttl
+-rw-r--r--   0        0        0      730 2023-11-06 13:42:05.323743 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2636.ttl
+-rw-r--r--   0        0        0      605 2023-11-06 13:42:05.357845 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2646.ttl
+-rw-r--r--   0        0        0     1035 2023-11-06 13:42:05.319297 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2659.ttl
+-rw-r--r--   0        0        0      694 2023-11-06 13:42:05.323413 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2665.ttl
+-rw-r--r--   0        0        0     7938 2023-11-06 13:42:05.327278 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2670.ttl
+-rw-r--r--   0        0        0      710 2023-11-06 13:42:05.321673 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2681-examples.txt
+-rw-r--r--   0        0        0     1569 2023-11-06 10:46:38.787254 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2681.ttl
+-rw-r--r--   0        0        0     4148 2023-11-06 13:42:05.340563 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2689.ttl
+-rw-r--r--   0        0        0      861 2023-11-06 13:42:05.320838 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-271-examples.txt
+-rw-r--r--   0        0        0     1199 2023-11-06 13:42:05.323109 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-271.ttl
+-rw-r--r--   0        0        0     2400 2023-11-06 13:42:05.319599 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2712.ttl
+-rw-r--r--   0        0        0      571 2023-11-06 13:42:01.900042 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2722-example.txt
+-rw-r--r--   0        0        0      684 2023-11-06 10:46:38.788677 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2722.ttl
+-rw-r--r--   0        0        0      912 2023-11-06 10:46:38.788974 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2740-examples.txt
+-rw-r--r--   0        0        0     1422 2023-11-06 13:42:05.321206 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2740.ttl
+-rw-r--r--   0        0        0      578 2023-11-06 13:42:05.318834 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-276.ttl
+-rw-r--r--   0        0        0     3011 2023-11-06 13:42:05.325145 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2766.ttl
+-rw-r--r--   0        0        0     2574 2023-11-06 13:42:05.343585 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2811-examples.txt
+-rw-r--r--   0        0        0    23963 2023-11-06 13:42:05.323957 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2811.ttl
+-rw-r--r--   0        0        0     1023 2023-11-06 13:42:05.324633 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2832-examples.txt
+-rw-r--r--   0        0        0     2098 2023-11-06 13:42:05.341140 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2832.ttl
+-rw-r--r--   0        0        0      743 2023-11-06 10:46:38.790957 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2858.ttl
+-rw-r--r--   0        0        0      836 2023-11-06 13:42:05.356799 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2862-examples.txt
+-rw-r--r--   0        0        0    15866 2023-11-06 10:46:38.791501 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2862.ttl
+-rw-r--r--   0        0        0      669 2023-11-06 10:46:38.791785 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2877.ttl
+-rw-r--r--   0        0        0      966 2023-11-06 10:46:38.792017 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2907.ttl
+-rw-r--r--   0        0        0      784 2023-11-06 10:46:38.792247 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2912.ttl
+-rw-r--r--   0        0        0      843 2023-11-06 13:42:05.355381 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2915.ttl
+-rw-r--r--   0        0        0      712 2023-11-06 10:46:38.792674 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2927.ttl
+-rw-r--r--   0        0        0     4841 2023-11-06 13:42:05.318987 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2989.ttl
+-rw-r--r--   0        0        0      676 2023-11-06 13:42:05.321008 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-3001.ttl
+-rw-r--r--   0        0        0     1005 2023-11-06 13:42:05.356012 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-3028-examples.txt
+-rw-r--r--   0        0        0     1004 2023-11-06 13:42:05.317942 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-3028.ttl
+-rw-r--r--   0        0        0      557 2023-11-06 13:42:05.326637 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-3052.ttl
+-rw-r--r--   0        0        0     2441 2023-11-06 13:42:05.341692 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-3057.ttl
+-rw-r--r--   0        0        0     1924 2023-11-06 13:42:05.323165 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-3058.ttl
+-rw-r--r--   0        0        0     1176 2023-11-06 13:42:05.323905 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-3123.ttl
+-rw-r--r--   0        0        0     1529 2023-11-06 13:42:05.321373 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-3134.ttl
+-rw-r--r--   0        0        0      875 2023-11-06 13:42:05.338987 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-3135-examples.txt
+-rw-r--r--   0        0        0      793 2023-11-06 13:42:05.323402 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-3135.ttl
+-rw-r--r--   0        0        0     2025 2023-11-06 10:46:38.795388 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-3281.ttl
+-rw-r--r--   0        0        0     2650 2023-11-06 10:46:38.795644 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-3392.ttl
+-rw-r--r--   0        0        0     5408 2023-11-06 13:42:05.345282 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-373-examples.txt
+-rw-r--r--   0        0        0     1660 2023-11-06 13:42:05.338056 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-373.ttl
+-rw-r--r--   0        0        0     5951 2023-11-06 13:42:05.354064 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-383-examples.txt
+-rw-r--r--   0        0        0     5360 2023-11-06 13:42:05.322490 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-383.ttl
+-rw-r--r--   0        0        0     1615 2023-11-06 13:42:05.324115 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-447-examples.txt
+-rw-r--r--   0        0        0     1624 2023-11-06 13:42:05.357020 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-447.ttl
+-rwxr-xr-x   0        0        0    10722 2023-11-06 10:46:38.797783 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-894-examples.txt
+-rw-r--r--   0        0        0     3868 2023-11-06 10:46:38.798003 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-894.ttl
+-rw-r--r--   0        0        0      767 2023-11-06 13:42:05.355578 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-987.ttl
+-rw-r--r--   0        0        0     1065 2023-11-06 10:46:38.798363 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-991.ttl
+-rw-r--r--   0        0        0      250 2023-11-06 13:42:05.319937 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-template-examples.txt
+-rwxr-xr-x   0        0        0      141 2023-11-06 10:46:38.798731 schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/pending-header.jsonld
+-rw-r--r--   0        0        0   405369 2023-11-06 13:42:05.326933 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/httpequivs.ttl
+-rw-r--r--   0        0        0  2625391 2023-11-06 13:42:05.321987 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schema-all.html
+-rw-r--r--   0        0        0  1029634 2023-11-06 13:42:05.342384 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-examples.txt
+-rw-r--r--   0        0        0   468380 2023-11-06 13:42:01.901455 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-http-properties.csv
+-rw-r--r--   0        0        0  2211808 2023-11-06 13:42:02.025395 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-http-types.csv
+-rw-r--r--   0        0        0  1406234 2023-11-06 13:42:05.327149 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-http.jsonld
+-rw-r--r--   0        0        0  2518956 2023-11-06 13:42:05.345003 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-http.nq
+-rw-r--r--   0        0        0  2107181 2023-11-06 13:42:05.315422 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-http.nt
+-rw-r--r--   0        0        0  1394942 2023-11-06 13:42:02.008497 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-http.rdf
+-rw-r--r--   0        0        0  1004249 2023-11-06 13:42:05.342383 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-http.ttl
+-rw-r--r--   0        0        0   474975 2023-11-06 13:42:01.905995 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-https-properties.csv
+-rw-r--r--   0        0        0  2273830 2023-11-06 13:42:02.073767 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-https-types.csv
+-rw-r--r--   0        0        0  1407818 2023-11-06 13:42:05.322827 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-https.jsonld
+-rw-r--r--   0        0        0  2566202 2023-11-06 13:42:05.319144 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-https.nq
+-rw-r--r--   0        0        0  2137956 2023-11-06 13:42:05.327609 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-https.nt
+-rw-r--r--   0        0        0  1404711 2023-11-06 13:42:02.099856 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-https.rdf
+-rw-r--r--   0        0        0  1005833 2023-11-06 13:42:05.354231 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-https.ttl
+-rw-r--r--   0        0        0   466682 2023-11-06 13:42:01.973265 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-http-properties.csv
+-rw-r--r--   0        0        0  2208772 2023-11-06 13:42:02.024129 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-http-types.csv
+-rw-r--r--   0        0        0  1399270 2023-11-06 13:42:05.315300 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-http.jsonld
+-rw-r--r--   0        0        0  2506415 2023-11-06 13:42:05.321736 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-http.nq
+-rw-r--r--   0        0        0  2096690 2023-11-06 13:42:05.353650 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-http.nt
+-rw-r--r--   0        0        0  1388192 2023-11-06 13:42:01.895548 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-http.rdf
+-rw-r--r--   0        0        0   999323 2023-11-06 13:42:05.345556 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-http.ttl
+-rw-r--r--   0        0        0   473251 2023-11-06 13:42:01.862291 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-https-properties.csv
+-rw-r--r--   0        0        0  2270736 2023-11-06 13:42:01.886658 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-https-types.csv
+-rw-r--r--   0        0        0  1400842 2023-11-06 13:42:05.314349 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-https.jsonld
+-rw-r--r--   0        0        0  2553413 2023-11-06 13:42:05.327262 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-https.nq
+-rw-r--r--   0        0        0  2127299 2023-11-06 13:42:05.321606 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-https.nt
+-rw-r--r--   0        0        0  1397919 2023-11-06 13:42:01.905826 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-https.rdf
+-rw-r--r--   0        0        0  1000895 2023-11-06 13:42:05.344554 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-https.ttl
+-rw-r--r--   0        0        0   349440 2023-11-06 13:42:05.314785 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-shapes.shacl
+-rw-r--r--   0        0        0   959610 2023-11-06 10:46:40.492031 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-shapes.shexj
+-rw-r--r--   0        0        0    58873 2023-11-06 13:42:05.327756 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-subclasses.shacl
+-rw-r--r--   0        0        0  1924602 2023-11-06 13:42:01.963437 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg.owl
+-rw-r--r--   0        0        0   173045 2023-11-06 10:46:40.500005 schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorgcontext.jsonld
+-rw-r--r--   0        0        0     4392 2024-02-04 20:25:18.308812 schemaorg_lite-0.1.8/schemaorg_lite/main.py
+-rw-r--r--   0        0        0     1560 1970-01-01 00:00:00.000000 schemaorg_lite-0.1.8/PKG-INFO
```

### Comparing `schemaorg_lite-0.1.7/LICENSE` & `schemaorg_lite-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/README.md` & `schemaorg_lite-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/pyproject.toml` & `schemaorg_lite-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 [tool.ruff]
 line-length = 88
 target-version = "py312"
 fix = true
 show-fixes = true
 output-format = "full"
 
+[tool.ruff.lint]
+ignore = [
+    "F821",
+]
+
 [tool.ruff.lint.isort]
 force-single-line = true
 
 [tool.ruff.lint.mccabe]
 max-complexity = 10
 
 [tool.ruff.lint.pydocstyle]
@@ -27,33 +32,33 @@
 
 [tool.creosote]
 paths = [
     "schemaorg_lite",
 ]
 deps-file = "pyproject.toml"
 exclude-deps = [
-    "pdm",
     "pytest",
+    "pdm",
+    "autotyping",
     "pdm-bump",
     "pre-commit",
-    "autotyping",
 ]
 
 [tool.codespell]
 skip = "*/data/*"
 quiet-level = 3
 ignore-words-list = "crate,uptodate"
 
 [tool.bandit]
 target = [
     "schemaorg_lite",
 ]
 skips = [
-    "B404",
     "B603",
+    "B404",
 ]
 
 [tool.black]
 target-version = [
     "py312",
 ]
 
@@ -77,15 +82,15 @@
 reportUnknownArgumentType = false
 reportPrivateUsage = "warning"
 pythonVersion = "3.12"
 pythonPlatform = "Darwin"
 
 [project]
 name = "schemaorg-lite"
-version = "0.1.7"
+version = "0.1.8"
 description = "Python functions for applied use of schema.org"
 dependencies = []
 requires-python = ">=3.12"
 readme = "README.md"
 keywords = [
     "openschemas",
     "schema.org",
```

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/__init__.py` & `schemaorg_lite-0.1.8/schemaorg_lite/data/__init__.py`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/attic/attic.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/attic/attic.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/auto/auto.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/auto/auto.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/bib/bsdo-1.0.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/bib/bsdo-1.0.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/bib/bsdo-atlas-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/bib/bsdo-atlas-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/bib/bsdo-audiobook-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/bib/bsdo-audiobook-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/bib/bsdo-chapter-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/bib/bsdo-chapter-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/bib/bsdo-collection-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/bib/bsdo-collection-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/bib/bsdo-newspaper-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/bib/bsdo-newspaper-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/bib/bsdo-thesis-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/bib/bsdo-thesis-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/bib/bsdo-translation-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/bib/bsdo-translation-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/bib/comics-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/bib/comics-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/health-lifesci/MedicalScholarlyArticle-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/health-lifesci/MedicalScholarlyArticle-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/health-lifesci/drug-example.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/health-lifesci/drug-example.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/health-lifesci/med-health-core.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/health-lifesci/med-health-core.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/health-lifesci/medicalCondition-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/health-lifesci/medicalCondition-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/health-lifesci/medicalGuideline-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/health-lifesci/medicalGuideline-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/health-lifesci/medicalWebpage-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/health-lifesci/medicalWebpage-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/health-lifesci/physical-activity-and-exercise.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/health-lifesci/physical-activity-and-exercise.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/meta/meta.jsonld.someday.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/meta/meta.jsonld.someday.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/meta/meta.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/meta/meta.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1045-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1045-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1045.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1045.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1050-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1050-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1050.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1050.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1062-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1062-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1062.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1062.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1083.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1083.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1156-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1156-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1156.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1156.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1244.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1244.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1253-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1253-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1253.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1253.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1375.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1375.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1389-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1389-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1397.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1397.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1401.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1401.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1423-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1423-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1423.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1423.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1425.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1425.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1448.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1448.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1457-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1457-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1457.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1457.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1495.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1495.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1525-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1525-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1525.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1525.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1559.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1559.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1576.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1576.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1589.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1589.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1591.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1591.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1624.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1624.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1672.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1672.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1688.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1688.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1689-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1689-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1698-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1698-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1741-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1741-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1755.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1755.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1758-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1758-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1758.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1758.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1759-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1759-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1759.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1759.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1779-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1779-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1779.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1779.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1797.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1797.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1810-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1810-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1810.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1810.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1816.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1816.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1828.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1828.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1842-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1842-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1842.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1842.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1886.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1886.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1909.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1909.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1950-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1950-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1950.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1950.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-1976.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-1976.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2021.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2021.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2083.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2083.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2085.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2085.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2108-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2108-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2108.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2108.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2109.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2109.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2110.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2110.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2111.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2111.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2126.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2126.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2140.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2140.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2173-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2173-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2173.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2173.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2192-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2192-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2192.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2192.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2242.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2242.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2244.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2244.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2288.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2288.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2289-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2289-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2289.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2289.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2294-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2294-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2296-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2296-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2296.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2296.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2300.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2300.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2311.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2311.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2329.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2329.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2348.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2348.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2358.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2358.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2366-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2366-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2373.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2373.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2374.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2374.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2381.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2381.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2384-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2384-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2384.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2384.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2394.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2394.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2396-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2396-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2396.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2396.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2405-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2405-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2405.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2405.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2418.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2418.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2419-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2419-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2419.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2419.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2421-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2421-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2427.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2427.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2450-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2450-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2450.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2450.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2454.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2454.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2460.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2460.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2469.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2469.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2482-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2482-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2483.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2483.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2490-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2490-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2490.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2490.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2500.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2500.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2506.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2506.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2514-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2514-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2514.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2514.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2521.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2521.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2526.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2526.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2534-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2534-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2534.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2534.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2543-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2543-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2543.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2543.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2564-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2564-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2564.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2564.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2599-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2599-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2599.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2599.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2605.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2605.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2611.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2611.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2636.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2636.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2646.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2646.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2659.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2659.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2665.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2665.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2670.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2670.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2681-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2681-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2681.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2681.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2689.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2689.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-271-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-271-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-271.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-271.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2712.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2712.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2722-example.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2722-example.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2722.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2722.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2740-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2740-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2740.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2740.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-276.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-276.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2766.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2766.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2811-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2811-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2811.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2811.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2832-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2832-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2832.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2832.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2858.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2858.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2862-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2862-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2862.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2862.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2877.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2877.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2907.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2907.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2912.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2912.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2915.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2915.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2927.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2927.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-2989.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-2989.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-3001.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-3001.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-3028-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-3028-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-3028.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-3028.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-3052.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-3052.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-3057.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-3057.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-3058.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-3058.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-3123.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-3123.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-3134.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-3134.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-3135-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-3135-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-3135.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-3135.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-3281.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-3281.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-3392.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-3392.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-373-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-373-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-373.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-373.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-383-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-383-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-383.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-383.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-447-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-447-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-447.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-447.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-894-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-894-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-894.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-894.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-987.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-987.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/ext/pending/issue-991.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/ext/pending/issue-991.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/httpequivs.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/httpequivs.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schema-all.html` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schema-all.html`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-examples.txt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-examples.txt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-http-properties.csv` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-http-properties.csv`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-http-types.csv` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-http-types.csv`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-http.jsonld` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-http.jsonld`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-http.nq` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-http.nq`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-http.nt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-http.nt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-http.rdf` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-http.rdf`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-http.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-http.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-https-properties.csv` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-https-properties.csv`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-https-types.csv` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-https-types.csv`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-https.jsonld` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-https.jsonld`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-https.nq` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-https.nq`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-https.nt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-https.nt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-https.rdf` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-https.rdf`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-all-https.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-all-https.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-http-properties.csv` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-http-properties.csv`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-http-types.csv` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-http-types.csv`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-http.jsonld` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-http.jsonld`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-http.nq` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-http.nq`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-http.nt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-http.nt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-http.rdf` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-http.rdf`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-http.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-http.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-https-properties.csv` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-https-properties.csv`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-https-types.csv` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-https-types.csv`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-https.jsonld` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-https.jsonld`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-https.nq` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-https.nq`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-https.nt` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-https.nt`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-https.rdf` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-https.rdf`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-current-https.ttl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-current-https.ttl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-shapes.shacl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-shapes.shacl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-shapes.shexj` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-shapes.shexj`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg-subclasses.shacl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg-subclasses.shacl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorg.owl` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorg.owl`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/data/releases/23.0/schemaorgcontext.jsonld` & `schemaorg_lite-0.1.8/schemaorg_lite/data/releases/23.0/schemaorgcontext.jsonld`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/schemaorg_lite/main.py` & `schemaorg_lite-0.1.8/schemaorg_lite/main.py`

 * *Files identical despite different names*

### Comparing `schemaorg_lite-0.1.7/PKG-INFO` & `schemaorg_lite-0.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schemaorg-lite
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python functions for applied use of schema.org
 Keywords: openschemas schema.org
 Author-Email: Vanessa Sochat <vsoch@users.noreply.github.com>, lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>, Vanessa Sochat <vsoch@users.noreply.github.com>
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
```

