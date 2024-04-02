# Comparing `tmp/imgori-0.2.6-py3-none-any.whl.zip` & `tmp/imgori-0.2.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,28 +1,28 @@
-Zip file size: 11839 bytes, number of entries: 26
+Zip file size: 11847 bytes, number of entries: 26
 -rwxr-xr-x  2.0 unx      139 b- defN 80-Jan-01 00:00 imgori/__init__.py
 -rw-r--r--  2.0 unx       50 b- defN 80-Jan-01 00:00 imgori/cli.py
 -rw-r--r--  2.0 unx       25 b- defN 80-Jan-01 00:00 imgori/commands/__init__.py
 -rw-r--r--  2.0 unx     1344 b- defN 80-Jan-01 00:00 imgori/commands/train.py
 -rwxr-xr-x  2.0 unx       72 b- defN 80-Jan-01 00:00 imgori/datasets/__init__.py
--rw-r--r--  2.0 unx     2223 b- defN 80-Jan-01 00:00 imgori/datasets/imgori.py
+-rw-r--r--  2.0 unx     2156 b- defN 80-Jan-01 00:00 imgori/datasets/imgori.py
 -rwxr-xr-x  2.0 unx      650 b- defN 80-Jan-01 00:00 imgori/datasets/mnist.py
 -rw-r--r--  2.0 unx      267 b- defN 80-Jan-01 00:00 imgori/datasets/utils.py
 -rw-r--r--  2.0 unx     1673 b- defN 80-Jan-01 00:00 imgori/imgori.py
 -rwxr-xr-x  2.0 unx      103 b- defN 80-Jan-01 00:00 imgori/nn/__init__.py
 -rw-r--r--  2.0 unx      436 b- defN 80-Jan-01 00:00 imgori/nn/efficientnet.py
 -rw-r--r--  2.0 unx      968 b- defN 80-Jan-01 00:00 imgori/nn/lenet.py
 -rw-r--r--  2.0 unx      448 b- defN 80-Jan-01 00:00 imgori/nn/mobilenet_v3.py
--rw-r--r--  2.0 unx      155 b- defN 80-Jan-01 00:00 imgori/optim.py
+-rw-r--r--  2.0 unx      202 b- defN 80-Jan-01 00:00 imgori/optim.py
 -rwxr-xr-x  2.0 unx       66 b- defN 80-Jan-01 00:00 imgori/trainers/__init__.py
--rw-r--r--  2.0 unx     3913 b- defN 80-Jan-01 00:00 imgori/trainers/imgori.py
+-rw-r--r--  2.0 unx     4073 b- defN 80-Jan-01 00:00 imgori/trainers/imgori.py
 -rw-r--r--  2.0 unx     4087 b- defN 80-Jan-01 00:00 imgori/trainers/mnist.py
 -rw-r--r--  2.0 unx       70 b- defN 80-Jan-01 00:00 imgori/trainers/trainer.py
 -rw-r--r--  2.0 unx     2398 b- defN 80-Jan-01 00:00 imgori/typing.py
 -rwxr-xr-x  2.0 unx      233 b- defN 80-Jan-01 00:00 imgori/utils/__init__.py
 -rw-r--r--  2.0 unx     1212 b- defN 80-Jan-01 00:00 imgori/utils/s3.py
 -rw-r--r--  2.0 unx      744 b- defN 80-Jan-01 00:00 imgori/utils/utils.py
--rw-r--r--  2.0 unx      681 b- defN 80-Jan-01 00:00 imgori-0.2.6.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 imgori-0.2.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       41 b- defN 80-Jan-01 00:00 imgori-0.2.6.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     2013 b- defN 16-Jan-01 00:00 imgori-0.2.6.dist-info/RECORD
-26 files, 24099 bytes uncompressed, 8621 bytes compressed:  64.2%
+-rw-r--r--  2.0 unx      681 b- defN 80-Jan-01 00:00 imgori-0.2.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 imgori-0.2.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       41 b- defN 80-Jan-01 00:00 imgori-0.2.7.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     2013 b- defN 16-Jan-01 00:00 imgori-0.2.7.dist-info/RECORD
+26 files, 24239 bytes uncompressed, 8629 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -60,20 +60,20 @@
 
 Filename: imgori/utils/s3.py
 Comment: 
 
 Filename: imgori/utils/utils.py
 Comment: 
 
-Filename: imgori-0.2.6.dist-info/METADATA
+Filename: imgori-0.2.7.dist-info/METADATA
 Comment: 
 
-Filename: imgori-0.2.6.dist-info/WHEEL
+Filename: imgori-0.2.7.dist-info/WHEEL
 Comment: 
 
-Filename: imgori-0.2.6.dist-info/entry_points.txt
+Filename: imgori-0.2.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: imgori-0.2.6.dist-info/RECORD
+Filename: imgori-0.2.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## imgori/datasets/imgori.py

```diff
@@ -15,26 +15,25 @@
 from .utils import read_image
 
 
 class ImgoriDataset(Dataset):
     def __init__(
         self,
         root: str,
-        phase: Phase | None = None,
+        phase: Phase,
         transform: Callable | None = None,
         cache: bool = True,
     ) -> None:
-        self.root = Path(root)
+        self.root = Path(root) / phase
         self.phase = phase
         self.transform = transform
         self.cache = cache
 
-        pattern = "*" if phase is None else f"{phase}/*"
         exts = get_image_extensions()
-        self.images = [p for p in self.root.rglob(pattern) if p.suffix in exts]
+        self.images = [p for p in self.root.rglob("*") if p.suffix in exts]
         if cache:
             logger.info("cache images")
             self.images = [read_image(p) for p in tqdm(self.images)]
 
     def __len__(self) -> int:
         return len(self.images) * len(Orientation)
```

## imgori/optim.py

```diff
@@ -2,7 +2,8 @@
 from torch import optim
 
 register(optim.Adam)
 register(optim.RAdam)
 register(optim.SGD)
 
 register(optim.lr_scheduler.StepLR)
+register(optim.lr_scheduler.CosineAnnealingLR)
```

## imgori/trainers/imgori.py

```diff
@@ -55,16 +55,16 @@
             tqdm.write(format_string)
 
             self.state["epoch"] = epoch + 1
 
     def train(self) -> None:
         self.model.train()
 
-        loss_metric = MeanMetric()
-        acc_metric = Accuracy(task="multiclass", num_classes=self.num_classes)
+        loss_metric = MeanMetric().to(self.device)
+        acc_metric = Accuracy(task="multiclass", num_classes=self.num_classes).to(self.device)
 
         for x, y in tqdm(self.train_loader):
             x = x.to(self.device)
             y = y.to(self.device)
 
             output = self.model(x)
             loss = F.cross_entropy(output, y)
@@ -77,20 +77,23 @@
             acc_metric.update(output, y)
 
         self.metrics.update(
             train_loss=loss_metric.compute().item(),
             train_acc=acc_metric.compute().item(),
         )
 
+        del loss_metric
+        del acc_metric
+
     @torch.no_grad()
     def validate(self) -> None:
         self.model.eval()
 
-        loss_metric = MeanMetric()
-        acc_metric = Accuracy(task="multiclass", num_classes=self.num_classes)
+        loss_metric = MeanMetric().to(self.device)
+        acc_metric = Accuracy(task="multiclass", num_classes=self.num_classes).to(self.device)
 
         for x, y in tqdm(self.valid_loader):
             x = x.to(self.device)
             y = y.to(self.device)
 
             output = self.model(x)
             loss = F.cross_entropy(output, y)
@@ -104,14 +107,17 @@
             self.save_checkpoint("best.pth")
 
         self.metrics.update(
             valid_loss=loss_metric.compute().item(),
             valid_acc=valid_acc,
         )
 
+        del loss_metric
+        del acc_metric
+
     def save_checkpoint(self, f: PathLike) -> None:
         self.model.eval()
 
         checkpoint = {
             "model": self.model.state_dict(),
             "optimizer": self.optimizer.state_dict(),
             "scheduler": self.scheduler.state_dict(),
```

## Comparing `imgori-0.2.6.dist-info/METADATA` & `imgori-0.2.7.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: imgori
-Version: 0.2.6
+Version: 0.2.7
 Summary: 
 Author: narumi
 Author-email: toucans-cutouts0f@icloud.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.34.15,<2.0.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: mlconfig (>=0.2.0,<0.3.0)
 Requires-Dist: mlflow-skinny (>=2.9.2,<3.0.0)
-Requires-Dist: torch (>=2.1.1,<3.0.0)
+Requires-Dist: torch (>=2.2.2,<3.0.0)
 Requires-Dist: torchmetrics (>=1.2.0,<2.0.0)
-Requires-Dist: torchvision (>=0.16.1,<0.17.0)
+Requires-Dist: torchvision (>=0.17.2,<0.18.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
```

## Comparing `imgori-0.2.6.dist-info/RECORD` & `imgori-0.2.7.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 imgori/__init__.py,sha256=m-TKDeSlZQa9GinSYP33dTy5mICDlUyXIzW6XEHSz_4,139
 imgori/cli.py,sha256=9-LsBqnc0-ncex4EbIOHEAGPw5xBXZ57pHZW1R7a1Pk,50
 imgori/commands/__init__.py,sha256=tNKqfMuVB5L96buP08z08lQhgFmW-OSxvVuodpRbQfM,25
 imgori/commands/train.py,sha256=8-K4aToL4z4mwRQ4AUL7ENwkqQ06SEuMhEu2fkBMfAQ,1344
 imgori/datasets/__init__.py,sha256=4IEJ1jDWbYPWQhyS0-aU3r4m5hJ58pZn0DSiYqnZyhc,72
-imgori/datasets/imgori.py,sha256=K5cScJbHQhMDFJKdT3X1DUGz9CeYyegySTkUS8Yczw8,2223
+imgori/datasets/imgori.py,sha256=OgfwW0sa1NgI7jibg7DPhO11BuMaxU7VOydlhjETANA,2156
 imgori/datasets/mnist.py,sha256=eAk2Ecyp51Xu84Y-RJi5VYiyBpTosX2IvsKpBiE3Fls,650
 imgori/datasets/utils.py,sha256=2fEk28jop1QgfwhiniYtEvbVdr3fE-DMDq9y0m8SVNM,267
 imgori/imgori.py,sha256=X4s-Vs2mJ-m4v6fQ3TSfvsB7FKlu4tdstwt927KTfu8,1673
 imgori/nn/__init__.py,sha256=Kc8dsNIqvRWAD0N9tkvLsqRL29ePjCEYQHaeQzG2U9k,103
 imgori/nn/efficientnet.py,sha256=QvKjk1q-CpdIesgOKUNtSjsdmPsXSxllWd1_8o_RMXc,436
 imgori/nn/lenet.py,sha256=g5gz1u_RAFSLuDvnMqDg2ZejoQk9lNBIZqCh-LP0Ws0,968
 imgori/nn/mobilenet_v3.py,sha256=eFENzM9P2ZJHNQ3UurqLAoRZgJargYPB7th_HdcM0hs,448
-imgori/optim.py,sha256=EmwDfKqFqkwJ_Pup94V01KSu1APp60bc4GJjBFy-39A,155
+imgori/optim.py,sha256=E_eXbOhpeYRqr70ghXTYLB7GeyNBsiTv3ycw2fe1VWU,202
 imgori/trainers/__init__.py,sha256=LA1hhnTzmv_EpMtqivqmMrIR6JLXFFlWBRFcASwiaGY,66
-imgori/trainers/imgori.py,sha256=9gF35ewAD2qrnBkt5ZZ3pTbdFQXjljUFUk1DSNq_es8,3913
+imgori/trainers/imgori.py,sha256=cCUgTc2HkLOVSvzvLxVQpTHF3ImoG77AmfKHlk5w4zU,4073
 imgori/trainers/mnist.py,sha256=2DAhfGS5BYr9Bf9JVK_8FxwXbycvGansGqtAXfmieYI,4087
 imgori/trainers/trainer.py,sha256=72H5BlWgjYNV1YOwiePjP-PlSANx-kzz3jhCItsZxJs,70
 imgori/typing.py,sha256=2dVGFx8tHvn69yBb587pnvOFTaGGq0-XTGakXq1NUyM,2398
 imgori/utils/__init__.py,sha256=Z6XbCnKBP5UGMxt60JvwNu69XDJkVSHHZSW1SManhCA,233
 imgori/utils/s3.py,sha256=JA6NeafTO4JtGsbuohNKfKSEK7m9Mf9QPxzAUZJAN2c,1212
 imgori/utils/utils.py,sha256=cnfH6VaOeBzZNVfsEIesXG6eTP1RgivFW5qjk_msOxg,744
-imgori-0.2.6.dist-info/METADATA,sha256=1XBufTulBmCwKz5ztTUvw76Yp6Te5kjxhEgVsm6O-tc,681
-imgori-0.2.6.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
-imgori-0.2.6.dist-info/entry_points.txt,sha256=RBRze5SLMBGEr6NDoc_nszbzHABf-V8Wl_-VYMRwwic,41
-imgori-0.2.6.dist-info/RECORD,,
+imgori-0.2.7.dist-info/METADATA,sha256=BwE2ePqj8jmma5qNamt9QTFKCwGMn-6bv7GTrN_vYHs,681
+imgori-0.2.7.dist-info/WHEEL,sha256=FMvqSimYX_P7y0a7UY-_Mc83r5zkBZsCYPm7Lr0Bsq4,88
+imgori-0.2.7.dist-info/entry_points.txt,sha256=RBRze5SLMBGEr6NDoc_nszbzHABf-V8Wl_-VYMRwwic,41
+imgori-0.2.7.dist-info/RECORD,,
```

