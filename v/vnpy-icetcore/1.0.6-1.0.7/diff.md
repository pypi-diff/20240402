# Comparing `tmp/vnpy_icetcore-1.0.6-py3-none-any.whl.zip` & `tmp/vnpy_icetcore-1.0.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 11708 bytes, number of entries: 10
+Zip file size: 11766 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat      365 b- defN 23-Jul-27 07:41 vnpy_icetcore/__init__.py
--rw-rw-rw-  2.0 fat     8251 b- defN 23-Nov-27 07:56 vnpy_icetcore/icetcore_datafeed.py
--rw-rw-rw-  2.0 fat    31837 b- defN 24-Apr-01 08:44 vnpy_icetcore/icetcore_gateway.py
+-rw-rw-rw-  2.0 fat     8395 b- defN 24-Apr-02 09:17 vnpy_icetcore/icetcore_datafeed.py
+-rw-rw-rw-  2.0 fat    31827 b- defN 24-Apr-02 07:34 vnpy_icetcore/icetcore_gateway.py
 -rw-rw-rw-  2.0 fat        1 b- defN 22-Dec-16 01:53 vnpy_icetcore/sample/__init__.py
 -rw-rw-rw-  2.0 fat     1897 b- defN 23-Nov-27 07:57 vnpy_icetcore/sample/run.py
--rw-rw-rw-  2.0 fat       30 b- defN 24-Apr-01 08:50 vnpy_icetcore-1.0.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      343 b- defN 24-Apr-01 08:50 vnpy_icetcore-1.0.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-01 08:50 vnpy_icetcore-1.0.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       14 b- defN 24-Apr-01 08:50 vnpy_icetcore-1.0.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      846 b- defN 24-Apr-01 08:50 vnpy_icetcore-1.0.6.dist-info/RECORD
-10 files, 43676 bytes uncompressed, 10246 bytes compressed:  76.5%
+-rw-rw-rw-  2.0 fat       30 b- defN 24-Apr-02 09:21 vnpy_icetcore-1.0.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      343 b- defN 24-Apr-02 09:21 vnpy_icetcore-1.0.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-02 09:21 vnpy_icetcore-1.0.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       14 b- defN 24-Apr-02 09:21 vnpy_icetcore-1.0.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      846 b- defN 24-Apr-02 09:21 vnpy_icetcore-1.0.7.dist-info/RECORD
+10 files, 43810 bytes uncompressed, 10304 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: vnpy_icetcore/sample/__init__.py
 Comment: 
 
 Filename: vnpy_icetcore/sample/run.py
 Comment: 
 
-Filename: vnpy_icetcore-1.0.6.dist-info/LICENSE
+Filename: vnpy_icetcore-1.0.7.dist-info/LICENSE
 Comment: 
 
-Filename: vnpy_icetcore-1.0.6.dist-info/METADATA
+Filename: vnpy_icetcore-1.0.7.dist-info/METADATA
 Comment: 
 
-Filename: vnpy_icetcore-1.0.6.dist-info/WHEEL
+Filename: vnpy_icetcore-1.0.7.dist-info/WHEEL
 Comment: 
 
-Filename: vnpy_icetcore-1.0.6.dist-info/top_level.txt
+Filename: vnpy_icetcore-1.0.7.dist-info/top_level.txt
 Comment: 
 
-Filename: vnpy_icetcore-1.0.6.dist-info/RECORD
+Filename: vnpy_icetcore-1.0.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## vnpy_icetcore/icetcore_datafeed.py

```diff
@@ -107,24 +107,25 @@
         # 只对衍生品合约才查询持仓量数据
         fields: list = ["open", "high", "low", "close", "volume"]
         if symbolhead=="TC.F." or symbolhead=="TC.O.":
             fields.append("open_interest")
 
         stime=start.date()
         df=[]
-        while(True):
-            if stime<end.date():
-                print()
-                his=self.api.getquotehistory(rq_interval,1,symbolhead+contract.name,stime.strftime('%Y%m%d')+"10",(stime+timedelta(days=1)).strftime('%Y%m%d')+"10")
-                if his:
-                    df=df+his
-                stime=stime+timedelta(days=1)
-            else:
-                break
-        #df=self.api.getquotehistory(rq_interval,1,symbolhead+contract.name,start,end)
+        if rq_interval<5:
+            while(True):
+                if stime<end.date()+timedelta(days=1):
+                    his=self.api.getquotehistory(rq_interval,1,symbolhead+contract.name,stime.strftime('%Y%m%d')+"01",(stime+timedelta(days=1)).strftime('%Y%m%d')+"08")
+                    if his:
+                        df=df+his
+                    stime=stime+timedelta(days=1)
+                else:
+                    break
+        else:
+            df=self.api.getquotehistory(rq_interval,1,symbolhead+contract.name,stime.strftime('%Y%m%d')+"01",(end+timedelta(days=2)).date().strftime('%Y%m%d')+"08")
         data: List[BarData] = []
         if df:
             for row in df:
                 dt: datetime = (row["DateTime"]- adjustment).replace(tzinfo=CHINA_TZ)
                 bar: BarData = BarData(
                     symbol=symbol,
                     exchange=exchange,
```

## vnpy_icetcore/icetcore_gateway.py

```diff
@@ -587,30 +587,30 @@
         self.gateway.on_tick(tick)
 
     # def onATM(self,datatype,symbol,data:dict):
     #     pass
     def onservertime(self, serverdt):
         self.current_date = serverdt.strftime("%Y%m%d")#.replace(tzinfo=CHINA_TZ)
     def onaccountlist(self,data,count):
-        self.gateway.userid=data[0]["Account"]
-        self.gateway.brokerid=data[0]["BrokerID"]
+        if count>0:
+            self.gateway.userid=data[0]["Account"]
+            self.gateway.brokerid=data[0]["BrokerID"]
     def onordereportreal(self,data):
         """委托更新推送"""
         if not self.gateway.contract_inited:
             return
         # if data["ExecType"]==10:
         #     self.gateway.write_error("交易委托失败",data["ReportID"])
         #     return
         # elif data['ExecType']==12:
         #     self.gateway.write_log("删改单失败："+data["ReportID"])
         #     return
         symbsplit=data["Symbol"].split(".")
         symbol: str =(symbsplit[2]+"."+self.gateway.api.getsymbol_id(data["Symbol"])) if "TC.F2." not in data["Symbol"] else (data["Exchange"]+"."+data["Symbol"].replace("TC.F2.",""))
         contract: ContractData= symbol_contract_map.get(symbol, None)
-        print(symbol,"  ",contract)
         timestamp: str = f"{data['TransactDate']} {data['TransactTime']}"
         dt: datetime = datetime.strptime(timestamp, "%Y%m%d %H%M%S")
         dt: datetime = dt.replace(tzinfo=CHINA_TZ)+timedelta(hours=8)
 
         tp: tuple = (data["OrderType"], data["TimeInForce"])
 
         order: OrderData = OrderData(
@@ -627,16 +627,14 @@
             datetime=dt,
             reference=data["UserKey1"],
             gateway_name=self.gateway_name
         )
         self.gateway.on_order(order)
 
         self.sysid_orderid_map[data["UserKey1"]] = data["ReportID"]
-
-
     def onfilledreportreal(self,data):
         """成交数据推送"""
         if not self.gateway.contract_inited:
             return
         symbsplit=data["Symbol"].split(".")
         symbol: str =(symbsplit[2]+"."+self.gateway.api.getsymbol_id(data["Symbol"])) if "TC.F2." not in data["Symbol"] else (data["Exchange"]+"."+data["Symbol"].replace("TC.F2.",""))
         contract: ContractData= symbol_contract_map.get(symbol, None)
```

## Comparing `vnpy_icetcore-1.0.6.dist-info/RECORD` & `vnpy_icetcore-1.0.7.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 vnpy_icetcore/__init__.py,sha256=vlksCqG8ci0F3UyKOvMiU7XJUadwlO0as1rDo7Ri1Nc,365
-vnpy_icetcore/icetcore_datafeed.py,sha256=NeuCtCLm-A3swboKTC1Kv4tKlidotBuEX6b6lEKgQBI,8251
-vnpy_icetcore/icetcore_gateway.py,sha256=Uekbus3hIEZzUpRB3wlZO7RAhe4TqfvoeF-e2WjlmPo,31837
+vnpy_icetcore/icetcore_datafeed.py,sha256=EkPhpx8lahDjieQ7pWLvyQvbYbmj99wVrijfSBtUbhU,8395
+vnpy_icetcore/icetcore_gateway.py,sha256=HYpbTaLmGiWF9RQ65b6RNqgRF5oZMPvY6lbDyP7iXy4,31827
 vnpy_icetcore/sample/__init__.py,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
 vnpy_icetcore/sample/run.py,sha256=heMCw3IK5h59dOlB1ps2pCF0xXMhuXiFoIsiIk8R-zw,1897
-vnpy_icetcore-1.0.6.dist-info/LICENSE,sha256=mQl03LAdwPIUbhG7swmKCJxrLH4XbG_nLJ6vthUG1ZY,30
-vnpy_icetcore-1.0.6.dist-info/METADATA,sha256=w7BOWbEogIs6_uh8Q5uCPnTor_m6tvB_IoF0LkLyjko,343
-vnpy_icetcore-1.0.6.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-vnpy_icetcore-1.0.6.dist-info/top_level.txt,sha256=aWQFbP-ECltOd0qINgHp1615sTYi_Zxc8X0ITb_7ttc,14
-vnpy_icetcore-1.0.6.dist-info/RECORD,,
+vnpy_icetcore-1.0.7.dist-info/LICENSE,sha256=mQl03LAdwPIUbhG7swmKCJxrLH4XbG_nLJ6vthUG1ZY,30
+vnpy_icetcore-1.0.7.dist-info/METADATA,sha256=x1VV3Y5ulwNkNiSPI70uf-IQNNl7V4gPHy3Fq4pI-og,343
+vnpy_icetcore-1.0.7.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+vnpy_icetcore-1.0.7.dist-info/top_level.txt,sha256=aWQFbP-ECltOd0qINgHp1615sTYi_Zxc8X0ITb_7ttc,14
+vnpy_icetcore-1.0.7.dist-info/RECORD,,
```

