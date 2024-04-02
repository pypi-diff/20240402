# Comparing `tmp/parsedmarc-8.9.3.tar.gz` & `tmp/parsedmarc-8.9.4.tar.gz`

## Comparing `parsedmarc-8.9.3.tar` & `parsedmarc-8.9.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0    72826 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/parsedmarc/__init__.py
--rw-r--r--   0        0        0    61310 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/parsedmarc/cli.py
--rw-r--r--   0        0        0    29836 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/parsedmarc/elastic.py
--rw-r--r--   0        0        0     7320 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/parsedmarc/kafkaclient.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/parsedmarc/log.py
--rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/parsedmarc/loganalytics.py
--rw-r--r--   0        0        0    28510 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/parsedmarc/opensearch.py
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/parsedmarc/s3.py
--rw-r--r--   0        0        0     7568 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/parsedmarc/splunk.py
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/parsedmarc/syslog.py
--rw-r--r--   0        0        0    18080 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/parsedmarc/utils.py
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/parsedmarc/mail/__init__.py
--rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/parsedmarc/mail/gmail.py
--rw-r--r--   0        0        0     9899 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/parsedmarc/mail/graph.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/parsedmarc/mail/imap.py
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/parsedmarc/mail/mailbox_connection.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/parsedmarc/resources/__init__.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/parsedmarc/resources/dbip/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/parsedmarc/resources/dbip/__init__.py
--rw-r--r--   0        0        0  8129156 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/parsedmarc/resources/dbip/dbip-country-lite.mmdb
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/parsedmarc/resources/maps/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/parsedmarc/resources/maps/__init__.py
--rw-r--r--   0        0        0    17351 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/parsedmarc/resources/maps/base_reverse_dns_map.csv
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/LICENSE
--rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/README.md
--rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/pyproject.toml
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 parsedmarc-8.9.3/PKG-INFO
+-rw-r--r--   0        0        0    72826 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/parsedmarc/__init__.py
+-rw-r--r--   0        0        0    61310 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/parsedmarc/cli.py
+-rw-r--r--   0        0        0    29836 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/parsedmarc/elastic.py
+-rw-r--r--   0        0        0     7320 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/parsedmarc/kafkaclient.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/parsedmarc/log.py
+-rw-r--r--   0        0        0     6611 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/parsedmarc/loganalytics.py
+-rw-r--r--   0        0        0    28510 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/parsedmarc/opensearch.py
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/parsedmarc/s3.py
+-rw-r--r--   0        0        0     7568 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/parsedmarc/splunk.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/parsedmarc/syslog.py
+-rw-r--r--   0        0        0    18080 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/parsedmarc/utils.py
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/parsedmarc/mail/__init__.py
+-rw-r--r--   0        0        0     5013 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/parsedmarc/mail/gmail.py
+-rw-r--r--   0        0        0     9899 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/parsedmarc/mail/graph.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/parsedmarc/mail/imap.py
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/parsedmarc/mail/mailbox_connection.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/parsedmarc/resources/__init__.py
+-rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/parsedmarc/resources/dbip/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/parsedmarc/resources/dbip/__init__.py
+-rw-r--r--   0        0        0  8129156 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/parsedmarc/resources/dbip/dbip-country-lite.mmdb
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/parsedmarc/resources/maps/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/parsedmarc/resources/maps/__init__.py
+-rw-r--r--   0        0        0    18793 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/parsedmarc/resources/maps/base_reverse_dns_map.csv
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/LICENSE
+-rw-r--r--   0        0        0     1948 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/README.md
+-rw-r--r--   0        0        0     1677 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/pyproject.toml
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 parsedmarc-8.9.4/PKG-INFO
```

### Comparing `parsedmarc-8.9.3/parsedmarc/__init__.py` & `parsedmarc-8.9.4/parsedmarc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 from parsedmarc.log import logger
 from parsedmarc.mail import MailboxConnection
 from parsedmarc.utils import get_base_domain, get_ip_address_info
 from parsedmarc.utils import is_outlook_msg, convert_outlook_msg
 from parsedmarc.utils import parse_email
 from parsedmarc.utils import timestamp_to_human, human_timestamp_to_datetime
 
-__version__ = "8.9.3"
+__version__ = "8.9.4"
 
 logger.debug("parsedmarc v{0}".format(__version__))
 
 feedback_report_regex = re.compile(r"^([\w\-]+): (.+)$", re.MULTILINE)
 xml_header_regex = re.compile(r"^<\?xml .*?>", re.MULTILINE)
 xml_schema_regex = re.compile(r"</??xs:schema.*>", re.MULTILINE)
 text_report_regex = re.compile(r"\s*([a-zA-Z\s]+):\s(.+)", re.MULTILINE)
```

### Comparing `parsedmarc-8.9.3/parsedmarc/cli.py` & `parsedmarc-8.9.4/parsedmarc/cli.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.9.3/parsedmarc/elastic.py` & `parsedmarc-8.9.4/parsedmarc/elastic.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.9.3/parsedmarc/kafkaclient.py` & `parsedmarc-8.9.4/parsedmarc/kafkaclient.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.9.3/parsedmarc/loganalytics.py` & `parsedmarc-8.9.4/parsedmarc/loganalytics.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.9.3/parsedmarc/opensearch.py` & `parsedmarc-8.9.4/parsedmarc/opensearch.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.9.3/parsedmarc/s3.py` & `parsedmarc-8.9.4/parsedmarc/s3.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.9.3/parsedmarc/splunk.py` & `parsedmarc-8.9.4/parsedmarc/splunk.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.9.3/parsedmarc/syslog.py` & `parsedmarc-8.9.4/parsedmarc/syslog.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.9.3/parsedmarc/utils.py` & `parsedmarc-8.9.4/parsedmarc/utils.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.9.3/parsedmarc/mail/gmail.py` & `parsedmarc-8.9.4/parsedmarc/mail/gmail.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.9.3/parsedmarc/mail/graph.py` & `parsedmarc-8.9.4/parsedmarc/mail/graph.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.9.3/parsedmarc/mail/imap.py` & `parsedmarc-8.9.4/parsedmarc/mail/imap.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.9.3/parsedmarc/mail/mailbox_connection.py` & `parsedmarc-8.9.4/parsedmarc/mail/mailbox_connection.py`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.9.3/parsedmarc/resources/dbip/dbip-country-lite.mmdb` & `parsedmarc-8.9.4/parsedmarc/resources/dbip/dbip-country-lite.mmdb`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.9.3/parsedmarc/resources/maps/README.md` & `parsedmarc-8.9.4/parsedmarc/resources/maps/README.md`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.9.3/parsedmarc/resources/maps/base_reverse_dns_map.csv` & `parsedmarc-8.9.4/parsedmarc/resources/maps/base_reverse_dns_map.csv`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 base_reverse_dns,name,type
 1e100.net,Google,Technology
+2tay.kz,2DAY Telecom LLP,ISP
 acelerate.net,AXS Bolivia S. A.,ISP
 admintek.net,Admintek,Web Host
 admintekcr.net,Admintek,Web Host
 adnsl.com,ADN Telecom,ISP
+adventconstructions.co.tz,Advent Construction Limited,Industrial
+afghan-wireless.com,Afgan Wireless,ISP
 af-k.de,I-NetPartner GmbH,ISP
 aila.org,American Immigration Lawyers Association,Nonprofit
 aknet.kg,AkNet,ISP
 albatros.uz,Albatros Health Care,Healthcare
 alembic.co.in,Alembic Pharmaceuticals,Healthcare
+alestra.net.mx,Alestra,ISP
 amazonses.com,Amazon SES,SaaS
 ambisys.net,Ambisys,Healthcare
 americanam.org,American Advanced Management,Healthcare
 amethyst.co.jp,Amethyst,Healthcare
 antelecom.net,Antelecom,ISP
 antispamcloud.com,N-Able,Email Security
 antispameurope.com,Hornetsecurity,Email Security
@@ -24,23 +28,28 @@
 asahikawa-med.ac.jp,Asahikawa Med,Healthcare
 ashtelstudios.com,Ashtel Studios,Healthcare
 askbis.com,"BIS, Inc.",Web Host
 assentportal.com,Assent,SaaS
 atmailcloud.com,atmail,Email Provider
 axtel.net,Axtel,ISP
 atw.ne.jp,ATW,Web Host
+azeronline.com,Azeronline,ISP
+barracuda.com,Barracuda,Email Security
 bayada.com,BAYADA Home Health Care,Healthcare
 bayer.de,Bayer,Healthcare
 bbtel.com,BBTEL,ISP
 beaumont.org,Corewell Health (Formerly Beaumont),Healthcare
 bigcommerce.net,BigCommerce,SaaS
+bisv.ru,Bisv.ru,ISP
 blacknight.com,Blacknight Solutions,Web Host
 bluehost.com,Bluehost,Web Host
+bluemission.net,Blue Mission,Web Host
 bluetie.com,BlueTie,MSP
 bohc.co.jp,Benefit One Inc.,Retail
+bracnet.net,BRACNet Limited,ISP
 braveriver.com,Brave River,MSP
 breezelineohio.net,Breezeline,ISP
 brinkster.com,Brinkster,Web Host
 buroserv.net.au,Brunoserv,ISP
 canonet.ne.jp,Canonet,MSP
 cardinalhealth.com,Cardinal Health,Healthcare
 carrierzone.com,carrierzone,Email Security
@@ -49,17 +58,18 @@
 charter.net,Charter,ISP
 chinaxingye.com,"Suzhou Sinye Materials Technology Co., Ltd.",Industrial
 circleamedical.com,Circle A Medical,Healthcare
 cirrushosting.com,Cirrus Hosting,Web Host
 ckt.net,Craw-Kan Telephone Cooperative,ISP
 clearwave.com,Clearwave Fiber,ISP
 climaideal.com,Clima Ideal,Retail
-cloudfilter.net,Proofpoint Cloudmark
+cloudfilter.net,Proofpoint Cloudmark,Email Security
 cloudflare.net,Cloudflare,SaaS
 cloud-sec-av.com,Check Point Avanan,Email Security
+cniteam.com,CNI,ISP
 colocrossing.com,ColoCrossing,ISP
 comcast.net,Comcast,ISP
 comcastbusiness.net,Comcast Business,ISP
 communitect.com,Solutionreach,SaaS
 concursolutions.com,SAP Concur,SaaS
 conoha.ne.jp,ConoHa,Web Host
 constantcontact.com,Constant Contact,Marketing
@@ -69,14 +79,15 @@
 creehan.com,Inovalon (Formerly Creehan & Company),Healthcare
 csod.com,Cornerstone,SaaS
 ctbcbank.com.ph,CTBC Bank (Philippines) Corp.,Finance
 cvent-planner.com,Cvent,SaaS
 cvtsv.com,Cvent,SaaS
 cwru.edu,Case Western Reserve University,University
 cyberlynk.net,CyberLynk,MSP
+dailyinvesthub.com,Daily Invest Hub,Finance
 damel.com,Damel Group,Food
 ddccommunications.com,DDC public affairs,Marketing
 diakovere.de,DIAKOVERE,Healthcare
 dimenoc.com,"HostDime.com, Inc.",Web Host
 dlivry.co,Twilio SendGrid,Marketing
 dosscloudservices.com,Doss Business Systems,MSP
 doteasy.com,Doteasy,Web Host
@@ -117,28 +128,30 @@
 flinnsci.com,Flinn Scientific,Healthcare
 flywheelsites.com,Flywheel,Web Host
 fmu.ac.jp,Fukushima Medical University,University
 formassembly.com,FormAssembly,Web Host
 fortimail.com,Fortinet FortiMail,Email Security
 forwardemail.net,ForwardEmail.net,Email Provider
 franchisemail.net,FranConnect,SaaS
+forthnet.gr,Nova,ISP
 fujita-hu.ac.jp,Fujita Health University,Healthcare
 fuse.net,Altafiber (Formerly Cincinnati Bell),ISP
 fusionconnect.com,Fusion Connect,MSP
 gandi.net,Gandi.net,Web Host
 gci.net,GCI,ISP
 globalit.com,Global IT,MSP
 gmu.edu,George Mason University,University
 gmx.com,GMX,Email Provider
 google.com,Google (Including Gmail and Google Workspace),Email Provider
 gosecure.net,GoSecure,Email Security
 gov.in,Indian government,Government
 gpphosted.com,Proofpoint (Government),Email Security
 grainger.com,Grainger Industrial Supply,Industrial
 gtnexus.com,Infor Nexus (Formerly GT Nexus),SaaS
+hanastar.net.id,HSnet,ISP
 harvard.edu,Harvard University,University
 healthall.com,UC Health
 healthproductsforyou.com,Health Products For You,Healthcare
 helpscout.net,Help Scout,SaaS
 hickorytech.net,Consolidated Communications,ISP
 highspot.com,Highspot,Marketing
 hinet.net,HiNet,ISP
@@ -150,36 +163,44 @@
 hostsevenplus.com,HostSevenPlus,Web Host
 hostwindsdns.com,Hostwinds,Web Host
 htc.net,HTC,ISP
 htmlservices.it,HTMLServices.it,MSP
 hubspotemail.net,HubSpot,Marketing
 hughston.com,Hughston Clinic,Healthcare
 ice.co.cr,Grupo ICE,Industrial
+ideaservers.net,Hetzner,Web Host
 idig.net,Canadian Web Hosting,Web Host
 improvmx.com,ImprovMX,Email Provider
-indemed.com,Cardinal Health at-home (Formerly Independence Medical),Healthcare
+indemed.com,Cardinal Health at-home (Formerly Independence Medical),Healthcare,
+infolink.ru,Infolink,ISP
 inforcloudsuite.com,Infor,SaaS
 inkyphishfence.com,INKY,Email Security
 inmotionhosting.com,InMotion Hosting,Web Host
 instantprint.com,Instant Print Corp,Print
 inxserver.de,Inxmail,Marketing
 ionblade.com,IonBLADE,Web Host
 iphmx.com,Cisco Cloud Email Security (CES),Email Security
 iphouse.net,ipHouse,Web Host
 ispgateway.de,domainfactory GmbH,Web Host
 isplevel.pro,ISPLevel,Web Host
 ispn.net,ISPN,MSP
-jonshopkins.edu,Jons Hopkins University,University
+issr.ru,Mobile TeleSystems,ISP
+iwashiya-nagai.co.jp,"Iwashiya Nagai Co., Ltd.",Healthcare
+jikei.ac.jp,The Jikei University,University
+johnshopkins.edu,Johns Hopkins University,University
 jweiland12.net,domainfactory GmbH,Web Host
 kagoya.net,KAGOYA,Web Host
 kalittacharters.com,Kalitta Charters,Logistics
+kcell.kz,Kcell,ISP
 kcn.ne.jp,KCN,ISP
 kddi.ne.jp,KIDDI,ISP
 kendall.cz,"GPS Praha, s.r.o.",Healthcare
 kennesawtrans.com,Kennesaw Transportation,Logistics
+kmtn.ru,Kostrom City Telephone Network,ISP
+knet.kg,Kyrgyztelecom,ISP
 kingswoodfacadesthailand.com,Kingswood Facades Thailand,Industrial
 kobe-u.ac.jp,Kobe University,University
 kodiaksys.com,ARIOS,SaaS
 kovacmed.com,KOVAC-MED,Healthcare
 kreativemachinez.tech,Kreative Machinez,Marketing
 ktc.kz,KTC Kazakhstan LLP,Industrial
 kundenserver.de,domainfactory GmbH,Web Host
@@ -189,37 +210,41 @@
 linkedin.com,LinkedIn,Social Media
 live-servers.net,Fasthosts Internet Ltd,Web Host
 locaweb.com.br,Locaweb,Web Host
 logix.in,Logix InfoSecurity,MSP
 lpn.co.th,L.P.N. Development PCL,Real Estate
 lstn.net,Limestone Networks,Web Host
 luxsci.com,LuxSci,Email Security
+mega.kg,Maga-Line,ISP
 mail.ru,Mail.ru,Email Provider
 mail2world.com,Mail2World,Email Provider
 mailchannels.net,MailChannels,Web Host
 mailcontrol.com,Forcepoint,Email Security
 mailgun.info,Mailgun,SaaS
 mailgun.net,Mailgun,SaaS
 mailhop.org,DuoCircle,Email Security
 mailhostbox.com,Unified Layer,Web Host
 mailinblack.com,Mailinblack,Email Security
 mailplug.co.kr,Mailplug,Email Provider
 mailplug.com,Mailplug,Email Provider
 mailroute.net,MailRoute,Email Security
+mailsecure.jp,"NTTPC Communications, Inc.",Email Security
 mailspamprotection.com,SiteGround,Web Host
+mark-itt.net,Point Internet,ISP
 marriott-service.com,Marriott,Travel
 materprivate.ie,Mater Private Network,Healthcare
 maxaninteirorsystems.com,Maxan Interior Systems,Industrial
 maximtech.com,Maximtech,Web Host
 mccooknet.com,McCookNet,Web Host
 mcdlv.net,Intuit Mailchimp,Marketing
 mchsi.com,MediacomCable,ISP
 mcsv.net,Intuit Mailchimp,Marketing
 me.com,Apple iCloud,Email Provider
 medline.com,Medline,Healthcare
+mega.kg,Mega-Line,ISP
 megacom.kg,MegaCom,ISP
 megamailservers.com,MegaMailServers,MSP
 mercranet.com,Mercranet,Web Host
 mercurygate.net,MercuryGate,SaaS
 messagelabs.com,Symantec Email Security,Email Security
 messagingengine.com,Fastmail,Email Provider
 mesvr.com,ReadNotify,Email Provider
@@ -231,28 +256,31 @@
 mit.edu,MIT,University
 mktomail.com,Marketo,Marketing
 mmrs.jp,Mirai Communication Network Inc.,Web Host
 molalla.net,Molalla Communications,ISP
 msgexch.com,Constant Contact,Marketing
 mtaroutes.com,N-able,Email Security
 mtasv.net,Postmark,SaaS
+mts.ru,MTS,ISP
 mwprem.net,NTT Com,ISP
+myworkday.com,Workday,SaaS
 mx.net,Silversky,Email Security
 mxrecord.io,Area 1 Email Security,Email Security
 mxrecord.mx,Area 1 Email Security,Email Security
 mxroute.com,MXroute,Email Provider
 mysecurecloudhost.com,World Host Group,Web Host
 my-tss.com,Performive,MSP
 mywhc.ca,Web Hosting Canada,Web Host
 nagoya-cu.ac.jp,Nagoya City University,University
 nahealth.com,Northern Arizona Healthcare,Healthcare
 name.com,Name.com,Web Host
 nano.uz,Nano Telecom,ISP
 naviexp.jp,NaviExp,MSP
 needles.co.kr,Tae Chang Industrial,Healthcare
+netroad.ru,Mobile TeleSystems,ISP
 netsolus.com,netsolus KC,MSP
 net-uno.net,"Net Uno, C.A.",ISP
 newsunseo.com,NewSunSEO,Marketing
 newtekwebhosting.com,Newtek Technology Solutions,Web Host
 ngpweb.com,Bonterra,Marketing
 nhisac.org,H-ISAC,Healthcare
 nicmail.ru,RU-CENTER,Email Provider
@@ -315,52 +343,59 @@
 qq.com,QQ,Email Provider
 quadax.com,Quadax,Healthcare
 quadranet.com,Quadranet,Web Host
 rackspace.com,Rackspace,Web Host
 ramsaysante.fr,Ramsay Santé,Healthcare
 rcn.com,RCN,ISP
 redexpertos.com,RedExpertos,Web Host
+redirection.net,Redirectionet,Web Host
 regiomed-kliniken.de,REGIOMED-KLINIKEN GmbH,Healthcare
-registrar-servers.com,Namecheap,Web Host
+registeredsite.com,Web.com,Web Host
 regxa.com,Regxa Cloud,Web Host
 riskonnectclearsight.com,Riskonnect ClearSight,SaaS
 ritternet.com,Ritter Communications,ISP
 rmx.de,Retarus GmbH,SaaS
 rootlayer.net,RootLayer LTD.,Web Host
 rsa.com,RSA,Technology
 rsgsv.net,Intuit Mailchimp,Marketing
 rt.ru,RT,Government Media
 rutgers.edu,Rutgers University,University
 rzone.de,Strato AG,Web Host
 saimanet.kg,Saima Telecom,ISP
 salesforce.com,Salesforce,SaaS
 samanage.com,SolarWinds Service Desk,SaaS
+sarkor.uz,Sarkor,ISP
 scorm.com,SCORM,SaaS
 secure.ne.jp,KIDDI,ISP
 secure-mails.com,Tata Communications,SaaS
 securemx.jp,IIJ SecureMX,Email Security
 secureserver.net,GoDaddy,Web Host
 sendgrid.net,Twilio SendGrid,Marketing
 seqtek.net,SEQTEK,MSP
 servconfig.com,InMotion Hosting,Web Host
 serverdata.net,GoDaddy,Web Host
 servicemail24.de,Arvato Systems,MSP
 service-now.com,ServiceNow,SaaS
 servidoresdns.net,Arsys,Web Host
+shatel.ir,Shatel,ISP
 showpad.com,Showpad,Marketing
+simus.uz,Simus,ISP
+siriustelecom.uz,Sirius Telecom,ISP
 siteprotect.com,SiteMail,Email Provider
 smartape.ru,Smart Ape LLC,Web Host
+smartspb.net,Smart Telecom,ISP
 smtp.com,SMTP.com,SaaS
 smtp25.com,Zix,Email Security
 smtp2go.com,SMTP2GO,SaaS
 sophos.com,Sophos,Email Security
 spamtitan.com,SpamTitan,Email Security
 sparkpostmail.com,SparkPost,Marketing
 spectrum.com,Spectrum,ISP
 srvape.com,Smart Ape LLC,Web Host
+stargatecommunications.com,X-Link Limited,ISP
 stanford.edu,Stanford University,University
 state.co.us,The State of Colorado,Government
 state.ma.us,The State of Massachusetts,Government
 state.ms.us,The State of Missouri,Government
 state.or.us,The State of Oregon,Government
 stellarllc.net,Gardonville Cooperative Telephone Association,ISP
 stewarthowe.com,Newfold Digital,Web Host
@@ -368,14 +403,15 @@
 stoneybrook.edu,Stoneybrook University,University
 strategictreasurer.com,Strategic Treasurer,Finance
 syn-alias.com,Synacor,SaaS
 synchronoss.net,Synchronoss,SaaS
 tachc.org,Texas Association of Community Health Centers (TACHC),Healthcare
 takethemameal.com,Take Them A Meal,SaaS
 telecom.kz,Kazakhtelecom,ISP
+telekom.rs,MTS,ISP
 tenders.net,Tenders.net,SaaS
 thechristhospital.com,The Christ Hospital,Healthcare
 thomsonreuters.com,Thomson Reuters,SaaS
 tical.com,Grupo Tical,Logistics
 timeweb.ru,Timeweb,Web Host
 tisco.mx,TISCO Networks,MSP
 tix.it,Tuscany Internet eXchange,ISP
@@ -383,16 +419,19 @@
 tmddedicated.com,TMDHosting,Web Host
 tohoku.ac.jp,Tohoku University,University
 tohoyk.co.jp,Toho Pharmaceutical,Healthcare
 tps.uz,TPS Telecom,ISP
 transtelecom.net,Trans Telecom,ISP
 trendmicro.com,Trend Micro,Email Security
 trendmicro.eu,Trend Micro,Email Security
+truemail.co.th,"True Internet Co., Ltd.",ISP
+ttk.ru,Joint Stock Company TransTeleCom,ISP
 tufts.edu,Tufts University,University
 ubc.ca,The University of British Columbia,University
+ucom.am,Ucom LLC,ISP
 uchealth.com,UC Health,Healthcare
 ucla.edu,UCLA,University
 uclouvain.be,UCLouvain,Healthcare
 ufanet.ru,Ufanet,ISP
 ufl.edu,University of Florida,University
 u-fukui.ac.jp,University of Fukui,University
 uhc.com,United Healthcare,Healthcare
@@ -409,21 +448,23 @@
 usp.br,University of São Paulo,University
 ussignalcom.net,US Signal,MSP
 utah.edu,University of Utah,University
 u-tokai.ac.jp,Toki University,University
 u-tokyo.ac.jp,University of Tokyo,University
 uvm.edu,University of Vermont,University
 va.gov,U.S. Department of Veterans Affairs,Government
+vdonsk.ru,Microel,ISP
 vedco.com,Vedco,Healthcare
 verginia.edu,University of Virginia,University
 verizon.net,Verizon,ISP
 verizonbusiness.com,Verizon Business,ISP
 videotron.ca,Videotron,ISP
 videotron.com,Videotron,ISP
 viecuri.nl,VieCuri,Healthcare
+viettel.vn,Viettel,ISP
 virtualhosting.hk,UDomain,Web Host
 vnpt.vn,VNPT,ISP
 vtext.com,Verizon SMS,ISP
 vulcnmold.com,VulcanMold,Industrial
 vwhs.org,Wally-Wide Health,Healthcare
 wadax.ne.jp,WADAX,Web Host
 wadax-sv.jp,WADAX,Web Host
@@ -433,29 +474,33 @@
 web-hosting.com,Namecheap,Web Host
 webzineonline.com,Webzine Online,Marketing
 wescor.com,Wescor Inc.,Healthcare
 westdc.net,"WestHost, Inc.",Web Host
 what-if.com,The Imagination Factory,MSP
 wightman.ca,Wrightman Telecom,ISP
 windstream.net,Windstream,ISP
+wntellecom.net.br,WN Tellecom,ISP
+wordpress.com,Wordpress.com,Web Host
 wpxhosting.com,WPX Hosting,Web Host
 wsh.care,The Woodlands Specialty Hospital,Healthcare
 wustl.edu,Washington University in St. Louis,University
+xbiz.ne.jp,Xserver,Web Host
 xceleratorsoftware.com,Key Software Systems Xcelerator,SaaS
 xecu.net,Xecunet,MSP
 xmission.com,XMission,SaaS
 xrea.com,XREA,Web Host
 xserver.jp,Xserver,Web Host
 yahoo.co.jp,Yahoo Japan,Email Provider
 yahoo.com,Yahoo,Email Provider
 yamaguchi-u.ac.jp,Yamaguchi University,University
 yamanashi.ac.jp,Yamanashi University,University
 yelpcorp.com,Yelp,Social Media
 yourconnect.com,"Yourconnect Co., Ltd.",Web Host
 your-server.de,Hetzner,Web Host
 yurekpharmacy.com,Yurek Pharmacy,Healthcare
 zaansmc.nl,Zaans Medical Center,Healthcare
+zare.com,Zare,Web Host
 zixsmbhosted.com,Zix,Email Security
 zixworks.com,Zix,Email Security
 zoho.com,Zoho,SaaS
 zohocorporation.com,Zoho,SaaS
 zoneedit.com,Zoneedit,Web Host
```

### Comparing `parsedmarc-8.9.3/.gitignore` & `parsedmarc-8.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.9.3/LICENSE` & `parsedmarc-8.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.9.3/README.md` & `parsedmarc-8.9.4/README.md`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.9.3/pyproject.toml` & `parsedmarc-8.9.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `parsedmarc-8.9.3/PKG-INFO` & `parsedmarc-8.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parsedmarc
-Version: 8.9.3
+Version: 8.9.4
 Summary: A Python package and CLI for parsing aggregate and forensic DMARC reports
 Project-URL: Homepage, https://domainaware.github.io/parsedmarc
 Author-email: Sean Whalen <whalenster@gmail.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Keywords: DMARC,parser,reporting
 Classifier: Development Status :: 5 - Production/Stable
```

