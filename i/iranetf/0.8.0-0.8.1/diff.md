# Comparing `tmp/iranetf-0.8.0.tar.gz` & `tmp/iranetf-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iranetf-0.8.0.tar", last modified: Fri Mar 17 10:32:45 2023, max compression
+gzip compressed data, was "iranetf-0.8.1.tar", last modified: Thu Apr 13 06:22:29 2023, max compression
```

## Comparing `iranetf-0.8.0.tar` & `iranetf-0.8.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-03-17 10:32:45.415381 iranetf-0.8.0/
--rw-rw-rw-   0        0        0    35149 2021-12-03 06:39:06.000000 iranetf-0.8.0/LICENSE
--rw-rw-rw-   0        0        0       44 2022-08-14 15:03:12.000000 iranetf-0.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0      720 2023-03-17 10:32:45.415381 iranetf-0.8.0/PKG-INFO
--rw-rw-rw-   0        0        0      152 2023-01-13 07:19:37.000000 iranetf-0.8.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-17 10:32:45.399760 iranetf-0.8.0/iranetf/
--rw-rw-rw-   0        0        0      860 2023-03-17 10:32:43.000000 iranetf-0.8.0/iranetf/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-17 10:32:45.415381 iranetf-0.8.0/iranetf/sites/
--rw-rw-rw-   0        0        0    10601 2023-03-17 10:13:19.000000 iranetf-0.8.0/iranetf/sites/__init__.py
--rw-rw-rw-   0        0        0    10516 2023-03-17 10:06:23.000000 iranetf-0.8.0/iranetf/sites/dataset.csv
-drwxrwxrwx   0        0        0        0 2023-03-17 10:32:45.415381 iranetf-0.8.0/iranetf.egg-info/
--rw-rw-rw-   0        0        0      720 2023-03-17 10:32:45.000000 iranetf-0.8.0/iranetf.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      322 2023-03-17 10:32:45.000000 iranetf-0.8.0/iranetf.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-17 10:32:45.000000 iranetf-0.8.0/iranetf.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-08-14 14:54:43.000000 iranetf-0.8.0/iranetf.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       70 2023-03-17 10:32:45.000000 iranetf-0.8.0/iranetf.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-03-17 10:32:45.000000 iranetf-0.8.0/iranetf.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      227 2023-03-16 12:43:40.000000 iranetf-0.8.0/pyproject.toml
--rw-rw-rw-   0        0        0       67 2022-03-23 04:25:25.000000 iranetf-0.8.0/pytest.ini
--rw-rw-rw-   0        0        0      817 2023-03-17 10:32:45.415381 iranetf-0.8.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-04-13 06:22:29.244557 iranetf-0.8.1/
+-rw-rw-rw-   0        0        0    35149 2021-12-03 06:39:06.000000 iranetf-0.8.1/LICENSE
+-rw-rw-rw-   0        0        0       44 2022-08-14 15:03:12.000000 iranetf-0.8.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      725 2023-04-13 06:22:29.244557 iranetf-0.8.1/PKG-INFO
+-rw-rw-rw-   0        0        0      152 2023-01-13 07:19:37.000000 iranetf-0.8.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-13 06:22:29.228936 iranetf-0.8.1/iranetf/
+-rw-rw-rw-   0        0        0      860 2023-04-13 06:22:26.000000 iranetf-0.8.1/iranetf/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-13 06:22:29.244557 iranetf-0.8.1/iranetf/sites/
+-rw-rw-rw-   0        0        0    10775 2023-04-13 05:38:47.000000 iranetf-0.8.1/iranetf/sites/__init__.py
+-rw-rw-rw-   0        0        0    10967 2023-04-13 05:45:10.000000 iranetf-0.8.1/iranetf/sites/dataset.csv
+drwxrwxrwx   0        0        0        0 2023-04-13 06:22:29.244557 iranetf-0.8.1/iranetf.egg-info/
+-rw-rw-rw-   0        0        0      725 2023-04-13 06:22:29.000000 iranetf-0.8.1/iranetf.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      312 2023-04-13 06:22:29.000000 iranetf-0.8.1/iranetf.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-13 06:22:29.000000 iranetf-0.8.1/iranetf.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-08-14 14:54:43.000000 iranetf-0.8.1/iranetf.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       70 2023-04-13 06:22:29.000000 iranetf-0.8.1/iranetf.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-04-13 06:22:29.000000 iranetf-0.8.1/iranetf.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1068 2023-04-13 06:06:07.000000 iranetf-0.8.1/pyproject.toml
+-rw-rw-rw-   0        0        0       67 2023-04-13 06:04:35.000000 iranetf-0.8.1/pytest.ini
+-rw-rw-rw-   0        0        0       42 2023-04-13 06:22:29.244557 iranetf-0.8.1/setup.cfg
```

### Comparing `iranetf-0.8.0/LICENSE` & `iranetf-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `iranetf-0.8.0/PKG-INFO` & `iranetf-0.8.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: iranetf
-Version: 0.8.0
+Version: 0.8.1
 Summary: a library to fetch data from iranetf.org
-Home-page: https://github.com/5j9/fipiran
-Author: 5j9
-Author-email: 5j9@users.noreply.github.com
+Author-email: 5j9 <5j9@users.noreply.github.com>
+Project-URL: Homepage, https://github.com/5j9/fipiran
 Project-URL: Bug Tracker, https://github.com/5j9/fipiran/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
```

### Comparing `iranetf-0.8.0/iranetf/__init__.py` & `iranetf-0.8.1/iranetf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.8.0'
+__version__ = '0.8.1'
 
 from datetime import datetime as _datetime
 
 from aiohttp import (
     ClientResponse as _ClientResponse,
     ClientSession as _ClientSession,
     ClientTimeout as _ClientTimeout,
```

### Comparing `iranetf-0.8.0/iranetf/sites/__init__.py` & `iranetf-0.8.1/iranetf/sites/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -221,23 +221,23 @@
 async def _url_type(domain: str) -> tuple:
     for protocol in ('https', 'http'):
         for SiteType in (RayanHamafza, TadbirPardaz):
             url = f'{protocol}://{domain}/'
             site = SiteType(url)
             try:
                 await site.live_navps()
-                domain = site.last_response.url
-                return f'{domain.scheme}://{domain.host}/', SiteType.__name__
             except (
                 _JSONDecodeError,
                 _ClientConnectorError,
                 _ServerTimeoutError,
                 _ClientOSError,
             ):
                 continue
+            last_url = site.last_response.url  # to avoid redirected URLs
+            return f'{last_url.scheme}://{last_url.host}/', SiteType.__name__
     return None, None
 
 
 async def _url_type_columns(domains):
     list_of_tuples = await _gather(*[_url_type(d) for d in domains])
     return zip(*list_of_tuples)
 
@@ -300,15 +300,16 @@
     return _DataFrame(
         tsetmc.dataset._L18S.values(),
         columns=['tsetmc_id', 'symbol', 'l30'],
         copy=False,
     ).drop(columns='l30')
 
 
-async def update_dataset():
+async def update_dataset() -> _DataFrame:
+    """Update dataset and return newly found that could not be added."""
     ds = load_dataset(site=False)
     fipiran_df = await _fipiran_data(ds)
 
     url, site_type = await _url_type_columns(fipiran_df['domain'])
     fipiran_df['url'] = url
     fipiran_df['site_type'] = site_type
 
@@ -335,7 +336,9 @@
         'symbol', 'name', 'type', 'tsetmc_id', 'fipiran_id', 'url', 'site_type'
     ]].to_csv(
         _DATASET_PATH,
         lineterminator='\n',
         encoding='utf-8-sig',
         index=False
     )
+
+    return new_fipiran_df[new_fipiran_df.tsetmc_id.notna()]
```

### Comparing `iranetf-0.8.0/iranetf/sites/dataset.csv` & `iranetf-0.8.1/iranetf/sites/dataset.csv`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 ارمغان,ارمغان ایرانیان,Fixed,31366347648583654,10920,http://armaghanfund.ir/,RayanHamafza
 اطلس,توسعه اطلس مفید,Stock,11427939669935844,11215,https://atlasetf.com/,TadbirPardaz
 اعتبار,نوع دوم اعتبار,Fixed,35163287528816137,12031,http://etebaretf2.com/,RayanHamafza
 اعتماد,اعتماد آفرین پارسیان,Fixed,66818022341772870,11315,http://eap-fund.com/,RayanHamafza
 افران,افرا نماد پایدار,Fixed,3846143218462419,11692,https://afra.fund/,RayanHamafza
 افق ملت,افق ملت,Stock,15451317146134956,11233,https://ofoghmellat.ir/,TadbirPardaz
 الماس,امین تدبیرگران فردا,Stock,28788598290160782,11260,http://fardaetf.tadbirfunds.ir/,RayanHamafza
-امین یکم,امین یکم فردا,Fixed,45728383369147894,11460,http://aminfarda.com/,
+امین یکم,امین یکم فردا,Fixed,45728383369147894,11460,http://aminfarda.ir/,TadbirPardaz
 انار,انار نماد ارزش,Stock,30215634246748564,11900,https://anar.fund/,RayanHamafza
 اهرم,سهامی اهرمی کاریزما,Stock,17914401175772326,11912,http://ahrom.charisma.ir/,LeveragedTadbirPardaz
 اوج,اوج دماوند,Stock,62575434414985179,11886,http://oujdamavandfund.ir/,RayanHamafza
 اوصتا,اندیشه ورزان صبا تامین,Fixed,57761388729898548,11588,https://sast.sabaamc.ir/,RayanHamafza
 اکسیژن,سهامی اکسیژن,Stock,50094941173290382,12035,http://oxygen.o2am.ir/,
 بذر,بذر امید آفرین,Stock,37222720235819361,11197,http://bazreomidfund.ir/,RayanHamafza
 تاراز,آوای تاراز زاگرس,Stock,24651394045981418,11922,http://tarazfund.ir/,RayanHamafza
@@ -35,14 +35,16 @@
 خاتم,خاتم ایساتیس پویا,Fixed,18865325633315847,11753,http://etf.isatispm.com/,RayanHamafza
 دارا,دارا الگوریتم,Fixed,62012736978844991,11660,http://darafund.ir/,RayanHamafza
 دارا یکم,واسطه گری مالی یکم,Stock,62235397452612911,11709,http://fi1fund.com/,RayanHamafza
 داریوش,ثروت داریوش,Stock,58789178087946067,11878,http://servat.dariush.fund/,RayanHamafza
 داریک,اعتماد داریک,Fixed,71076372178147339,11725,http://etemaddarik.ir/,RayanHamafza
 درسا,قابل معامله سهامی درسا,Stock,34581754264880199,11962,http://dorsaetf.com/,RayanHamafza
 دریا,دریای آبی فیروزه,Stock,11285885633824855,12039,https://daryaetf.ir/,TadbirPardaz
+درین,درین بها بازار,Fixed,21077182490095731,12086,http://dorinfund.com/,RayanHamafza
+رابین,توسعه افق رابین,Fixed,33527290777160784,12052,http://rabinetf.ir/,RayanHamafza
 رایکا,نوع دوم رایکا,Fixed,66105959479616770,12024,http://raykaetf.com/,RayanHamafza
 رشد,رشد پایدار آبان,Fixed,48287767791629523,11667,https://rpfund.ir/,TadbirPardaz
 رماس,راهبرد ممتاز ابن سینا,Stock,22002589755112021,11803,http://emacofund.ir/,RayanHamafza
 زر,پشتوانه سکه طلای زرافشان امید ایرانیان,Commodity,33254899395816171,11530,http://omidgoldfund.ir/,RayanHamafza
 زرفام,زرفام آشنا,Commodity,33144542989832366,11967,https://goldfund.ir/,RayanHamafza
 زرین,زرین کوروش,Stock,50139638026536387,11774,http://zarinfunds.com/,RayanHamafza
 زیتون,زیتون نماد پایا,Mixed,28551661889797217,11888,https://zeytoon.fund/,RayanHamafza
@@ -66,24 +68,26 @@
 لبخند,لبخند فارابی,Fixed,31569200988534548,12002,https://labkhand.irfarabi.ir/,TadbirPardaz
 مانی,ثابت مانی,Fixed,61265100181977543,11859,https://manifunds.ir/,TadbirPardaz
 مثقال,در اوراق بهادار مبتنی بر طلای زرین آگاه,Commodity,32469128621155736,11899,http://zarinagahfund.com/,RayanHamafza
 مدیر,مدیریت ثروت صندوق بازنشستگی کشوری,Stock,65576885779918210,11736,https://modirfund.ir/,TadbirPardaz
 مروارید,مروارید بها بازار,Stock,31248540252187559,11929,http://morvaridfund.ir/,RayanHamafza
 نخل,در اوراق بهادار با درآمد ثابت خلیج فارس,Fixed,27797446447955609,11989,http://nakhl.pgibc.ir/,RayanHamafza
 نهال,طلای سرخ نو ویرا,Commodity,12913156843322499,11772,http://ngmf.ir/,RayanHamafza
+نیلی,نوع دوم نیلی دماوند,Fixed,31188566503248753,12070,http://nilidamavandfund.ir/,RayanHamafza
 هامرز,اعتماد هامرز,Fixed,50503654866742146,11920,https://hummersfund.ir/,TadbirPardaz
 هم وزن,قابل معامله شاخصی کیان,Stock,47041908051542008,11924,http://kianfunds6.ir/,MabnaDP
 همای,همای آگاه,Fixed,15494954332657697,11767,https://homayeagah.ir/,RayanHamafza
 هیوا,ثروت هیوا,Stock,62845384302495432,11998,http://hiwafund.ir/,RayanHamafza
 وبازار,شاخصی بازار آشنا,Stock,41286608288791633,11763,http://indexfund.ir/,RayanHamafza
 ویستا,سهام ویستا,Stock,58852293795036597,11885,http://vistasahm.ir/,RayanHamafza
 پادا,پاداش سرمایه پارس,Stock,67522512921942106,11470,http://padashparsfund.com/,RayanHamafza
 پاداش,ارزش پاداش,Fixed,43267179898797137,11955,http://arzeshpadash.com/,RayanHamafza
 پارند,پارند پایدار سپهر,Fixed,70595828753641750,11416,https://parandfund.ir/,RayanHamafza
 پالایش,پالایشی یکم,Stock,67675656072510693,11745,http://p1fund.ir/,RayanHamafza
+پتروآگاه,بخشی پتروشیمی آگاه,Stock,37828981835497620,12093,http://petroagahfund.ir/,RayanHamafza
 پرتو,پرتو پایش پیشرو,Stock,48818952524587858,12048,http://partofund.ir/,
 کارا,نوع دوم کارا,Fixed,71843282162462661,11883,http://kara.charisma.ir/,RayanHamafza
 کاردان,تجارت شاخصی کاردان,Stock,65023851436340574,11312,https://iran-kfunds3.ir/,TadbirPardaz
 کاریس,سهامی سپند کاریزما,Stock,69067576215760005,11183,http://scetf.ir/,RayanHamafza
 کارین,با درآمد ثابت نگین سامان,Fixed,16056283141617755,11500,https://iran-kfunds4.ir/,TadbirPardaz
 کامیاب,کامیاب آشنا,Fixed,16040900750729921,11838,http://kamyabfund.ir/,RayanHamafza
 کمند,با درآمد ثابت کمند,Fixed,34718633636164421,11513,http://kamandfixedincome.com/,RayanHamafza
```

### Comparing `iranetf-0.8.0/iranetf.egg-info/PKG-INFO` & `iranetf-0.8.1/iranetf.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 Metadata-Version: 2.1
 Name: iranetf
-Version: 0.8.0
+Version: 0.8.1
 Summary: a library to fetch data from iranetf.org
-Home-page: https://github.com/5j9/fipiran
-Author: 5j9
-Author-email: 5j9@users.noreply.github.com
+Author-email: 5j9 <5j9@users.noreply.github.com>
+Project-URL: Homepage, https://github.com/5j9/fipiran
 Project-URL: Bug Tracker, https://github.com/5j9/fipiran/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
```

