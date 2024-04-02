# Comparing `tmp/shippo-3.0.0rc1.tar.gz` & `tmp/shippo-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shippo-3.0.0rc1.tar", last modified: Fri Mar 29 19:54:05 2024, max compression
+gzip compressed data, was "shippo-3.1.0.tar", last modified: Tue Apr  2 18:54:17 2024, max compression
```

## Comparing `shippo-3.0.0rc1.tar` & `shippo-3.1.0.tar`

### file list

```diff
@@ -1,241 +1,241 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:54:05.112109 shippo-3.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (127)    11959 2024-03-29 19:54:05.112109 shippo-3.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9994 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 19:54:05.112109 shippo-3.0.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:54:05.076108 shippo-3.0.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:54:05.080108 shippo-3.0.0rc1/src/shippo/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:54:05.080108 shippo-3.0.0rc1/src/shippo/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    12958 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/batches.py
--rw-r--r--   0 runner    (1001) docker     (127)    21946 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/carrier_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     7759 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/carrier_parcel_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/customs_declarations.py
--rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/customs_items.py
--rw-r--r--   0 runner    (1001) docker     (127)    10177 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/manifests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:54:05.080108 shippo-3.0.0rc1/src/shippo/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:54:05.100108 shippo-3.0.0rc1/src/shippo/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/addresscompletecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/addresscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/addressimporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/addresspaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/addressvalidationresults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/addressvalidationresultsmessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/alcohol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/batchcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/batchshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/batchshipmentbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/batchshipmentpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/carrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/carrieraccountbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/carrieraccountchronopostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/carrieraccountcolissimocreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/carrieraccountcorreoscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/carrieraccountdpddecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/carrieraccountdpdukcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/carrieraccounthermesukcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/carrieraccountpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/carrieraccountregistrationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/carrieraccountservicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/carrieraccountupscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/carrieraccountupscreaterequestparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/carrieraccountuspscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/carrierparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/carriers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/cod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/connectexistingownupsaccountrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/customerreference.py
--rw-r--r--   0 runner    (1001) docker     (127)    11041 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/customsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8977 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/customsdeclarationcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/customsdeclarationpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/customsexporteridentification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/customsinvoicedcharges.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/customsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/customsitembase.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/customsitempaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/customstaxidentification.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/dangerousgoodslithiumbatteries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/dangerousgoodsobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/defaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/defaultparceltemplateupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/departmentnumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/distanceunit.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/distanceunittemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/distanceunitusertemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/dryice.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/errormessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/instanttransactionrequestbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/insurance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/invoicenumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/labelfiletype.py
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/lineitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/lineitembase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/liverate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/liveratecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/liveratepaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/manifestcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/manifestpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/objectstate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/ordercreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/orderpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2791 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/parcelcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/parcelextra.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/parcelinsurance.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/parcelpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3546 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/parcelrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10231 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/parceltemplateenumset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/pickup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/pickupbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/ponumber.py
--rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/ratemessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/ratepaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/refund.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/refundpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/refundrequestbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/rmanumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/servicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/servicegroupaccountandservicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/servicegroupcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/servicegrouptype.py
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/servicegroupupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/servicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)    41853 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/servicelevelenumset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/shipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/shipmentcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/shipmentextra.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/shipmentpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/shippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/shippoaccountpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/shippoaccountupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/track.py
--rw-r--r--   0 runner    (1001) docker     (127)     2622 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/trackingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/trackingstatuslocationbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/trackingstatussubstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/tracksrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6790 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/transactioncreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/transactionpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/upsconnectexistingownaccountparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     4017 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/userparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2262 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/userparceltemplateupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2284 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/components/weightunit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:54:05.100108 shippo-3.0.0rc1/src/shippo/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/errors/badrequestwithdetail.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/errors/badrequestwitherror.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:54:05.108108 shippo-3.0.0rc1/src/shippo/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/addshipmentstobatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/createaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/createbatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/createcarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/createcustomsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/createcustomsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/createliverate.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/createmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/createorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/createparcel.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/createpickup.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/createrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/createservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/createshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/createshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/createtrack.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/createtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/createuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/deletedefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/deleteservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/deleteuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/getaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/getbatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/getcarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/getcarrierparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/getcarrierregistrationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/getcustomsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/getcustomsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/getdefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/getmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/getorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/getparcel.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/getrate.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/getrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/getshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/getshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/gettrack.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/gettransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/getuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/listaddresses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/listcarrieraccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/listcarrierparceltemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/listcustomsdeclarations.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/listcustomsitems.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/listmanifests.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/listorders.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/listparcels.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/listrefunds.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/listservicegroups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/listshipmentrates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/listshipmentratesbycurrencycode.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/listshipments.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/listshippoaccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/listtransactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/listuserparceltemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/purchasebatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/registercarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/removeshipmentsfrombatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/updatecarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/updatedefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/updateservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/updateshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/updateuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/models/operations/validateaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)    10477 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)    10076 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/pickups.py
--rw-r--r--   0 runner    (1001) docker     (127)    10851 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/rates.py
--rw-r--r--   0 runner    (1001) docker     (127)    14245 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/rates_at_checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)     9492 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/refunds.py
--rw-r--r--   0 runner    (1001) docker     (127)    14939 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    12847 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/service_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    11104 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/shipments.py
--rw-r--r--   0 runner    (1001) docker     (127)    13831 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/shippo_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8899 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/tracking_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    10273 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17347 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/user_parcel_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:54:05.112109 shippo-3.0.0rc1/src/shippo/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    29904 2024-03-29 19:53:56.000000 shippo-3.0.0rc1/src/shippo/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 19:54:05.080108 shippo-3.0.0rc1/src/shippo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11959 2024-03-29 19:54:04.000000 shippo-3.0.0rc1/src/shippo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10964 2024-03-29 19:54:05.000000 shippo-3.0.0rc1/src/shippo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 19:54:04.000000 shippo-3.0.0rc1/src/shippo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-29 19:54:04.000000 shippo-3.0.0rc1/src/shippo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-29 19:54:04.000000 shippo-3.0.0rc1/src/shippo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:54:17.773461 shippo-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-04-02 18:54:17.773461 shippo-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9993 2024-04-02 18:54:05.000000 shippo-3.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 18:54:17.773461 shippo-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-04-02 18:54:05.000000 shippo-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:54:17.741461 shippo-3.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:54:17.745461 shippo-3.1.0/src/shippo/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:54:17.745461 shippo-3.1.0/src/shippo/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13412 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18586 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22608 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/carrier_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8017 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/carrier_parcel_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10756 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/customs_declarations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10449 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/customs_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10533 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/manifests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:54:17.745461 shippo-3.1.0/src/shippo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:54:17.761461 shippo-3.1.0/src/shippo/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/addresscompletecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/addresscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/addressimporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/addresspaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/addressvalidationresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/addressvalidationresultsmessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/alcohol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/batchcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/batchshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/batchshipmentbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/batchshipmentpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountchronopostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountcolissimocreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountcorreoscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountdpddecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountdpdukcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccounthermesukcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountregistrationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountservicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountupscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountupscreaterequestparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrieraccountuspscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carrierparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/carriers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/cod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/connectexistingownupsaccountrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/customerreference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11041 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/customsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8977 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/customsdeclarationcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/customsdeclarationpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/customsexporteridentification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/customsinvoicedcharges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/customsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/customsitembase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/customsitempaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/customstaxidentification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/dangerousgoodslithiumbatteries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/dangerousgoodsobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/defaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/defaultparceltemplateupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/departmentnumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/distanceunit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/dryice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/errormessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/instanttransactionrequestbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/insurance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/invoicenumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/labelfiletype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/lineitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/lineitembase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/liverate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/liveratecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/liveratepaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/manifestcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/manifestpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/objectstate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/ordercreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/orderpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/parcelcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/parcelextra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/parcelinsurance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/parcelpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/parcelrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10231 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/parceltemplateenumset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/pickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/pickupbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/ponumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/ratemessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/ratepaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/refund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/refundpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/refundrequestbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/rmanumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/servicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/servicegroupaccountandservicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/servicegroupcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/servicegrouptype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/servicegroupupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/servicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41853 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/servicelevelenumset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/shipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/shipmentcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/shipmentextra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/shipmentpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/shippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/shippoaccountpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/shippoaccountupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/trackingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/trackingstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/trackingstatuslocationbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/trackingstatussubstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/tracksrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/transactioncreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/transactionpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/transactionstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/upsconnectexistingownaccountparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/userparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/userparceltemplateupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/components/weightunit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:54:17.761461 shippo-3.1.0/src/shippo/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/errors/badrequestwithdetail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/errors/badrequestwitherror.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:54:17.773461 shippo-3.1.0/src/shippo/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/addshipmentstobatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createbatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createcarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createcustomsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createcustomsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createliverate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createparcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createpickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createtrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/createuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/deletedefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/deleteservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/deleteuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getbatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getcarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getcarrierparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getcarrierregistrationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getcustomsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getcustomsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getdefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getparcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/gettrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/gettransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/getuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listaddresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listcarrieraccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listcarrierparceltemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listcustomsdeclarations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listcustomsitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listmanifests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listorders.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listparcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listrefunds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listservicegroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listshipmentrates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listshipmentratesbycurrencycode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listshipments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listshippoaccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listtransactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/listuserparceltemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/purchasebatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/registercarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/removeshipmentsfrombatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/updatecarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/updatedefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/updateservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/updateshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/updateuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/models/operations/validateaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10833 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10432 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4185 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/pickups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11207 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14693 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/rates_at_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9848 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/refunds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14966 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13295 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/service_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11460 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/shipments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14285 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/shippo_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9169 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/tracking_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10397 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17893 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/user_parcel_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:54:17.773461 shippo-3.1.0/src/shippo/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30026 2024-04-02 18:54:05.000000 shippo-3.1.0/src/shippo/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 18:54:17.745461 shippo-3.1.0/src/shippo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11997 2024-04-02 18:54:17.000000 shippo-3.1.0/src/shippo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10959 2024-04-02 18:54:17.000000 shippo-3.1.0/src/shippo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 18:54:17.000000 shippo-3.1.0/src/shippo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-02 18:54:17.000000 shippo-3.1.0/src/shippo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 18:54:17.000000 shippo-3.1.0/src/shippo.egg-info/top_level.txt
```

### Comparing `shippo-3.0.0rc1/PKG-INFO` & `shippo-3.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: shippo
-Version: 3.0.0rc1
+Version: 3.1.0
 Summary: Python Client SDK Generated by Speakeasy
-Home-page: UNKNOWN
+Home-page: https://github.com/goshippo/shippo-python-sdk.git
 Author: Shippo
 License: UNKNOWN
 Description: # <img src="https://docs.goshippo.com/images/Logo.png" width="30" alt="Shippo logo"> Shippo Python SDK 
         
         Shippo is a shipping API that connects you with [multiple shipping carriers](https://goshippo.com/carriers) (such as USPS, UPS, DHL, Canada Post, Australia Post, and many others) through one interface.
         
         You must register for a [Shippo account](https://apps.goshippo.com/join) to use our API. It's free to sign up. Only pay to print a live label, test labels are free.
@@ -65,15 +65,15 @@
         For example, you could specify a header for every request that this sdk makes as follows:
         ```python
         import shippo
         import requests
         
         http_client = requests.Session()
         http_client.headers.update({'x-custom-header': 'someValue'})
-        s = shippo.Shippo(client: http_client)
+        s = shippo.Shippo(client=http_client)
         ```
         <!-- End Custom HTTP Client [http-client] -->
         
         ## Documentation
         Review our full guides and references at [https://docs.goshippo.com/](https://docs.goshippo.com/).
         
         <!-- Start Available Resources and Operations [operations] -->
```

### Comparing `shippo-3.0.0rc1/README.md` & `shippo-3.1.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 For example, you could specify a header for every request that this sdk makes as follows:
 ```python
 import shippo
 import requests
 
 http_client = requests.Session()
 http_client.headers.update({'x-custom-header': 'someValue'})
-s = shippo.Shippo(client: http_client)
+s = shippo.Shippo(client=http_client)
 ```
 <!-- End Custom HTTP Client [http-client] -->
 
 ## Documentation
 Review our full guides and references at [https://docs.goshippo.com/](https://docs.goshippo.com/).
 
 <!-- Start Available Resources and Operations [operations] -->
```

### Comparing `shippo-3.0.0rc1/setup.py` & `shippo-3.1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,17 +6,18 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="shippo",
-    version="3.0.0rc1",
+    version="3.1.0",
     author="Shippo",
     description="Python Client SDK Generated by Speakeasy",
+    url="https://github.com/goshippo/shippo-python-sdk.git",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi>=2023.7.22",
         "charset-normalizer>=3.2.0",
         "dataclasses-json>=0.6.4",
```

### Comparing `shippo-3.0.0rc1/src/shippo/_hooks/registration.py` & `shippo-3.1.0/src/shippo/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/_hooks/sdkhooks.py` & `shippo-3.1.0/src/shippo/_hooks/sdkhooks.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests
 from .types import SDKInitHook, BeforeRequestContext, BeforeRequestHook, AfterSuccessContext, AfterSuccessHook, AfterErrorContext, AfterErrorHook, Hooks
 from .registration import init_hooks
-from typing import List, Optional, Tuple, Union
+from typing import List, Optional, Tuple
 
 
 class SDKHooks(Hooks):
     def __init__(self):
         self.sdk_init_hooks: List[SDKInitHook] = []
         self.before_request_hooks: List[BeforeRequestHook] = []
         self.after_success_hooks: List[AfterSuccessHook] = []
@@ -27,27 +27,29 @@
         self.after_error_hooks.append(hook)
 
     def sdk_init(self, base_url: str, client: requests.Session) -> Tuple[str, requests.Session]:
         for hook in self.sdk_init_hooks:
             base_url, client = hook.sdk_init(base_url, client)
         return base_url, client
 
-    def before_request(self, hook_ctx: BeforeRequestContext, request: requests.PreparedRequest) -> Union[requests.PreparedRequest, Exception]:
+    def before_request(self, hook_ctx: BeforeRequestContext, request: requests.PreparedRequest) -> requests.PreparedRequest:
         for hook in self.before_request_hooks:
-            request = hook.before_request(hook_ctx, request)
-            if isinstance(request, Exception):
-                raise request
+            out = hook.before_request(hook_ctx, request)
+            if isinstance(out, Exception):
+                raise out
+            request = out
 
         return request
 
     def after_success(self, hook_ctx: AfterSuccessContext, response: requests.Response) -> requests.Response:
         for hook in self.after_success_hooks:
-            response = hook.after_success(hook_ctx, response)
-            if isinstance(response, Exception):
-                raise response
+            out = hook.after_success(hook_ctx, response)
+            if isinstance(out, Exception):
+                raise out
+            response = out
         return response
 
     def after_error(self, hook_ctx: AfterErrorContext, response: Optional[requests.Response], error: Optional[Exception]) -> Tuple[Optional[requests.Response], Optional[Exception]]:
         for hook in self.after_error_hooks:
             result = hook.after_error(hook_ctx, response, error)
             if isinstance(result, Exception):
                 raise result
```

### Comparing `shippo-3.0.0rc1/src/shippo/_hooks/types.py` & `shippo-3.1.0/src/shippo/_hooks/types.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,23 +13,27 @@
     def __init__(self, operation_id: str, oauth2_scopes: Optional[List[str]], security_source: Optional[Union[Any, Callable[[], Any]]]):
         self.operation_id = operation_id
         self.oauth2_scopes = oauth2_scopes
         self.security_source = security_source
 
 
 class BeforeRequestContext(HookContext):
-    pass
+    def __init__(self, hook_ctx: HookContext):
+        super().__init__(hook_ctx.operation_id, hook_ctx.oauth2_scopes, hook_ctx.security_source)
 
 
 class AfterSuccessContext(HookContext):
-    pass
+    def __init__(self, hook_ctx: HookContext):
+        super().__init__(hook_ctx.operation_id, hook_ctx.oauth2_scopes, hook_ctx.security_source)
+    
 
 
 class AfterErrorContext(HookContext):
-    pass
+    def __init__(self, hook_ctx: HookContext):
+        super().__init__(hook_ctx.operation_id, hook_ctx.oauth2_scopes, hook_ctx.security_source)
 
 
 class SDKInitHook(ABC):
     @abstractmethod
     def sdk_init(self, base_url: str, client: requests_http.Session) -> Tuple[str, requests_http.Session]:
         pass
 
@@ -38,21 +42,21 @@
     @abstractmethod
     def before_request(self, hook_ctx: BeforeRequestContext, request: requests_http.PreparedRequest) -> Union[requests_http.PreparedRequest, Exception]:
         pass
 
 
 class AfterSuccessHook(ABC):
     @abstractmethod
-    def after_success(self, hook_ctx: AfterSuccessContext, response: requests_http.Response) -> Union[requests_http.PreparedRequest, Exception]:
+    def after_success(self, hook_ctx: AfterSuccessContext, response: requests_http.Response) -> Union[requests_http.Response, Exception]:
         pass
 
 
 class AfterErrorHook(ABC):
     @abstractmethod
-    def after_error(self, hook_ctx: AfterErrorContext, response: Optional[requests_http.Response], error: Optional[Exception]) -> Union[Tuple[Optional[requests_http.PreparedRequest], Optional[Exception]], Exception]:
+    def after_error(self, hook_ctx: AfterErrorContext, response: Optional[requests_http.Response], error: Optional[Exception]) -> Union[Tuple[Optional[requests_http.Response], Optional[Exception]], Exception]:
         pass
 
 
 class Hooks(ABC):
     @abstractmethod
     def register_sdk_init_hook(self, hook: SDKInitHook):
         pass
```

### Comparing `shippo-3.0.0rc1/src/shippo/addresses.py` & `shippo-3.1.0/src/shippo/addresses.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
-from shippo._hooks import HookContext
+from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import Optional
 
 class Addresses:
     r"""Addresses are the locations a parcel is being shipped **from** and **to**. They represent company and residential places. Among other things, you can use address objects to create shipments, calculate shipping rates, and purchase shipping labels.
     <SchemaDefinition schemaRef=\"#/components/schemas/Address\"/>
     """
@@ -41,37 +41,36 @@
         headers = { **utils.get_headers(request), **headers }
         query_params = { **utils.get_query_params(operations.ListAddressesRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.AddressPaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -104,37 +103,36 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 201:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Address])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -164,37 +162,36 @@
         
         headers = { **utils.get_headers(request), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Address])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -224,37 +221,36 @@
         
         headers = { **utils.get_headers(request), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Address])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
```

### Comparing `shippo-3.0.0rc1/src/shippo/batches.py` & `shippo-3.1.0/src/shippo/batches.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
-from shippo._hooks import HookContext
+from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import List, Optional
 
 class Batches:
     r"""A batch is a technique for creating multiple labels at once. Use the  batch object to create and purchase many shipments in two API calls. After creating the batch, retrieve the batch to verify that all shipments are valid. You can add and remove shipments after you have created the batch. When all shipments are valid you can purchase the batch and retrieve all the shipping labels.
     <SchemaDefinition schemaRef=\"#/components/schemas/Batch\"/>
 
@@ -50,37 +50,36 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Batch])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -113,37 +112,36 @@
         
         headers = { **utils.get_headers(request), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Batch])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -177,37 +175,36 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Batch])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -240,37 +237,36 @@
         
         headers = { **utils.get_headers(request), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Batch])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -304,37 +300,36 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Batch])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
```

### Comparing `shippo-3.0.0rc1/src/shippo/carrier_accounts.py` & `shippo-3.1.0/src/shippo/carrier_accounts.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
-from shippo._hooks import HookContext
+from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import Optional, Union
 
 class CarrierAccounts:
     r"""Carriers are the companies who deliver your package. Shippo uses Carrier account objects as credentials to retrieve shipping rates and purchase labels from shipping Carriers.
 
     <SchemaDefinition schemaRef=\"#/components/schemas/CarrierAccount\"/>
@@ -40,37 +40,36 @@
         headers = { **utils.get_headers(request), **headers }
         query_params = { **utils.get_query_params(operations.ListCarrierAccountsRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.CarrierAccountPaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -103,44 +102,43 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 201:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.CarrierAccount])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.BadRequestWithDetail)
                 raise out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -170,37 +168,36 @@
         
         headers = { **utils.get_headers(request), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.CarrierAccount])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -234,37 +231,36 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.CarrierAccount])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -297,44 +293,43 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['400','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 201:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.CarrierAccount])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code == 400:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, errors.BadRequestWithError)
                 raise out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -365,37 +360,36 @@
         headers = { **utils.get_headers(request), **headers }
         query_params = { **utils.get_query_params(operations.GetCarrierRegistrationStatusRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.CarrierAccountRegistrationStatus])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
```

### Comparing `shippo-3.0.0rc1/src/shippo/carrier_parcel_templates.py` & `shippo-3.1.0/src/shippo/carrier_parcel_templates.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
-from shippo._hooks import HookContext
+from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import List, Optional
 
 class CarrierParcelTemplates:
     r"""A carrier parcel template represents a package used for shipping that has preset dimensions defined by a carrier. Some examples of a carrier parcel template include USPS Flat Rate Box and Fedex Small Pak. When using a carrier parcel template, the rates returned may be limited to the carrier that provides the box. You can create user parcel templates using a carrier parcel template. Shippo takes the dimensions of the carrier parcel template but you must configure the weight.
 
     <SchemaDefinition schemaRef=\"#/components/schemas/CarrierParcelTemplate\"/>
@@ -42,37 +42,36 @@
         headers = { **utils.get_headers(request), **headers }
         query_params = { **utils.get_query_params(operations.ListCarrierParcelTemplatesRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[components.CarrierParcelTemplate]])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -102,37 +101,36 @@
         
         headers = { **utils.get_headers(request), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.CarrierParcelTemplate])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
```

### Comparing `shippo-3.0.0rc1/src/shippo/customs_declarations.py` & `shippo-3.1.0/src/shippo/customs_items.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,204 +1,200 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
-from shippo._hooks import HookContext
+from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import Optional
 
-class CustomsDeclarations:
-    r"""Customs declarations are relevant information, including one or multiple customs items, you need to provide for
-    customs clearance for your international shipments.
-    <SchemaDefinition schemaRef=\"#/components/schemas/CustomsDeclaration\"/>
+class CustomsItems:
+    r"""Customs declarations are relevant information, including one or multiple customs items, you need to provide for customs clearance for your international shipments.
+    <SchemaDefinition schemaRef=\"#/components/schemas/CustomsItem\"/>
     """
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def list(self, page: Optional[int] = None, results: Optional[int] = None, shippo_api_version: Optional[str] = None) -> components.CustomsDeclarationPaginatedList:
-        r"""List all customs declarations
-        Returns a a list of all customs declaration objects
+    def list(self, page: Optional[int] = None, results: Optional[int] = None, shippo_api_version: Optional[str] = None) -> components.CustomsItemPaginatedList:
+        r"""List all customs items
+        Returns a list all customs items objects.
         """
-        hook_ctx = HookContext(operation_id='ListCustomsDeclarations', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.ListCustomsDeclarationsRequest(
+        hook_ctx = HookContext(operation_id='ListCustomsItems', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.ListCustomsItemsRequest(
             page=page,
             results=results,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/customs/declarations'
+        url = base_url + '/customs/items'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request), **headers }
-        query_params = { **utils.get_query_params(operations.ListCustomsDeclarationsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.ListCustomsItemsRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.CustomsDeclarationPaginatedList])
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[components.CustomsItemPaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def create(self, shippo_api_version: Optional[str] = None, customs_declaration_create_request: Optional[components.CustomsDeclarationCreateRequest] = None) -> components.CustomsDeclaration:
-        r"""Create a new customs declaration
-        Creates a new customs declaration object
+    def create(self, shippo_api_version: Optional[str] = None, customs_item_base: Optional[components.CustomsItemBase] = None) -> components.CustomsItem:
+        r"""Create a new customs item
+        Creates a new customs item object.
         """
-        hook_ctx = HookContext(operation_id='CreateCustomsDeclaration', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.CreateCustomsDeclarationRequest(
+        hook_ctx = HookContext(operation_id='CreateCustomsItem', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.CreateCustomsItemRequest(
             shippo_api_version=shippo_api_version,
-            customs_declaration_create_request=customs_declaration_create_request,
+            customs_item_base=customs_item_base,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/customs/declarations'
+        url = base_url + '/customs/items'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCustomsDeclarationRequest, "customs_declaration_create_request", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCustomsItemRequest, "customs_item_base", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 201:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.CustomsDeclaration])
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[components.CustomsItem])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def get(self, customs_declaration_id: str, page: Optional[int] = None, shippo_api_version: Optional[str] = None) -> components.CustomsDeclaration:
-        r"""Retrieve a customs declaration
-        Returns an existing customs declaration using an object ID
+    def get(self, customs_item_id: str, page: Optional[int] = None, shippo_api_version: Optional[str] = None) -> components.CustomsItem:
+        r"""Retrieve a customs item
+        Returns an existing customs item using an object ID
         """
-        hook_ctx = HookContext(operation_id='GetCustomsDeclaration', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.GetCustomsDeclarationRequest(
-            customs_declaration_id=customs_declaration_id,
+        hook_ctx = HookContext(operation_id='GetCustomsItem', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.GetCustomsItemRequest(
+            customs_item_id=customs_item_id,
             page=page,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCustomsDeclarationRequest, base_url, '/customs/declarations/{CustomsDeclarationId}', request)
+        url = utils.generate_url(operations.GetCustomsItemRequest, base_url, '/customs/items/{CustomsItemId}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request), **headers }
-        query_params = { **utils.get_query_params(operations.GetCustomsDeclarationRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.GetCustomsItemRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.CustomsDeclaration])
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[components.CustomsItem])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `shippo-3.0.0rc1/src/shippo/customs_items.py` & `shippo-3.1.0/src/shippo/manifests.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,203 +1,204 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
-from shippo._hooks import HookContext
+from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import Optional
 
-class CustomsItems:
-    r"""Customs declarations are relevant information, including one or multiple customs items, you need to provide for customs clearance for your international shipments.
-    <SchemaDefinition schemaRef=\"#/components/schemas/CustomsItem\"/>
+class Manifests:
+    r"""A manifest is a single-page document with a barcode that carriers can scan to accept all packages into transit without the need to scan each item individually.
+    They are close-outs of shipping labels of a certain day. Some carriers require manifests to  process the shipments.
+
+    <SchemaDefinition schemaRef=\"#/components/schemas/Manifest\"/>
+
+    # Manifest Errors
+    The following codes and messages are the possible errors that may occur when creating Manifests.
+    <SchemaDefinition schemaRef=\"#/components/schemas/ManifestErrors\"/>
     """
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def list(self, page: Optional[int] = None, results: Optional[int] = None, shippo_api_version: Optional[str] = None) -> components.CustomsItemPaginatedList:
-        r"""List all customs items
-        Returns a list all customs items objects.
+    def list(self, page: Optional[int] = None, results: Optional[int] = None, shippo_api_version: Optional[str] = None) -> components.ManifestPaginatedList:
+        r"""List all manifests
+        Returns a list of all manifest objects.
         """
-        hook_ctx = HookContext(operation_id='ListCustomsItems', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.ListCustomsItemsRequest(
+        hook_ctx = HookContext(operation_id='ListManifests', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.ListManifestsRequest(
             page=page,
             results=results,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/customs/items'
+        url = base_url + '/manifests'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request), **headers }
-        query_params = { **utils.get_query_params(operations.ListCustomsItemsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(operations.ListManifestsRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.CustomsItemPaginatedList])
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[components.ManifestPaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def create(self, shippo_api_version: Optional[str] = None, customs_item_base: Optional[components.CustomsItemBase] = None) -> components.CustomsItem:
-        r"""Create a new customs item
-        Creates a new customs item object.
+    def create(self, shippo_api_version: Optional[str] = None, manifest_create_request: Optional[components.ManifestCreateRequest] = None) -> components.Manifest:
+        r"""Create a new manifest
+        Creates a new manifest object.
         """
-        hook_ctx = HookContext(operation_id='CreateCustomsItem', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.CreateCustomsItemRequest(
+        hook_ctx = HookContext(operation_id='CreateManifest', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.CreateManifestRequest(
             shippo_api_version=shippo_api_version,
-            customs_item_base=customs_item_base,
+            manifest_create_request=manifest_create_request,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/customs/items'
+        url = base_url + '/manifests'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCustomsItemRequest, "customs_item_base", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateManifestRequest, "manifest_create_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 201:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.CustomsItem])
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[components.Manifest])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def get(self, customs_item_id: str, page: Optional[int] = None, shippo_api_version: Optional[str] = None) -> components.CustomsItem:
-        r"""Retrieve a customs item
-        Returns an existing customs item using an object ID
+    def get(self, manifest_id: str, shippo_api_version: Optional[str] = None) -> components.Manifest:
+        r"""Retrieve a manifest
+        Returns an existing manifest using an object ID.
         """
-        hook_ctx = HookContext(operation_id='GetCustomsItem', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.GetCustomsItemRequest(
-            customs_item_id=customs_item_id,
-            page=page,
+        hook_ctx = HookContext(operation_id='GetManifest', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.GetManifestRequest(
+            manifest_id=manifest_id,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCustomsItemRequest, base_url, '/customs/items/{CustomsItemId}', request)
+        url = utils.generate_url(operations.GetManifestRequest, base_url, '/manifests/{ManifestId}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request), **headers }
-        query_params = { **utils.get_query_params(operations.GetCustomsItemRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.CustomsItem])
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[components.Manifest])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `shippo-3.0.0rc1/src/shippo/manifests.py` & `shippo-3.1.0/src/shippo/refunds.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,207 +1,195 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
-from shippo._hooks import HookContext
+from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import Optional
 
-class Manifests:
-    r"""A manifest is a single-page document with a barcode that carriers can scan to accept all packages into transit without the need to scan each item individually.
-    They are close-outs of shipping labels of a certain day. Some carriers require manifests to  process the shipments.
-
-    <SchemaDefinition schemaRef=\"#/components/schemas/Manifest\"/>
-
-    # Manifest Errors
-    The following codes and messages are the possible errors that may occur when creating Manifests.
-    <SchemaDefinition schemaRef=\"#/components/schemas/ManifestErrors\"/>
+class Refunds:
+    r"""Refunds are reimbursements for successfully created but unused shipping labels or other charges.
+    <SchemaDefinition schemaRef=\"#/components/schemas/Refund\"/>
     """
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def list(self, page: Optional[int] = None, results: Optional[int] = None, shippo_api_version: Optional[str] = None) -> components.ManifestPaginatedList:
-        r"""List all manifests
-        Returns a list of all manifest objects.
+    def create(self, shippo_api_version: Optional[str] = None, refund_request_body: Optional[components.RefundRequestBody] = None) -> components.Refund:
+        r"""Create a refund
+        Creates a new refund object.
         """
-        hook_ctx = HookContext(operation_id='ListManifests', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.ListManifestsRequest(
-            page=page,
-            results=results,
+        hook_ctx = HookContext(operation_id='CreateRefund', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.CreateRefundRequest(
             shippo_api_version=shippo_api_version,
+            refund_request_body=refund_request_body,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/manifests'
+        url = base_url + '/refunds'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request), **headers }
-        query_params = { **utils.get_query_params(operations.ListManifestsRequest, request), **query_params }
+        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateRefundRequest, "refund_request_body", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
-        if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.ManifestPaginatedList])
+        if http_res.status_code == 201:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[components.Refund])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def create(self, shippo_api_version: Optional[str] = None, manifest_create_request: Optional[components.ManifestCreateRequest] = None) -> components.Manifest:
-        r"""Create a new manifest
-        Creates a new manifest object.
+    def list(self, shippo_api_version: Optional[str] = None) -> components.RefundPaginatedList:
+        r"""List all refunds
+        Returns a list all refund objects.
         """
-        hook_ctx = HookContext(operation_id='CreateManifest', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.CreateManifestRequest(
+        hook_ctx = HookContext(operation_id='ListRefunds', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.ListRefundsRequest(
             shippo_api_version=shippo_api_version,
-            manifest_create_request=manifest_create_request,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/manifests'
+        url = base_url + '/refunds/'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateManifestRequest, "manifest_create_request", False, True, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
-        if http_res.status_code == 201:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.Manifest])
+        if http_res.status_code == 200:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[components.RefundPaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def get(self, manifest_id: str, shippo_api_version: Optional[str] = None) -> components.Manifest:
-        r"""Retrieve a manifest
-        Returns an existing manifest using an object ID.
+    def get(self, refund_id: str, shippo_api_version: Optional[str] = None) -> components.Refund:
+        r"""Retrieve a refund
+        Returns an existing rate using a rate object ID.
         """
-        hook_ctx = HookContext(operation_id='GetManifest', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.GetManifestRequest(
-            manifest_id=manifest_id,
+        hook_ctx = HookContext(operation_id='GetRefund', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.GetRefundRequest(
+            refund_id=refund_id,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetManifestRequest, base_url, '/manifests/{ManifestId}', request)
+        url = utils.generate_url(operations.GetRefundRequest, base_url, '/refunds/{RefundId}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.Manifest])
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[components.Refund])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
```

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/__init__.py` & `shippo-3.1.0/src/shippo/models/components/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,16 +51,14 @@
 from .dangerousgoodsbiologicalmaterial import *
 from .dangerousgoodslithiumbatteries import *
 from .dangerousgoodsobject import *
 from .defaultparceltemplate import *
 from .defaultparceltemplateupdaterequest import *
 from .departmentnumber import *
 from .distanceunit import *
-from .distanceunittemplate import *
-from .distanceunitusertemplate import *
 from .dryice import *
 from .errormessage import *
 from .instanttransactionrequestbody import *
 from .insurance import *
 from .invoicenumber import *
 from .labelfiletype import *
 from .lineitem import *
@@ -106,21 +104,23 @@
 from .shipmentextra import *
 from .shipmentpaginatedlist import *
 from .shippoaccount import *
 from .shippoaccountpaginatedlist import *
 from .shippoaccountupdaterequest import *
 from .track import *
 from .trackingstatus import *
+from .trackingstatusenum import *
 from .trackingstatuslocationbase import *
 from .trackingstatussubstatus import *
 from .tracksrequest import *
 from .transaction import *
 from .transactioncreaterequest import *
 from .transactionpaginatedlist import *
+from .transactionstatusenum import *
 from .upsconnectexistingownaccountparameters import *
 from .userparceltemplate import *
 from .userparceltemplateupdaterequest import *
 from .userparceltemplatewithcarriertemplatecreaterequest import *
 from .userparceltemplatewithoutcarriertemplatecreaterequest import *
 from .weightunit import *
 
-__all__ = ["Address","AddressCompleteCreateRequest","AddressCreateRequest","AddressImporter","AddressPaginatedList","AddressValidationResults","AddressValidationResultsMessage","Alcohol","AncillaryEndorsement","Attributes","B13aFilingOption","Batch","BatchCreateRequest","BatchShipment","BatchShipmentBase","BatchShipmentPaginatedList","BatchStatus","Billing","BuildingLocationType","BuildingType","CarrierAccount","CarrierAccountBase","CarrierAccountCanadaPostCreateParameters","CarrierAccountCanadaPostCreateRequest","CarrierAccountChronopostCreateRequest","CarrierAccountColissimoCreateRequest","CarrierAccountColissimoCreateRequestParameters","CarrierAccountCorreosCreateRequest","CarrierAccountCorreosCreateRequestParameters","CarrierAccountDHLExpressCreateRequest","CarrierAccountDHLExpressCreateRequestParameters","CarrierAccountDPDUKCreateRequest","CarrierAccountDPDUKCreateRequestParameters","CarrierAccountDeutschePostCreateRequest","CarrierAccountDeutschePostCreateRequestParameters","CarrierAccountDpdDeCreateRequest","CarrierAccountDpdDeCreateRequestParameters","CarrierAccountHermesUKCreateRequest","CarrierAccountHermesUKCreateRequestParameters","CarrierAccountPaginatedList","CarrierAccountPosteItalianeCreateRequest","CarrierAccountPosteItalianeCreateRequestParameters","CarrierAccountRegistrationStatus","CarrierAccountServiceLevel","CarrierAccountUPSCreateRequest","CarrierAccountUPSCreateRequestParameters","CarrierAccountUSPSCreateRequest","CarrierAccountUSPSCreateRequestParameters","CarrierParcelTemplate","Carriers","Cod","Code","ConnectExistingOwnUPSAccountRequest","ContentsType","CustomerReference","CustomsDeclaration","CustomsDeclarationAddressImporter","CustomsDeclarationCreateRequest","CustomsDeclarationCreateRequestB13aFilingOption","CustomsDeclarationCreateRequestContentsType","CustomsDeclarationCreateRequestEelPfc","CustomsDeclarationCreateRequestIncoterm","CustomsDeclarationCreateRequestNonDeliveryOption","CustomsDeclarationPaginatedList","CustomsExporterIdentification","CustomsInvoicedCharges","CustomsItem","CustomsItemBase","CustomsItemPaginatedList","CustomsTaxIdentification","CustomsTaxIdentificationType","DangerousGoodsBiologicalMaterial","DangerousGoodsCode","DangerousGoodsLithiumBatteries","DangerousGoodsObject","DefaultParcelTemplate","DefaultParcelTemplateUpdateRequest","DepartmentNumber","DistanceUnit","DistanceUnitTemplate","DistanceUnitUserTemplate","DryIce","EelPfc","ErrorMessage","Incoterm","InstantTransactionRequestBody","InstantTransactionRequestBodyLabelFileType","Insurance","InvoiceNumber","LabelFileType","LasershipAttrs","LineItem","LineItemBase","LiveRate","LiveRateCreateRequest","LiveRatePaginatedList","Location","Manifest","ManifestCreateRequest","ManifestPaginatedList","ManifestStatus","Messages","NonDeliveryOption","ObjectResults","ObjectState","Order","OrderCreateRequest","OrderCreateRequestOrderStatus","OrderPaginatedList","OrderStatus","Parameters","Parcel","ParcelCreateRequest","ParcelExtra","ParcelInsurance","ParcelInsuranceProvider","ParcelObjectState","ParcelPaginatedList","ParcelRequest","ParcelTemplateAramexAustralia","ParcelTemplateCouriersPlease","ParcelTemplateDHLeCommerce","ParcelTemplateDPDUK","ParcelTemplateFedEx","ParcelTemplateUPS","ParcelTemplateUSPS","PaymentMethod","Pickup","PickupBase","PickupStatus","PoNumber","PreferredDeliveryTimeframe","Provider","Rate","RateMessage","RatePaginatedList","RecipientType","Refund","RefundPaginatedList","RefundRequestBody","RefundStatus","ReturnServiceType","RmaNumber","Security","ServiceGroup","ServiceGroupAccountAndServiceLevel","ServiceGroupCreateRequest","ServiceGroupType","ServiceGroupUpdateRequest","ServiceLevel","ServiceLevelAPCPostal","ServiceLevelAPG","ServiceLevelAirterra","ServiceLevelAramexAustralia","ServiceLevelAsendia","ServiceLevelAustraliaPost","ServiceLevelAxleHire","ServiceLevelBetterTrucks","ServiceLevelCDL","ServiceLevelCanadaPost","ServiceLevelChronopost","ServiceLevelColissimo","ServiceLevelCorreosEspana","ServiceLevelCouriersPlease","ServiceLevelDHLExpress","ServiceLevelDHLGermany","ServiceLevelDHLeCommerce","ServiceLevelDPDDE","ServiceLevelDPDUK","ServiceLevelDeutschePost","ServiceLevelEvriUK","ServiceLevelFedEx","ServiceLevelGLSUS","ServiceLevelGlobegistics","ServiceLevelLSO","ServiceLevelLasership","ServiceLevelMaergo","ServiceLevelMondialRelay","ServiceLevelOnTrac","ServiceLevelParcelforce","ServiceLevelPostItaliane","ServiceLevelPurolator","ServiceLevelRoyalMail","ServiceLevelSendle","ServiceLevelSwyft","ServiceLevelUDS","ServiceLevelUPS","ServiceLevelUSPS","ServiceLevelVeho","ServiceLevelePostGlobal","Shipment","ShipmentCreateRequest","ShipmentExtra","ShipmentPaginatedList","ShipmentStatus","ShippoAccount","ShippoAccountPaginatedList","ShippoAccountUpdateRequest","ShopApp","SignatureConfirmation","Source","Status","Track","TrackingStatus","TrackingStatusLocationBase","TrackingStatusStatus","TrackingStatusSubstatus","TracksRequest","Transaction","TransactionCreateRequest","TransactionMessages","TransactionPaginatedList","TransactionStatus","Type","UPSConnectExistingOwnAccountParameters","UserParcelTemplate","UserParcelTemplateUpdateRequest","UserParcelTemplateWithCarrierTemplateCreateRequest","UserParcelTemplateWithoutCarrierTemplateCreateRequest","WeightUnit"]
+__all__ = ["Address","AddressCompleteCreateRequest","AddressCreateRequest","AddressImporter","AddressPaginatedList","AddressValidationResults","AddressValidationResultsMessage","Alcohol","AncillaryEndorsement","Attributes","B13aFilingOption","Batch","BatchCreateRequest","BatchShipment","BatchShipmentBase","BatchShipmentPaginatedList","BatchStatus","Billing","BuildingLocationType","BuildingType","CarrierAccount","CarrierAccountBase","CarrierAccountCanadaPostCreateParameters","CarrierAccountCanadaPostCreateRequest","CarrierAccountChronopostCreateRequest","CarrierAccountColissimoCreateRequest","CarrierAccountColissimoCreateRequestParameters","CarrierAccountCorreosCreateRequest","CarrierAccountCorreosCreateRequestParameters","CarrierAccountDHLExpressCreateRequest","CarrierAccountDHLExpressCreateRequestParameters","CarrierAccountDPDUKCreateRequest","CarrierAccountDPDUKCreateRequestParameters","CarrierAccountDeutschePostCreateRequest","CarrierAccountDeutschePostCreateRequestParameters","CarrierAccountDpdDeCreateRequest","CarrierAccountDpdDeCreateRequestParameters","CarrierAccountHermesUKCreateRequest","CarrierAccountHermesUKCreateRequestParameters","CarrierAccountPaginatedList","CarrierAccountPosteItalianeCreateRequest","CarrierAccountPosteItalianeCreateRequestParameters","CarrierAccountRegistrationStatus","CarrierAccountServiceLevel","CarrierAccountUPSCreateRequest","CarrierAccountUPSCreateRequestParameters","CarrierAccountUSPSCreateRequest","CarrierAccountUSPSCreateRequestParameters","CarrierParcelTemplate","Carriers","Cod","Code","ConnectExistingOwnUPSAccountRequest","ContentsType","CustomerReference","CustomsDeclaration","CustomsDeclarationAddressImporter","CustomsDeclarationCreateRequest","CustomsDeclarationCreateRequestB13aFilingOption","CustomsDeclarationCreateRequestContentsType","CustomsDeclarationCreateRequestEelPfc","CustomsDeclarationCreateRequestIncoterm","CustomsDeclarationCreateRequestNonDeliveryOption","CustomsDeclarationPaginatedList","CustomsExporterIdentification","CustomsInvoicedCharges","CustomsItem","CustomsItemBase","CustomsItemPaginatedList","CustomsTaxIdentification","CustomsTaxIdentificationType","DangerousGoodsBiologicalMaterial","DangerousGoodsCode","DangerousGoodsLithiumBatteries","DangerousGoodsObject","DefaultParcelTemplate","DefaultParcelTemplateUpdateRequest","DepartmentNumber","DistanceUnit","DryIce","EelPfc","ErrorMessage","Incoterm","InstantTransactionRequestBody","InstantTransactionRequestBodyLabelFileType","Insurance","InvoiceNumber","LabelFileType","LasershipAttrs","LineItem","LineItemBase","LiveRate","LiveRateCreateRequest","LiveRatePaginatedList","Location","Manifest","ManifestCreateRequest","ManifestPaginatedList","ManifestStatus","Messages","NonDeliveryOption","ObjectResults","ObjectState","Order","OrderCreateRequest","OrderCreateRequestOrderStatus","OrderPaginatedList","OrderStatus","Parameters","Parcel","ParcelCreateRequest","ParcelExtra","ParcelInsurance","ParcelInsuranceProvider","ParcelObjectState","ParcelPaginatedList","ParcelRequest","ParcelTemplateAramexAustralia","ParcelTemplateCouriersPlease","ParcelTemplateDHLeCommerce","ParcelTemplateDPDUK","ParcelTemplateFedEx","ParcelTemplateUPS","ParcelTemplateUSPS","PaymentMethod","Pickup","PickupBase","PickupStatus","PoNumber","PreferredDeliveryTimeframe","Provider","Rate","RateMessage","RatePaginatedList","RecipientType","Refund","RefundPaginatedList","RefundRequestBody","RefundStatus","ReturnServiceType","RmaNumber","Security","ServiceGroup","ServiceGroupAccountAndServiceLevel","ServiceGroupCreateRequest","ServiceGroupType","ServiceGroupUpdateRequest","ServiceLevel","ServiceLevelAPCPostal","ServiceLevelAPG","ServiceLevelAirterra","ServiceLevelAramexAustralia","ServiceLevelAsendia","ServiceLevelAustraliaPost","ServiceLevelAxleHire","ServiceLevelBetterTrucks","ServiceLevelCDL","ServiceLevelCanadaPost","ServiceLevelChronopost","ServiceLevelColissimo","ServiceLevelCorreosEspana","ServiceLevelCouriersPlease","ServiceLevelDHLExpress","ServiceLevelDHLGermany","ServiceLevelDHLeCommerce","ServiceLevelDPDDE","ServiceLevelDPDUK","ServiceLevelDeutschePost","ServiceLevelEvriUK","ServiceLevelFedEx","ServiceLevelGLSUS","ServiceLevelGlobegistics","ServiceLevelLSO","ServiceLevelLasership","ServiceLevelMaergo","ServiceLevelMondialRelay","ServiceLevelOnTrac","ServiceLevelParcelforce","ServiceLevelPostItaliane","ServiceLevelPurolator","ServiceLevelRoyalMail","ServiceLevelSendle","ServiceLevelSwyft","ServiceLevelUDS","ServiceLevelUPS","ServiceLevelUSPS","ServiceLevelVeho","ServiceLevelePostGlobal","Shipment","ShipmentCreateRequest","ShipmentExtra","ShipmentPaginatedList","ShipmentStatus","ShippoAccount","ShippoAccountPaginatedList","ShippoAccountUpdateRequest","ShopApp","SignatureConfirmation","Source","Status","Track","TrackingStatus","TrackingStatusEnum","TrackingStatusLocationBase","TrackingStatusSubstatus","TracksRequest","Transaction","TransactionCreateRequest","TransactionMessages","TransactionPaginatedList","TransactionStatusEnum","Type","UPSConnectExistingOwnAccountParameters","UserParcelTemplate","UserParcelTemplateUpdateRequest","UserParcelTemplateWithCarrierTemplateCreateRequest","UserParcelTemplateWithoutCarrierTemplateCreateRequest","WeightUnit"]
```

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/address.py` & `shippo-3.1.0/src/shippo/models/components/address.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/addresscompletecreaterequest.py` & `shippo-3.1.0/src/shippo/models/components/addresscompletecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/addresscreaterequest.py` & `shippo-3.1.0/src/shippo/models/components/addresscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/addressimporter.py` & `shippo-3.1.0/src/shippo/models/components/addressimporter.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/addresspaginatedlist.py` & `shippo-3.1.0/src/shippo/models/components/addresspaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/addressvalidationresults.py` & `shippo-3.1.0/src/shippo/models/components/addressvalidationresults.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/addressvalidationresultsmessage.py` & `shippo-3.1.0/src/shippo/models/components/addressvalidationresultsmessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/alcohol.py` & `shippo-3.1.0/src/shippo/models/components/alcohol.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/batch.py` & `shippo-3.1.0/src/shippo/models/components/batch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/batchcreaterequest.py` & `shippo-3.1.0/src/shippo/models/components/batchcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/batchshipment.py` & `shippo-3.1.0/src/shippo/models/components/batchshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/batchshipmentbase.py` & `shippo-3.1.0/src/shippo/models/components/batchshipmentbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/batchshipmentpaginatedlist.py` & `shippo-3.1.0/src/shippo/models/components/batchshipmentpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/billing.py` & `shippo-3.1.0/src/shippo/models/components/billing.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/carrieraccount.py` & `shippo-3.1.0/src/shippo/models/components/carrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/carrieraccountbase.py` & `shippo-3.1.0/src/shippo/models/components/carrieraccountbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py` & `shippo-3.1.0/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py` & `shippo-3.1.0/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/carrieraccountchronopostcreaterequest.py` & `shippo-3.1.0/src/shippo/models/components/carrieraccountchronopostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/carrieraccountcolissimocreaterequest.py` & `shippo-3.1.0/src/shippo/models/components/carrieraccountcolissimocreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/carrieraccountcorreoscreaterequest.py` & `shippo-3.1.0/src/shippo/models/components/carrieraccountcorreoscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py` & `shippo-3.1.0/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py` & `shippo-3.1.0/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py` & `shippo-3.1.0/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/carrieraccountdpddecreaterequest.py` & `shippo-3.1.0/src/shippo/models/components/carrieraccountdpddecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/carrieraccountdpdukcreaterequest.py` & `shippo-3.1.0/src/shippo/models/components/carrieraccountdpdukcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/carrieraccounthermesukcreaterequest.py` & `shippo-3.1.0/src/shippo/models/components/carrieraccounthermesukcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/carrieraccountpaginatedlist.py` & `shippo-3.1.0/src/shippo/models/components/carrieraccountpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py` & `shippo-3.1.0/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/carrieraccountregistrationstatus.py` & `shippo-3.1.0/src/shippo/models/components/carrieraccountregistrationstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/carrieraccountservicelevel.py` & `shippo-3.1.0/src/shippo/models/components/carrieraccountservicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/carrieraccountupscreaterequest.py` & `shippo-3.1.0/src/shippo/models/components/carrieraccountupscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/carrieraccountupscreaterequestparameters.py` & `shippo-3.1.0/src/shippo/models/components/carrieraccountupscreaterequestparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/carrieraccountuspscreaterequest.py` & `shippo-3.1.0/src/shippo/models/components/carrieraccountuspscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/carrierparceltemplate.py` & `shippo-3.1.0/src/shippo/models/components/carrierparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/carriers.py` & `shippo-3.1.0/src/shippo/models/components/carriers.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/cod.py` & `shippo-3.1.0/src/shippo/models/components/cod.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/connectexistingownupsaccountrequest.py` & `shippo-3.1.0/src/shippo/models/components/connectexistingownupsaccountrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/customerreference.py` & `shippo-3.1.0/src/shippo/models/components/customerreference.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/customsdeclaration.py` & `shippo-3.1.0/src/shippo/models/components/customsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/customsdeclarationcreaterequest.py` & `shippo-3.1.0/src/shippo/models/components/customsdeclarationcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/customsdeclarationpaginatedlist.py` & `shippo-3.1.0/src/shippo/models/components/customsdeclarationpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/customsexporteridentification.py` & `shippo-3.1.0/src/shippo/models/components/customsexporteridentification.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/customsinvoicedcharges.py` & `shippo-3.1.0/src/shippo/models/components/customsinvoicedcharges.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/customsitem.py` & `shippo-3.1.0/src/shippo/models/components/customsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/customsitembase.py` & `shippo-3.1.0/src/shippo/models/components/customsitembase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/customsitempaginatedlist.py` & `shippo-3.1.0/src/shippo/models/components/customsitempaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/customstaxidentification.py` & `shippo-3.1.0/src/shippo/models/components/customstaxidentification.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py` & `shippo-3.1.0/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/dangerousgoodslithiumbatteries.py` & `shippo-3.1.0/src/shippo/models/components/dangerousgoodslithiumbatteries.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/dangerousgoodsobject.py` & `shippo-3.1.0/src/shippo/models/components/dangerousgoodsobject.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/defaultparceltemplate.py` & `shippo-3.1.0/src/shippo/models/components/defaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/defaultparceltemplateupdaterequest.py` & `shippo-3.1.0/src/shippo/models/components/defaultparceltemplateupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/departmentnumber.py` & `shippo-3.1.0/src/shippo/models/components/departmentnumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/dryice.py` & `shippo-3.1.0/src/shippo/models/components/dryice.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/errormessage.py` & `shippo-3.1.0/src/shippo/models/components/errormessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/instanttransactionrequestbody.py` & `shippo-3.1.0/src/shippo/models/components/instanttransactionrequestbody.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/insurance.py` & `shippo-3.1.0/src/shippo/models/components/insurance.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/invoicenumber.py` & `shippo-3.1.0/src/shippo/models/components/invoicenumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/labelfiletype.py` & `shippo-3.1.0/src/shippo/models/components/labelfiletype.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/lineitem.py` & `shippo-3.1.0/src/shippo/models/components/lineitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/lineitembase.py` & `shippo-3.1.0/src/shippo/models/components/lineitembase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/liverate.py` & `shippo-3.1.0/src/shippo/models/components/liverate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/liveratecreaterequest.py` & `shippo-3.1.0/src/shippo/models/components/liveratecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/liveratepaginatedlist.py` & `shippo-3.1.0/src/shippo/models/components/liveratepaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/location.py` & `shippo-3.1.0/src/shippo/models/components/location.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/manifest.py` & `shippo-3.1.0/src/shippo/models/components/manifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/manifestcreaterequest.py` & `shippo-3.1.0/src/shippo/models/components/manifestcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/manifestpaginatedlist.py` & `shippo-3.1.0/src/shippo/models/components/manifestpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/order.py` & `shippo-3.1.0/src/shippo/models/components/order.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/ordercreaterequest.py` & `shippo-3.1.0/src/shippo/models/components/ordercreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/orderpaginatedlist.py` & `shippo-3.1.0/src/shippo/models/components/orderpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/parcel.py` & `shippo-3.1.0/src/shippo/models/components/parcel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
-from .distanceunittemplate import DistanceUnitTemplate
+from .distanceunit import DistanceUnit
 from .parcelextra import ParcelExtra
 from .parceltemplateenumset import ParcelTemplateAramexAustralia, ParcelTemplateCouriersPlease, ParcelTemplateDHLeCommerce, ParcelTemplateDPDUK, ParcelTemplateFedEx, ParcelTemplateUPS, ParcelTemplateUSPS
 from .weightunit import WeightUnit
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from enum import Enum
 from shippo import utils
@@ -17,16 +17,16 @@
     r"""A Parcel will only be valid when all required values have been sent and validated successfully."""
     VALID = 'VALID'
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Parcel:
-    distance_unit: DistanceUnitTemplate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit') }})
-    r"""The measure unit used for length, width and height. Required if template is not specified."""
+    distance_unit: DistanceUnit = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit') }})
+    r"""The measure unit used for length, width and height."""
     height: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height') }})
     r"""**Required if template is not specified**<br>
     Height of the parcel. Up to six digits in front and four digits after the decimal separator are accepted.
     """
     length: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('length') }})
     r"""**Required if template is not specified**<br>
     Length of the Parcel. Up to six digits in front and four digits after the decimal separator are accepted.
```

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/parcelcreaterequest.py` & `shippo-3.1.0/src/shippo/models/components/parcelcreaterequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .distanceunittemplate import DistanceUnitTemplate
+from .distanceunit import DistanceUnit
 from .parceltemplateenumset import ParcelTemplateAramexAustralia, ParcelTemplateCouriersPlease, ParcelTemplateDHLeCommerce, ParcelTemplateDPDUK, ParcelTemplateFedEx, ParcelTemplateUPS, ParcelTemplateUSPS
 from .weightunit import WeightUnit
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import Optional, Union
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ParcelCreateRequest:
-    distance_unit: DistanceUnitTemplate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit') }})
-    r"""The measure unit used for length, width and height. Required if template is not specified."""
+    distance_unit: DistanceUnit = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit') }})
+    r"""The measure unit used for length, width and height."""
     height: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height') }})
     r"""**Required if template is not specified**<br>
     Height of the parcel. Up to six digits in front and four digits after the decimal separator are accepted.
     """
     length: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('length') }})
     r"""**Required if template is not specified**<br>
     Length of the Parcel. Up to six digits in front and four digits after the decimal separator are accepted.
```

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/parcelextra.py` & `shippo-3.1.0/src/shippo/models/components/parcelextra.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/parcelinsurance.py` & `shippo-3.1.0/src/shippo/models/components/parcelinsurance.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/parcelpaginatedlist.py` & `shippo-3.1.0/src/shippo/models/components/parcelpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/parcelrequest.py` & `shippo-3.1.0/src/shippo/models/components/parcelrequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .distanceunittemplate import DistanceUnitTemplate
+from .distanceunit import DistanceUnit
 from .parcelextra import ParcelExtra
 from .parceltemplateenumset import ParcelTemplateAramexAustralia, ParcelTemplateCouriersPlease, ParcelTemplateDHLeCommerce, ParcelTemplateDPDUK, ParcelTemplateFedEx, ParcelTemplateUPS, ParcelTemplateUSPS
 from .weightunit import WeightUnit
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import Optional, Union
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class ParcelRequest:
-    distance_unit: DistanceUnitTemplate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit') }})
-    r"""The measure unit used for length, width and height. Required if template is not specified."""
+    distance_unit: DistanceUnit = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit') }})
+    r"""The measure unit used for length, width and height."""
     height: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height') }})
     r"""Required if template is not specified. Height of the parcel. Up to six digits in front and four digits after the decimal separator are accepted."""
     length: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('length') }})
     r"""Required if template is not specified. Length of the Parcel. Up to six digits in front and four digits after the decimal separator are accepted."""
     mass_unit: WeightUnit = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('mass_unit') }})
     r"""The unit used for weight."""
     weight: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight') }})
```

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/parceltemplateenumset.py` & `shippo-3.1.0/src/shippo/models/components/parceltemplateenumset.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/pickup.py` & `shippo-3.1.0/src/shippo/models/components/pickup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/pickupbase.py` & `shippo-3.1.0/src/shippo/models/components/pickupbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/ponumber.py` & `shippo-3.1.0/src/shippo/models/components/ponumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/rate.py` & `shippo-3.1.0/src/shippo/models/components/rate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/ratemessage.py` & `shippo-3.1.0/src/shippo/models/components/ratemessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/ratepaginatedlist.py` & `shippo-3.1.0/src/shippo/models/components/ratepaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/refund.py` & `shippo-3.1.0/src/shippo/models/components/refund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/refundpaginatedlist.py` & `shippo-3.1.0/src/shippo/models/components/refundpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/refundrequestbody.py` & `shippo-3.1.0/src/shippo/models/components/refundrequestbody.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/rmanumber.py` & `shippo-3.1.0/src/shippo/models/components/rmanumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/servicegroup.py` & `shippo-3.1.0/src/shippo/models/components/servicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/servicegroupaccountandservicelevel.py` & `shippo-3.1.0/src/shippo/models/components/servicegroupaccountandservicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/servicegroupcreaterequest.py` & `shippo-3.1.0/src/shippo/models/components/servicegroupcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/servicegrouptype.py` & `shippo-3.1.0/src/shippo/models/components/servicegrouptype.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/servicegroupupdaterequest.py` & `shippo-3.1.0/src/shippo/models/components/servicegroupupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/servicelevel.py` & `shippo-3.1.0/src/shippo/models/components/servicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/servicelevelenumset.py` & `shippo-3.1.0/src/shippo/models/components/servicelevelenumset.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/shipment.py` & `shippo-3.1.0/src/shippo/models/components/shipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/shipmentcreaterequest.py` & `shippo-3.1.0/src/shippo/models/components/shipmentcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/shipmentextra.py` & `shippo-3.1.0/src/shippo/models/components/shipmentextra.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/shipmentpaginatedlist.py` & `shippo-3.1.0/src/shippo/models/components/shipmentpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/shippoaccount.py` & `shippo-3.1.0/src/shippo/models/components/shippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/shippoaccountpaginatedlist.py` & `shippo-3.1.0/src/shippo/models/components/shippoaccountpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/shippoaccountupdaterequest.py` & `shippo-3.1.0/src/shippo/models/components/shippoaccountupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/track.py` & `shippo-3.1.0/src/shippo/models/components/track.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/trackingstatus.py` & `shippo-3.1.0/src/shippo/models/components/trackingstatus.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,40 +1,31 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
+from .trackingstatusenum import TrackingStatusEnum
 from .trackingstatuslocationbase import TrackingStatusLocationBase
 from .trackingstatussubstatus import TrackingStatusSubstatus
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
-from enum import Enum
 from shippo import utils
 from typing import Optional
 
-class TrackingStatusStatus(str, Enum):
-    r"""Indicates the high level status of the shipment."""
-    UNKNOWN = 'UNKNOWN'
-    PRE_TRANSIT = 'PRE_TRANSIT'
-    TRANSIT = 'TRANSIT'
-    DELIVERED = 'DELIVERED'
-    RETURNED = 'RETURNED'
-    FAILURE = 'FAILURE'
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class TrackingStatus:
     r"""The latest tracking information of this shipment."""
     location: TrackingStatusLocationBase = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('location') }})
     r"""An object containing zip, city, state and country information of the tracking event."""
     object_created: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_created'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
     object_id: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_id') }})
     object_updated: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('object_updated'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
-    status: TrackingStatusStatus = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
+    status: TrackingStatusEnum = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status') }})
     r"""Indicates the high level status of the shipment."""
     status_date: datetime = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status_date'), 'encoder': utils.datetimeisoformat(False), 'decoder': dateutil.parser.isoparse }})
     r"""Date and time when the carrier scanned this tracking event. This is displayed in UTC."""
     status_details: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status_details') }})
     r"""The human-readable description of the status."""
     substatus: Optional[TrackingStatusSubstatus] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('substatus'), 'exclude': lambda f: f is None }})
     r"""A finer-grained classification of the tracking event."""
```

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/trackingstatuslocationbase.py` & `shippo-3.1.0/src/shippo/models/components/trackingstatuslocationbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/trackingstatussubstatus.py` & `shippo-3.1.0/src/shippo/models/components/trackingstatussubstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/tracksrequest.py` & `shippo-3.1.0/src/shippo/models/components/tracksrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/transaction.py` & `shippo-3.1.0/src/shippo/models/components/transaction.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,26 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
 from .labelfiletype import LabelFileType
 from .objectstate import ObjectState
+from .trackingstatusenum import TrackingStatusEnum
+from .transactionstatusenum import TransactionStatusEnum
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
-from enum import Enum
 from shippo import utils
 from typing import List, Optional
 
 
 @dataclasses.dataclass
 class TransactionMessages:
     pass
 
-class TransactionStatus(str, Enum):
-    r"""Indicates the status of the Transaction."""
-    WAITING = 'WAITING'
-    QUEUED = 'QUEUED'
-    SUCCESS = 'SUCCESS'
-    ERROR = 'ERROR'
-    REFUNDED = 'REFUNDED'
-    REFUNDPENDING = 'REFUNDPENDING'
-    REFUNDREJECTED = 'REFUNDREJECTED'
-
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class Transaction:
     commercial_invoice_url: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('commercial_invoice_url'), 'exclude': lambda f: f is None }})
     r"""A URL pointing to the commercial invoice as a 8.5x11 inch PDF file.
     A value will only be returned if the Transactions has been processed successfully and if the shipment is international.
@@ -67,23 +58,23 @@
     r"""A URL pointing directly to the QR code in PNG format.
     A value will only be returned if requested using qr_code_requested flag and the carrier provides such an option.
     """
     rate: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('rate'), 'exclude': lambda f: f is None }})
     r"""ID of the Rate object for which a Label has to be obtained.
     Please note that only rates that are not older than 7 days can be purchased in order to ensure up-to-date pricing.
     """
-    status: Optional[TransactionStatus] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
+    status: Optional[TransactionStatusEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('status'), 'exclude': lambda f: f is None }})
     r"""Indicates the status of the Transaction."""
     test: Optional[bool] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('test'), 'exclude': lambda f: f is None }})
     r"""Indicates whether the object has been created in test mode."""
     tracking_number: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tracking_number'), 'exclude': lambda f: f is None }})
     r"""The carrier-specific tracking number that can be used to track the Shipment.
     A value will only be returned if the Rate is for a trackable Shipment and if the Transactions has been processed successfully.
     """
-    tracking_status: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tracking_status'), 'exclude': lambda f: f is None }})
-    r"""Indicates the high level status of the shipment: `UNKNOWN`, `DELIVERED`, `TRANSIT`, `FAILURE`, `RETURNED`."""
+    tracking_status: Optional[TrackingStatusEnum] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tracking_status'), 'exclude': lambda f: f is None }})
+    r"""Indicates the high level status of the shipment."""
     tracking_url_provider: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tracking_url_provider'), 'exclude': lambda f: f is None }})
     r"""A link to track this item on the carrier-provided tracking website.
     A value will only be returned if tracking is available and the carrier provides such a service.
     """
```

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/transactioncreaterequest.py` & `shippo-3.1.0/src/shippo/models/components/transactioncreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/transactionpaginatedlist.py` & `shippo-3.1.0/src/shippo/models/components/transactionpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/upsconnectexistingownaccountparameters.py` & `shippo-3.1.0/src/shippo/models/components/upsconnectexistingownaccountparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/userparceltemplate.py` & `shippo-3.1.0/src/shippo/models/components/userparceltemplate.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 import dateutil.parser
 from .carrierparceltemplate import CarrierParcelTemplate
-from .distanceunitusertemplate import DistanceUnitUserTemplate
+from .distanceunit import DistanceUnit
 from .weightunit import WeightUnit
 from dataclasses_json import Undefined, dataclass_json
 from datetime import datetime
 from shippo import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class UserParcelTemplate:
-    distance_unit: Optional[DistanceUnitUserTemplate] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit'), 'exclude': lambda f: f is None }})
-    r"""The measure unit used for length, width and height. Required, but if using a preset carrier template then this field must be empty."""
+    distance_unit: Optional[DistanceUnit] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit'), 'exclude': lambda f: f is None }})
+    r"""The measure unit used for length, width and height."""
     height: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height'), 'exclude': lambda f: f is None }})
     r"""The height of the package, in units specified by the `distance_unit` attribute. Required, but if using a preset carrier template then this field must be empty."""
     length: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('length'), 'exclude': lambda f: f is None }})
     r"""The length of the package, in units specified by the `distance_unit` attribute. Required, but if using a preset carrier template then this field must be empty."""
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
     r"""The name of the User Parcel Template"""
     weight: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weight'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/userparceltemplateupdaterequest.py` & `shippo-3.1.0/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .distanceunitusertemplate import DistanceUnitUserTemplate
+from .distanceunit import DistanceUnit
 from .weightunit import WeightUnit
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class UserParcelTemplateUpdateRequest:
-    distance_unit: DistanceUnitUserTemplate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit') }})
-    r"""The measure unit used for length, width and height. Required, but if using a preset carrier template then this field must be empty."""
+class UserParcelTemplateWithoutCarrierTemplateCreateRequest:
+    distance_unit: DistanceUnit = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit') }})
+    r"""The measure unit used for length, width and height."""
     height: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height') }})
     r"""The height of the package, in units specified by the `distance_unit` attribute. Required, but if using a preset carrier template then this field must be empty."""
     length: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('length') }})
     r"""The length of the package, in units specified by the `distance_unit` attribute. Required, but if using a preset carrier template then this field must be empty."""
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
     r"""The name of the User Parcel Template"""
     width: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width') }})
```

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py` & `shippo-3.1.0/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py` & `shippo-3.1.0/src/shippo/models/components/userparceltemplateupdaterequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .distanceunitusertemplate import DistanceUnitUserTemplate
+from .distanceunit import DistanceUnit
 from .weightunit import WeightUnit
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
-class UserParcelTemplateWithoutCarrierTemplateCreateRequest:
-    distance_unit: DistanceUnitUserTemplate = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit') }})
-    r"""The measure unit used for length, width and height. Required, but if using a preset carrier template then this field must be empty."""
+class UserParcelTemplateUpdateRequest:
+    distance_unit: DistanceUnit = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('distance_unit') }})
+    r"""The measure unit used for length, width and height."""
     height: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height') }})
     r"""The height of the package, in units specified by the `distance_unit` attribute. Required, but if using a preset carrier template then this field must be empty."""
     length: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('length') }})
     r"""The length of the package, in units specified by the `distance_unit` attribute. Required, but if using a preset carrier template then this field must be empty."""
     name: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name') }})
     r"""The name of the User Parcel Template"""
     width: str = dataclasses.field(metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width') }})
```

### Comparing `shippo-3.0.0rc1/src/shippo/models/errors/badrequestwithdetail.py` & `shippo-3.1.0/src/shippo/models/errors/badrequestwithdetail.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/errors/badrequestwitherror.py` & `shippo-3.1.0/src/shippo/models/errors/badrequestwitherror.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/errors/sdkerror.py` & `shippo-3.1.0/src/shippo/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/__init__.py` & `shippo-3.1.0/src/shippo/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/addshipmentstobatch.py` & `shippo-3.1.0/src/shippo/models/operations/addshipmentstobatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/createaddress.py` & `shippo-3.1.0/src/shippo/models/operations/createaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/createbatch.py` & `shippo-3.1.0/src/shippo/models/operations/createbatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/createcarrieraccount.py` & `shippo-3.1.0/src/shippo/models/operations/createcarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/createcustomsdeclaration.py` & `shippo-3.1.0/src/shippo/models/operations/createcustomsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/createcustomsitem.py` & `shippo-3.1.0/src/shippo/models/operations/createcustomsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/createliverate.py` & `shippo-3.1.0/src/shippo/models/operations/createliverate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/createmanifest.py` & `shippo-3.1.0/src/shippo/models/operations/createmanifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/createorder.py` & `shippo-3.1.0/src/shippo/models/operations/createorder.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/createparcel.py` & `shippo-3.1.0/src/shippo/models/operations/createparcel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/createpickup.py` & `shippo-3.1.0/src/shippo/models/operations/createpickup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/createrefund.py` & `shippo-3.1.0/src/shippo/models/operations/createrefund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/createservicegroup.py` & `shippo-3.1.0/src/shippo/models/operations/createservicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/createshipment.py` & `shippo-3.1.0/src/shippo/models/operations/createshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/createshippoaccount.py` & `shippo-3.1.0/src/shippo/models/operations/createshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/createtrack.py` & `shippo-3.1.0/src/shippo/models/operations/createtrack.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/createtransaction.py` & `shippo-3.1.0/src/shippo/models/operations/createtransaction.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/createuserparceltemplate.py` & `shippo-3.1.0/src/shippo/models/operations/createuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/deletedefaultparceltemplate.py` & `shippo-3.1.0/src/shippo/models/operations/deletedefaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/deleteservicegroup.py` & `shippo-3.1.0/src/shippo/models/operations/deleteservicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/deleteuserparceltemplate.py` & `shippo-3.1.0/src/shippo/models/operations/deleteuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/getaddress.py` & `shippo-3.1.0/src/shippo/models/operations/getaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/getbatch.py` & `shippo-3.1.0/src/shippo/models/operations/getbatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/getcarrieraccount.py` & `shippo-3.1.0/src/shippo/models/operations/getcarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/getcarrierparceltemplate.py` & `shippo-3.1.0/src/shippo/models/operations/getcarrierparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/getcarrierregistrationstatus.py` & `shippo-3.1.0/src/shippo/models/operations/getcarrierregistrationstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/getcustomsdeclaration.py` & `shippo-3.1.0/src/shippo/models/operations/getcustomsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/getcustomsitem.py` & `shippo-3.1.0/src/shippo/models/operations/getcustomsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/getmanifest.py` & `shippo-3.1.0/src/shippo/models/operations/getmanifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/getorder.py` & `shippo-3.1.0/src/shippo/models/operations/getorder.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/getparcel.py` & `shippo-3.1.0/src/shippo/models/operations/getparcel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/getrate.py` & `shippo-3.1.0/src/shippo/models/operations/getrate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/getrefund.py` & `shippo-3.1.0/src/shippo/models/operations/getrefund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/getshipment.py` & `shippo-3.1.0/src/shippo/models/operations/getshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/getshippoaccount.py` & `shippo-3.1.0/src/shippo/models/operations/getshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/gettrack.py` & `shippo-3.1.0/src/shippo/models/operations/gettrack.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/gettransaction.py` & `shippo-3.1.0/src/shippo/models/operations/gettransaction.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/getuserparceltemplate.py` & `shippo-3.1.0/src/shippo/models/operations/getuserparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/listaddresses.py` & `shippo-3.1.0/src/shippo/models/operations/listaddresses.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/listcarrieraccounts.py` & `shippo-3.1.0/src/shippo/models/operations/listcarrieraccounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/listcarrierparceltemplates.py` & `shippo-3.1.0/src/shippo/models/operations/listcarrierparceltemplates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/listcustomsdeclarations.py` & `shippo-3.1.0/src/shippo/models/operations/listcustomsdeclarations.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/listcustomsitems.py` & `shippo-3.1.0/src/shippo/models/operations/listcustomsitems.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/listmanifests.py` & `shippo-3.1.0/src/shippo/models/operations/listmanifests.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/listorders.py` & `shippo-3.1.0/src/shippo/models/operations/listorders.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/listparcels.py` & `shippo-3.1.0/src/shippo/models/operations/listparcels.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/listshipmentrates.py` & `shippo-3.1.0/src/shippo/models/operations/listshipmentrates.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/listshipmentratesbycurrencycode.py` & `shippo-3.1.0/src/shippo/models/operations/listshipmentratesbycurrencycode.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/listshipments.py` & `shippo-3.1.0/src/shippo/models/operations/listshipments.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/listshippoaccounts.py` & `shippo-3.1.0/src/shippo/models/operations/listshippoaccounts.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/listtransactions.py` & `shippo-3.1.0/src/shippo/models/operations/removeshipmentsfrombatch.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from typing import Optional
+from typing import List, Optional
 
 
 @dataclasses.dataclass
-class ListTransactionsRequest:
-    page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
-    r"""The page number you want to select"""
-    results: Optional[int] = dataclasses.field(default=25, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
-    r"""The number of results to return per page (max 100)"""
+class RemoveShipmentsFromBatchRequest:
+    batch_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'BatchId', 'style': 'simple', 'explode': False }})
+    r"""Object ID of the batch"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
+    request_body: Optional[List[str]] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    r"""Array of shipments object ids to remove from the batch"""
```

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/purchasebatch.py` & `shippo-3.1.0/src/shippo/models/operations/purchasebatch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/registercarrieraccount.py` & `shippo-3.1.0/src/shippo/models/operations/registercarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/removeshipmentsfrombatch.py` & `shippo-3.1.0/src/shippo/models/operations/updateuserparceltemplate.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from typing import List, Optional
+from ...models.components import userparceltemplateupdaterequest as components_userparceltemplateupdaterequest
+from typing import Optional
 
 
 @dataclasses.dataclass
-class RemoveShipmentsFromBatchRequest:
-    batch_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'BatchId', 'style': 'simple', 'explode': False }})
-    r"""Object ID of the batch"""
+class UpdateUserParcelTemplateRequest:
+    user_parcel_template_object_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'UserParcelTemplateObjectId', 'style': 'simple', 'explode': False }})
+    r"""Object ID of the user parcel template"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
-    request_body: Optional[List[str]] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
-    r"""Array of shipments object ids to remove from the batch"""
+    user_parcel_template_update_request: Optional[components_userparceltemplateupdaterequest.UserParcelTemplateUpdateRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
```

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/updatecarrieraccount.py` & `shippo-3.1.0/src/shippo/models/operations/updatecarrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/updatedefaultparceltemplate.py` & `shippo-3.1.0/src/shippo/models/operations/updatedefaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/updateservicegroup.py` & `shippo-3.1.0/src/shippo/models/operations/updateservicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/updateshippoaccount.py` & `shippo-3.1.0/src/shippo/models/operations/updateshippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/models/operations/validateaddress.py` & `shippo-3.1.0/src/shippo/models/operations/validateaddress.py`

 * *Files identical despite different names*

### Comparing `shippo-3.0.0rc1/src/shippo/orders.py` & `shippo-3.1.0/src/shippo/orders.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
-from shippo._hooks import HookContext
+from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import Optional
 
 class Orders:
     r"""An order is a request from a customer to purchase goods from a merchant.
     Use the orders object to load orders from your system to the Shippo dashboard.
     You can use the orders object to create, retrieve, list, and manage orders programmatically. 
@@ -52,37 +52,36 @@
         headers = { **utils.get_headers(request), **headers }
         query_params = { **utils.get_query_params(operations.ListOrdersRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.OrderPaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -115,37 +114,36 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 201:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Order])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -175,37 +173,36 @@
         
         headers = { **utils.get_headers(request), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Order])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
```

### Comparing `shippo-3.0.0rc1/src/shippo/parcels.py` & `shippo-3.1.0/src/shippo/parcels.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
-from shippo._hooks import HookContext
+from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import Optional
 
 class Parcels:
     r"""A parcel is an item you are shipping. The parcel object includes details about its physical make-up of the parcel. It includes dimensions and weight that Shippo uses to calculate rates.
     <SchemaDefinition schemaRef=\"#/components/schemas/Parcel\"/>
 
@@ -45,37 +45,36 @@
         headers = { **utils.get_headers(request), **headers }
         query_params = { **utils.get_query_params(operations.ListParcelsRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.ParcelPaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -108,37 +107,36 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 201:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Parcel])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -168,37 +166,36 @@
         
         headers = { **utils.get_headers(request), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Parcel])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
```

### Comparing `shippo-3.0.0rc1/src/shippo/pickups.py` & `shippo-3.1.0/src/shippo/pickups.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
-from shippo._hooks import HookContext
+from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import Optional
 
 class Pickups:
     r"""A pickup is when you schedule a carrier to collect a package for delivery.
     Use Shippo’s pickups endpoint to schedule pickups with USPS and DHL Express for eligible shipments that you have already created.
     <SchemaDefinition schemaRef=\"#/components/schemas/Pickup\"/>
@@ -43,37 +43,36 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 201:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Pickup])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
```

### Comparing `shippo-3.0.0rc1/src/shippo/rates.py` & `shippo-3.1.0/src/shippo/rates.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
-from shippo._hooks import HookContext
+from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import Optional
 
 class Rates:
     r"""A rate is the cost to ship a parcel from a carrier. The rate object details the service level including the cost and transit time.
     <SchemaDefinition schemaRef=\"#/components/schemas/Rate\"/>
     """
@@ -39,37 +39,36 @@
         
         headers = { **utils.get_headers(request), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Rate])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -102,37 +101,36 @@
         headers = { **utils.get_headers(request), **headers }
         query_params = { **utils.get_query_params(operations.ListShipmentRatesRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.RatePaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -164,37 +162,36 @@
         headers = { **utils.get_headers(request), **headers }
         query_params = { **utils.get_query_params(operations.ListShipmentRatesByCurrencyCodeRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.RatePaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
```

### Comparing `shippo-3.0.0rc1/src/shippo/rates_at_checkout.py` & `shippo-3.1.0/src/shippo/rates_at_checkout.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
-from shippo._hooks import HookContext
+from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import Optional
 
 class RatesAtCheckout:
     r"""Rates at checkout is a tool for merchants to display up-to-date shipping estimates based on what's in their customers cart and where they’re shipping to.
     Merchants set up curated shipping options for customers in the checkout flow based on data in the shopping cart. The request must include the **to** address and item information. Optional fields are the **from** address and package information. If the optional fields are not included, the service will use the default address and/or package configured for rates at checkout. The response is a list of shipping options based on the Service Group configuration.
     (see <a href=\"#tag/Service-Groups\">Service Group configuration</a> for details).
@@ -52,37 +52,36 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.LiveRatePaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -111,37 +110,36 @@
         
         headers = { **utils.get_headers(request), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.DefaultParcelTemplate])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -174,37 +172,36 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.DefaultParcelTemplate])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -233,32 +230,31 @@
         
         headers = { **utils.get_headers(request), **headers }
         headers['Accept'] = '*/*'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('DELETE', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         res = operations.DeleteDefaultParcelTemplateResponse()
         
         if http_res.status_code == 204:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `shippo-3.0.0rc1/src/shippo/refunds.py` & `shippo-3.1.0/src/shippo/tracking_status.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,201 +1,164 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
-from shippo._hooks import HookContext
+from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import Optional
 
-class Refunds:
-    r"""Refunds are reimbursements for successfully created but unused shipping labels or other charges.
-    <SchemaDefinition schemaRef=\"#/components/schemas/Refund\"/>
+class TrackingStatus:
+    r"""<p style=\\"text-align: center; background-color: #F2F3F4;\\"></br>
+    If you purchased your shipping label through Shippo, you can also get all the tracking details of your Shipment 
+    from the <a href=\"#tag/Transactions\">Transaction</a> object.
+    </br></br></p>
+    A tracking status of a package is an indication of current location of a package in the supply chain. For example,  sorting, warehousing, or out for delivery. Use the tracking status object to track the location of your shipments.
+
+    When using your <a href=\"https://docs.goshippo.com/docs/guides_general/authentication/\">Test</a> token for tracking, you need to use Shippo's 
+    predefined tokens for testing different tracking statuses. You can find more information in our 
+    <a href=\"https://docs.goshippo.com/docs/tracking/tracking/\">Tracking tutorial</a> on how to do this, and what the 
+    payloads look like.      
+    <SchemaDefinition schemaRef=\"#/components/schemas/Track\"/>
     """
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create(self, shippo_api_version: Optional[str] = None, refund_request_body: Optional[components.RefundRequestBody] = None) -> components.Refund:
-        r"""Create a refund
-        Creates a new refund object.
+    def create(self, shippo_api_version: Optional[str] = None, tracks_request: Optional[components.TracksRequest] = None) -> components.Track:
+        r"""Register a tracking webhook
+        Registers a webhook that will send HTTP notifications to you when the status of your tracked package changes. For more details on creating a webhook, see our guides on <a href=\"https://docs.goshippo.com/docs/tracking/webhooks/\">Webhooks</a> and <a href=\"https://docs.goshippo.com/docs/tracking/tracking/\">Tracking</a>.
         """
-        hook_ctx = HookContext(operation_id='CreateRefund', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.CreateRefundRequest(
+        hook_ctx = HookContext(operation_id='CreateTrack', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.CreateTrackRequest(
             shippo_api_version=shippo_api_version,
-            refund_request_body=refund_request_body,
+            tracks_request=tracks_request,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/refunds'
+        url = base_url + '/tracks'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateRefundRequest, "refund_request_body", False, True, 'json')
+        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateTrackRequest, "tracks_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
-        if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+        if utils.match_status_codes(['400','4XX','5XX'], http_res.status_code):
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 201:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.Refund])
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[components.Track])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
-        else:
-            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
-
-    
-    
-    def list(self, shippo_api_version: Optional[str] = None) -> components.RefundPaginatedList:
-        r"""List all refunds
-        Returns a list all refund objects.
-        """
-        hook_ctx = HookContext(operation_id='ListRefunds', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.ListRefundsRequest(
-            shippo_api_version=shippo_api_version,
-        )
-        
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
-        
-        url = base_url + '/refunds/'
-        
-        if callable(self.sdk_configuration.security):
-            headers, query_params = utils.get_security(self.sdk_configuration.security())
-        else:
-            headers, query_params = utils.get_security(self.sdk_configuration.security)
-        
-        headers = { **utils.get_headers(request), **headers }
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
-        client = self.sdk_configuration.client
-        
-        try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
-            http_res = client.send(req)
-        except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
-
-        if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
-                raise e
-        else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
-        
-        
-        
-        if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.RefundPaginatedList])
-                return out
+        elif http_res.status_code == 400:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.BadRequestWithDetail)
+                raise out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def get(self, refund_id: str, shippo_api_version: Optional[str] = None) -> components.Refund:
-        r"""Retrieve a refund
-        Returns an existing rate using a rate object ID.
+    def get(self, tracking_number: str, carrier: str, shippo_api_version: Optional[str] = None) -> components.Track:
+        r"""Get a tracking status
+        Returns the tracking status of a shipment using a carrier name and a tracking number.
         """
-        hook_ctx = HookContext(operation_id='GetRefund', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.GetRefundRequest(
-            refund_id=refund_id,
+        hook_ctx = HookContext(operation_id='GetTrack', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.GetTrackRequest(
+            tracking_number=tracking_number,
+            carrier=carrier,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetRefundRequest, base_url, '/refunds/{RefundId}', request)
+        url = utils.generate_url(operations.GetTrackRequest, base_url, '/tracks/{Carrier}/{TrackingNumber}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
-        if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+        if utils.match_status_codes(['400','4XX','5XX'], http_res.status_code):
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.Refund])
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[components.Track])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code == 400:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.BadRequestWithDetail)
+                raise out
+            
+            content_type = http_res.headers.get('Content-Type')
+            raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
```

### Comparing `shippo-3.0.0rc1/src/shippo/sdk.py` & `shippo-3.1.0/src/shippo/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from .sdkconfiguration import SDKConfiguration
 from .service_groups import ServiceGroups
 from .shipments import Shipments
 from .shippo_accounts import ShippoAccounts
 from .tracking_status import TrackingStatus
 from .transactions import Transactions
 from .user_parcel_templates import UserParcelTemplates
+from .utils.retries import RetryConfig
 from shippo import utils
 from shippo._hooks import SDKHooks
 from shippo.models import components
 from typing import Callable, Dict, Optional, Union
 
 class Shippo:
     r"""Shippo external API.: Use this API to integrate with the Shippo service"""
@@ -170,30 +171,30 @@
 
     def __init__(self,
                  api_key_header: Union[str, Callable[[], str]],
                  server_idx: Optional[int] = None,
                  server_url: Optional[str] = None,
                  url_params: Optional[Dict[str, str]] = None,
                  client: Optional[requests_http.Session] = None,
-                 retry_config: Optional[utils.RetryConfig] = None
+                 retry_config: Optional[RetryConfig] = None
                  ) -> None:
         """Instantiates the SDK configuring it with the provided parameters.
 
         :param api_key_header: The api_key_header required for authentication
         :type api_key_header: Union[str, Callable[[], str]]
         :param server_idx: The index of the server to use for all operations
         :type server_idx: int
         :param server_url: The server URL to use for all operations
         :type server_url: str
         :param url_params: Parameters to optionally template the server URL with
         :type url_params: Dict[str, str]
         :param client: The requests.Session HTTP client to use for all operations
         :type client: requests_http.Session
         :param retry_config: The utils.RetryConfig to use globally
-        :type retry_config: utils.RetryConfig
+        :type retry_config: RetryConfig
         """
         if client is None:
             client = requests_http.Session()
 
         if callable(api_key_header):
             def security():
                 return components.Security(api_key_header = api_key_header())
```

### Comparing `shippo-3.0.0rc1/src/shippo/sdkconfiguration.py` & `shippo-3.1.0/src/shippo/sdkconfiguration.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,38 +3,38 @@
 
 import requests as requests_http
 from ._hooks import SDKHooks
 from .utils import utils
 from .utils.retries import RetryConfig
 from dataclasses import dataclass
 from shippo.models import components
-from typing import Callable, Dict, Tuple, Union
+from typing import Callable, Dict, Optional, Tuple, Union
 
 
 SERVERS = [
     'https://api.goshippo.com',
 ]
 """Contains the list of servers available to the SDK"""
 
 @dataclass
 class SDKConfiguration:
     client: requests_http.Session
     security: Union[components.Security,Callable[[], components.Security]] = None
-    server_url: str = ''
-    server_idx: int = 0
+    server_url: Optional[str] = ''
+    server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = '2018-02-08'
-    sdk_version: str = '3.0.0rc1'
-    gen_version: str = '2.286.7'
-    user_agent: str = 'speakeasy-sdk/python 3.0.0rc1 2.286.7 2018-02-08 shippo'
-    retry_config: RetryConfig = None
-    _hooks: SDKHooks = None
+    sdk_version: str = '3.1.0'
+    gen_version: str = '2.298.0'
+    user_agent: str = 'speakeasy-sdk/python 3.1.0 2.298.0 2018-02-08 shippo'
+    retry_config: Optional[RetryConfig] = None
+    _hooks: Optional[SDKHooks] = None
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
-        if self.server_url:
+        if self.server_url is not None and self.server_url != '':
             return utils.remove_suffix(self.server_url, '/'), {}
         if self.server_idx is None:
             self.server_idx = 0
 
         return SERVERS[self.server_idx], {}
```

### Comparing `shippo-3.0.0rc1/src/shippo/service_groups.py` & `shippo-3.1.0/src/shippo/service_groups.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
-from shippo._hooks import HookContext
+from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import List, Optional
 
 class ServiceGroups:
     r"""A service group is a set of service levels grouped together.
     Rates at checkout uses services groups to present available shipping options to customers in their shopping basket.
     <SchemaDefinition schemaRef=\"#/components/schemas/ServiceGroup\"/>
@@ -39,37 +39,36 @@
         
         headers = { **utils.get_headers(request), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[components.ServiceGroup]])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -102,37 +101,36 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 201:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.ServiceGroup])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -165,37 +163,36 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.ServiceGroup])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -225,32 +222,31 @@
         
         headers = { **utils.get_headers(request), **headers }
         headers['Accept'] = '*/*'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('DELETE', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         res = operations.DeleteServiceGroupResponse()
         
         if http_res.status_code == 204:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
```

### Comparing `shippo-3.0.0rc1/src/shippo/shipments.py` & `shippo-3.1.0/src/shippo/shipments.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
-from shippo._hooks import HookContext
+from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import Optional
 
 class Shipments:
     r"""A shipment is the act of transporting goods. A shipment object contains **to** and **from** addresses, and the parcel details that you are shipping. You can use the shipment object to retrieve shipping rates and purchase a shipping label.
     <SchemaDefinition schemaRef=\"#/components/schemas/Shipment\"/>
 
@@ -62,37 +62,36 @@
         headers = { **utils.get_headers(request), **headers }
         query_params = { **utils.get_query_params(operations.ListShipmentsRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.ShipmentPaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -125,37 +124,36 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 201:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Shipment])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -185,37 +183,36 @@
         
         headers = { **utils.get_headers(request), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Shipment])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
```

### Comparing `shippo-3.0.0rc1/src/shippo/shippo_accounts.py` & `shippo-3.1.0/src/shippo/shippo_accounts.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
-from shippo._hooks import HookContext
+from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import Optional
 
 class ShippoAccounts:
     r"""Shippo Accounts are used by Shippo Platform Accounts to create and manage Managed Shippo Accounts.
     Managed Shippo Accounts are headless accounts that represent your customers. They are opaque to your end customers, meaning customers do not need to create their own Shippo login or have a billing relationship with Shippo. 
     They can be used by marketplaces, e-commerce platforms, and third-party logistics providers who want to offer, seamless, built-in shipping functionality to their customers. 
@@ -43,37 +43,36 @@
         headers = { **utils.get_headers(request), **headers }
         query_params = { **utils.get_query_params(operations.ListShippoAccountsRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.ShippoAccountPaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -106,37 +105,36 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.ShippoAccount])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -166,37 +164,36 @@
         
         headers = { **utils.get_headers(request), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.ShippoAccount])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -230,37 +227,36 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.ShippoAccount])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
```

### Comparing `shippo-3.0.0rc1/src/shippo/tracking_status.py` & `shippo-3.1.0/src/shippo/customs_declarations.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,166 +1,204 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
-from shippo._hooks import HookContext
+from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import Optional
 
-class TrackingStatus:
-    r"""<p style=\\"text-align: center; background-color: #F2F3F4;\\"></br>
-    If you purchased your shipping label through Shippo, you can also get all the tracking details of your Shipment 
-    from the <a href=\"#tag/Transactions\">Transaction</a> object.
-    </br></br></p>
-    A tracking status of a package is an indication of current location of a package in the supply chain. For example,  sorting, warehousing, or out for delivery. Use the tracking status object to track the location of your shipments.
-
-    When using your <a href=\"https://docs.goshippo.com/docs/guides_general/authentication/\">Test</a> token for tracking, you need to use Shippo's 
-    predefined tokens for testing different tracking statuses. You can find more information in our 
-    <a href=\"https://docs.goshippo.com/docs/tracking/tracking/\">Tracking tutorial</a> on how to do this, and what the 
-    payloads look like.      
-    <SchemaDefinition schemaRef=\"#/components/schemas/Track\"/>
+class CustomsDeclarations:
+    r"""Customs declarations are relevant information, including one or multiple customs items, you need to provide for
+    customs clearance for your international shipments.
+    <SchemaDefinition schemaRef=\"#/components/schemas/CustomsDeclaration\"/>
     """
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create(self, shippo_api_version: Optional[str] = None, tracks_request: Optional[components.TracksRequest] = None) -> components.Track:
-        r"""Register a tracking webhook
-        Registers a webhook that will send HTTP notifications to you when the status of your tracked package changes. For more details on creating a webhook, see our guides on <a href=\"https://docs.goshippo.com/docs/tracking/webhooks/\">Webhooks</a> and <a href=\"https://docs.goshippo.com/docs/tracking/tracking/\">Tracking</a>.
+    def list(self, page: Optional[int] = None, results: Optional[int] = None, shippo_api_version: Optional[str] = None) -> components.CustomsDeclarationPaginatedList:
+        r"""List all customs declarations
+        Returns a a list of all customs declaration objects
         """
-        hook_ctx = HookContext(operation_id='CreateTrack', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.CreateTrackRequest(
+        hook_ctx = HookContext(operation_id='ListCustomsDeclarations', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.ListCustomsDeclarationsRequest(
+            page=page,
+            results=results,
             shippo_api_version=shippo_api_version,
-            tracks_request=tracks_request,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/tracks'
+        url = base_url + '/customs/declarations'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateTrackRequest, "tracks_request", False, True, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(operations.ListCustomsDeclarationsRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
-        if utils.match_status_codes(['400','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+        if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
-        if http_res.status_code == 201:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.Track])
+        if http_res.status_code == 200:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[components.CustomsDeclarationPaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 400:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequestWithDetail)
-                raise out
+        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
+            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
+
+    
+    
+    def create(self, shippo_api_version: Optional[str] = None, customs_declaration_create_request: Optional[components.CustomsDeclarationCreateRequest] = None) -> components.CustomsDeclaration:
+        r"""Create a new customs declaration
+        Creates a new customs declaration object
+        """
+        hook_ctx = HookContext(operation_id='CreateCustomsDeclaration', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.CreateCustomsDeclarationRequest(
+            shippo_api_version=shippo_api_version,
+            customs_declaration_create_request=customs_declaration_create_request,
+        )
+        
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        
+        url = base_url + '/customs/declarations'
+        
+        if callable(self.sdk_configuration.security):
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
+        else:
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
+        
+        headers = { **utils.get_headers(request), **headers }
+        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCustomsDeclarationRequest, "customs_declaration_create_request", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
+        
+        try:
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            http_res = client.send(req)
+        except Exception as e:
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
+
+        if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
+                raise e
+            if result is not None:
+                http_res = result
+        else:
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
+        
+        
+        
+        if http_res.status_code == 201:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[components.CustomsDeclaration])
+                return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def get(self, tracking_number: str, carrier: str, shippo_api_version: Optional[str] = None) -> components.Track:
-        r"""Get a tracking status
-        Returns the tracking status of a shipment using a carrier name and a tracking number.
+    def get(self, customs_declaration_id: str, page: Optional[int] = None, shippo_api_version: Optional[str] = None) -> components.CustomsDeclaration:
+        r"""Retrieve a customs declaration
+        Returns an existing customs declaration using an object ID
         """
-        hook_ctx = HookContext(operation_id='GetTrack', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.GetTrackRequest(
-            tracking_number=tracking_number,
-            carrier=carrier,
+        hook_ctx = HookContext(operation_id='GetCustomsDeclaration', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.GetCustomsDeclarationRequest(
+            customs_declaration_id=customs_declaration_id,
+            page=page,
             shippo_api_version=shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetTrackRequest, base_url, '/tracks/{Carrier}/{TrackingNumber}', request)
+        url = utils.generate_url(operations.GetCustomsDeclarationRequest, base_url, '/customs/declarations/{CustomsDeclarationId}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers = { **utils.get_headers(request), **headers }
+        query_params = { **utils.get_query_params(operations.GetCustomsDeclarationRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
-        if utils.match_status_codes(['400','4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+        if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.Track])
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[components.CustomsDeclaration])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code == 400:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, errors.BadRequestWithDetail)
-                raise out
-            
-            content_type = http_res.headers.get('Content-Type')
-            raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
```

### Comparing `shippo-3.0.0rc1/src/shippo/transactions.py` & `shippo-3.1.0/src/shippo/transactions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
-from shippo._hooks import HookContext
+from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import Optional, Union
 
 class Transactions:
     r"""A transaction is the purchase of a shipping label from a shipping provider for a specific service. You can print purchased labels and used them to ship a parcel with a carrier, such as USPS or FedEx.
     <SchemaDefinition schemaRef=\"#/components/schemas/Transaction\"/>
     """
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def list(self, page: Optional[int] = None, results: Optional[int] = None, shippo_api_version: Optional[str] = None) -> components.TransactionPaginatedList:
+    def list(self, request: operations.ListTransactionsRequest) -> components.TransactionPaginatedList:
         r"""List all shipping labels
         Returns a list of all transaction objects.
         """
         hook_ctx = HookContext(operation_id='ListTransactions', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.ListTransactionsRequest(
-            page=page,
-            results=results,
-            shippo_api_version=shippo_api_version,
-        )
-        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
         url = base_url + '/transactions'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
@@ -41,37 +35,36 @@
         headers = { **utils.get_headers(request), **headers }
         query_params = { **utils.get_query_params(operations.ListTransactionsRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.TransactionPaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -104,37 +97,36 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 201:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Transaction])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -164,37 +156,36 @@
         
         headers = { **utils.get_headers(request), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.Transaction])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
```

### Comparing `shippo-3.0.0rc1/src/shippo/user_parcel_templates.py` & `shippo-3.1.0/src/shippo/user_parcel_templates.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
-from shippo._hooks import HookContext
+from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import List, Optional, Union
 
 class UserParcelTemplates:
     r"""A user parcel template represents a package used for shipping that has preset dimensions and attributes defined
     by you. They are useful for capturing attributes of parcel-types you frequently use for shipping, allowing 
     them to be defined once and then used for many shipments. These parcel templates can also be used for live rates.
@@ -43,37 +43,36 @@
         
         headers = { **utils.get_headers(request), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[List[components.UserParcelTemplate]])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -112,37 +111,36 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.UserParcelTemplate])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -172,32 +170,31 @@
         
         headers = { **utils.get_headers(request), **headers }
         headers['Accept'] = '*/*'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('DELETE', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         res = operations.DeleteUserParcelTemplateResponse()
         
         if http_res.status_code == 204:
             pass
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
@@ -231,37 +228,36 @@
         
         headers = { **utils.get_headers(request), **headers }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.UserParcelTemplate])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -295,37 +291,36 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[components.UserParcelTemplate])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
```

### Comparing `shippo-3.0.0rc1/src/shippo/utils/retries.py` & `shippo-3.1.0/src/shippo/utils/retries.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,20 +71,20 @@
                             raise TemporaryError(res)
                     else:
                         parsed_code = int(code)
 
                         if res.status_code == parsed_code:
                             raise TemporaryError(res)
             except requests.exceptions.ConnectionError as exception:
-                if retries.config.config.retry_connection_errors:
+                if retries.config.retry_connection_errors:
                     raise
 
                 raise PermanentError(exception) from exception
             except requests.exceptions.Timeout as exception:
-                if retries.config.config.retry_connection_errors:
+                if retries.config.retry_connection_errors:
                     raise
 
                 raise PermanentError(exception) from exception
             except TemporaryError:
                 raise
             except Exception as exception:
                 raise PermanentError(exception) from exception
```

### Comparing `shippo-3.0.0rc1/src/shippo/utils/utils.py` & `shippo-3.1.0/src/shippo/utils/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -268,28 +268,28 @@
                 params = {**params, **_get_delimited_query_params(
                     metadata, f_name, value, "|")}
             else:
                 raise Exception('not yet implemented')
     return params
 
 
-def get_headers(headers_params: Any) -> Dict[str, str]:
+def get_headers(headers_params: Any, gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]] = None) -> Dict[str, str]:
     if headers_params is None:
         return {}
 
     headers: Dict[str, str] = {}
 
     param_fields: Tuple[Field, ...] = fields(headers_params)
     for field in param_fields:
         metadata = field.metadata.get('header')
         if not metadata:
             continue
 
-        value = _serialize_header(metadata.get(
-            'explode', False), getattr(headers_params, field.name))
+        value = _populate_from_globals(field.name, getattr(headers_params, field.name), 'header', gbls)
+        value = _serialize_header(metadata.get('explode', False), value)
 
         if value != '':
             headers[metadata.get('field_name', field.name)] = value
 
     return headers
```

### Comparing `shippo-3.0.0rc1/src/shippo.egg-info/PKG-INFO` & `shippo-3.1.0/src/shippo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: shippo
-Version: 3.0.0rc1
+Version: 3.1.0
 Summary: Python Client SDK Generated by Speakeasy
-Home-page: UNKNOWN
+Home-page: https://github.com/goshippo/shippo-python-sdk.git
 Author: Shippo
 License: UNKNOWN
 Description: # <img src="https://docs.goshippo.com/images/Logo.png" width="30" alt="Shippo logo"> Shippo Python SDK 
         
         Shippo is a shipping API that connects you with [multiple shipping carriers](https://goshippo.com/carriers) (such as USPS, UPS, DHL, Canada Post, Australia Post, and many others) through one interface.
         
         You must register for a [Shippo account](https://apps.goshippo.com/join) to use our API. It's free to sign up. Only pay to print a live label, test labels are free.
@@ -65,15 +65,15 @@
         For example, you could specify a header for every request that this sdk makes as follows:
         ```python
         import shippo
         import requests
         
         http_client = requests.Session()
         http_client.headers.update({'x-custom-header': 'someValue'})
-        s = shippo.Shippo(client: http_client)
+        s = shippo.Shippo(client=http_client)
         ```
         <!-- End Custom HTTP Client [http-client] -->
         
         ## Documentation
         Review our full guides and references at [https://docs.goshippo.com/](https://docs.goshippo.com/).
         
         <!-- Start Available Resources and Operations [operations] -->
```

### Comparing `shippo-3.0.0rc1/src/shippo.egg-info/SOURCES.txt` & `shippo-3.1.0/src/shippo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -84,16 +84,14 @@
 src/shippo/models/components/dangerousgoodsbiologicalmaterial.py
 src/shippo/models/components/dangerousgoodslithiumbatteries.py
 src/shippo/models/components/dangerousgoodsobject.py
 src/shippo/models/components/defaultparceltemplate.py
 src/shippo/models/components/defaultparceltemplateupdaterequest.py
 src/shippo/models/components/departmentnumber.py
 src/shippo/models/components/distanceunit.py
-src/shippo/models/components/distanceunittemplate.py
-src/shippo/models/components/distanceunitusertemplate.py
 src/shippo/models/components/dryice.py
 src/shippo/models/components/errormessage.py
 src/shippo/models/components/instanttransactionrequestbody.py
 src/shippo/models/components/insurance.py
 src/shippo/models/components/invoicenumber.py
 src/shippo/models/components/labelfiletype.py
 src/shippo/models/components/lineitem.py
@@ -139,20 +137,22 @@
 src/shippo/models/components/shipmentextra.py
 src/shippo/models/components/shipmentpaginatedlist.py
 src/shippo/models/components/shippoaccount.py
 src/shippo/models/components/shippoaccountpaginatedlist.py
 src/shippo/models/components/shippoaccountupdaterequest.py
 src/shippo/models/components/track.py
 src/shippo/models/components/trackingstatus.py
+src/shippo/models/components/trackingstatusenum.py
 src/shippo/models/components/trackingstatuslocationbase.py
 src/shippo/models/components/trackingstatussubstatus.py
 src/shippo/models/components/tracksrequest.py
 src/shippo/models/components/transaction.py
 src/shippo/models/components/transactioncreaterequest.py
 src/shippo/models/components/transactionpaginatedlist.py
+src/shippo/models/components/transactionstatusenum.py
 src/shippo/models/components/upsconnectexistingownaccountparameters.py
 src/shippo/models/components/userparceltemplate.py
 src/shippo/models/components/userparceltemplateupdaterequest.py
 src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
 src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
 src/shippo/models/components/weightunit.py
 src/shippo/models/errors/__init__.py
```

