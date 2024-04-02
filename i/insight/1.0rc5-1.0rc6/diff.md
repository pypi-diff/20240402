# Comparing `tmp/insight-1.0rc5-py3-none-any.whl.zip` & `tmp/insight-1.0rc6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,31 +1,33 @@
-Zip file size: 141880 bytes, number of entries: 29
--rw-r--r--  2.0 unx      105 b- defN 24-Feb-16 09:07 insight/__init__.py
--rw-r--r--  2.0 unx     4698 b- defN 24-Feb-16 09:07 insight/check.py
--rw-r--r--  2.0 unx    18466 b- defN 24-Feb-16 09:07 insight/plot.py
--rw-r--r--  2.0 unx       55 b- defN 24-Feb-16 09:07 insight/py.typed
--rw-r--r--  2.0 unx      158 b- defN 24-Feb-16 09:07 insight/version.py
--rw-r--r--  2.0 unx       39 b- defN 24-Feb-16 09:07 insight/alembic/README
--rw-r--r--  2.0 unx      263 b- defN 24-Feb-16 09:07 insight/alembic/alembic.ini
--rw-r--r--  2.0 unx     2677 b- defN 24-Feb-16 09:07 insight/alembic/env.py
--rw-r--r--  2.0 unx      371 b- defN 24-Feb-16 09:07 insight/alembic/main.py
--rw-r--r--  2.0 unx      510 b- defN 24-Feb-16 09:07 insight/alembic/script.py.mako
--rw-r--r--  2.0 unx     2390 b- defN 24-Feb-16 09:07 insight/alembic/versions/9aca5ae68ff5_add_initial_tables.py
--rw-r--r--  2.0 unx      890 b- defN 24-Feb-16 09:07 insight/alembic/versions/a2198ae60b44_added_version_name_unique_constaint.py
--rw-r--r--  2.0 unx      879 b- defN 24-Feb-16 09:07 insight/alembic/versions/d2198fd60b0e_added_result_run_id.py
--rw-r--r--  2.0 unx      114 b- defN 24-Feb-16 09:07 insight/database/__init__.py
--rw-r--r--  2.0 unx     1682 b- defN 24-Feb-16 09:07 insight/database/schema.py
--rw-r--r--  2.0 unx     6422 b- defN 24-Feb-16 09:07 insight/database/utils.py
--rw-r--r--  2.0 unx   248132 b- defN 24-Feb-16 09:07 insight/fonts/SourceSansPro-Regular.ttf
--rw-r--r--  2.0 unx      995 b- defN 24-Feb-16 09:07 insight/metrics/__init__.py
--rw-r--r--  2.0 unx    12831 b- defN 24-Feb-16 09:07 insight/metrics/base.py
--rw-r--r--  2.0 unx     4502 b- defN 24-Feb-16 09:07 insight/metrics/confidence_interval.py
--rw-r--r--  2.0 unx    19144 b- defN 24-Feb-16 09:07 insight/metrics/metrics.py
--rw-r--r--  2.0 unx     5922 b- defN 24-Feb-16 09:07 insight/metrics/metrics_usage.py
--rw-r--r--  2.0 unx     4678 b- defN 24-Feb-16 09:07 insight/metrics/utils.py
--rw-r--r--  2.0 unx     1524 b- defN 24-Feb-16 09:07 insight-1.0rc5.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     7560 b- defN 24-Feb-16 09:07 insight-1.0rc5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-16 09:07 insight-1.0rc5.dist-info/WHEEL
--rw-r--r--  2.0 unx       65 b- defN 24-Feb-16 09:07 insight-1.0rc5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        8 b- defN 24-Feb-16 09:07 insight-1.0rc5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2483 b- defN 24-Feb-16 09:07 insight-1.0rc5.dist-info/RECORD
-29 files, 347655 bytes uncompressed, 137856 bytes compressed:  60.3%
+Zip file size: 143148 bytes, number of entries: 31
+-rw-r--r--  2.0 unx      105 b- defN 24-Mar-06 10:45 insight/__init__.py
+-rw-r--r--  2.0 unx     4698 b- defN 24-Mar-06 10:45 insight/check.py
+-rw-r--r--  2.0 unx    18466 b- defN 24-Mar-06 10:45 insight/plot.py
+-rw-r--r--  2.0 unx       55 b- defN 24-Mar-06 10:45 insight/py.typed
+-rw-r--r--  2.0 unx      158 b- defN 24-Mar-06 10:45 insight/version.py
+-rw-r--r--  2.0 unx       39 b- defN 24-Mar-06 10:45 insight/alembic/README
+-rw-r--r--  2.0 unx      263 b- defN 24-Mar-06 10:45 insight/alembic/alembic.ini
+-rw-r--r--  2.0 unx     2677 b- defN 24-Mar-06 10:45 insight/alembic/env.py
+-rw-r--r--  2.0 unx      371 b- defN 24-Mar-06 10:45 insight/alembic/main.py
+-rw-r--r--  2.0 unx      510 b- defN 24-Mar-06 10:45 insight/alembic/script.py.mako
+-rw-r--r--  2.0 unx      675 b- defN 24-Mar-06 10:45 insight/alembic/versions/495f69cbfe6d_add_result_sub_run.py
+-rw-r--r--  2.0 unx     2390 b- defN 24-Mar-06 10:45 insight/alembic/versions/9aca5ae68ff5_add_initial_tables.py
+-rw-r--r--  2.0 unx      890 b- defN 24-Mar-06 10:45 insight/alembic/versions/a2198ae60b44_added_version_name_unique_constaint.py
+-rw-r--r--  2.0 unx      879 b- defN 24-Mar-06 10:45 insight/alembic/versions/d2198fd60b0e_added_result_run_id.py
+-rw-r--r--  2.0 unx      772 b- defN 24-Mar-06 10:45 insight/alembic/versions/eaf7bb3598af_version_unique_constraint.py
+-rw-r--r--  2.0 unx      114 b- defN 24-Mar-06 10:45 insight/database/__init__.py
+-rw-r--r--  2.0 unx     1748 b- defN 24-Mar-06 10:45 insight/database/schema.py
+-rw-r--r--  2.0 unx     6422 b- defN 24-Mar-06 10:45 insight/database/utils.py
+-rw-r--r--  2.0 unx   248132 b- defN 24-Mar-06 10:45 insight/fonts/SourceSansPro-Regular.ttf
+-rw-r--r--  2.0 unx      995 b- defN 24-Mar-06 10:45 insight/metrics/__init__.py
+-rw-r--r--  2.0 unx    13022 b- defN 24-Mar-06 10:45 insight/metrics/base.py
+-rw-r--r--  2.0 unx     4502 b- defN 24-Mar-06 10:45 insight/metrics/confidence_interval.py
+-rw-r--r--  2.0 unx    19144 b- defN 24-Mar-06 10:45 insight/metrics/metrics.py
+-rw-r--r--  2.0 unx     5922 b- defN 24-Mar-06 10:45 insight/metrics/metrics_usage.py
+-rw-r--r--  2.0 unx     4678 b- defN 24-Mar-06 10:45 insight/metrics/utils.py
+-rw-r--r--  2.0 unx     1524 b- defN 24-Mar-06 10:45 insight-1.0rc6.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     7560 b- defN 24-Mar-06 10:45 insight-1.0rc6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-06 10:45 insight-1.0rc6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       65 b- defN 24-Mar-06 10:45 insight-1.0rc6.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        8 b- defN 24-Mar-06 10:45 insight-1.0rc6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2720 b- defN 24-Mar-06 10:45 insight-1.0rc6.dist-info/RECORD
+31 files, 349596 bytes uncompressed, 138722 bytes compressed:  60.3%
```

## zipnote {}

```diff
@@ -24,23 +24,29 @@
 
 Filename: insight/alembic/main.py
 Comment: 
 
 Filename: insight/alembic/script.py.mako
 Comment: 
 
+Filename: insight/alembic/versions/495f69cbfe6d_add_result_sub_run.py
+Comment: 
+
 Filename: insight/alembic/versions/9aca5ae68ff5_add_initial_tables.py
 Comment: 
 
 Filename: insight/alembic/versions/a2198ae60b44_added_version_name_unique_constaint.py
 Comment: 
 
 Filename: insight/alembic/versions/d2198fd60b0e_added_result_run_id.py
 Comment: 
 
+Filename: insight/alembic/versions/eaf7bb3598af_version_unique_constraint.py
+Comment: 
+
 Filename: insight/database/__init__.py
 Comment: 
 
 Filename: insight/database/schema.py
 Comment: 
 
 Filename: insight/database/utils.py
@@ -63,26 +69,26 @@
 
 Filename: insight/metrics/metrics_usage.py
 Comment: 
 
 Filename: insight/metrics/utils.py
 Comment: 
 
-Filename: insight-1.0rc5.dist-info/LICENSE.md
+Filename: insight-1.0rc6.dist-info/LICENSE.md
 Comment: 
 
-Filename: insight-1.0rc5.dist-info/METADATA
+Filename: insight-1.0rc6.dist-info/METADATA
 Comment: 
 
-Filename: insight-1.0rc5.dist-info/WHEEL
+Filename: insight-1.0rc6.dist-info/WHEEL
 Comment: 
 
-Filename: insight-1.0rc5.dist-info/entry_points.txt
+Filename: insight-1.0rc6.dist-info/entry_points.txt
 Comment: 
 
-Filename: insight-1.0rc5.dist-info/top_level.txt
+Filename: insight-1.0rc6.dist-info/top_level.txt
 Comment: 
 
-Filename: insight-1.0rc5.dist-info/RECORD
+Filename: insight-1.0rc6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## insight/version.py

```diff
@@ -1,4 +1,4 @@
 # file generated by setuptools_scm
 # don't change, don't track in version control
-__version__ = version = '1.0rc5'
+__version__ = version = '1.0rc6'
 __version_tuple__ = version_tuple = (1, 0)
```

## insight/database/schema.py

```diff
@@ -39,11 +39,12 @@
     id = mapped_column(INTEGER, primary_key=True)
     metric_id = mapped_column(INTEGER, ForeignKey("metric.id"))
     dataset_id = mapped_column(INTEGER, ForeignKey("dataset.id"))
     version_id = mapped_column(INTEGER, ForeignKey("version.id"))
     value = mapped_column(FLOAT)
     created_at = mapped_column(TIMESTAMP, default=func.now())
     run_id = mapped_column(VARCHAR(50), nullable=True, default=None)
+    sub_run = mapped_column(INTEGER, nullable=True, default=None)
 
     metric: Mapped[Metric] = relationship("Metric")
     dataset: Mapped[Dataset] = relationship("Dataset")
     version: Mapped[Version] = relationship("Version")
```

## insight/metrics/base.py

```diff
@@ -84,14 +84,16 @@
             category: The category of the metric.
 
         `version` and `run_id` are taken from `VERSION` and `RUN_ID` envvars.
         """
         version = os.getenv("VERSION")
         version = version if version else "Unversioned"
         run_id = os.getenv("RUN_ID")
+        sub_run_var = os.getenv("SUB_RUN")
+        sub_run: ty.Optional[int] = int(sub_run_var) if sub_run_var else None
 
         if model is None or utils is None:
             raise ModuleNotFoundError(
                 "The database module is not available. Please install it using the command: pip install 'insight[db]'"
             )
 
         if self._session is None:
@@ -112,14 +114,15 @@
                 )
                 result = model.Result(
                     metric_id=metric_id,
                     dataset_id=dataset_id,
                     version_id=version_id,
                     value=value,
                     run_id=run_id,
+                    sub_run=sub_run,
                 )
                 session.add(result)
                 session.commit()
         else:
             metric_id = utils.get_metric_id(self.name, session, category=category)
             version_id = utils.get_version_id(version, session)
             dataset_id = utils.get_df_id(
@@ -127,14 +130,15 @@
             )
             result = model.Result(
                 metric_id=metric_id,
                 dataset_id=dataset_id,
                 version_id=version_id,
                 value=value,
                 run_id=run_id,
+                sub_run=sub_run,
             )
             session.add(result)
 
 
 class OneColumnMetric(_Metric):
     """
     An abstract base class from which more specific single column metrics are derived.
```

## Comparing `insight-1.0rc5.dist-info/LICENSE.md` & `insight-1.0rc6.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `insight-1.0rc5.dist-info/METADATA` & `insight-1.0rc6.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insight
-Version: 1.0rc5
+Version: 1.0rc6
 Summary: A python library for monitoring, comparing and extracting insights from data.
 Author-email: "Synthesized Ltd." <ml@synthesized.io>, Daniel Sabanov <daniel@sadogursky.com>, Simon Swan <shk.swan@gmail.com>
 License: BSD 3-Clause License
 Project-URL: homepage, https://github.com/synthesized-io/insight
 Project-URL: documentation, https://docs.synthesized.io/
 Project-URL: repository, https://github.com/synthesized-io/insight
 Keywords: metrics,data,evaluation
```

## Comparing `insight-1.0rc5.dist-info/RECORD` & `insight-1.0rc6.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 insight/__init__.py,sha256=xLJGDMqC6EUc5RHzR29tDLtqX5RpjU0eCEyq6fFjdDM,105
 insight/check.py,sha256=ehkc74f9QrfR9LQH_nkvl5-HiQfOj_ysv2GJPSIOHGY,4698
 insight/plot.py,sha256=UZQbdsx6UzRwYSBRZh4AP517FOkkGmrlNNBoalQVDJk,18466
 insight/py.typed,sha256=qnPosECVBhmu93QEiwwk_ZCOnBi9rCDTghOj8q9vO28,55
-insight/version.py,sha256=1s_DKfbTJy_DxdfYcwhGizCaUXB0HsmCugXfbJhCptM,158
+insight/version.py,sha256=tJ55KH5U9SefkXsYWl_c4RWVFhNpdjJ6NCfjrazCff0,158
 insight/alembic/README,sha256=heMzebYwlGhnE8_4CWJ4LS74WoEZjBy-S-mIJRxAEKI,39
 insight/alembic/alembic.ini,sha256=-CcgudhSKY6M0IE3jMhzZEwwCf0uT09Oob1UQsz0mH4,263
 insight/alembic/env.py,sha256=g9kZOvpd0y98gpDYQ_Klni9bsPXymUNxpt6yJQf-_So,2677
 insight/alembic/main.py,sha256=pVL8XIChxi9TbfuYm_r4QUwOuN_ctdVh2kvuveoq2aQ,371
 insight/alembic/script.py.mako,sha256=HNlf26BI1xvQKjiUojnj15BPrVUfVVr81IOgliJf83c,510
+insight/alembic/versions/495f69cbfe6d_add_result_sub_run.py,sha256=EOaxyi-g4ttYGzdY7-Os1slTAZg8iFLOtBH37O6Mqn0,675
 insight/alembic/versions/9aca5ae68ff5_add_initial_tables.py,sha256=h5-IipYoNY3xmsUKltQac0slz7JGUWOTNyn6fxDCfHk,2390
 insight/alembic/versions/a2198ae60b44_added_version_name_unique_constaint.py,sha256=ET-YWv5PpybqLWoZM95Ri1aVhqZGRjz5OiCerCtBQ3o,890
 insight/alembic/versions/d2198fd60b0e_added_result_run_id.py,sha256=nePuKW2g4-ca30PVW1TrN7hV1Vn5pGieHhrKSHKZ-HM,879
+insight/alembic/versions/eaf7bb3598af_version_unique_constraint.py,sha256=BWhAVvuM3QXCI9j6uQIgpDWpJVTYjbwQ1EojcXPhNIo,772
 insight/database/__init__.py,sha256=pjNiVUAszisjPd_NtaFrIt86bISQ2d47Z5YsZnuQPC8,114
-insight/database/schema.py,sha256=rcxuh90_wnZmoXnAovxtVvpF6Ok6vEDWzJaa3Jfabgo,1682
+insight/database/schema.py,sha256=1kV1ffbjLPXUQEOmyY67InPBbuMlGXYtlkmOJJOtEwo,1748
 insight/database/utils.py,sha256=6o9N2CV9kuwfNgW_XRq7m5ToCGK14ee4Sisnl1Svwi0,6422
 insight/fonts/SourceSansPro-Regular.ttf,sha256=4Kys7T9WhjkMTC7Y07RHxyVmAlLRogpx_atREKQ1xGM,248132
 insight/metrics/__init__.py,sha256=OjwnoZo4OhnC2rgUgqB7uiaIf99w-uxfQEvExUXk-64,995
-insight/metrics/base.py,sha256=ufTOv7dL4vMWEbvCN4ePcC7vkzi_kHan5CWAqlEXX8U,12831
+insight/metrics/base.py,sha256=0BeFcT7uueJhabQr-V3wk7Y3dAnR-ozw20Sb8hQPy1g,13022
 insight/metrics/confidence_interval.py,sha256=Ue-WeZ1xDo8UIwxFM7Bs3H87v1Zsa7K22QJBMQuikCA,4502
 insight/metrics/metrics.py,sha256=7BIuKHVgB3QZjVhSzgweZLHRmhAVKLXa_BE1FIMG11E,19144
 insight/metrics/metrics_usage.py,sha256=fur8-b2mN5ikvG61XZjbabWyo8p2c6YGiaCF6ABx1SI,5922
 insight/metrics/utils.py,sha256=7uXQ8BjBlBtZl8NQnj6L_xsq0AVZ31UcPG0oNWvOMU4,4678
-insight-1.0rc5.dist-info/LICENSE.md,sha256=34SRBo9CjVZA5fRJlHGryTj8lTHZTjs08E1kJbwJRnk,1524
-insight-1.0rc5.dist-info/METADATA,sha256=GE8mEIQz9e0QETb-6lWh6EqxO3GALCmpVnV_EFTEG2Y,7560
-insight-1.0rc5.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-insight-1.0rc5.dist-info/entry_points.txt,sha256=Q4xIL7XTkLG2nNUXJzJ6U62U8HcAtPJREcYMGkJXBd4,65
-insight-1.0rc5.dist-info/top_level.txt,sha256=pKf63GB5OJ7SlPu4UTEv6k66v0aatCrZDC04F1xETSc,8
-insight-1.0rc5.dist-info/RECORD,,
+insight-1.0rc6.dist-info/LICENSE.md,sha256=34SRBo9CjVZA5fRJlHGryTj8lTHZTjs08E1kJbwJRnk,1524
+insight-1.0rc6.dist-info/METADATA,sha256=mj4ZHvOrpunw_T-t1zu1e4sCk3nhpHDXTnGJzBDLUJE,7560
+insight-1.0rc6.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+insight-1.0rc6.dist-info/entry_points.txt,sha256=Q4xIL7XTkLG2nNUXJzJ6U62U8HcAtPJREcYMGkJXBd4,65
+insight-1.0rc6.dist-info/top_level.txt,sha256=pKf63GB5OJ7SlPu4UTEv6k66v0aatCrZDC04F1xETSc,8
+insight-1.0rc6.dist-info/RECORD,,
```

