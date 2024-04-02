# Comparing `tmp/edumfa-1.4.0.tar.gz` & `tmp/edumfa-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edumfa-1.4.0.tar", last modified: Tue Mar 19 17:58:26 2024, max compression
+gzip compressed data, was "edumfa-1.5.0.tar", last modified: Tue Apr  2 12:57:52 2024, max compression
```

## Comparing `edumfa-1.4.0.tar` & `edumfa-1.5.0.tar`

### file list

```diff
@@ -1,944 +1,989 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.329602 edumfa-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-03-19 17:58:21.000000 edumfa-1.4.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (127)    32387 2024-03-19 17:58:21.000000 edumfa-1.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      315 2024-03-19 17:58:21.000000 edumfa-1.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-03-19 17:58:26.329602 edumfa-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-03-19 17:58:21.000000 edumfa-1.4.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.165599 edumfa-1.4.0/deploy/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-19 17:58:21.000000 edumfa-1.4.0/deploy/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.165599 edumfa-1.4.0/deploy/apache/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-19 17:58:21.000000 edumfa-1.4.0/deploy/apache/edumfaapp.wsgi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.165599 edumfa-1.4.0/deploy/apache/sites-available/
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-03-19 17:58:21.000000 edumfa-1.4.0/deploy/apache/sites-available/edumfa.conf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.165599 edumfa-1.4.0/deploy/crontab/
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-19 17:58:21.000000 edumfa-1.4.0/deploy/crontab/edumfa
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-03-19 17:58:21.000000 edumfa-1.4.0/deploy/docker-compose-example.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.165599 edumfa-1.4.0/deploy/docker-example/
--rw-r--r--   0 runner    (1001) docker     (127)     6420 2024-03-19 17:58:21.000000 edumfa-1.4.0/deploy/docker-example/edumfa-policy.conf
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-19 17:58:21.000000 edumfa-1.4.0/deploy/docker-example/edumfa-setup.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-03-19 17:58:21.000000 edumfa-1.4.0/deploy/docker-example/edumfa.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)      726 2024-03-19 17:58:21.000000 edumfa-1.4.0/deploy/docker-setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.165599 edumfa-1.4.0/deploy/edumfa/
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-03-19 17:58:21.000000 edumfa-1.4.0/deploy/edumfa/dictionary
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.165599 edumfa-1.4.0/deploy/gunicorn/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-19 17:58:21.000000 edumfa-1.4.0/deploy/gunicorn/edumfaapp.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-19 17:58:21.000000 edumfa-1.4.0/deploy/logging.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.165599 edumfa-1.4.0/deploy/nginx/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-19 17:58:21.000000 edumfa-1.4.0/deploy/nginx/edumfaapp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.165599 edumfa-1.4.0/deploy/nginx/sites-available/
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-03-19 17:58:21.000000 edumfa-1.4.0/deploy/nginx/sites-available/edumfa
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.165599 edumfa-1.4.0/deploy/privacyidea/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-19 17:58:21.000000 edumfa-1.4.0/deploy/privacyidea/enckey
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.145599 edumfa-1.4.0/deploy/uwsgi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.165599 edumfa-1.4.0/deploy/uwsgi/apps-available/
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-19 17:58:21.000000 edumfa-1.4.0/deploy/uwsgi/apps-available/edumfa.xml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.165599 edumfa-1.4.0/edumfa/
--rw-r--r--   0 runner    (1001) docker     (127)      916 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.173599 edumfa-1.4.0/edumfa/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    18346 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/before_after.py
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/caconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/clienttype.py
--rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/edumfaserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.173599 edumfa-1.4.0/edumfa/api/lib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/lib/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5200 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/lib/policyhelper.py
--rw-r--r--   0 runner    (1001) docker     (127)    41925 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/lib/postpolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)   101628 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/lib/prepolicy.py
--rw-r--r--   0 runner    (1001) docker     (127)    17803 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/lib/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    15527 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/machineresolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/periodictask.py
--rw-r--r--   0 runner    (1001) docker     (127)    18770 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/radiusserver.py
--rw-r--r--   0 runner    (1001) docker     (127)    10790 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/realm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/recover.py
--rw-r--r--   0 runner    (1001) docker     (127)     7117 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/register.py
--rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/serviceid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/smsgateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/smtpserver.py
--rw-r--r--   0 runner    (1001) docker     (127)    12631 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/system.py
--rw-r--r--   0 runner    (1001) docker     (127)    55643 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/tokengroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/ttype.py
--rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    29126 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/api/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)    10326 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/app.py
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/babel.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.181599 edumfa-1.4.0/edumfa/lib/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.181599 edumfa-1.4.0/edumfa/lib/applications/
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/applications/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/applications/luks.py
--rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/applications/offline.py
--rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/applications/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)     7274 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/audit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.185599 edumfa-1.4.0/edumfa/lib/auditmodules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/auditmodules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8769 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/auditmodules/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/auditmodules/containeraudit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/auditmodules/loggeraudit.py
--rw-r--r--   0 runner    (1001) docker     (127)    26334 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/auditmodules/sqlaudit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/authcache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.185599 edumfa-1.4.0/edumfa/lib/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/caconnector.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.185599 edumfa-1.4.0/edumfa/lib/caconnectors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/caconnectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/caconnectors/baseca.py
--rw-r--r--   0 runner    (1001) docker     (127)    10664 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/caconnectors/caservice_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11729 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/caconnectors/caservice_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    27145 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/caconnectors/localca.py
--rw-r--r--   0 runner    (1001) docker     (127)    17292 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/caconnectors/msca.py
--rw-r--r--   0 runner    (1001) docker     (127)     5900 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/challenge.py
--rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/challengeresponsedecorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/clientapplication.py
--rw-r--r--   0 runner    (1001) docker     (127)    37215 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/counter.py
--rw-r--r--   0 runner    (1001) docker     (127)    28674 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/edumfaserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     6314 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/error.py
--rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/event.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.189599 edumfa-1.4.0/edumfa/lib/eventhandler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/eventhandler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24840 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/eventhandler/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/eventhandler/counterhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/eventhandler/customuserattributeshandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/eventhandler/federationhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6358 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/eventhandler/logginghandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/eventhandler/requestmangler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/eventhandler/responsemangler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8919 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/eventhandler/scripthandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    30653 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/eventhandler/tokenhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)    21561 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/eventhandler/usernotification.py
--rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/eventhandler/webhookeventhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/framework.py
--rw-r--r--   0 runner    (1001) docker     (127)    29337 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/importotp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7419 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    19552 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/machine.py
--rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/machineresolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.189599 edumfa-1.4.0/edumfa/lib/machines/
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/machines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/machines/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/machines/hosts.py
--rw-r--r--   0 runner    (1001) docker     (127)    14366 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/machines/ldap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.189599 edumfa-1.4.0/edumfa/lib/monitoringmodules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/monitoringmodules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/monitoringmodules/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/monitoringmodules/sqlstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/monitoringstats.py
--rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/passwordreset.py
--rw-r--r--   0 runner    (1001) docker     (127)    12715 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/periodictask.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.189599 edumfa-1.4.0/edumfa/lib/pinhandling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/pinhandling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/pinhandling/base.py
--rw-r--r--   0 runner    (1001) docker     (127)   146757 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    28842 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/policydecorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.189599 edumfa-1.4.0/edumfa/lib/queues/
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/queues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/queues/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/queues/huey_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/radiusserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8015 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/realm.py
--rw-r--r--   0 runner    (1001) docker     (127)    14818 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.189599 edumfa-1.4.0/edumfa/lib/resolvers/
--rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/resolvers/HTTPResolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    56725 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/resolvers/LDAPIdResolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    15166 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/resolvers/PasswdIdResolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    10885 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/resolvers/SCIMIdResolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    28267 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/resolvers/SQLIdResolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8590 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/resolvers/UserIdResolver.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/resolvers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.193600 edumfa-1.4.0/edumfa/lib/security/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13784 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/security/aeshsm.py
--rw-r--r--   0 runner    (1001) docker     (127)    16464 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/security/default.py
--rw-r--r--   0 runner    (1001) docker     (127)    14478 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/security/encryptkey.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.193600 edumfa-1.4.0/edumfa/lib/security/password/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/security/password/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/serviceid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.193600 edumfa-1.4.0/edumfa/lib/smsprovider/
--rw-r--r--   0 runner    (1001) docker     (127)     9043 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/smsprovider/FirebaseProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/smsprovider/HttpMessageToUidProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/smsprovider/HttpSMSProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)    12565 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/smsprovider/SMSProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/smsprovider/ScriptSMSProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/smsprovider/SipgateSMSProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/smsprovider/SmppSMSProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/smsprovider/SmtpSMSProvider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/smsprovider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13922 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/smtpserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/sqlutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/subscriptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.193600 edumfa-1.4.0/edumfa/lib/task/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/task/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/task/eventcounter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/task/simplestats.py
--rw-r--r--   0 runner    (1001) docker     (127)    96268 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    68419 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokenclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokengroup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.201600 edumfa-1.4.0/edumfa/lib/tokens/
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/HMAC.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/applicationspecificpasswordtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    25837 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/certificatetoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/daplugtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    16746 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/daypasswordtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    22719 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/emailtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    18983 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/foureyestoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    33207 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/hotptoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    15903 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/indexedsecrettoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/mOTP.py
--rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/motptoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    14133 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/ocra.py
--rw-r--r--   0 runner    (1001) docker     (127)    10863 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/ocratoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/papertoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/passwordtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    46777 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/pushtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/questionnairetoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    22143 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/radiustoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/registrationtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/remotetoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    25368 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/smstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/spasstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     5806 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/sshkeytoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     8130 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/tantoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    19949 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/tiqrtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    27633 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/totptoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/u2f.py
--rw-r--r--   0 runner    (1001) docker     (127)    23127 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/u2ftoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/vasco.py
--rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/vascotoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    89138 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/webauthn.py
--rw-r--r--   0 runner    (1001) docker     (127)    65414 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/webauthntoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/yubicotoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    16984 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/tokens/yubikeytoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    30149 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/usercache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.201600 edumfa-1.4.0/edumfa/lib/utils/
--rw-r--r--   0 runner    (1001) docker     (127)    55043 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/utils/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/lib/utils/export.py
--rw-r--r--   0 runner    (1001) docker     (127)    71279 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/messages.pot
--rw-r--r--   0 runner    (1001) docker     (127)   121289 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.201600 edumfa-1.4.0/edumfa/static/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/app.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.153599 edumfa-1.4.0/edumfa/static/components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.149599 edumfa-1.4.0/edumfa/static/components/audit/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.205600 edumfa-1.4.0/edumfa/static/components/audit/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/audit/controllers/auditControllers.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.205600 edumfa-1.4.0/edumfa/static/components/audit/factories/
--rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/audit/factories/audit.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.205600 edumfa-1.4.0/edumfa/static/components/audit/states/
--rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/audit/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.205600 edumfa-1.4.0/edumfa/static/components/audit/views/
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/audit/views/audit.html
--rw-r--r--   0 runner    (1001) docker     (127)    11055 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/audit/views/audit.log.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.149599 edumfa-1.4.0/edumfa/static/components/components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.205600 edumfa-1.4.0/edumfa/static/components/components/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/components/controllers/componentControllers.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.205600 edumfa-1.4.0/edumfa/static/components/components/factories/
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/components/factories/component.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.205600 edumfa-1.4.0/edumfa/static/components/components/states/
--rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/components/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.205600 edumfa-1.4.0/edumfa/static/components/components/views/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/components/views/component.clienttype.html
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/components/views/component.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.149599 edumfa-1.4.0/edumfa/static/components/config/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.205600 edumfa-1.4.0/edumfa/static/components/config/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)    50570 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/controllers/configControllers.js
--rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/controllers/eduMfaServerController.js
--rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/controllers/eventController.js
--rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/controllers/ldapMachineResolverController.js
--rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/controllers/periodicTaskController.js
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/controllers/radiusServerController.js
--rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/controllers/serviceidController.js
--rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/controllers/smsgatewayController.js
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/controllers/smtpServerController.js
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/controllers/tokengroupController.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.209600 edumfa-1.4.0/edumfa/static/components/config/factories/
--rw-r--r--   0 runner    (1001) docker     (127)    32353 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/factories/config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.209600 edumfa-1.4.0/edumfa/static/components/config/states/
--rw-r--r--   0 runner    (1001) docker     (127)    19924 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.217600 edumfa-1.4.0/edumfa/static/components/config/views/
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.caconnectors.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.caconnectors.local.html
--rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.caconnectors.microsoft.html
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.edumfaserver.edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.edumfaserver.list.html
--rw-r--r--   0 runner    (1001) docker     (127)    15020 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.events.details.html
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.events.html
--rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.events.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.html
--rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.machineresolvers.html
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.mresolvers.hosts.html
--rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.mresolvers.ldap.html
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.mresolvers.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.periodictasks.details.html
--rw-r--r--   0 runner    (1001) docker     (127)      872 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.periodictasks.html
--rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.periodictasks.list.html
--rw-r--r--   0 runner    (1001) docker     (127)    22234 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.policies.details.html
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.policies.html
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.policies.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.radius.edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.radius.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.realms.html
--rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.realms.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.resolvers.html
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.resolvers.http.html
--rw-r--r--   0 runner    (1001) docker     (127)    14914 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.resolvers.ldap.html
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.resolvers.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.resolvers.passwd.html
--rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.resolvers.scim.html
--rw-r--r--   0 runner    (1001) docker     (127)    10128 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.resolvers.sql.html
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.serviceid.edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.serviceid.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.smsgateway.edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.smsgateway.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.smtp.edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.smtp.list.html
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.system.doc.html
--rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.system.edit.html
--rw-r--r--   0 runner    (1001) docker     (127)    13600 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.system.html
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.token.daypassword.html
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.token.email.html
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.token.hotp.html
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.token.question.html
--rw-r--r--   0 runner    (1001) docker     (127)      639 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.token.radius.html
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.token.remote.html
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.token.sms.html
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.token.tiqr.html
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.token.totp.html
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.token.u2f.html
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.token.webauthn.html
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.token.yubico.html
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.token.yubikey.html
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.tokengroup.edit.html
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.tokengroup.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/config.tokens.html
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/config/views/dialog.confirm_delete.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.149599 edumfa-1.4.0/edumfa/static/components/dashboard/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.217600 edumfa-1.4.0/edumfa/static/components/dashboard/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/dashboard/controllers/dashboardControllers.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.217600 edumfa-1.4.0/edumfa/static/components/dashboard/states/
--rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/dashboard/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.217600 edumfa-1.4.0/edumfa/static/components/dashboard/views/
--rw-r--r--   0 runner    (1001) docker     (127)     8881 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/dashboard/views/dashboard.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.149599 edumfa-1.4.0/edumfa/static/components/dialogs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.221600 edumfa-1.4.0/edumfa/static/components/dialogs/views/
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/dialogs/views/dialog.about.html
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/dialogs/views/dialog.autocreate_realm.html
--rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/dialogs/views/dialog.lock.html
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/dialogs/views/dialog.no.token.html
--rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/dialogs/views/dialog.welcome.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.149599 edumfa-1.4.0/edumfa/static/components/directives/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.221600 edumfa-1.4.0/edumfa/static/components/directives/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)    19746 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/directives/controllers/directives.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.221600 edumfa-1.4.0/edumfa/static/components/directives/views/
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/directives/views/directive.assigntoken.html
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/directives/views/directive.assignuser.html
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/directives/views/directive.attachmachine.html
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/directives/views/directive.attachtoken.html
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/directives/views/directive.csvdownload.html
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/directives/views/directive.filter.table.html
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/directives/views/directive.policyconditions.html
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/directives/views/directive.tokendata.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.221600 edumfa-1.4.0/edumfa/static/components/filters/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/filters/filters.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.149599 edumfa-1.4.0/edumfa/static/components/login/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.221600 edumfa-1.4.0/edumfa/static/components/login/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)    30344 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/login/controllers/loginControllers.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.221600 edumfa-1.4.0/edumfa/static/components/login/factories/
--rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/login/factories/auth.js
--rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/login/factories/u2f.js
--rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/login/factories/webauthn.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.221600 edumfa-1.4.0/edumfa/static/components/login/states/
--rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/login/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.225600 edumfa-1.4.0/edumfa/static/components/login/views/
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/login/views/enter-response.html
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/login/views/login.html
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/login/views/offline.html
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/login/views/pinchange.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.153599 edumfa-1.4.0/edumfa/static/components/machine/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.225600 edumfa-1.4.0/edumfa/static/components/machine/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/machine/controllers/machineController.js
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/machine/controllers/machineDetailsController.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.225600 edumfa-1.4.0/edumfa/static/components/machine/factories/
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/machine/factories/machine.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.225600 edumfa-1.4.0/edumfa/static/components/machine/states/
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/machine/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.225600 edumfa-1.4.0/edumfa/static/components/machine/views/
--rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/machine/views/machine.details.html
--rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/machine/views/machine.html
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/machine/views/machine.list.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.153599 edumfa-1.4.0/edumfa/static/components/recovery/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.225600 edumfa-1.4.0/edumfa/static/components/recovery/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/recovery/controllers/recoveryControllers.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.225600 edumfa-1.4.0/edumfa/static/components/recovery/factories/
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/recovery/factories/recoveryFactory.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.225600 edumfa-1.4.0/edumfa/static/components/recovery/states/
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/recovery/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.225600 edumfa-1.4.0/edumfa/static/components/recovery/views/
--rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/recovery/views/recovery.html
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/recovery/views/recovery.reset.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.153599 edumfa-1.4.0/edumfa/static/components/register/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.225600 edumfa-1.4.0/edumfa/static/components/register/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/register/controllers/registerControllers.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.225600 edumfa-1.4.0/edumfa/static/components/register/factories/
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/register/factories/registerFactory.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.225600 edumfa-1.4.0/edumfa/static/components/register/states/
--rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/register/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.225600 edumfa-1.4.0/edumfa/static/components/register/views/
--rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/register/views/register.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.153599 edumfa-1.4.0/edumfa/static/components/token/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.229600 edumfa-1.4.0/edumfa/static/components/token/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/controllers/tokenApplicationsController.js
--rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/controllers/tokenChallengesController.js
--rw-r--r--   0 runner    (1001) docker     (127)    29864 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/controllers/tokenControllers.js
--rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/controllers/tokenDetailController.js
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/controllers/tokenGetSerialController.js
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/controllers/tokenLostController.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.229600 edumfa-1.4.0/edumfa/static/components/token/factories/
--rw-r--r--   0 runner    (1001) docker     (127)    12956 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/factories/token.js
--rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/factories/validate.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.229600 edumfa-1.4.0/edumfa/static/components/token/states/
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.237600 edumfa-1.4.0/edumfa/static/components/token/views/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/dialog.ask_token_delete.html
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.applications.html
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.applications.offline.html
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.applications.ssh.html
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.assign.html
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.challenges.html
--rw-r--r--   0 runner    (1001) docker     (127)    32395 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.details.html
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.display.apps.html
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.4eyes.html
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.applspec.html
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.certificate.html
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.daypassword.html
--rw-r--r--   0 runner    (1001) docker     (127)      981 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.email.html
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.hotp.html
--rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.html
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.indexedsecret.html
--rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.motp.html
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.paper.html
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.push.html
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.question.html
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.radius.html
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.registration.html
--rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.remote.html
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.sms.html
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.spass.html
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.sshkey.html
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.tan.html
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.tiqr.html
--rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.totp.html
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.u2f.html
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.vasco.html
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.webauthn.html
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.yubico.html
--rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.yubikey.html
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enrolled.applspec.html
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enrolled.certificate.html
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enrolled.daypassword.html
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enrolled.hotp.html
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enrolled.motp.html
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enrolled.paper.html
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enrolled.push.html
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enrolled.registration.html
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enrolled.tan.html
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enrolled.tiqr.html
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enrolled.totp.html
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enrolled.u2f.html
--rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.enrolled.webauthn.html
--rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.getserial.html
--rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.html
--rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.import.html
--rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa/static/components/token/views/token.lost.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.237600 edumfa-1.4.0/edumfa/static/components/translation/
--rw-r--r--   0 runner    (1001) docker     (127)   557561 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/components/translation/translations.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.153599 edumfa-1.4.0/edumfa/static/components/user/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.241600 edumfa-1.4.0/edumfa/static/components/user/controllers/
--rw-r--r--   0 runner    (1001) docker     (127)    19169 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/components/user/controllers/userControllers.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.241600 edumfa-1.4.0/edumfa/static/components/user/factories/
--rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/components/user/factories/user.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.241600 edumfa-1.4.0/edumfa/static/components/user/states/
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/components/user/states/states.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.241600 edumfa-1.4.0/edumfa/static/components/user/views/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/components/user/views/dialog.ask_user_delete.html
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/components/user/views/user.add.dynamic.form.fields.html
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/components/user/views/user.add.html
--rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/components/user/views/user.details.html
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/components/user/views/user.html
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/components/user/views/user.list.html
--rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/components/user/views/user.password.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.157599 edumfa-1.4.0/edumfa/static/contrib/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.245600 edumfa-1.4.0/edumfa/static/contrib/css/
--rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/css/angular-inform.css
--rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/css/angular-inform.css.map
--rw-r--r--   0 runner    (1001) docker     (127)    25682 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/css/bootstrap-theme.css
--rw-r--r--   0 runner    (1001) docker     (127)    48005 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/css/bootstrap-theme.css.map
--rw-r--r--   0 runner    (1001) docker     (127)   145933 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/css/bootstrap.css
--rw-r--r--   0 runner    (1001) docker     (127)   390887 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/css/bootstrap.css.map
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/css/hotkeys.css
--rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/css/isteven-multi-select.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.245600 edumfa-1.4.0/edumfa/static/contrib/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    20127 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (127)   108738 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (127)    45404 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.woff2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.249601 edumfa-1.4.0/edumfa/static/contrib/js/
--rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/js/angular-inform.js
--rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/js/angular-inform.js.map
--rw-r--r--   0 runner    (1001) docker     (127)  1377909 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/js/angular.js
--rw-r--r--   0 runner    (1001) docker     (127)    75484 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/js/bootstrap.js
--rw-r--r--   0 runner    (1001) docker     (127)    53486 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/js/hotkeys.js
--rw-r--r--   0 runner    (1001) docker     (127)   288580 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/js/jquery.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.253600 edumfa-1.4.0/edumfa/static/contrib/js/ngmodules/
--rw-r--r--   0 runner    (1001) docker     (127)    32388 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/js/ngmodules/angular-gettext.js
--rw-r--r--   0 runner    (1001) docker     (127)    16000 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/js/ngmodules/angular-idle.js
--rw-r--r--   0 runner    (1001) docker     (127)    33197 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/js/ngmodules/angular-sanitize.js
--rw-r--r--   0 runner    (1001) docker     (127)   487964 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/js/ngmodules/angular-ui-router.js
--rw-r--r--   0 runner    (1001) docker     (127)   760134 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/js/ngmodules/angular-ui-router.js.map
--rw-r--r--   0 runner    (1001) docker     (127)    53338 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/js/ngmodules/isteven-multi-select.js
--rw-r--r--   0 runner    (1001) docker     (127)    81683 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/js/ngmodules/ng-file-upload.js
--rw-r--r--   0 runner    (1001) docker     (127)    20905 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/js/u2f-api.js
--rw-r--r--   0 runner    (1001) docker     (127)   276562 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/js/ui-bootstrap-tpls.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.253600 edumfa-1.4.0/edumfa/static/contrib/js/webauthn-client/
--rw-r--r--   0 runner    (1001) docker     (127)    20759 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/contrib/js/webauthn-client/edumfa-webauthn.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.257601 edumfa-1.4.0/edumfa/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/css/baseline.css
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/css/content.css
--rw-r--r--   0 runner    (1001) docker     (127)    24602 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/css/eduMFA-logo.png
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/css/highlight.css
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/css/menu.css
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/css/papertoken.css
--rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/css/signin.css
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/css/table-ui.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.257601 edumfa-1.4.0/edumfa/static/customize/
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/customize/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/favicon.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.257601 edumfa-1.4.0/edumfa/static/img/
--rw-r--r--   0 runner    (1001) docker     (127)   195931 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/img/FIDO-U2F-Security-Key-444x444.png
--rw-r--r--   0 runner    (1001) docker     (127)    47610 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/img/plugup.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   336777 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/img/solokeys.png
--rw-r--r--   0 runner    (1001) docker     (127)   107999 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/img/u2fzero.png
--rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.257601 edumfa-1.4.0/edumfa/static/providers/
--rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/providers/errorMessageProvider.js
--rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/providers/versioningProvider.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.261601 edumfa-1.4.0/edumfa/static/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/templates/baseline.html
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/templates/cert_request_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/templates/deactivated.html
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/templates/documentation.rst
--rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/templates/footer.html
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/templates/header.html
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/templates/menu.html
--rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/templates/token_enrolled.html
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/static/update_contrib.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.161599 edumfa-1.4.0/edumfa/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.157599 edumfa-1.4.0/edumfa/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.261601 edumfa-1.4.0/edumfa/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    23376 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    84098 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.157599 edumfa-1.4.0/edumfa/translations/de/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.261601 edumfa-1.4.0/edumfa/translations/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    95309 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/de/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   127521 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/de/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.157599 edumfa-1.4.0/edumfa/translations/es/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.261601 edumfa-1.4.0/edumfa/translations/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    81449 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/es/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   118619 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/es/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.157599 edumfa-1.4.0/edumfa/translations/fr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.261601 edumfa-1.4.0/edumfa/translations/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    53719 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/fr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   104451 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/fr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.157599 edumfa-1.4.0/edumfa/translations/it/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.261601 edumfa-1.4.0/edumfa/translations/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    26784 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/it/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    87343 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/it/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.157599 edumfa-1.4.0/edumfa/translations/nl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.265601 edumfa-1.4.0/edumfa/translations/nl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    85965 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/nl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   120848 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/nl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.157599 edumfa-1.4.0/edumfa/translations/pl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.265601 edumfa-1.4.0/edumfa/translations/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/pl/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    73216 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/pl/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.157599 edumfa-1.4.0/edumfa/translations/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.265601 edumfa-1.4.0/edumfa/translations/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    78400 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/pt_BR/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   115604 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/pt_BR/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.157599 edumfa-1.4.0/edumfa/translations/ro/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.265601 edumfa-1.4.0/edumfa/translations/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    10507 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/ro/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    79882 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/ro/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.157599 edumfa-1.4.0/edumfa/translations/ru/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.265601 edumfa-1.4.0/edumfa/translations/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    33313 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/ru/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    96048 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/ru/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.157599 edumfa-1.4.0/edumfa/translations/si/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.265601 edumfa-1.4.0/edumfa/translations/si/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/si/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)    73291 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/si/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.161599 edumfa-1.4.0/edumfa/translations/tr/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.265601 edumfa-1.4.0/edumfa/translations/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    82030 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/tr/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   117846 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/tr/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.161599 edumfa-1.4.0/edumfa/translations/zh_Hans/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.269601 edumfa-1.4.0/edumfa/translations/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    68507 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/zh_Hans/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   104457 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/zh_Hans/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.161599 edumfa-1.4.0/edumfa/translations/zh_Hant/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.269601 edumfa-1.4.0/edumfa/translations/zh_Hant/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)    70327 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/zh_Hant/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)   105843 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/translations/zh_Hant/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.269601 edumfa-1.4.0/edumfa/webui/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/webui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/webui/certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9124 2024-03-19 17:58:22.000000 edumfa-1.4.0/edumfa/webui/login.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    62952 2024-03-19 17:58:21.000000 edumfa-1.4.0/edumfa-manage
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.325602 edumfa-1.4.0/edumfa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-03-19 17:58:26.000000 edumfa-1.4.0/edumfa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    31391 2024-03-19 17:58:26.000000 edumfa-1.4.0/edumfa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 17:58:26.000000 edumfa-1.4.0/edumfa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 17:58:25.000000 edumfa-1.4.0/edumfa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-19 17:58:26.000000 edumfa-1.4.0/edumfa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-19 17:58:26.000000 edumfa-1.4.0/edumfa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.269601 edumfa-1.4.0/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/README
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/alembic.ini
--rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/script.py.mako
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.281601 edumfa-1.4.0/migrations/versions/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/006d4747f858_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/00762b3f7a60_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/0c7123345224_.py
--rw-r--r--   0 runner    (1001) docker     (127)     5545 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/0d011e94a8e8_.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/140ba0ca4f07_.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/145ce80decd_.py
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/14a1bcb10018_.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/19f727d285e2_.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/1a0710df148b_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/1a69e5e5e2ac_.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/1edda52b619f_.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/204d8d4f351e_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/205bda834127_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/20969b4cbf06_.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/2118e566df16_.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/2181294eed0b_.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/22558d9f3178_.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/239995464c48_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/2551ee982544_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/2ac117d0a6f5_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/2c9430cfc66b_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/307a4fbe8a05_.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/3236a1abf1c6_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/3429d523e51f_.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/36428afb2457_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/37e6b49fc686_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/3ae3c668f444_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/3ba618f6b820_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/3c6e9dd7fbac_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/3d7f8b29cbb1_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/3f7e8583ea2_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/4023571658f8_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/4238eac8ccab_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/449903fb6e35_.py
--rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/48ee74b8a7c8_.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/49a04e560d96_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/4a0aec37e7cf_.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/4d9178fa8336_.py
--rw-r--r--   0 runner    (1001) docker     (127)    19377 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/4f32a4e1bf33_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/50adc980d625_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/5402fd96fbca_.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/58e4f7ebb705_.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/59ef3e03bc62_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/5cb310101a1f_.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/631ec59e1ca6_.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/849170064430_.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/86f40f535d7c_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/888b56ed5dcb_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/89e57ed16379_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/8d40dbcfda25_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/9155f0d3d028_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/a28f2733897b_.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/a63df077051a_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/a7e91b18a460_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/b9131d0686eb_.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/cb6d7b7bae63_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/d2ae8e54b628_.py
--rw-r--r--   0 runner    (1001) docker     (127)      360 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/d3c0f0403a84_.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/d415d490eb05_.py
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/d5870fd2f2a4_.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/d6b40a745e5_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/d756b34061ff_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/dceb6cd3c41e_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/e360c56bcf8c_.py
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/e5cbeb7c177_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/ef29ba43e290_.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/fa07bd604a75.py
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/fabcf24d9304_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-03-19 17:58:22.000000 edumfa-1.4.0/migrations/versions/ff26585932ec_.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-03-19 17:58:22.000000 edumfa-1.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-19 17:58:26.329602 edumfa-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-03-19 17:58:22.000000 edumfa-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.305601 edumfa-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    28189 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/ldap3mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/mscamock.py
--rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/pkcs11mock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/queuemock.py
--rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/radiusmock.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/redismock.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/smppmock.py
--rw-r--r--   0 runner    (1001) docker     (127)     7690 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/smtpmock.py
--rw-r--r--   0 runner    (1001) docker     (127)    35694 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_2stepinit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_applications.py
--rw-r--r--   0 runner    (1001) docker     (127)    20710 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_audit.py
--rw-r--r--   0 runner    (1001) docker     (127)    48917 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_caconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_clienttype.py
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_edumfaserver.py
--rw-r--r--   0 runner    (1001) docker     (127)    35517 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_events.py
--rw-r--r--   0 runner    (1001) docker     (127)   193396 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_lib_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    19077 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_lib_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_machineresolver.py
--rw-r--r--   0 runner    (1001) docker     (127)    38769 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_machines.py
--rw-r--r--   0 runner    (1001) docker     (127)    16166 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_machines_serviceid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_offline_no_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_periodictask.py
--rw-r--r--   0 runner    (1001) docker     (127)    36128 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    26177 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_push_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_radiusserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     8398 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_register.py
--rw-r--r--   0 runner    (1001) docker     (127)    76125 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_serviceids.py
--rw-r--r--   0 runner    (1001) docker     (127)    14259 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_smsgateway.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_smtpserver.py
--rw-r--r--   0 runner    (1001) docker     (127)    62186 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_system.py
--rw-r--r--   0 runner    (1001) docker     (127)   192982 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_tokengroup.py
--rw-r--r--   0 runner    (1001) docker     (127)    21541 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_ttype.py
--rw-r--r--   0 runner    (1001) docker     (127)    29544 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_u2f.py
--rw-r--r--   0 runner    (1001) docker     (127)    33114 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_users.py
--rw-r--r--   0 runner    (1001) docker     (127)   302927 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_api_validate.py
--rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_app.py
--rw-r--r--   0 runner    (1001) docker     (127)    45689 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_db_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_applications.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    23056 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_audit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_authcache.py
--rw-r--r--   0 runner    (1001) docker     (127)    31138 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_caconnector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_challenges.py
--rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_clientapplication.py
--rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_counter.py
--rw-r--r--   0 runner    (1001) docker     (127)    35302 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)    13267 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_edumfaserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_eventhandler_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)    60534 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_eventhandler_usernotification.py
--rw-r--r--   0 runner    (1001) docker     (127)   113340 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_events.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_framework.py
--rw-r--r--   0 runner    (1001) docker     (127)    29545 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_importotp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_lifecycle.py
--rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_machine_resolver_ldap.py
--rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_machines.py
--rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_machinetokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_monitoringstats.py
--rw-r--r--   0 runner    (1001) docker     (127)    20699 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_periodictask.py
--rw-r--r--   0 runner    (1001) docker     (127)    75326 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)    36401 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_policydecorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_pooling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_queue.py
--rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_radiusserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_realm.py
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_recovery.py
--rw-r--r--   0 runner    (1001) docker     (127)   123815 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_serviceid.py
--rw-r--r--   0 runner    (1001) docker     (127)    32074 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_smsprovider.py
--rw-r--r--   0 runner    (1001) docker     (127)    10949 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_smtpserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_sqlutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_task_eventcounter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_task_simplestats.py
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tasks.py
--rw-r--r--   0 runner    (1001) docker     (127)    97642 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_token.py
--rw-r--r--   0 runner    (1001) docker     (127)    38128 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokenclass.py
--rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokengroup.py
--rw-r--r--   0 runner    (1001) docker     (127)    36699 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokens_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)    25260 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokens_daplug.py
--rw-r--r--   0 runner    (1001) docker     (127)    27651 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokens_daypassword.py
--rw-r--r--   0 runner    (1001) docker     (127)    21128 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokens_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokens_foureyes.py
--rw-r--r--   0 runner    (1001) docker     (127)    34350 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokens_hotp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokens_indexedsecret.py
--rw-r--r--   0 runner    (1001) docker     (127)     7183 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokens_motp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokens_paper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokens_passwordtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)    75419 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokens_push.py
--rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokens_questionnaire.py
--rw-r--r--   0 runner    (1001) docker     (127)    16576 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokens_radius.py
--rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokens_registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     9417 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokens_remote.py
--rw-r--r--   0 runner    (1001) docker     (127)    20806 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokens_sms.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokens_spass.py
--rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokens_ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokens_tan.py
--rw-r--r--   0 runner    (1001) docker     (127)    31214 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokens_tiqr.py
--rw-r--r--   0 runner    (1001) docker     (127)    34079 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokens_totp.py
--rw-r--r--   0 runner    (1001) docker     (127)    22536 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokens_u2f.py
--rw-r--r--   0 runner    (1001) docker     (127)    10413 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokens_vasco.py
--rw-r--r--   0 runner    (1001) docker     (127)    50926 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokens_webauthn.py
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokens_yubico.py
--rw-r--r--   0 runner    (1001) docker     (127)    10230 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_tokens_yubikey.py
--rw-r--r--   0 runner    (1001) docker     (127)    22413 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    26644 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_usercache.py
--rw-r--r--   0 runner    (1001) docker     (127)    45888 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_lib_utils_compare.py
--rw-r--r--   0 runner    (1001) docker     (127)    38033 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_mock_ldap3.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_resolver_realm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_ui_certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/test_ui_login.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.313601 edumfa-1.4.0/tests/testdata/
--rw-r--r--   0 runner    (1001) docker     (127)   195931 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/FIDO-U2F-Security-Key-444x444.png
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/NetKnights.pem
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.161599 edumfa-1.4.0/tests/testdata/altstatic/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.313601 edumfa-1.4.0/tests/testdata/altstatic/templates/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/altstatic/templates/testui.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.313601 edumfa-1.4.0/tests/testdata/attestation/
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/attestation/yubico.pem
--rw-r--r--   0 runner    (1001) docker     (127)    16384 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/audit.sqlite
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.313601 edumfa-1.4.0/tests/testdata/ca/
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/ca/cacert.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/ca/cakey.pem
--rw-r--r--   0 runner    (1001) docker     (127)    15874 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/ca/index.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/ca/index.txt.attr
--rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/ca/openssl.cnf
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/ca/serial
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/ca/templates.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/dictionary
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/does_not_exist
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/emailtemplate.html
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/empty.oath
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/enckey
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/enckey.enc
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/fancytoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/firebase-test.json
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/google-services.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.317602 edumfa-1.4.0/tests/testdata/gpg/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/gpg/public.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/gpg/pubring.gpg
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/gpg/random_seed
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/gpg/secring.gpg
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/gpg/trustdb.gpg
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/hosts
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/import.oath
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/import.oath.asc
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/jwt_sign.key
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/logging.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/logging.yml
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/logging_broken.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.317602 edumfa-1.4.0/tests/testdata/msca-connector/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/msca-connector/ca.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/msca-connector/privacyidea-encrypted.key
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/msca-connector/privacyidea.key
--rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/msca-connector/privacyidea.pem
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/ocra.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/passwd
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/passwd-duplicate-name
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/passwords
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/policy.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/policy_empty_file.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/private.pem
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/pskc-aes.xml
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/pskc-password.xml
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/public.pem
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/pw-2nd-resolver
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.317602 edumfa-1.4.0/tests/testdata/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)       19 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/scripts/fail.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/scripts/ls.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)       19 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/scripts/success.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/test.sub
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/test2.sub
--rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/testuser-api.sqlite
--rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/testuser.sqlite
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/testusercache.sqlite
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.317602 edumfa-1.4.0/tests/testdata/trusted_attestation_roots/
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/trusted_attestation_roots/solokeys_device_attestation_ca.pem
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/trusted_attestation_roots/yubico_u2f_device_attestation_ca.pem
--rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/yubico-oath-long.csv
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/yubico-oath.csv
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-19 17:58:22.000000 edumfa-1.4.0/tests/testdata/yubico.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 17:58:26.325602 edumfa-1.4.0/tools/
--rwxr-xr-x   0 runner    (1001) docker     (127)      768 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/creategoogleauthenticator-file
--rwxr-xr-x   0 runner    (1001) docker     (127)     2551 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-authorizedkeys
--rwxr-xr-x   0 runner    (1001) docker     (127)     1766 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-convert-base32.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2876 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-convert-token
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-convert-token.1
--rwxr-xr-x   0 runner    (1001) docker     (127)     3230 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-convert-xml-to-csv
--rwxr-xr-x   0 runner    (1001) docker     (127)     2440 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-create-ad-users
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-create-ad-users.1
--rwxr-xr-x   0 runner    (1001) docker     (127)     1940 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-create-certificate
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-create-certificate.1
--rwxr-xr-x   0 runner    (1001) docker     (127)     1985 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-create-pwidresolver-user
--rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-create-pwidresolver-user.1
--rwxr-xr-x   0 runner    (1001) docker     (127)     1608 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-create-sqlidresolver-user
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-create-sqlidresolver-user.1
--rwxr-xr-x   0 runner    (1001) docker     (127)      795 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-create-userdb
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-create-userdb.1
--rwxr-xr-x   0 runner    (1001) docker     (127)     6703 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-cron
--rwxr-xr-x   0 runner    (1001) docker     (127)     7030 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-diag
--rwxr-xr-x   0 runner    (1001) docker     (127)     6991 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-expired-users
--rwxr-xr-x   0 runner    (1001) docker     (127)     1354 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-export-edumfa-counter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4514 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-export-linotp-counter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3719 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-fetchssh
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-fetchssh.1
--rwxr-xr-x   0 runner    (1001) docker     (127)     2500 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-fix-access-rights
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-fix-access-rights.1
--rwxr-xr-x   0 runner    (1001) docker     (127)     3541 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-get-serial
--rwxr-xr-x   0 runner    (1001) docker     (127)     4940 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-get-unused-tokens
--rwxr-xr-x   0 runner    (1001) docker     (127)    25361 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-migrate-linotp.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2525 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-pip-update
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-pip-update.1
--rwxr-xr-x   0 runner    (1001) docker     (127)     5761 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-queue-huey
--rwxr-xr-x   0 runner    (1001) docker     (127)      643 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-schema-upgrade
--rwxr-xr-x   0 runner    (1001) docker     (127)    11397 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-standalone
--rwxr-xr-x   0 runner    (1001) docker     (127)     8176 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-sync-owncloud.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    31889 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-token-janitor
--rwxr-xr-x   0 runner    (1001) docker     (127)     3746 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-update-counter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5391 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-update-linotp-counter.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5471 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-user-action
--rwxr-xr-x   0 runner    (1001) docker     (127)     3674 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/edumfa-usercache-cleanup
--rwxr-xr-x   0 runner    (1001) docker     (127)     1476 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/getgooglecodes
--rwxr-xr-x   0 runner    (1001) docker     (127)     3049 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/reset-edumfa
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-19 17:58:22.000000 edumfa-1.4.0/tools/ssha.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.284088 edumfa-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8120 2024-04-02 12:57:39.000000 edumfa-1.5.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (127)    32387 2024-04-02 12:57:39.000000 edumfa-1.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-04-02 12:57:39.000000 edumfa-1.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-04-02 12:57:52.284088 edumfa-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5632 2024-04-02 12:57:39.000000 edumfa-1.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.112086 edumfa-1.5.0/deploy/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.112086 edumfa-1.5.0/deploy/apache/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/apache/edumfaapp.wsgi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.112086 edumfa-1.5.0/deploy/apache/sites-available/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/apache/sites-available/edumfa-venv.conf
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/apache/sites-available/edumfa.conf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.092086 edumfa-1.5.0/deploy/config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.112086 edumfa-1.5.0/deploy/config/freeradius2/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/config/freeradius2/edumfa
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/config/freeradius2/mods-perl-edumfa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.112086 edumfa-1.5.0/deploy/config/freeradius3/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/config/freeradius3/edumfa
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/config/freeradius3/mods-perl-edumfa
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.112086 edumfa-1.5.0/deploy/crontab/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/crontab/edumfa
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/docker-compose-example.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.116086 edumfa-1.5.0/deploy/docker-example/
+-rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/docker-example/edumfa-policy.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/docker-example/edumfa-setup.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/docker-example/edumfa.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)      726 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/docker-setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.116086 edumfa-1.5.0/deploy/edumfa/
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/edumfa/dictionary
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/edumfa/edumfa.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    21848 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/edumfa_radius.pm
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.116086 edumfa-1.5.0/deploy/gunicorn/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/gunicorn/edumfaapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/logging.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.116086 edumfa-1.5.0/deploy/nginx/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/nginx/edumfaapp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.116086 edumfa-1.5.0/deploy/nginx/sites-available/
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/nginx/sites-available/edumfa
+-rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/rlm_perl.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.116086 edumfa-1.5.0/deploy/ubuntu/
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu/changelog
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu/clean
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu/compat
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu/control
+-rw-r--r--   0 runner    (1001) docker     (127)    32387 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu/copyright
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu/rules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.120086 edumfa-1.5.0/deploy/ubuntu/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu/source/format
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu/source/options
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.116086 edumfa-1.5.0/deploy/ubuntu-radius/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu-radius/changelog
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu-radius/compat
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu-radius/control
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu-radius/copyright
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu-radius/edumfa-radius.install
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu-radius/edumfa-radius.postinst
+-rw-r--r--   0 runner    (1001) docker     (127)      351 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu-radius/edumfa-radius.postrm
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu-radius/rules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.116086 edumfa-1.5.0/deploy/ubuntu-radius/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu-radius/source/format
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.120086 edumfa-1.5.0/deploy/ubuntu-server/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu-server/changelog
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu-server/clean
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu-server/compat
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu-server/control
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu-server/edumfa-apache2.install
+-rw-r--r--   0 runner    (1001) docker     (127)     6122 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu-server/edumfa-apache2.postinst
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu-server/edumfa-apache2.postrm
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu-server/edumfa-nginx.install
+-rw-r--r--   0 runner    (1001) docker     (127)     5581 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu-server/edumfa-nginx.postinst
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu-server/edumfa-nginx.postrm
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu-server/rules
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.120086 edumfa-1.5.0/deploy/ubuntu-server/source/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu-server/source/format
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/ubuntu-server/source/options
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.092086 edumfa-1.5.0/deploy/uwsgi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.120086 edumfa-1.5.0/deploy/uwsgi/apps-available/
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-02 12:57:39.000000 edumfa-1.5.0/deploy/uwsgi/apps-available/edumfa.xml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.120086 edumfa-1.5.0/edumfa/
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.128086 edumfa-1.5.0/edumfa/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4222 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18346 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16376 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/before_after.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/caconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/clienttype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4438 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/edumfaserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7416 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.128086 edumfa-1.5.0/edumfa/api/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/lib/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5631 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/lib/policyhelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41925 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/lib/postpolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101628 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/lib/prepolicy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17803 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/lib/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15527 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5083 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/machineresolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7937 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/periodictask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18770 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/radiusserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10790 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/realm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3436 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/recover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7117 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/register.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6730 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5232 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/serviceid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5462 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/smsgateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5678 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/smtpserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12631 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55749 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5289 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/tokengroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4855 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/ttype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29126 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/api/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10326 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/babel.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6727 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.136087 edumfa-1.5.0/edumfa/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.136087 edumfa-1.5.0/edumfa/lib/applications/
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5830 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/applications/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/applications/luks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8071 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/applications/offline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4624 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/applications/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7274 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4574 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/audit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.140087 edumfa-1.5.0/edumfa/lib/auditmodules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/auditmodules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8769 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/auditmodules/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4803 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/auditmodules/containeraudit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/auditmodules/loggeraudit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26334 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/auditmodules/sqlaudit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6116 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/authcache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.140087 edumfa-1.5.0/edumfa/lib/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11818 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/caconnector.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.140087 edumfa-1.5.0/edumfa/lib/caconnectors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/caconnectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/caconnectors/baseca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10664 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/caconnectors/caservice_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11729 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/caconnectors/caservice_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27145 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/caconnectors/localca.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17292 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/caconnectors/msca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5900 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9658 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/challengeresponsedecorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/clientapplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37215 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28674 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5180 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/edumfaserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6314 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13496 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/event.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.140087 edumfa-1.5.0/edumfa/lib/eventhandler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/eventhandler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24840 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/eventhandler/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/eventhandler/counterhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4322 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/eventhandler/customuserattributeshandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7332 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/eventhandler/federationhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6358 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/eventhandler/logginghandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7509 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/eventhandler/requestmangler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6452 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/eventhandler/responsemangler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8919 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/eventhandler/scripthandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30653 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/eventhandler/tokenhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21561 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/eventhandler/usernotification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6898 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/eventhandler/webhookeventhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29337 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/importotp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7419 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19552 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11009 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/machineresolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.144086 edumfa-1.5.0/edumfa/lib/machines/
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/machines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5809 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/machines/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5828 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/machines/hosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14366 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/machines/ldap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.144086 edumfa-1.5.0/edumfa/lib/monitoringmodules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/monitoringmodules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/monitoringmodules/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7803 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/monitoringmodules/sqlstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/monitoringstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5598 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/passwordreset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12715 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/periodictask.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.144086 edumfa-1.5.0/edumfa/lib/pinhandling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/pinhandling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/pinhandling/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)   146757 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28842 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/policydecorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.144086 edumfa-1.5.0/edumfa/lib/queues/
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/queues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/queues/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/queues/huey_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/radiusserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8015 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/realm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14818 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.144086 edumfa-1.5.0/edumfa/lib/resolvers/
+-rw-r--r--   0 runner    (1001) docker     (127)     7221 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/resolvers/HTTPResolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56725 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/resolvers/LDAPIdResolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15166 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/resolvers/PasswdIdResolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10885 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/resolvers/SCIMIdResolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28267 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/resolvers/SQLIdResolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8590 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/resolvers/UserIdResolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/resolvers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.144086 edumfa-1.5.0/edumfa/lib/security/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13784 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/security/aeshsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16464 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/security/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14478 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/security/encryptkey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.144086 edumfa-1.5.0/edumfa/lib/security/password/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/security/password/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/serviceid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.148087 edumfa-1.5.0/edumfa/lib/smsprovider/
+-rw-r--r--   0 runner    (1001) docker     (127)     9043 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/smsprovider/FirebaseProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11897 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/smsprovider/HttpMessageToUidProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12084 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/smsprovider/HttpSMSProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12565 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/smsprovider/SMSProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/smsprovider/ScriptSMSProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4235 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/smsprovider/SipgateSMSProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6344 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/smsprovider/SmppSMSProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5552 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/smsprovider/SmtpSMSProvider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/smsprovider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13922 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/smtpserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4502 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/sqlutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5206 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/subscriptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.148087 edumfa-1.5.0/edumfa/lib/task/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/task/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/task/eventcounter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3539 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/task/simplestats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    96866 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68419 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokenclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokengroup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.156087 edumfa-1.5.0/edumfa/lib/tokens/
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/HMAC.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/applicationspecificpasswordtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25837 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/certificatetoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8437 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/daplugtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16746 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/daypasswordtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22719 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/emailtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18983 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/foureyestoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33207 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/hotptoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15903 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/indexedsecrettoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5155 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/mOTP.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/motptoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14133 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/ocra.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10863 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/ocratoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5179 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/papertoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6723 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/passwordtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46777 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/pushtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14249 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/questionnairetoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22143 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/radiustoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5709 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/registrationtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12204 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/remotetoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25368 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/smstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5253 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/spasstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5806 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/sshkeytoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8130 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/tantoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19949 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/tiqrtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27633 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/totptoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9775 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/u2f.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23127 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/u2ftoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5717 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/vasco.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7039 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/vascotoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    89138 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/webauthn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    66614 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/webauthntoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8523 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/yubicotoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16984 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/tokens/yubikeytoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30149 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9668 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/usercache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.156087 edumfa-1.5.0/edumfa/lib/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)    55043 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/utils/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3965 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/lib/utils/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    71279 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (127)   121289 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.156087 edumfa-1.5.0/edumfa/static/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8220 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/app.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.104086 edumfa-1.5.0/edumfa/static/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.096086 edumfa-1.5.0/edumfa/static/components/audit/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.156087 edumfa-1.5.0/edumfa/static/components/audit/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/audit/controllers/auditControllers.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.156087 edumfa-1.5.0/edumfa/static/components/audit/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     2038 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/audit/factories/audit.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.156087 edumfa-1.5.0/edumfa/static/components/audit/states/
+-rw-r--r--   0 runner    (1001) docker     (127)     1902 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/audit/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.156087 edumfa-1.5.0/edumfa/static/components/audit/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/audit/views/audit.html
+-rw-r--r--   0 runner    (1001) docker     (127)    11055 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/audit/views/audit.log.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.096086 edumfa-1.5.0/edumfa/static/components/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.156087 edumfa-1.5.0/edumfa/static/components/components/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/components/controllers/componentControllers.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.156087 edumfa-1.5.0/edumfa/static/components/components/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/components/factories/component.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.156087 edumfa-1.5.0/edumfa/static/components/components/states/
+-rw-r--r--   0 runner    (1001) docker     (127)     1955 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/components/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.156087 edumfa-1.5.0/edumfa/static/components/components/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/components/views/component.clienttype.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/components/views/component.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.096086 edumfa-1.5.0/edumfa/static/components/config/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.160087 edumfa-1.5.0/edumfa/static/components/config/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)    50570 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/controllers/configControllers.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3648 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/controllers/eduMfaServerController.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11316 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/controllers/eventController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3236 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/controllers/ldapMachineResolverController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/controllers/periodicTaskController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/controllers/radiusServerController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3044 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/controllers/serviceidController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4843 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/controllers/smsgatewayController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/controllers/smtpServerController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/controllers/tokengroupController.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.160087 edumfa-1.5.0/edumfa/static/components/config/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)    32353 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/factories/config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.160087 edumfa-1.5.0/edumfa/static/components/config/states/
+-rw-r--r--   0 runner    (1001) docker     (127)    19924 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.172087 edumfa-1.5.0/edumfa/static/components/config/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.caconnectors.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6518 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.caconnectors.local.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6204 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.caconnectors.microsoft.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.edumfaserver.edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.edumfaserver.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)    15020 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.events.details.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.events.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3586 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.events.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1890 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.machineresolvers.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.mresolvers.hosts.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8217 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.mresolvers.ldap.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.mresolvers.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7503 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.periodictasks.details.html
+-rw-r--r--   0 runner    (1001) docker     (127)      872 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.periodictasks.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2163 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.periodictasks.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)    22234 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.policies.details.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.policies.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.policies.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4469 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.radius.edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.radius.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.realms.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6002 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.realms.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2248 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.resolvers.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.resolvers.http.html
+-rw-r--r--   0 runner    (1001) docker     (127)    14914 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.resolvers.ldap.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.resolvers.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.resolvers.passwd.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3342 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.resolvers.scim.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10128 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.resolvers.sql.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.serviceid.edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.serviceid.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.smsgateway.edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.smsgateway.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.smtp.edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.smtp.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.system.doc.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8912 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.system.edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)    13600 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.system.html
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.token.daypassword.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.token.email.html
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.token.hotp.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.token.question.html
+-rw-r--r--   0 runner    (1001) docker     (127)      639 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.token.radius.html
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.token.remote.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.token.sms.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.token.tiqr.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.token.totp.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.token.u2f.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.token.webauthn.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.token.yubico.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.token.yubikey.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.tokengroup.edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.tokengroup.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/config.tokens.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/config/views/dialog.confirm_delete.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.100086 edumfa-1.5.0/edumfa/static/components/dashboard/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.172087 edumfa-1.5.0/edumfa/static/components/dashboard/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)     8518 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/dashboard/controllers/dashboardControllers.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.172087 edumfa-1.5.0/edumfa/static/components/dashboard/states/
+-rw-r--r--   0 runner    (1001) docker     (127)     1554 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/dashboard/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.172087 edumfa-1.5.0/edumfa/static/components/dashboard/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     8881 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/dashboard/views/dashboard.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.100086 edumfa-1.5.0/edumfa/static/components/dialogs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.172087 edumfa-1.5.0/edumfa/static/components/dialogs/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/dialogs/views/dialog.about.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/dialogs/views/dialog.autocreate_realm.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1878 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/dialogs/views/dialog.lock.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/dialogs/views/dialog.no.token.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4006 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/dialogs/views/dialog.welcome.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.100086 edumfa-1.5.0/edumfa/static/components/directives/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.172087 edumfa-1.5.0/edumfa/static/components/directives/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)    19746 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/directives/controllers/directives.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.176087 edumfa-1.5.0/edumfa/static/components/directives/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/directives/views/directive.assigntoken.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/directives/views/directive.assignuser.html
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/directives/views/directive.attachmachine.html
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/directives/views/directive.attachtoken.html
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/directives/views/directive.csvdownload.html
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/directives/views/directive.filter.table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3462 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/directives/views/directive.policyconditions.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/directives/views/directive.tokendata.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.176087 edumfa-1.5.0/edumfa/static/components/filters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/filters/filters.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.100086 edumfa-1.5.0/edumfa/static/components/login/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.176087 edumfa-1.5.0/edumfa/static/components/login/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)    30344 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/login/controllers/loginControllers.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.176087 edumfa-1.5.0/edumfa/static/components/login/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/login/factories/auth.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/login/factories/u2f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5077 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/login/factories/webauthn.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.176087 edumfa-1.5.0/edumfa/static/components/login/states/
+-rw-r--r--   0 runner    (1001) docker     (127)     2564 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/login/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.176087 edumfa-1.5.0/edumfa/static/components/login/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/login/views/enter-response.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/login/views/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/login/views/offline.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/login/views/pinchange.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.100086 edumfa-1.5.0/edumfa/static/components/machine/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.176087 edumfa-1.5.0/edumfa/static/components/machine/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/machine/controllers/machineController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/machine/controllers/machineDetailsController.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.176087 edumfa-1.5.0/edumfa/static/components/machine/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/machine/factories/machine.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.176087 edumfa-1.5.0/edumfa/static/components/machine/states/
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/machine/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.180087 edumfa-1.5.0/edumfa/static/components/machine/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     7085 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/machine/views/machine.details.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/machine/views/machine.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/machine/views/machine.list.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.100086 edumfa-1.5.0/edumfa/static/components/recovery/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.180087 edumfa-1.5.0/edumfa/static/components/recovery/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/recovery/controllers/recoveryControllers.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.180087 edumfa-1.5.0/edumfa/static/components/recovery/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/recovery/factories/recoveryFactory.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.180087 edumfa-1.5.0/edumfa/static/components/recovery/states/
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/recovery/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.180087 edumfa-1.5.0/edumfa/static/components/recovery/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/recovery/views/recovery.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/recovery/views/recovery.reset.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.100086 edumfa-1.5.0/edumfa/static/components/register/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.180087 edumfa-1.5.0/edumfa/static/components/register/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/register/controllers/registerControllers.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.180087 edumfa-1.5.0/edumfa/static/components/register/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/register/factories/registerFactory.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.180087 edumfa-1.5.0/edumfa/static/components/register/states/
+-rw-r--r--   0 runner    (1001) docker     (127)     1656 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/register/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.180087 edumfa-1.5.0/edumfa/static/components/register/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     4193 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/register/views/register.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.104086 edumfa-1.5.0/edumfa/static/components/token/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.180087 edumfa-1.5.0/edumfa/static/components/token/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)     3020 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/controllers/tokenApplicationsController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2030 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/controllers/tokenChallengesController.js
+-rw-r--r--   0 runner    (1001) docker     (127)    29864 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/controllers/tokenControllers.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17169 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/controllers/tokenDetailController.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/controllers/tokenGetSerialController.js
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/controllers/tokenLostController.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.180087 edumfa-1.5.0/edumfa/static/components/token/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)    12956 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/factories/token.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1515 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/factories/validate.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.180087 edumfa-1.5.0/edumfa/static/components/token/states/
+-rw-r--r--   0 runner    (1001) docker     (127)     4761 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.192087 edumfa-1.5.0/edumfa/static/components/token/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/dialog.ask_token_delete.html
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.applications.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.applications.offline.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2714 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.applications.ssh.html
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.assign.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.challenges.html
+-rw-r--r--   0 runner    (1001) docker     (127)    32395 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.details.html
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.display.apps.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.4eyes.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.applspec.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.certificate.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.daypassword.html
+-rw-r--r--   0 runner    (1001) docker     (127)      981 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.email.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.hotp.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10466 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.html
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.indexedsecret.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1555 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.motp.html
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.paper.html
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.push.html
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.question.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.radius.html
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.registration.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.remote.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.sms.html
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.spass.html
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.sshkey.html
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.tan.html
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.tiqr.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3185 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.totp.html
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.u2f.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.vasco.html
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.webauthn.html
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.yubico.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1676 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.yubikey.html
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enrolled.applspec.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enrolled.certificate.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enrolled.daypassword.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enrolled.hotp.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enrolled.motp.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enrolled.paper.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enrolled.push.html
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enrolled.registration.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enrolled.tan.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enrolled.tiqr.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enrolled.totp.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enrolled.u2f.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1729 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.enrolled.webauthn.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3826 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.getserial.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7095 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5263 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.import.html
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/token/views/token.lost.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.192087 edumfa-1.5.0/edumfa/static/components/translation/
+-rw-r--r--   0 runner    (1001) docker     (127)   557560 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/translation/translations.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.104086 edumfa-1.5.0/edumfa/static/components/user/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.192087 edumfa-1.5.0/edumfa/static/components/user/controllers/
+-rw-r--r--   0 runner    (1001) docker     (127)    19169 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/user/controllers/userControllers.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.192087 edumfa-1.5.0/edumfa/static/components/user/factories/
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/user/factories/user.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.192087 edumfa-1.5.0/edumfa/static/components/user/states/
+-rw-r--r--   0 runner    (1001) docker     (127)     3003 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/user/states/states.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.196087 edumfa-1.5.0/edumfa/static/components/user/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/user/views/dialog.ask_user_delete.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/user/views/user.add.dynamic.form.fields.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/user/views/user.add.html
+-rw-r--r--   0 runner    (1001) docker     (127)     8616 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/user/views/user.details.html
+-rw-r--r--   0 runner    (1001) docker     (127)     4158 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/user/views/user.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/user/views/user.list.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2731 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/components/user/views/user.password.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.104086 edumfa-1.5.0/edumfa/static/contrib/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.196087 edumfa-1.5.0/edumfa/static/contrib/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     3304 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/css/angular-inform.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3424 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/css/angular-inform.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)    25682 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/css/bootstrap-theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)    48005 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/css/bootstrap-theme.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)   145933 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/css/bootstrap.css
+-rw-r--r--   0 runner    (1001) docker     (127)   390887 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/css/bootstrap.css.map
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/css/hotkeys.css
+-rw-r--r--   0 runner    (1001) docker     (127)     7021 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/css/isteven-multi-select.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.200087 edumfa-1.5.0/edumfa/static/contrib/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    20127 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   108738 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    45404 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    23424 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    18028 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.204087 edumfa-1.5.0/edumfa/static/contrib/js/
+-rw-r--r--   0 runner    (1001) docker     (127)     4944 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/js/angular-inform.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/js/angular-inform.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)  1377909 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/js/angular.js
+-rw-r--r--   0 runner    (1001) docker     (127)    75484 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/js/bootstrap.js
+-rw-r--r--   0 runner    (1001) docker     (127)    53486 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/js/hotkeys.js
+-rw-r--r--   0 runner    (1001) docker     (127)   288580 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/js/jquery.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.208087 edumfa-1.5.0/edumfa/static/contrib/js/ngmodules/
+-rw-r--r--   0 runner    (1001) docker     (127)    32388 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/js/ngmodules/angular-gettext.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16000 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/js/ngmodules/angular-idle.js
+-rw-r--r--   0 runner    (1001) docker     (127)    33197 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/js/ngmodules/angular-sanitize.js
+-rw-r--r--   0 runner    (1001) docker     (127)   487964 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/js/ngmodules/angular-ui-router.js
+-rw-r--r--   0 runner    (1001) docker     (127)   760134 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/js/ngmodules/angular-ui-router.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)    53338 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/js/ngmodules/isteven-multi-select.js
+-rw-r--r--   0 runner    (1001) docker     (127)    81683 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/js/ngmodules/ng-file-upload.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20905 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/js/u2f-api.js
+-rw-r--r--   0 runner    (1001) docker     (127)   276562 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/js/ui-bootstrap-tpls.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.208087 edumfa-1.5.0/edumfa/static/contrib/js/webauthn-client/
+-rw-r--r--   0 runner    (1001) docker     (127)    20759 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/contrib/js/webauthn-client/edumfa-webauthn.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.208087 edumfa-1.5.0/edumfa/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/css/baseline.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/css/content.css
+-rw-r--r--   0 runner    (1001) docker     (127)    24602 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/css/eduMFA-logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/css/highlight.css
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/css/menu.css
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/css/papertoken.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1098 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/css/signin.css
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/css/table-ui.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.208087 edumfa-1.5.0/edumfa/static/customize/
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/customize/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.212087 edumfa-1.5.0/edumfa/static/img/
+-rw-r--r--   0 runner    (1001) docker     (127)   195931 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/img/FIDO-U2F-Security-Key-444x444.png
+-rw-r--r--   0 runner    (1001) docker     (127)    47610 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/img/plugup.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   336777 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/img/solokeys.png
+-rw-r--r--   0 runner    (1001) docker     (127)   107999 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/img/u2fzero.png
+-rw-r--r--   0 runner    (1001) docker     (127)     8044 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.212087 edumfa-1.5.0/edumfa/static/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     6315 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/providers/errorMessageProvider.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/providers/versioningProvider.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.212087 edumfa-1.5.0/edumfa/static/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/templates/baseline.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/templates/cert_request_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/templates/deactivated.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3060 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/templates/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     7950 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/templates/footer.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/templates/header.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7838 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/templates/menu.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1797 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/templates/token_enrolled.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/static/update_contrib.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.108086 edumfa-1.5.0/edumfa/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.104086 edumfa-1.5.0/edumfa/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.212087 edumfa-1.5.0/edumfa/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    23376 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    84098 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.104086 edumfa-1.5.0/edumfa/translations/de/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.216087 edumfa-1.5.0/edumfa/translations/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    95309 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/de/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   127521 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/de/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.104086 edumfa-1.5.0/edumfa/translations/es/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.216087 edumfa-1.5.0/edumfa/translations/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    81449 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   118619 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.104086 edumfa-1.5.0/edumfa/translations/fr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.216087 edumfa-1.5.0/edumfa/translations/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    53719 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/fr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   104451 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/fr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.104086 edumfa-1.5.0/edumfa/translations/it/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.216087 edumfa-1.5.0/edumfa/translations/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    26784 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/it/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    87343 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/it/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.108086 edumfa-1.5.0/edumfa/translations/nl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.216087 edumfa-1.5.0/edumfa/translations/nl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    85965 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/nl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   120848 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/nl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.108086 edumfa-1.5.0/edumfa/translations/pl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.216087 edumfa-1.5.0/edumfa/translations/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/pl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    73216 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/pl/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.108086 edumfa-1.5.0/edumfa/translations/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.220087 edumfa-1.5.0/edumfa/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    78400 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/pt_BR/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   115604 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/pt_BR/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.108086 edumfa-1.5.0/edumfa/translations/ro/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.220087 edumfa-1.5.0/edumfa/translations/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    10507 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/ro/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    79882 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/ro/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.108086 edumfa-1.5.0/edumfa/translations/ru/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.220087 edumfa-1.5.0/edumfa/translations/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    33313 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/ru/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    96048 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/ru/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.108086 edumfa-1.5.0/edumfa/translations/si/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.220087 edumfa-1.5.0/edumfa/translations/si/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/si/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)    73291 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/si/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.108086 edumfa-1.5.0/edumfa/translations/tr/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.220087 edumfa-1.5.0/edumfa/translations/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    82030 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/tr/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   117846 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/tr/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.108086 edumfa-1.5.0/edumfa/translations/zh_Hans/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.220087 edumfa-1.5.0/edumfa/translations/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    68507 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/zh_Hans/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   104457 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/zh_Hans/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.108086 edumfa-1.5.0/edumfa/translations/zh_Hant/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.220087 edumfa-1.5.0/edumfa/translations/zh_Hant/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)    70327 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/zh_Hant/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)   105843 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/translations/zh_Hant/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.224087 edumfa-1.5.0/edumfa/webui/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/webui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/webui/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9124 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa/webui/login.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    62952 2024-04-02 12:57:39.000000 edumfa-1.5.0/edumfa-manage
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.280088 edumfa-1.5.0/edumfa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8537 2024-04-02 12:57:52.000000 edumfa-1.5.0/edumfa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    32602 2024-04-02 12:57:52.000000 edumfa-1.5.0/edumfa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:57:52.000000 edumfa-1.5.0/edumfa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 12:57:51.000000 edumfa-1.5.0/edumfa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-02 12:57:52.000000 edumfa-1.5.0/edumfa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-02 12:57:52.000000 edumfa-1.5.0/edumfa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.224087 edumfa-1.5.0/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/README
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/alembic.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     3509 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/script.py.mako
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.236087 edumfa-1.5.0/migrations/versions/
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/006d4747f858_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/00762b3f7a60_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/0c7123345224_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6702 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/0d011e94a8e8_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/140ba0ca4f07_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/145ce80decd_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/14a1bcb10018_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/19f727d285e2_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/1a0710df148b_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/1a69e5e5e2ac_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/1edda52b619f_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/204d8d4f351e_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/205bda834127_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/20969b4cbf06_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/2118e566df16_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/2181294eed0b_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/22558d9f3178_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/239995464c48_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/2551ee982544_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/2ac117d0a6f5_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/2c9430cfc66b_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/307a4fbe8a05_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/3236a1abf1c6_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/3429d523e51f_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/36428afb2457_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/37e6b49fc686_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/3ae3c668f444_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/3ba618f6b820_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/3c6e9dd7fbac_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/3d7f8b29cbb1_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/3f7e8583ea2_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/4023571658f8_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/4238eac8ccab_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/449903fb6e35_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10211 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/48ee74b8a7c8_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/49a04e560d96_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/4a0aec37e7cf_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/4d9178fa8336_.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19377 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/4f32a4e1bf33_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/50adc980d625_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2009 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/5402fd96fbca_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/58e4f7ebb705_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/59ef3e03bc62_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3197 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/5cb310101a1f_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/631ec59e1ca6_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/849170064430_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/86f40f535d7c_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/888b56ed5dcb_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/89e57ed16379_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1200 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/8d40dbcfda25_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/9155f0d3d028_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/a28f2733897b_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/a63df077051a_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/a7e91b18a460_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/b9131d0686eb_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/cb6d7b7bae63_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3034 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/d2ae8e54b628_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      360 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/d3c0f0403a84_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/d415d490eb05_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/d5870fd2f2a4_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/d6b40a745e5_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/d756b34061ff_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/dceb6cd3c41e_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3059 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/e360c56bcf8c_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/e5cbeb7c177_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/ef29ba43e290_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/fa07bd604a75.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/fabcf24d9304_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-02 12:57:39.000000 edumfa-1.5.0/migrations/versions/ff26585932ec_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-04-02 12:57:39.000000 edumfa-1.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-02 12:57:52.284088 edumfa-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     5298 2024-04-02 12:57:39.000000 edumfa-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.260087 edumfa-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9966 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28189 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/ldap3mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/mscamock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6848 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/pkcs11mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/queuemock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3992 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/radiusmock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/redismock.py
+-rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5066 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/smppmock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7690 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/smtpmock.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35694 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_2stepinit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20710 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48917 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9180 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_caconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_clienttype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_edumfaserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35517 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)   193396 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_lib_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19077 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_lib_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7403 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_machineresolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38769 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_machines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16166 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_machines_serviceid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_offline_no_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13094 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_periodictask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36128 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26177 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_push_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6776 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_radiusserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8398 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_register.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76125 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4664 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_serviceids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14259 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_smsgateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_smtpserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62186 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)   195170 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4649 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_tokengroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21541 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_ttype.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29544 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_u2f.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33114 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)   302927 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_api_validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9183 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45689 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_db_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9078 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_applications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23056 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7745 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_authcache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31138 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_caconnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_challenges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5542 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_clientapplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11734 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5797 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35302 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13267 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_edumfaserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_eventhandler_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60534 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_eventhandler_usernotification.py
+-rw-r--r--   0 runner    (1001) docker     (127)   113340 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_framework.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29545 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_importotp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_lifecycle.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7147 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_machine_resolver_ldap.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8642 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_machines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9378 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_machinetokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5020 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_monitoringstats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20699 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_periodictask.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75326 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36401 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_policydecorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_pooling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3604 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_queue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4663 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_radiusserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3615 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_realm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_recovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)   123815 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_serviceid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32074 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_smsprovider.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10949 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_smtpserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4110 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_sqlutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_task_eventcounter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3659 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_task_simplestats.py
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97908 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38128 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokenclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2261 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokengroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36699 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokens_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25260 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokens_daplug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27651 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokens_daypassword.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21128 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokens_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokens_foureyes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34350 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokens_hotp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokens_indexedsecret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7183 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokens_motp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokens_paper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1858 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokens_passwordtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75419 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokens_push.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokens_questionnaire.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16576 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokens_radius.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokens_registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9417 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokens_remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20806 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokens_sms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokens_spass.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5902 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokens_ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokens_tan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31214 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokens_tiqr.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34079 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokens_totp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22536 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokens_u2f.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10413 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokens_vasco.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50926 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokens_webauthn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokens_yubico.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10230 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_tokens_yubikey.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22413 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26644 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_usercache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45888 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5566 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_lib_utils_compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38033 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_mock_ldap3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_resolver_realm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6367 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_ui_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/test_ui_login.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.268087 edumfa-1.5.0/tests/testdata/
+-rw-r--r--   0 runner    (1001) docker     (127)   195931 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/FIDO-U2F-Security-Key-444x444.png
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/NetKnights.pem
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.108086 edumfa-1.5.0/tests/testdata/altstatic/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.268087 edumfa-1.5.0/tests/testdata/altstatic/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/altstatic/templates/testui.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.268087 edumfa-1.5.0/tests/testdata/attestation/
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/attestation/yubico.pem
+-rw-r--r--   0 runner    (1001) docker     (127)    16384 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/audit.sqlite
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.268087 edumfa-1.5.0/tests/testdata/ca/
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/ca/cacert.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/ca/cakey.pem
+-rw-r--r--   0 runner    (1001) docker     (127)    15874 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/ca/index.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/ca/index.txt.attr
+-rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/ca/openssl.cnf
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/ca/serial
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/ca/templates.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4109 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/dictionary
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/does_not_exist
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/emailtemplate.html
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/empty.oath
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/enckey
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/enckey.enc
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/fancytoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/firebase-test.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/google-services.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.272087 edumfa-1.5.0/tests/testdata/gpg/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/gpg/public.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/gpg/pubring.gpg
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/gpg/random_seed
+-rw-r--r--   0 runner    (1001) docker     (127)     2509 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/gpg/secring.gpg
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/gpg/trustdb.gpg
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/hosts
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/import.oath
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/import.oath.asc
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/jwt_sign.key
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/logging.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/logging.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/logging_broken.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.272087 edumfa-1.5.0/tests/testdata/msca-connector/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/msca-connector/ca.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/msca-connector/privacyidea-encrypted.key
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/msca-connector/privacyidea.key
+-rw-r--r--   0 runner    (1001) docker     (127)     1996 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/msca-connector/privacyidea.pem
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/ocra.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/passwd
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/passwd-duplicate-name
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/passwords
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/policy.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/policy_empty_file.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/private.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/pskc-aes.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/pskc-password.xml
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/public.pem
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/pw-2nd-resolver
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.272087 edumfa-1.5.0/tests/testdata/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       19 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/scripts/fail.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       20 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/scripts/ls.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)       19 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/scripts/success.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/test.sub
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/test2.sub
+-rw-r--r--   0 runner    (1001) docker     (127)     2048 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/testuser-api.sqlite
+-rw-r--r--   0 runner    (1001) docker     (127)     5120 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/testuser.sqlite
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/testusercache.sqlite
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.272087 edumfa-1.5.0/tests/testdata/trusted_attestation_roots/
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/trusted_attestation_roots/solokeys_device_attestation_ca.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/trusted_attestation_roots/yubico_u2f_device_attestation_ca.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     4192 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/yubico-oath-long.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/yubico-oath.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-02 12:57:39.000000 edumfa-1.5.0/tests/testdata/yubico.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 12:57:52.280088 edumfa-1.5.0/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      768 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/creategoogleauthenticator-file
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2551 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-authorizedkeys
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1766 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-convert-base32.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2876 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-convert-token
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-convert-token.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3230 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-convert-xml-to-csv
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2440 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-create-ad-users
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-create-ad-users.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1940 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-create-certificate
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-create-certificate.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1985 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-create-pwidresolver-user
+-rw-r--r--   0 runner    (1001) docker     (127)     1192 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-create-pwidresolver-user.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1608 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-create-sqlidresolver-user
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-create-sqlidresolver-user.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)      795 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-create-userdb
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-create-userdb.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6703 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-cron
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7030 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-diag
+-rwxr-xr-x   0 runner    (1001) docker     (127)     6991 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-expired-users
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1354 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-export-edumfa-counter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4514 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-export-linotp-counter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3719 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-fetchssh
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-fetchssh.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2500 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-fix-access-rights
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-fix-access-rights.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3541 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-get-serial
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4940 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-get-unused-tokens
+-rwxr-xr-x   0 runner    (1001) docker     (127)    25361 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-migrate-linotp.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2525 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-pip-update
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-pip-update.1
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5761 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-queue-huey
+-rwxr-xr-x   0 runner    (1001) docker     (127)      643 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-schema-upgrade
+-rwxr-xr-x   0 runner    (1001) docker     (127)    11397 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-standalone
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8176 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-sync-owncloud.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    31889 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-token-janitor
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3746 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-update-counter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5391 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-update-linotp-counter.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5471 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-user-action
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3674 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/edumfa-usercache-cleanup
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1476 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/getgooglecodes
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3049 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/reset-edumfa
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-02 12:57:39.000000 edumfa-1.5.0/tools/ssha.py
```

### Comparing `edumfa-1.4.0/AUTHORS.md` & `edumfa-1.5.0/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/LICENSE` & `edumfa-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/PKG-INFO` & `edumfa-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edumfa
-Version: 1.4.0
+Version: 1.5.0
 Summary: eduMFA: identity, multifactor authentication (OTP), authorization, audit
 Home-page: https://www.edumfa.io
 Author: edumfa.io
 Author-email: edumfa@listserv.dfn.de
 License: AGPLv3
 Keywords: OTP,two factor authentication,management,security
 Classifier: Framework :: Flask
```

### Comparing `edumfa-1.4.0/README.rst` & `edumfa-1.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/deploy/apache/sites-available/edumfa.conf` & `edumfa-1.5.0/deploy/apache/sites-available/edumfa.conf`

 * *Files 18% similar despite different names*

```diff
@@ -11,47 +11,58 @@
 		AllowOverride None
 	</Directory>
 
         # Yubico servers use /wsapi/2.0/verify as the path in the
         # validation URL. Some tools (e.g. Kolab 2fa) let the 
         # user/admin change the api host, but not the rest of
         # the URL. Uncomment the following two lines to reroute 
-        # the api URL internally to privacyideas /ttype/yubikey.
+        # the api URL internally to eduMFAs /ttype/yubikey.
         #RewriteEngine  on
         #RewriteRule    "^/wsapi/2.0/verify"  "/ttype/yubikey" [PT]
 
 	# We can run several instances on different paths with different configurations
 	WSGIScriptAlias /      /etc/edumfa/edumfaapp.wsgi
+	#WSGIScriptAlias /instance1      /home/edumfa/src/edumfa/deploy/edumfaapp1.wsgi
+	#WSGIScriptAlias /instance2      /home/edumfa/src/edumfa/deploy/edumfaapp2.wsgi
+	#WSGIScriptAlias /instance3      /home/edumfa/src/edumfa/deploy/edumfaapp3.wsgi
 	#
-	# The daemon is running as user 'privacyidea'
+	# The daemon is running as user 'edumfa'
 	# This user should have access to the encKey database encryption file
 	WSGIDaemonProcess edumfa processes=1 threads=15 display-name=%{GROUP} user=edumfa
 	WSGIProcessGroup edumfa
+	WSGIApplicationGroup %{GLOBAL}
 	WSGIPassAuthorization On
 
 	ErrorLog /var/log/apache2/error.log
 
 	LogLevel warn
 	# Do not use %q! This will reveal all parameters, including setting PINs and Keys!
 	# Using SSL_CLINET_S_DN_CN will show you, which administrator did what task
-	LogFormat "%h %l %u %t %>s \"%m %U %H\"  %b \"%{Referer}i\" \"%{User-agent}i\"" edumfa
-	CustomLog /var/log/apache2/ssl_access.log edumfa
+	LogFormat "%h %l %u %t %>s \"%m %U %H\"  %b \"%{Referer}i\" \"%{User-agent}i\"" eduMFA
+	CustomLog /var/log/apache2/ssl_access.log eduMFA
 
 	#   SSL Engine Switch:
 	#   Enable/Disable SSL for this virtual host.
 	SSLEngine on
-        SSLProtocol ALL -SSLv2 -SSLv3
-	SSLHonorCipherOrder On 
-	SSLCipherSuite ECDH+AESGCM:DH+AESGCM:ECDH+AES256:DH+AES256:ECDH+AES128:DH+AES:RSA+AESGCM:RSA+AES:!aNULL:!MD5:!DSS
+        SSLProtocol ALL -SSLv2 -SSLv3 -TLSv1 -TLSv1.1
+	SSLHonorCipherOrder On
+	SSLCipherSuite          ECDHE-ECDSA-AES256-GCM-SHA384:ECDHE-RSA-AES256-GCM-SHA384:ECDHE-ECDSA-CHACHA20-POLY1305:ECDHE-RSA-CHACHA20-POLY1305:ECDHE-ECDSA-AES128-GCM-SHA256:ECDHE-RSA-AES128-GCM-SHA256:ECDHE-ECDSA-AES256-SHA384:ECDHE-RSA-AES256-SHA384:ECDHE-ECDSA-AES128-SHA256:ECDHE-RSA-AES128-SHA256
+	SSLCompression          off
+	SSLSessionTickets       off
+
+	# You can turn on HSTS. But as long as you have no valid certificate, this can cause
+	# some trouble
+	# HSTS (mod_headers is required) (1209600 seconds = 2 weeks)
+	# Header always set Strict-Transport-Security "max-age=1209600"
 
 
 	#   If both key and certificate are stored in the same file, only the
 	#   SSLCertificateFile directive is needed.
-	SSLCertificateFile    /etc/ssl/certs/edumfa.pem
-	SSLCertificateKeyFile /etc/ssl/private/edumfa.key
+	SSLCertificateFile    /etc/ssl/certs/edumfaserver.pem
+	SSLCertificateKeyFile /etc/ssl/private/edumfaserver.key
 
 	<FilesMatch "\.(cgi|shtml|phtml|php)$">
 		SSLOptions +StdEnvVars
 	</FilesMatch>
 	<Directory /usr/lib/cgi-bin>
 		SSLOptions +StdEnvVars
 	</Directory>
@@ -60,18 +71,17 @@
 		downgrade-1.0 force-response-1.0
 
 
 </VirtualHost>
 
 # If you want to forward http request to https enable the
 # following virtual host.
-#<VirtualHost _default_:80>
-#	# This will enable the Rewrite capabilities
-#	RewriteEngine On
-#
-#	# This checks to make sure the connection is not already HTTPS
-#	RewriteCond %{HTTPS} !=on
-#	RewriteRule ^/?(.*) https://%{SERVER_NAME}/$1 [R,L]
-#</VirtualHost>
+<VirtualHost _default_:80>
+	# This will enable the Rewrite capabilities
+	RewriteEngine On
+
+	# This checks to make sure the connection is not already HTTPS
+	RewriteCond %{HTTPS} !=on
+	RewriteRule ^/?(.*) https://%{SERVER_NAME}/$1 [R,L]
+</VirtualHost>
 
 # vim: syntax=apache ts=4 sw=4 sts=4 sr noet
-
```

### Comparing `edumfa-1.4.0/deploy/docker-compose-example.yml` & `edumfa-1.5.0/deploy/docker-compose-example.yml`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/deploy/docker-example/edumfa-policy.conf` & `edumfa-1.5.0/deploy/docker-example/edumfa-policy.conf`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
                       'resolver': [],
                       'scope': 'webui',
                       'time': '',
                       'user': []},
                   {   'action': {   'webauthn_authenticator_attestation_form': 'none',
                                     'webauthn_authenticator_attestation_level': 'none',
                                     'webauthn_relying_party_id': 'edumfa-test.local',
-                                    'webauthn_relying_party_name': 'pi.edumfa-test.local',
+                                    'webauthn_relying_party_name': 'edumfa.edumfa-test.local',
                                     'webauthn_resident_key': 'preferred',
                                     'webauthn_user_verification_requirement': 'preferred'},
                       'active': True,
                       'adminrealm': [],
                       'adminuser': [],
                       'check_all_resolvers': False,
                       'client': [],
```

### Comparing `edumfa-1.4.0/deploy/docker-example/edumfa.cfg` & `edumfa-1.5.0/deploy/docker-example/edumfa.cfg`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/deploy/docker-setup.sh` & `edumfa-1.5.0/deploy/docker-setup.sh`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/deploy/edumfa/dictionary` & `edumfa-1.5.0/deploy/edumfa/dictionary`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/deploy/logging.cfg` & `edumfa-1.5.0/deploy/logging.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Rollover the logfile at midnight
 class=logging.handlers.RotatingFileHandler
 formatter=detail
 level=DEBUG
 args=('/var/log/edumfa/edumfa.log')
 # Limit log file to 10MB
 # keep 14 backups of the log file
-#args=('/var/log/privacyidea/privacyidea.log', 'a', 10000000, 14)
+#args=('/var/log/edumfa/edumfa.log', 'a', 10000000, 14)
 
 [loggers]
 keys=root,edumfa
 
 [logger_edumfa]
 handlers=file
 qualname=edumfa
```

### Comparing `edumfa-1.4.0/deploy/nginx/sites-available/edumfa` & `edumfa-1.5.0/deploy/nginx/sites-available/edumfa`

 * *Files 4% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 #}
 
 server {
         listen 443 ssl;
         server_name     $hostname;
         ssl_certificate /etc/ssl/certs/edumfa-bundle.crt;
         ssl_certificate_key /etc/ssl/private/edumfa.key;
-	ssl_prefer_server_ciphers On; 
-	ssl_protocols TLSv1 TLSv1.1 TLSv1.2; 
+	ssl_prefer_server_ciphers On;
+	ssl_protocols TLSv1 TLSv1.1 TLSv1.2;
 	ssl_ciphers ECDH+AESGCM:DH+AESGCM:ECDH+AES256:DH+AES256:ECDH+AES128:DH+AES:RSA+AESGCM:RSA+AES:!aNULL:!MD5:!DSS;
 
         access_log      /var/log/edumfa/access.log;
         error_log       /var/log/edumfa/error.log info;
 
         location / {
                 uwsgi_pass      unix:/run/uwsgi/app/edumfa/edumfa.socket;
@@ -26,12 +26,12 @@
                 uwsgi_param SCRIPT_NAME '';
         }
 
         # Yubico servers use /wsapi/2.0/verify as the path in the
         # validation URL. Some tools (e.g. Kolab 2fa) let the 
         # user/admin change the api host, but not the rest of
         # the URL. Uncomment the following two lines to reroute 
-        # the api URL internally to privacyideas /ttype/yubikey.
+        # the api URL internally to eduMFAs /ttype/yubikey.
         #rewrite ^/wsapi/2.0/verify(.*)  /ttype/yubikey$1 last;
 
 }
```

### Comparing `edumfa-1.4.0/edumfa/__init__.py` & `edumfa-1.5.0/edumfa/__init__.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/__init__.py` & `edumfa-1.5.0/edumfa/api/__init__.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/application.py` & `edumfa-1.5.0/edumfa/api/application.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/audit.py` & `edumfa-1.5.0/edumfa/api/audit.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/auth.py` & `edumfa-1.5.0/edumfa/api/auth.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/before_after.py` & `edumfa-1.5.0/edumfa/api/before_after.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/caconnector.py` & `edumfa-1.5.0/edumfa/api/caconnector.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/clienttype.py` & `edumfa-1.5.0/edumfa/api/clienttype.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/edumfaserver.py` & `edumfa-1.5.0/edumfa/api/edumfaserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/event.py` & `edumfa-1.5.0/edumfa/api/event.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/lib/decorators.py` & `edumfa-1.5.0/edumfa/api/lib/decorators.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/lib/policyhelper.py` & `edumfa-1.5.0/edumfa/api/lib/policyhelper.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 Like policies, that are supposed to read and pass parameters during enrollment of a token.
 """
 
 import logging
 from edumfa.lib.log import log_with
 from edumfa.lib.policy import Match, SCOPE, ACTION
 from edumfa.lib.error import PolicyError
+from edumfa.lib.tokens.webauthntoken import WEBAUTHNACTION
 
 log = logging.getLogger(__name__)
 
 
 @log_with(log)
 def get_init_tokenlabel_parameters(g, params=None, token_type="hotp", user_object=None):
     """
@@ -47,14 +48,20 @@
     params = params or {}
     label_pols = Match.user(g, scope=SCOPE.ENROLL, action=ACTION.TOKENLABEL,
                             user_object=user_object).action_values(unique=True, allow_white_space_in_action=True)
     if len(label_pols) == 1:
         # The policy was set, so we need to set the tokenlabel in the request.
         params[ACTION.TOKENLABEL] = list(label_pols)[0]
 
+    label_pols = Match.user(g, scope=SCOPE.ENROLL, action=WEBAUTHNACTION.TOKENLABEL,
+                            user_object=user_object).action_values(unique=True, allow_white_space_in_action=True)
+    if len(label_pols) == 1:
+        # The policy was set, so we need to set the tokenlabel in the request.
+        params[WEBAUTHNACTION.TOKENLABEL] = list(label_pols)[0]
+
     issuer_pols = Match.user(g, scope=SCOPE.ENROLL, action=ACTION.TOKENISSUER,
                              user_object=user_object).action_values(unique=True, allow_white_space_in_action=True)
     if len(issuer_pols) == 1:
         params[ACTION.TOKENISSUER] = list(issuer_pols)[0]
 
     imageurl_pols = Match.user(g, scope=SCOPE.ENROLL, action=ACTION.APPIMAGEURL,
                                user_object=user_object).action_values(unique=True, allow_white_space_in_action=True)
```

### Comparing `edumfa-1.4.0/edumfa/api/lib/postpolicy.py` & `edumfa-1.5.0/edumfa/api/lib/postpolicy.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/lib/prepolicy.py` & `edumfa-1.5.0/edumfa/api/lib/prepolicy.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/lib/utils.py` & `edumfa-1.5.0/edumfa/api/lib/utils.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/machine.py` & `edumfa-1.5.0/edumfa/api/machine.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/machineresolver.py` & `edumfa-1.5.0/edumfa/api/machineresolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/monitoring.py` & `edumfa-1.5.0/edumfa/api/monitoring.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/periodictask.py` & `edumfa-1.5.0/edumfa/api/periodictask.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/policy.py` & `edumfa-1.5.0/edumfa/api/policy.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/radiusserver.py` & `edumfa-1.5.0/edumfa/api/radiusserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/realm.py` & `edumfa-1.5.0/edumfa/api/realm.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/recover.py` & `edumfa-1.5.0/edumfa/api/recover.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/register.py` & `edumfa-1.5.0/edumfa/api/register.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/resolver.py` & `edumfa-1.5.0/edumfa/api/resolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/serviceid.py` & `edumfa-1.5.0/edumfa/api/serviceid.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/smsgateway.py` & `edumfa-1.5.0/edumfa/api/smsgateway.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/smtpserver.py` & `edumfa-1.5.0/edumfa/api/smtpserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/system.py` & `edumfa-1.5.0/edumfa/api/system.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/token.py` & `edumfa-1.5.0/edumfa/api/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,14 +158,15 @@
     :jsonparam 2stepinit: set to =1 in conjunction with genkey=1 if you want
                     a 2 step initialization process. Additional policies have to be set
                     see :ref:`2step_enrollment`.
     :jsonparam otpkeyformat: used to supply the OTP key in alternate formats, currently
                             hex or base32check (see :ref:`2step_enrollment`)
     :jsonparam rollover: Set this to 1 or true to indicate, that you want to rollover a token.
                     This is mandatory to rollover tokens, that are in the clientwait state.
+    :jsonparam info: string representation of a json object whose key-value pairs will be set as tokeninfo.
 
     :return: a json result with a boolean "result": true
 
     Depending on the token type there can be additional parameters.
     In the tokenclass you can see additional parameters in the method ``update``
     when looking for ``getParam`` functions.
 
@@ -1210,15 +1211,15 @@
 @log_with(log)
 def modify_tokeninfo_api(serial):
     """
     Modifies tokeninfo entries for a token. Already existing entries
     with the same key are overwritten, keys with null value are deleted
 
     :jsonparam dict info: dictionary with key value pairs. keys with null value are deleted. always make sure not to
-    : include keys with null value by accident!
+    include keys with null value by accident!
     :param serial: the serial number/identifier of the token
     :return: returns value=True in case at least one token matching the serial could be found
     :rtype: bool
     """
     tokeninfo = getParam(request.all_data, "info", required, allow_empty=False)
     count = 0
     if type(tokeninfo) is not dict:
```

### Comparing `edumfa-1.4.0/edumfa/api/tokengroup.py` & `edumfa-1.5.0/edumfa/api/tokengroup.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/ttype.py` & `edumfa-1.5.0/edumfa/api/ttype.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/user.py` & `edumfa-1.5.0/edumfa/api/user.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/api/validate.py` & `edumfa-1.5.0/edumfa/api/validate.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/app.py` & `edumfa-1.5.0/edumfa/app.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/config.py` & `edumfa-1.5.0/edumfa/config.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/__init__.py` & `edumfa-1.5.0/edumfa/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/applications/__init__.py` & `edumfa-1.5.0/edumfa/lib/applications/__init__.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/applications/base.py` & `edumfa-1.5.0/edumfa/lib/applications/base.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/applications/luks.py` & `edumfa-1.5.0/edumfa/lib/applications/luks.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/applications/offline.py` & `edumfa-1.5.0/edumfa/lib/applications/offline.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/applications/ssh.py` & `edumfa-1.5.0/edumfa/lib/applications/ssh.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/apps.py` & `edumfa-1.5.0/edumfa/lib/apps.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/audit.py` & `edumfa-1.5.0/edumfa/lib/audit.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/auditmodules/base.py` & `edumfa-1.5.0/edumfa/lib/auditmodules/base.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/auditmodules/containeraudit.py` & `edumfa-1.5.0/edumfa/lib/auditmodules/containeraudit.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/auditmodules/loggeraudit.py` & `edumfa-1.5.0/edumfa/lib/auditmodules/loggeraudit.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/auditmodules/sqlaudit.py` & `edumfa-1.5.0/edumfa/lib/auditmodules/sqlaudit.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/auth.py` & `edumfa-1.5.0/edumfa/lib/auth.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/authcache.py` & `edumfa-1.5.0/edumfa/lib/authcache.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/caconnector.py` & `edumfa-1.5.0/edumfa/lib/caconnector.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/caconnectors/baseca.py` & `edumfa-1.5.0/edumfa/lib/caconnectors/baseca.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/caconnectors/caservice_pb2.py` & `edumfa-1.5.0/edumfa/lib/caconnectors/caservice_pb2.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/caconnectors/caservice_pb2_grpc.py` & `edumfa-1.5.0/edumfa/lib/caconnectors/caservice_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/caconnectors/localca.py` & `edumfa-1.5.0/edumfa/lib/caconnectors/localca.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/caconnectors/msca.py` & `edumfa-1.5.0/edumfa/lib/caconnectors/msca.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/challenge.py` & `edumfa-1.5.0/edumfa/lib/challenge.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/challengeresponsedecorators.py` & `edumfa-1.5.0/edumfa/lib/challengeresponsedecorators.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/clientapplication.py` & `edumfa-1.5.0/edumfa/lib/clientapplication.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/config.py` & `edumfa-1.5.0/edumfa/lib/config.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/counter.py` & `edumfa-1.5.0/edumfa/lib/counter.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/crypto.py` & `edumfa-1.5.0/edumfa/lib/crypto.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/decorators.py` & `edumfa-1.5.0/edumfa/lib/decorators.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/edumfaserver.py` & `edumfa-1.5.0/edumfa/lib/edumfaserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/error.py` & `edumfa-1.5.0/edumfa/lib/error.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/event.py` & `edumfa-1.5.0/edumfa/lib/event.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/eventhandler/base.py` & `edumfa-1.5.0/edumfa/lib/eventhandler/base.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/eventhandler/counterhandler.py` & `edumfa-1.5.0/edumfa/lib/eventhandler/counterhandler.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/eventhandler/customuserattributeshandler.py` & `edumfa-1.5.0/edumfa/lib/eventhandler/customuserattributeshandler.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/eventhandler/federationhandler.py` & `edumfa-1.5.0/edumfa/lib/eventhandler/federationhandler.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/eventhandler/logginghandler.py` & `edumfa-1.5.0/edumfa/lib/eventhandler/logginghandler.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/eventhandler/requestmangler.py` & `edumfa-1.5.0/edumfa/lib/eventhandler/requestmangler.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/eventhandler/responsemangler.py` & `edumfa-1.5.0/edumfa/lib/eventhandler/responsemangler.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/eventhandler/scripthandler.py` & `edumfa-1.5.0/edumfa/lib/eventhandler/scripthandler.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/eventhandler/tokenhandler.py` & `edumfa-1.5.0/edumfa/lib/eventhandler/tokenhandler.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/eventhandler/usernotification.py` & `edumfa-1.5.0/edumfa/lib/eventhandler/usernotification.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/eventhandler/webhookeventhandler.py` & `edumfa-1.5.0/edumfa/lib/eventhandler/webhookeventhandler.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/framework.py` & `edumfa-1.5.0/edumfa/lib/framework.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/importotp.py` & `edumfa-1.5.0/edumfa/lib/importotp.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/lifecycle.py` & `edumfa-1.5.0/edumfa/lib/lifecycle.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/log.py` & `edumfa-1.5.0/edumfa/lib/log.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/machine.py` & `edumfa-1.5.0/edumfa/lib/machine.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/machineresolver.py` & `edumfa-1.5.0/edumfa/lib/machineresolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/machines/__init__.py` & `edumfa-1.5.0/edumfa/lib/machines/__init__.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/machines/base.py` & `edumfa-1.5.0/edumfa/lib/machines/base.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/machines/hosts.py` & `edumfa-1.5.0/edumfa/lib/machines/hosts.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/machines/ldap.py` & `edumfa-1.5.0/edumfa/lib/machines/ldap.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/monitoringmodules/base.py` & `edumfa-1.5.0/edumfa/lib/monitoringmodules/base.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/monitoringmodules/sqlstats.py` & `edumfa-1.5.0/edumfa/lib/monitoringmodules/sqlstats.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/monitoringstats.py` & `edumfa-1.5.0/edumfa/lib/monitoringstats.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/passwordreset.py` & `edumfa-1.5.0/edumfa/lib/passwordreset.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/periodictask.py` & `edumfa-1.5.0/edumfa/lib/periodictask.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/pinhandling/base.py` & `edumfa-1.5.0/edumfa/lib/pinhandling/base.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/policy.py` & `edumfa-1.5.0/edumfa/lib/policy.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/policydecorators.py` & `edumfa-1.5.0/edumfa/lib/policydecorators.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/pooling.py` & `edumfa-1.5.0/edumfa/lib/pooling.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/queue.py` & `edumfa-1.5.0/edumfa/lib/queue.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/queues/__init__.py` & `edumfa-1.5.0/edumfa/lib/queues/__init__.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/queues/base.py` & `edumfa-1.5.0/edumfa/lib/queues/base.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/queues/huey_queue.py` & `edumfa-1.5.0/edumfa/lib/queues/huey_queue.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/radiusserver.py` & `edumfa-1.5.0/edumfa/lib/radiusserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/realm.py` & `edumfa-1.5.0/edumfa/lib/realm.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/resolver.py` & `edumfa-1.5.0/edumfa/lib/resolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/resolvers/HTTPResolver.py` & `edumfa-1.5.0/edumfa/lib/resolvers/HTTPResolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/resolvers/LDAPIdResolver.py` & `edumfa-1.5.0/edumfa/lib/resolvers/LDAPIdResolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/resolvers/PasswdIdResolver.py` & `edumfa-1.5.0/edumfa/lib/resolvers/PasswdIdResolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/resolvers/SCIMIdResolver.py` & `edumfa-1.5.0/edumfa/lib/resolvers/SCIMIdResolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/resolvers/SQLIdResolver.py` & `edumfa-1.5.0/edumfa/lib/resolvers/SQLIdResolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/resolvers/UserIdResolver.py` & `edumfa-1.5.0/edumfa/lib/resolvers/UserIdResolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/security/aeshsm.py` & `edumfa-1.5.0/edumfa/lib/security/aeshsm.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/security/default.py` & `edumfa-1.5.0/edumfa/lib/security/default.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/security/encryptkey.py` & `edumfa-1.5.0/edumfa/lib/security/encryptkey.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/serviceid.py` & `edumfa-1.5.0/edumfa/lib/serviceid.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/smsprovider/FirebaseProvider.py` & `edumfa-1.5.0/edumfa/lib/smsprovider/FirebaseProvider.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/smsprovider/HttpMessageToUidProvider.py` & `edumfa-1.5.0/edumfa/lib/smsprovider/HttpMessageToUidProvider.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/smsprovider/HttpSMSProvider.py` & `edumfa-1.5.0/edumfa/lib/smsprovider/HttpSMSProvider.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/smsprovider/SMSProvider.py` & `edumfa-1.5.0/edumfa/lib/smsprovider/SMSProvider.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/smsprovider/ScriptSMSProvider.py` & `edumfa-1.5.0/edumfa/lib/smsprovider/ScriptSMSProvider.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/smsprovider/SipgateSMSProvider.py` & `edumfa-1.5.0/edumfa/lib/smsprovider/SipgateSMSProvider.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/smsprovider/SmppSMSProvider.py` & `edumfa-1.5.0/edumfa/lib/smsprovider/SmppSMSProvider.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/smsprovider/SmtpSMSProvider.py` & `edumfa-1.5.0/edumfa/lib/smsprovider/SmtpSMSProvider.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/smsprovider/__init__.py` & `edumfa-1.5.0/edumfa/lib/smsprovider/__init__.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/smtpserver.py` & `edumfa-1.5.0/edumfa/lib/smtpserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/sqlutils.py` & `edumfa-1.5.0/edumfa/lib/sqlutils.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/subscriptions.py` & `edumfa-1.5.0/edumfa/lib/subscriptions.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/task/base.py` & `edumfa-1.5.0/edumfa/lib/task/base.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/task/eventcounter.py` & `edumfa-1.5.0/edumfa/lib/task/eventcounter.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/task/simplestats.py` & `edumfa-1.5.0/edumfa/lib/task/simplestats.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/token.py` & `edumfa-1.5.0/edumfa/lib/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 """
 This module contains all top level token functions.
 It depends on the models, lib.user and lib.tokenclass (which depends on the
 tokenclass implementations like lib.tokens.hotptoken)
 
 This is the middleware/glue between the HTTP API and the database
 """
-
+import json
 import traceback
 import string
 import datetime
 import os
 import logging
 
 from sqlalchemy import (and_, func)
@@ -991,15 +991,16 @@
     :param param: initialization parameters like
 
         ::
 
             {
                 "serial": ..., (optional)
                 "type": ...., (optional, default=hotp)
-                "otpkey": ...
+                "otpkey": ...,
+                "info": ... (optional)
             }
 
     :type param: dict
     :param user: the token owner
     :type user: User Object
     :param tokenrealms: the realms, to which the token should belong
     :type tokenrealms: list
@@ -1050,14 +1051,22 @@
     # Assign the token to all tokenrealms
     if tokenrealms and isinstance(tokenrealms, list):
         realms.extend(tokenrealms)
     # and to the user realm
     if user and user.realm:
         realms.append(user.realm)
 
+    # Check tokeninfo parameter
+    tokeninfo = param.get("info")
+    if tokeninfo:
+        if type(tokeninfo) is not dict:
+            tokeninfo = json.loads(tokeninfo)
+        if type(tokeninfo) is not dict:
+            raise ParameterError("Parameter 'info' must be a string representation of a json object (key-value pairs) or a python dict. but is of type {0!r}", type(tokeninfo))
+
     try:
         # Save the token to the database
         if token_count == 0:
             db_token.save()
 
         # the tokenclass object is created
         tokenobject = create_tokenclass_object(db_token)
@@ -1087,14 +1096,20 @@
 
     # We only set the tokenkind here, if it was explicitly set in the
     # init_token call.
     # In all other cases it is set in the update method of the tokenclass.
     if tokenkind:
         tokenobject.add_tokeninfo("tokenkind", tokenkind)
 
+    # Set tokeninfo
+    if tokeninfo:
+        for key, value in tokeninfo.items():
+            if value:
+                tokenobject.add_tokeninfo(key, value)
+
     # Set the validity period
     validity_period_start = param.get("validity_period_start")
     validity_period_end = param.get("validity_period_end")
     if validity_period_end:
         tokenobject.set_validity_period_end(validity_period_end)
     if validity_period_start:
         tokenobject.set_validity_period_start(validity_period_start)
```

### Comparing `edumfa-1.4.0/edumfa/lib/tokenclass.py` & `edumfa-1.5.0/edumfa/lib/tokenclass.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokengroup.py` & `edumfa-1.5.0/edumfa/lib/tokengroup.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/HMAC.py` & `edumfa-1.5.0/edumfa/lib/tokens/HMAC.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/applicationspecificpasswordtoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/applicationspecificpasswordtoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/certificatetoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/certificatetoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/daplugtoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/daplugtoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/daypasswordtoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/daypasswordtoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/emailtoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/emailtoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/foureyestoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/foureyestoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/hotptoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/hotptoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/indexedsecrettoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/indexedsecrettoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/mOTP.py` & `edumfa-1.5.0/edumfa/lib/tokens/mOTP.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/motptoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/motptoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/ocra.py` & `edumfa-1.5.0/edumfa/lib/tokens/ocra.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/ocratoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/ocratoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/papertoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/papertoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/passwordtoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/passwordtoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/pushtoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/pushtoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/questionnairetoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/questionnairetoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/radiustoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/radiustoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/registrationtoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/registrationtoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/remotetoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/remotetoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/smstoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/smstoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/spasstoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/spasstoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/sshkeytoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/sshkeytoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/tantoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/tantoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/tiqrtoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/tiqrtoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/totptoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/totptoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/u2f.py` & `edumfa-1.5.0/edumfa/lib/tokens/u2f.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/u2ftoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/u2ftoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/vasco.py` & `edumfa-1.5.0/edumfa/lib/tokens/vasco.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/vascotoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/vascotoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/webauthn.py` & `edumfa-1.5.0/edumfa/lib/tokens/webauthn.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/webauthntoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/webauthntoken.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,16 @@
 from edumfa.lib.log import log_with
 import logging
 from edumfa.lib import _
 from edumfa.lib.policy import SCOPE, GROUP, ACTION
 from edumfa.lib.user import User
 from edumfa.lib.utils import hexlify_and_unicode, is_true, to_unicode, convert_imagefile_to_dataimage
 from flask import current_app
+import datetime
+from dateutil.tz import tzlocal
 
 __doc__ = """
 WebAuthn  is the Web Authentication API specified by the FIDO Alliance.
 The register and authentication process is described here:
 
 https://w3c.github.io/webauthn/#sctn-rp-operations
 
@@ -522,14 +524,15 @@
     USER_VERIFICATION_REQUIREMENT = 'webauthn_user_verification_requirement'
     PUBLIC_KEY_CREDENTIAL_ALGORITHMS = 'webauthn_public_key_credential_algorithms'
     AUTHENTICATOR_ATTESTATION_FORM = 'webauthn_authenticator_attestation_form'
     AUTHENTICATOR_ATTESTATION_LEVEL = 'webauthn_authenticator_attestation_level'
     AUTHENTICATOR_RESIDENT_KEY = 'webauthn_resident_key'
     USERNAMELESS_AUTHN = 'webauthn_usernameless_authn'
     USERNAMELESS_REALM_POLICY = 'webauthn_usernameless_realm_policy'
+    TOKENLABEL = 'webauthn_tokenlabel'
     REQ = 'webauthn_req'
     AVOID_DOUBLE_REGISTRATION = 'webauthn_avoid_double_registration'
 
 
 class WEBAUTHNINFO(object):
     """
     Token info fields used by WebAuthn
@@ -791,15 +794,21 @@
                         'group': GROUP.TOKEN
                     },
                     ACTION.CHALLENGETEXT: {
                         'type': 'str',
                         'desc': _("Use an alternate challenge text for telling the "
                                   "user to confirm with his WebAuthn device."),
                         'group': WEBAUTHNGROUP.WEBAUTHN
-                    }
+                    },
+                    WEBAUTHNACTION.TOKENLABEL: {
+                        'type': 'str',
+                        'desc': _("The label for a new enrolled Passkey token. "
+                                "Possible tags are <code>{user}</code>, <code>{realm}</code>, "
+                                "<code>{serial}</code>, <code>{givenname}</code> and <code>{surname}</code>."),
+                        'group': WEBAUTHNGROUP.WEBAUTHN},
                 }
             }
         }
 
         if key:
             ret = res.get(key, {})
         else:
@@ -1054,26 +1063,32 @@
                 # Get the other webauthn tokens of the user
                 webauthn_toks = get_tokens(tokentype=self.type, user=self.user)
                 # add their credential ids
                 for tok in webauthn_toks:
                     if tok.token.rollout_state != ROLLOUTSTATE.CLIENTWAIT:
                         credential_id = tok.decrypt_otpkey()
                         credential_ids.append(credential_id)
+            
+            tokenlabel = params.get(WEBAUTHNACTION.TOKENLABEL, "{givenname} {surname} ({user})")
+            label = tokenlabel.replace("<s>", self.token.serial).replace("<u>", self.user.login).replace("<r>", self.user.realm)
+            label = label.format(serial=self.token.serial, user=self.user.login, realm=self.user.realm,
+                                 givenname=self.user.info.get("givenname", ""),
+                                 surname=self.user.info.get("surname", ""))
 
             public_key_credential_creation_options = WebAuthnMakeCredentialOptions(
                 challenge=webauthn_b64_encode(nonce),
                 rp_name=getParam(params,
                                  WEBAUTHNACTION.RELYING_PARTY_NAME,
                                  required),
                 rp_id=getParam(params,
                                WEBAUTHNACTION.RELYING_PARTY_ID,
                                required),
                 user_id=self.token.serial,
                 user_name=user.login,
-                user_display_name=str(user),
+                user_display_name=label,
                 timeout=getParam(params,
                                  WEBAUTHNACTION.TIMEOUT,
                                  required),
                 attestation=getParam(params,
                                      WEBAUTHNACTION.AUTHENTICATOR_ATTESTATION_FORM,
                                      required),
                 user_verification=getParam(params,
@@ -1322,14 +1337,17 @@
                                       "realm": token.user.realm,
                                       "resolver": token.user.resolver
                                       }
                 reply_dict["message"] = "Username-less authentication worked!"
                 reply_dict["serial"] = token.token.serial
                 reply_dict["type"] = token.token.tokentype
                 if count != -1:
+                    token.add_tokeninfo(ACTION.LASTAUTH,
+                                        datetime.datetime.now(tzlocal()))
+                    token.inc_count_auth_success()
                     return True, reply_dict
                 else:
                     return False, reply_dict
             except Exception as e:
                 return False, reply_dict
         else:
             # Not all necessary data provided.
```

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/yubicotoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/yubicotoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/tokens/yubikeytoken.py` & `edumfa-1.5.0/edumfa/lib/tokens/yubikeytoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/user.py` & `edumfa-1.5.0/edumfa/lib/user.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/usercache.py` & `edumfa-1.5.0/edumfa/lib/usercache.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/utils/__init__.py` & `edumfa-1.5.0/edumfa/lib/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/utils/compare.py` & `edumfa-1.5.0/edumfa/lib/utils/compare.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/lib/utils/export.py` & `edumfa-1.5.0/edumfa/lib/utils/export.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/messages.pot` & `edumfa-1.5.0/edumfa/messages.pot`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/models.py` & `edumfa-1.5.0/edumfa/models.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/README.md` & `edumfa-1.5.0/edumfa/static/README.md`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/app.js` & `edumfa-1.5.0/edumfa/static/app.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/audit/controllers/auditControllers.js` & `edumfa-1.5.0/edumfa/static/components/audit/controllers/auditControllers.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/audit/factories/audit.js` & `edumfa-1.5.0/edumfa/static/components/audit/factories/audit.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/audit/states/states.js` & `edumfa-1.5.0/edumfa/static/components/audit/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/audit/views/audit.html` & `edumfa-1.5.0/edumfa/static/components/audit/views/audit.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/audit/views/audit.log.html` & `edumfa-1.5.0/edumfa/static/components/audit/views/audit.log.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/components/controllers/componentControllers.js` & `edumfa-1.5.0/edumfa/static/components/components/controllers/componentControllers.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/components/factories/component.js` & `edumfa-1.5.0/edumfa/static/components/components/factories/component.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/components/states/states.js` & `edumfa-1.5.0/edumfa/static/components/components/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/components/views/component.clienttype.html` & `edumfa-1.5.0/edumfa/static/components/components/views/component.clienttype.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/components/views/component.html` & `edumfa-1.5.0/edumfa/static/components/components/views/component.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/controllers/configControllers.js` & `edumfa-1.5.0/edumfa/static/components/config/controllers/configControllers.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/controllers/eduMfaServerController.js` & `edumfa-1.5.0/edumfa/static/components/config/controllers/eduMfaServerController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/controllers/eventController.js` & `edumfa-1.5.0/edumfa/static/components/config/controllers/eventController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/controllers/ldapMachineResolverController.js` & `edumfa-1.5.0/edumfa/static/components/config/controllers/ldapMachineResolverController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/controllers/periodicTaskController.js` & `edumfa-1.5.0/edumfa/static/components/config/controllers/periodicTaskController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/controllers/radiusServerController.js` & `edumfa-1.5.0/edumfa/static/components/config/controllers/radiusServerController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/controllers/serviceidController.js` & `edumfa-1.5.0/edumfa/static/components/config/controllers/serviceidController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/controllers/smsgatewayController.js` & `edumfa-1.5.0/edumfa/static/components/config/controllers/smsgatewayController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/controllers/smtpServerController.js` & `edumfa-1.5.0/edumfa/static/components/config/controllers/smtpServerController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/controllers/tokengroupController.js` & `edumfa-1.5.0/edumfa/static/components/config/controllers/tokengroupController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/factories/config.js` & `edumfa-1.5.0/edumfa/static/components/config/factories/config.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/states/states.js` & `edumfa-1.5.0/edumfa/static/components/config/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.caconnectors.list.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.caconnectors.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.caconnectors.local.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.caconnectors.local.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.caconnectors.microsoft.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.caconnectors.microsoft.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.edumfaserver.edit.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.edumfaserver.edit.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.edumfaserver.list.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.edumfaserver.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.events.details.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.events.details.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.events.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.events.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.events.list.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.events.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.machineresolvers.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.machineresolvers.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.mresolvers.hosts.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.mresolvers.hosts.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.mresolvers.ldap.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.mresolvers.ldap.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.mresolvers.list.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.mresolvers.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.periodictasks.details.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.periodictasks.details.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.periodictasks.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.periodictasks.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.periodictasks.list.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.periodictasks.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.policies.details.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.policies.details.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.policies.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.policies.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.policies.list.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.policies.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.radius.edit.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.radius.edit.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.radius.list.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.radius.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.realms.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.realms.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.realms.list.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.realms.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.resolvers.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.resolvers.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.resolvers.http.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.resolvers.http.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.resolvers.ldap.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.resolvers.ldap.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.resolvers.list.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.resolvers.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.resolvers.passwd.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.resolvers.passwd.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.resolvers.scim.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.resolvers.scim.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.resolvers.sql.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.resolvers.sql.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.serviceid.edit.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.serviceid.edit.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.serviceid.list.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.serviceid.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.smsgateway.edit.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.smsgateway.edit.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.smsgateway.list.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.smsgateway.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.smtp.edit.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.smtp.edit.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.smtp.list.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.smtp.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.system.edit.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.system.edit.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.system.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.system.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.token.daypassword.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.token.daypassword.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.token.email.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.token.email.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.token.hotp.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.token.hotp.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.token.question.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.token.question.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.token.radius.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.token.radius.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.token.remote.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.token.remote.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.token.sms.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.token.sms.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.token.tiqr.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.token.tiqr.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.token.totp.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.token.totp.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.token.u2f.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.token.u2f.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.token.webauthn.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.token.webauthn.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.token.yubico.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.token.yubico.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.token.yubikey.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.token.yubikey.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.tokengroup.edit.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.tokengroup.edit.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.tokengroup.list.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.tokengroup.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/config.tokens.html` & `edumfa-1.5.0/edumfa/static/components/config/views/config.tokens.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/config/views/dialog.confirm_delete.html` & `edumfa-1.5.0/edumfa/static/components/config/views/dialog.confirm_delete.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/dashboard/controllers/dashboardControllers.js` & `edumfa-1.5.0/edumfa/static/components/dashboard/controllers/dashboardControllers.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/dashboard/states/states.js` & `edumfa-1.5.0/edumfa/static/components/dashboard/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/dashboard/views/dashboard.html` & `edumfa-1.5.0/edumfa/static/components/dashboard/views/dashboard.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/dialogs/views/dialog.about.html` & `edumfa-1.5.0/edumfa/static/components/dialogs/views/dialog.about.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/dialogs/views/dialog.autocreate_realm.html` & `edumfa-1.5.0/edumfa/static/components/dialogs/views/dialog.autocreate_realm.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/dialogs/views/dialog.lock.html` & `edumfa-1.5.0/edumfa/static/components/dialogs/views/dialog.lock.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/dialogs/views/dialog.no.token.html` & `edumfa-1.5.0/edumfa/static/components/dialogs/views/dialog.no.token.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/dialogs/views/dialog.welcome.html` & `edumfa-1.5.0/edumfa/static/components/dialogs/views/dialog.welcome.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/directives/controllers/directives.js` & `edumfa-1.5.0/edumfa/static/components/directives/controllers/directives.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/directives/views/directive.assigntoken.html` & `edumfa-1.5.0/edumfa/static/components/directives/views/directive.assigntoken.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/directives/views/directive.assignuser.html` & `edumfa-1.5.0/edumfa/static/components/directives/views/directive.assignuser.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/directives/views/directive.attachmachine.html` & `edumfa-1.5.0/edumfa/static/components/directives/views/directive.attachmachine.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/directives/views/directive.attachtoken.html` & `edumfa-1.5.0/edumfa/static/components/directives/views/directive.attachtoken.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/directives/views/directive.policyconditions.html` & `edumfa-1.5.0/edumfa/static/components/directives/views/directive.policyconditions.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/directives/views/directive.tokendata.html` & `edumfa-1.5.0/edumfa/static/components/directives/views/directive.tokendata.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/filters/filters.js` & `edumfa-1.5.0/edumfa/static/components/filters/filters.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/login/controllers/loginControllers.js` & `edumfa-1.5.0/edumfa/static/components/login/controllers/loginControllers.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/login/factories/auth.js` & `edumfa-1.5.0/edumfa/static/components/login/factories/auth.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/login/factories/u2f.js` & `edumfa-1.5.0/edumfa/static/components/login/factories/u2f.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/login/factories/webauthn.js` & `edumfa-1.5.0/edumfa/static/components/login/factories/webauthn.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/login/states/states.js` & `edumfa-1.5.0/edumfa/static/components/login/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/login/views/enter-response.html` & `edumfa-1.5.0/edumfa/static/components/login/views/enter-response.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/login/views/login.html` & `edumfa-1.5.0/edumfa/static/components/login/views/login.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/login/views/pinchange.html` & `edumfa-1.5.0/edumfa/static/components/login/views/pinchange.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/machine/controllers/machineController.js` & `edumfa-1.5.0/edumfa/static/components/machine/controllers/machineController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/machine/controllers/machineDetailsController.js` & `edumfa-1.5.0/edumfa/static/components/machine/controllers/machineDetailsController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/machine/factories/machine.js` & `edumfa-1.5.0/edumfa/static/components/machine/factories/machine.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/machine/states/states.js` & `edumfa-1.5.0/edumfa/static/components/machine/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/machine/views/machine.details.html` & `edumfa-1.5.0/edumfa/static/components/machine/views/machine.details.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/machine/views/machine.html` & `edumfa-1.5.0/edumfa/static/components/machine/views/machine.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/machine/views/machine.list.html` & `edumfa-1.5.0/edumfa/static/components/machine/views/machine.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/recovery/controllers/recoveryControllers.js` & `edumfa-1.5.0/edumfa/static/components/recovery/controllers/recoveryControllers.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/recovery/factories/recoveryFactory.js` & `edumfa-1.5.0/edumfa/static/components/recovery/factories/recoveryFactory.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/recovery/states/states.js` & `edumfa-1.5.0/edumfa/static/components/recovery/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/recovery/views/recovery.html` & `edumfa-1.5.0/edumfa/static/components/recovery/views/recovery.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/recovery/views/recovery.reset.html` & `edumfa-1.5.0/edumfa/static/components/recovery/views/recovery.reset.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/register/controllers/registerControllers.js` & `edumfa-1.5.0/edumfa/static/components/register/controllers/registerControllers.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/register/factories/registerFactory.js` & `edumfa-1.5.0/edumfa/static/components/register/factories/registerFactory.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/register/states/states.js` & `edumfa-1.5.0/edumfa/static/components/register/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/register/views/register.html` & `edumfa-1.5.0/edumfa/static/components/register/views/register.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/controllers/tokenApplicationsController.js` & `edumfa-1.5.0/edumfa/static/components/token/controllers/tokenApplicationsController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/controllers/tokenChallengesController.js` & `edumfa-1.5.0/edumfa/static/components/token/controllers/tokenChallengesController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/controllers/tokenControllers.js` & `edumfa-1.5.0/edumfa/static/components/token/controllers/tokenControllers.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/controllers/tokenDetailController.js` & `edumfa-1.5.0/edumfa/static/components/token/controllers/tokenDetailController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/controllers/tokenGetSerialController.js` & `edumfa-1.5.0/edumfa/static/components/token/controllers/tokenGetSerialController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/controllers/tokenLostController.js` & `edumfa-1.5.0/edumfa/static/components/token/controllers/tokenLostController.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/factories/token.js` & `edumfa-1.5.0/edumfa/static/components/token/factories/token.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/factories/validate.js` & `edumfa-1.5.0/edumfa/static/components/token/factories/validate.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/states/states.js` & `edumfa-1.5.0/edumfa/static/components/token/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/dialog.ask_token_delete.html` & `edumfa-1.5.0/edumfa/static/components/token/views/dialog.ask_token_delete.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.applications.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.applications.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.applications.offline.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.applications.offline.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.applications.ssh.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.applications.ssh.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.assign.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.assign.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.challenges.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.challenges.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.details.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.details.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.4eyes.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.4eyes.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.applspec.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.applspec.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.certificate.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.certificate.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.daypassword.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.daypassword.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.email.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.email.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.hotp.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.hotp.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.html`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         <!-- Extended attributes -->
         <uib-accordion ng-hide="$state.includes('token.wizard') ||
                         loggedInUser.role=='user'">
             <div uib-accordion-group
                  class="panel-default"
                  is-open="isOpen">
                 <uib-accordion-heading ng-click="isOpen=!isOpen">
-                    <div >{{ 'Extended Atttributes'|translate }}
+                    <div >{{ 'Extended Attributes'|translate }}
                         <span class="pull-right glyphicon" aria-hidden="true"
                            ng-class="{'glyphicon-chevron-down': isOpen, 'glyphicon-chevron-right': !isOpen}">
                         </span>
                     </div>
                 </uib-accordion-heading>
 
                 <div class="form-group col-sm-6">
```

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.indexedsecret.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.indexedsecret.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.motp.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.motp.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.push.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.push.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.question.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.question.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.radius.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.radius.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.remote.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.remote.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.sms.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.sms.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.sshkey.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.sshkey.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.totp.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.totp.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.vasco.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.vasco.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.yubico.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.yubico.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enroll.yubikey.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enroll.yubikey.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enrolled.certificate.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enrolled.certificate.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enrolled.daypassword.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enrolled.daypassword.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enrolled.hotp.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enrolled.hotp.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enrolled.motp.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enrolled.motp.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enrolled.paper.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enrolled.paper.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enrolled.push.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enrolled.push.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enrolled.registration.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enrolled.registration.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enrolled.tan.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enrolled.tan.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enrolled.tiqr.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enrolled.tiqr.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enrolled.totp.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enrolled.totp.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enrolled.u2f.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enrolled.u2f.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.enrolled.webauthn.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.enrolled.webauthn.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.getserial.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.getserial.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.import.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.import.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.list.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/token/views/token.lost.html` & `edumfa-1.5.0/edumfa/static/components/token/views/token.lost.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/translation/translations.js` & `edumfa-1.5.0/edumfa/static/components/translation/translations.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -801,15 +801,15 @@
         "Error fetching policy template": "Fehler beim Laden der Richtlinien-Vorlage",
         "Error fetching policy templates.": "Fehler beim Laden der Richtlinien-Vorlagen.",
         "Error in U2F response.": "Fehler in der U2F-Antwort.",
         "Error in WebAuthn response.": "Fehler in der WebAuthn-Antwort.",
         "Events": "Ereignisse",
         "Examples": "Beispiele",
         "Expiration": "Gültig bis",
-        "Extended Atttributes": "Erweiterte Attribute",
+        "Extended Attributes": "Erweiterte Attribute",
         "Fail counter": "Fehlerzähler",
         "Failed to delete user.": "Löschen des Benutzers fehlgeschlagen.",
         "Failed to reset your password.": "Zurücksetzen des Passworts fehlgeschlagen.",
         "Failed to set PIN.": "Setzen der PIN fehlgeschlagen.",
         "Failed to update user.": "Aktualisieren des Benutzers fehlgeschlagen.",
         "File name": "Dateiname",
         "Fingerprint": "Fingerabdruck",
```

### Comparing `edumfa-1.4.0/edumfa/static/components/user/controllers/userControllers.js` & `edumfa-1.5.0/edumfa/static/components/user/controllers/userControllers.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/user/factories/user.js` & `edumfa-1.5.0/edumfa/static/components/user/factories/user.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/user/states/states.js` & `edumfa-1.5.0/edumfa/static/components/user/states/states.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/user/views/dialog.ask_user_delete.html` & `edumfa-1.5.0/edumfa/static/components/user/views/dialog.ask_user_delete.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/user/views/user.add.dynamic.form.fields.html` & `edumfa-1.5.0/edumfa/static/components/user/views/user.add.dynamic.form.fields.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/user/views/user.add.html` & `edumfa-1.5.0/edumfa/static/components/user/views/user.add.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/user/views/user.details.html` & `edumfa-1.5.0/edumfa/static/components/user/views/user.details.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/user/views/user.html` & `edumfa-1.5.0/edumfa/static/components/user/views/user.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/user/views/user.list.html` & `edumfa-1.5.0/edumfa/static/components/user/views/user.list.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/components/user/views/user.password.html` & `edumfa-1.5.0/edumfa/static/components/user/views/user.password.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/css/angular-inform.css` & `edumfa-1.5.0/edumfa/static/contrib/css/angular-inform.css`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/css/angular-inform.css.map` & `edumfa-1.5.0/edumfa/static/contrib/css/angular-inform.css.map`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/css/bootstrap-theme.css` & `edumfa-1.5.0/edumfa/static/contrib/css/bootstrap-theme.css`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/css/bootstrap-theme.css.map` & `edumfa-1.5.0/edumfa/static/contrib/css/bootstrap-theme.css.map`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/css/bootstrap.css` & `edumfa-1.5.0/edumfa/static/contrib/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/css/bootstrap.css.map` & `edumfa-1.5.0/edumfa/static/contrib/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/css/hotkeys.css` & `edumfa-1.5.0/edumfa/static/contrib/css/hotkeys.css`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/css/isteven-multi-select.css` & `edumfa-1.5.0/edumfa/static/contrib/css/isteven-multi-select.css`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.eot` & `edumfa-1.5.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.svg` & `edumfa-1.5.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.ttf` & `edumfa-1.5.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.woff` & `edumfa-1.5.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.woff2` & `edumfa-1.5.0/edumfa/static/contrib/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/js/angular-inform.js` & `edumfa-1.5.0/edumfa/static/contrib/js/angular-inform.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/js/angular-inform.js.map` & `edumfa-1.5.0/edumfa/static/contrib/js/angular-inform.js.map`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/js/angular.js` & `edumfa-1.5.0/edumfa/static/contrib/js/angular.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/js/bootstrap.js` & `edumfa-1.5.0/edumfa/static/contrib/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/js/hotkeys.js` & `edumfa-1.5.0/edumfa/static/contrib/js/hotkeys.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/js/jquery.js` & `edumfa-1.5.0/edumfa/static/contrib/js/jquery.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/js/ngmodules/angular-gettext.js` & `edumfa-1.5.0/edumfa/static/contrib/js/ngmodules/angular-gettext.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/js/ngmodules/angular-idle.js` & `edumfa-1.5.0/edumfa/static/contrib/js/ngmodules/angular-idle.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/js/ngmodules/angular-sanitize.js` & `edumfa-1.5.0/edumfa/static/contrib/js/ngmodules/angular-sanitize.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/js/ngmodules/angular-ui-router.js` & `edumfa-1.5.0/edumfa/static/contrib/js/ngmodules/angular-ui-router.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/js/ngmodules/angular-ui-router.js.map` & `edumfa-1.5.0/edumfa/static/contrib/js/ngmodules/angular-ui-router.js.map`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/js/ngmodules/isteven-multi-select.js` & `edumfa-1.5.0/edumfa/static/contrib/js/ngmodules/isteven-multi-select.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/js/ngmodules/ng-file-upload.js` & `edumfa-1.5.0/edumfa/static/contrib/js/ngmodules/ng-file-upload.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/js/u2f-api.js` & `edumfa-1.5.0/edumfa/static/contrib/js/u2f-api.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/js/ui-bootstrap-tpls.js` & `edumfa-1.5.0/edumfa/static/contrib/js/ui-bootstrap-tpls.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/contrib/js/webauthn-client/edumfa-webauthn.js` & `edumfa-1.5.0/edumfa/static/contrib/js/webauthn-client/edumfa-webauthn.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/css/content.css` & `edumfa-1.5.0/edumfa/static/css/content.css`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/css/eduMFA-logo.png` & `edumfa-1.5.0/edumfa/static/css/eduMFA-logo.png`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/css/menu.css` & `edumfa-1.5.0/edumfa/static/css/menu.css`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/css/papertoken.css` & `edumfa-1.5.0/edumfa/static/css/papertoken.css`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/css/signin.css` & `edumfa-1.5.0/edumfa/static/css/signin.css`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/customize/README.rst` & `edumfa-1.5.0/edumfa/static/customize/README.rst`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/favicon.png` & `edumfa-1.5.0/edumfa/static/favicon.png`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/img/FIDO-U2F-Security-Key-444x444.png` & `edumfa-1.5.0/edumfa/static/img/FIDO-U2F-Security-Key-444x444.png`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/img/plugup.jpg` & `edumfa-1.5.0/edumfa/static/img/plugup.jpg`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/img/solokeys.png` & `edumfa-1.5.0/edumfa/static/img/solokeys.png`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/img/u2fzero.png` & `edumfa-1.5.0/edumfa/static/img/u2fzero.png`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/package-lock.json` & `edumfa-1.5.0/edumfa/static/package-lock.json`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/package.json` & `edumfa-1.5.0/edumfa/static/package.json`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/providers/errorMessageProvider.js` & `edumfa-1.5.0/edumfa/static/providers/errorMessageProvider.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/providers/versioningProvider.js` & `edumfa-1.5.0/edumfa/static/providers/versioningProvider.js`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/templates/cert_request_form.html` & `edumfa-1.5.0/edumfa/static/templates/cert_request_form.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/templates/documentation.rst` & `edumfa-1.5.0/edumfa/static/templates/documentation.rst`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/templates/footer.html` & `edumfa-1.5.0/edumfa/static/templates/footer.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/templates/header.html` & `edumfa-1.5.0/edumfa/static/templates/header.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/templates/index.html` & `edumfa-1.5.0/edumfa/static/templates/index.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/templates/menu.html` & `edumfa-1.5.0/edumfa/static/templates/menu.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/templates/token_enrolled.html` & `edumfa-1.5.0/edumfa/static/templates/token_enrolled.html`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/static/update_contrib.sh` & `edumfa-1.5.0/edumfa/static/update_contrib.sh`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/translations/cs/LC_MESSAGES/messages.mo` & `edumfa-1.5.0/edumfa/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/translations/cs/LC_MESSAGES/messages.po` & `edumfa-1.5.0/edumfa/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/translations/de/LC_MESSAGES/messages.mo` & `edumfa-1.5.0/edumfa/translations/de/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/translations/de/LC_MESSAGES/messages.po` & `edumfa-1.5.0/edumfa/translations/de/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/translations/es/LC_MESSAGES/messages.mo` & `edumfa-1.5.0/edumfa/translations/es/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/translations/es/LC_MESSAGES/messages.po` & `edumfa-1.5.0/edumfa/translations/es/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/translations/fr/LC_MESSAGES/messages.mo` & `edumfa-1.5.0/edumfa/translations/fr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/translations/fr/LC_MESSAGES/messages.po` & `edumfa-1.5.0/edumfa/translations/fr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/translations/it/LC_MESSAGES/messages.mo` & `edumfa-1.5.0/edumfa/translations/it/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/translations/it/LC_MESSAGES/messages.po` & `edumfa-1.5.0/edumfa/translations/it/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/translations/nl/LC_MESSAGES/messages.mo` & `edumfa-1.5.0/edumfa/translations/nl/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/translations/nl/LC_MESSAGES/messages.po` & `edumfa-1.5.0/edumfa/translations/nl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/translations/pl/LC_MESSAGES/messages.po` & `edumfa-1.5.0/edumfa/translations/pl/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/translations/pt_BR/LC_MESSAGES/messages.mo` & `edumfa-1.5.0/edumfa/translations/pt_BR/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/translations/pt_BR/LC_MESSAGES/messages.po` & `edumfa-1.5.0/edumfa/translations/pt_BR/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/translations/ro/LC_MESSAGES/messages.mo` & `edumfa-1.5.0/edumfa/translations/ro/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/translations/ro/LC_MESSAGES/messages.po` & `edumfa-1.5.0/edumfa/translations/ro/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/translations/ru/LC_MESSAGES/messages.mo` & `edumfa-1.5.0/edumfa/translations/ru/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/translations/ru/LC_MESSAGES/messages.po` & `edumfa-1.5.0/edumfa/translations/ru/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/translations/si/LC_MESSAGES/messages.mo` & `edumfa-1.5.0/edumfa/translations/si/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/translations/si/LC_MESSAGES/messages.po` & `edumfa-1.5.0/edumfa/translations/si/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/translations/tr/LC_MESSAGES/messages.mo` & `edumfa-1.5.0/edumfa/translations/tr/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/translations/tr/LC_MESSAGES/messages.po` & `edumfa-1.5.0/edumfa/translations/tr/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/translations/zh_Hans/LC_MESSAGES/messages.mo` & `edumfa-1.5.0/edumfa/translations/zh_Hans/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/translations/zh_Hans/LC_MESSAGES/messages.po` & `edumfa-1.5.0/edumfa/translations/zh_Hans/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/translations/zh_Hant/LC_MESSAGES/messages.mo` & `edumfa-1.5.0/edumfa/translations/zh_Hant/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/translations/zh_Hant/LC_MESSAGES/messages.po` & `edumfa-1.5.0/edumfa/translations/zh_Hant/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/webui/certificate.py` & `edumfa-1.5.0/edumfa/webui/certificate.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa/webui/login.py` & `edumfa-1.5.0/edumfa/webui/login.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa-manage` & `edumfa-1.5.0/edumfa-manage`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/edumfa.egg-info/PKG-INFO` & `edumfa-1.5.0/edumfa.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edumfa
-Version: 1.4.0
+Version: 1.5.0
 Summary: eduMFA: identity, multifactor authentication (OTP), authorization, audit
 Home-page: https://www.edumfa.io
 Author: edumfa.io
 Author-email: edumfa@listserv.dfn.de
 License: AGPLv3
 Keywords: OTP,two factor authentication,management,security
 Classifier: Framework :: Flask
```

### Comparing `edumfa-1.4.0/edumfa.egg-info/SOURCES.txt` & `edumfa-1.5.0/edumfa.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,26 +4,63 @@
 README.rst
 edumfa-manage
 requirements.txt
 setup.py
 deploy/README.md
 deploy/docker-compose-example.yml
 deploy/docker-setup.sh
+deploy/edumfa_radius.pm
 deploy/logging.cfg
+deploy/rlm_perl.ini
 deploy/apache/edumfaapp.wsgi
+deploy/apache/sites-available/edumfa-venv.conf
 deploy/apache/sites-available/edumfa.conf
+deploy/config/freeradius2/edumfa
+deploy/config/freeradius2/mods-perl-edumfa
+deploy/config/freeradius3/edumfa
+deploy/config/freeradius3/mods-perl-edumfa
 deploy/crontab/edumfa
 deploy/docker-example/edumfa-policy.conf
 deploy/docker-example/edumfa-setup.sh
 deploy/docker-example/edumfa.cfg
 deploy/edumfa/dictionary
+deploy/edumfa/edumfa.cfg
 deploy/gunicorn/edumfaapp.py
 deploy/nginx/edumfaapp.py
 deploy/nginx/sites-available/edumfa
-deploy/privacyidea/enckey
+deploy/ubuntu/changelog
+deploy/ubuntu/clean
+deploy/ubuntu/compat
+deploy/ubuntu/control
+deploy/ubuntu/copyright
+deploy/ubuntu/rules
+deploy/ubuntu-radius/changelog
+deploy/ubuntu-radius/compat
+deploy/ubuntu-radius/control
+deploy/ubuntu-radius/copyright
+deploy/ubuntu-radius/edumfa-radius.install
+deploy/ubuntu-radius/edumfa-radius.postinst
+deploy/ubuntu-radius/edumfa-radius.postrm
+deploy/ubuntu-radius/rules
+deploy/ubuntu-radius/source/format
+deploy/ubuntu-server/changelog
+deploy/ubuntu-server/clean
+deploy/ubuntu-server/compat
+deploy/ubuntu-server/control
+deploy/ubuntu-server/edumfa-apache2.install
+deploy/ubuntu-server/edumfa-apache2.postinst
+deploy/ubuntu-server/edumfa-apache2.postrm
+deploy/ubuntu-server/edumfa-nginx.install
+deploy/ubuntu-server/edumfa-nginx.postinst
+deploy/ubuntu-server/edumfa-nginx.postrm
+deploy/ubuntu-server/rules
+deploy/ubuntu-server/source/format
+deploy/ubuntu-server/source/options
+deploy/ubuntu/source/format
+deploy/ubuntu/source/options
 deploy/uwsgi/apps-available/edumfa.xml
 edumfa/__init__.py
 edumfa/app.py
 edumfa/babel.cfg
 edumfa/config.py
 edumfa/messages.pot
 edumfa/models.py
```

### Comparing `edumfa-1.4.0/edumfa.egg-info/requires.txt` & `edumfa-1.5.0/edumfa.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/env.py` & `edumfa-1.5.0/migrations/env.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/006d4747f858_.py` & `edumfa-1.5.0/migrations/versions/006d4747f858_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/00762b3f7a60_.py` & `edumfa-1.5.0/migrations/versions/00762b3f7a60_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/0c7123345224_.py` & `edumfa-1.5.0/migrations/versions/0c7123345224_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/0d011e94a8e8_.py` & `edumfa-1.5.0/migrations/versions/0d011e94a8e8_.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""empty message
+"""Migrate from privacyIDEA to eduMFA
 
 Revision ID: 0d011e94a8e8
 Revises: 5cb310101a1f
 Create Date: 2024-02-17 08:50:59.295124
 
 """
 from sqlalchemy import orm
@@ -18,68 +18,83 @@
 
 def dialect_supports_sequences():
     migration_context = context.get_context()
     return migration_context.dialect.supports_sequences
 
 
 def upgrade():
+
+    print("Migrating from privacyIDEA to eduMFA")
     try:
+        print(" * Renaming column privacyidea_server to edumfa_server")
         op.alter_column("pidea_audit", "privacyidea_server", new_column_name="edumfa_server", existing_type=sa.String(length=255))
+        print(" * Renaming table pidea_audit to mfa_audit")
         op.rename_table("pidea_audit", "mfa_audit")
     except Exception as e:
         print("Renaming table pidea_audit to mfa_audit failed")
         print(e)
     try:
+        print(" * Renaming table privacyideaserver to edumfaserver")
         op.rename_table("privacyideaserver", "edumfaserver")
     except Exception as e:
         print("Renaming table privacyideaserver to edumfaserver failed")
         print(e)
 
     try:
         if dialect_supports_sequences():
             if context.get_context().dialect.name in ['mariadb', 'mysql']:
+                print(" * Renaming table privacyideaserver_seq to edumfaserver_seq")
                 op.rename_table("privacyideaserver_seq", "edumfaserver_seq")
             else:
+                print(" * Renaming sequence privacyideaserver_id_seq to edumfaserver_id_seq")
                 op.execute("ALTER SEQUENCE privacyideaserver_id_seq RENAME TO edumfaserver_id_seq")
     except Exception as e:
         print("Renaming sequence for privacyideaserver to edumfaserver failed")
         print(e)
 
     try:
+        print(" * Renaming column pinode to edumfanode")
         op.alter_column("policy", "pinode", new_column_name="edumfanode", existing_type=sa.String(length=256))
     except Exception as e:
         print("Migrating pinode to edumfanode failed")
         print(e)
 
     bind = op.get_bind()
     session = orm.Session(bind=bind)
     try:
+        print(" * Replacing login_mode=privacyIDEA with login_mode=eduMFA")
         for row in session.query(Policy).filter(Policy.action.like("login_mode=privacyIDEA")):
+            print(f' ** Replacing login_mode in policy {row.name} (id: {row.id}) with existing action {row.action}')
             row.action = row.action.replace("login_mode=privacyIDEA", "login_mode=eduMFA")
         session.commit()
     except Exception as e:
         session.rollback()
         print("Failed to update login modes!")
         print(e)
 
     session = orm.Session(bind=bind)
     try:
+        print(" * Replacing privacyideaserver_read and privacyideaserver_write policies ")
         for row in session.query(Policy).filter(Policy.action.like("privacyideaserver_read")):
+            print(f' ** Replacing policy for {row.name} ({row.id}) with action {row.action}')
             row.action = row.action.replace("privacyideaserver_read", "edumfaserver_read")
         for row in session.query(Policy).filter(Policy.action.like("privacyideaserver_write")):
+            print(f' ** Replacing policy for {row.name} ({row.id}) with action {row.action}')
             row.action = row.action.replace("privacyideaserver_write", "edumfaserver_write")
         session.commit()
     except Exception as e:
         session.rollback()
         print("Failed to update admin policy!")
         print(e)
 
     session = orm.Session(bind=bind)
     try:
+        print(" * Replacing providernames for smsgateways")
         for row in session.query(SMSGateway).filter(SMSGateway.providermodule.like("privacyidea.lib.%")):
+            print(f' ** Replacing providername for {row.identifier} ({row.id}) with provider {row.providermodule}')
             row.providermodule = row.providermodule.replace("privacyidea.lib.", "edumfa.lib.")
         session.commit()
     except Exception as e:
         session.rollback()
         print("Failed to update SmsGateway providermodules!")
         print(e)
```

### Comparing `edumfa-1.4.0/migrations/versions/145ce80decd_.py` & `edumfa-1.5.0/migrations/versions/145ce80decd_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/14a1bcb10018_.py` & `edumfa-1.5.0/migrations/versions/14a1bcb10018_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/19f727d285e2_.py` & `edumfa-1.5.0/migrations/versions/19f727d285e2_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/1a0710df148b_.py` & `edumfa-1.5.0/migrations/versions/1a0710df148b_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/1a69e5e5e2ac_.py` & `edumfa-1.5.0/migrations/versions/1a69e5e5e2ac_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/1edda52b619f_.py` & `edumfa-1.5.0/migrations/versions/1edda52b619f_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/204d8d4f351e_.py` & `edumfa-1.5.0/migrations/versions/204d8d4f351e_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/205bda834127_.py` & `edumfa-1.5.0/migrations/versions/205bda834127_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/20969b4cbf06_.py` & `edumfa-1.5.0/migrations/versions/20969b4cbf06_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/2118e566df16_.py` & `edumfa-1.5.0/migrations/versions/2118e566df16_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/2181294eed0b_.py` & `edumfa-1.5.0/migrations/versions/2181294eed0b_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/22558d9f3178_.py` & `edumfa-1.5.0/migrations/versions/22558d9f3178_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/239995464c48_.py` & `edumfa-1.5.0/migrations/versions/239995464c48_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/2551ee982544_.py` & `edumfa-1.5.0/migrations/versions/2551ee982544_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/2ac117d0a6f5_.py` & `edumfa-1.5.0/migrations/versions/2ac117d0a6f5_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/2c9430cfc66b_.py` & `edumfa-1.5.0/migrations/versions/2c9430cfc66b_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/307a4fbe8a05_.py` & `edumfa-1.5.0/migrations/versions/307a4fbe8a05_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/3236a1abf1c6_.py` & `edumfa-1.5.0/migrations/versions/3236a1abf1c6_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/3429d523e51f_.py` & `edumfa-1.5.0/migrations/versions/3429d523e51f_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/36428afb2457_.py` & `edumfa-1.5.0/migrations/versions/36428afb2457_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/37e6b49fc686_.py` & `edumfa-1.5.0/migrations/versions/37e6b49fc686_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/3ae3c668f444_.py` & `edumfa-1.5.0/migrations/versions/3ae3c668f444_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/3ba618f6b820_.py` & `edumfa-1.5.0/migrations/versions/3ba618f6b820_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/3c6e9dd7fbac_.py` & `edumfa-1.5.0/migrations/versions/3c6e9dd7fbac_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/3d7f8b29cbb1_.py` & `edumfa-1.5.0/migrations/versions/3d7f8b29cbb1_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/3f7e8583ea2_.py` & `edumfa-1.5.0/migrations/versions/3f7e8583ea2_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/4023571658f8_.py` & `edumfa-1.5.0/migrations/versions/4023571658f8_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/4238eac8ccab_.py` & `edumfa-1.5.0/migrations/versions/4238eac8ccab_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/449903fb6e35_.py` & `edumfa-1.5.0/migrations/versions/449903fb6e35_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/48ee74b8a7c8_.py` & `edumfa-1.5.0/migrations/versions/48ee74b8a7c8_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/49a04e560d96_.py` & `edumfa-1.5.0/migrations/versions/49a04e560d96_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/4a0aec37e7cf_.py` & `edumfa-1.5.0/migrations/versions/4a0aec37e7cf_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/4d9178fa8336_.py` & `edumfa-1.5.0/migrations/versions/4d9178fa8336_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/4f32a4e1bf33_.py` & `edumfa-1.5.0/migrations/versions/4f32a4e1bf33_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/50adc980d625_.py` & `edumfa-1.5.0/migrations/versions/50adc980d625_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/5402fd96fbca_.py` & `edumfa-1.5.0/migrations/versions/5402fd96fbca_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/58e4f7ebb705_.py` & `edumfa-1.5.0/migrations/versions/58e4f7ebb705_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/59ef3e03bc62_.py` & `edumfa-1.5.0/migrations/versions/59ef3e03bc62_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/5cb310101a1f_.py` & `edumfa-1.5.0/migrations/versions/5cb310101a1f_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/631ec59e1ca6_.py` & `edumfa-1.5.0/migrations/versions/631ec59e1ca6_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/849170064430_.py` & `edumfa-1.5.0/migrations/versions/849170064430_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/86f40f535d7c_.py` & `edumfa-1.5.0/migrations/versions/86f40f535d7c_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/888b56ed5dcb_.py` & `edumfa-1.5.0/migrations/versions/888b56ed5dcb_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/89e57ed16379_.py` & `edumfa-1.5.0/migrations/versions/89e57ed16379_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/8d40dbcfda25_.py` & `edumfa-1.5.0/migrations/versions/8d40dbcfda25_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/9155f0d3d028_.py` & `edumfa-1.5.0/migrations/versions/9155f0d3d028_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/a28f2733897b_.py` & `edumfa-1.5.0/migrations/versions/a28f2733897b_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/a63df077051a_.py` & `edumfa-1.5.0/migrations/versions/a63df077051a_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/a7e91b18a460_.py` & `edumfa-1.5.0/migrations/versions/a7e91b18a460_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/b9131d0686eb_.py` & `edumfa-1.5.0/migrations/versions/b9131d0686eb_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/cb6d7b7bae63_.py` & `edumfa-1.5.0/migrations/versions/cb6d7b7bae63_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/d2ae8e54b628_.py` & `edumfa-1.5.0/migrations/versions/d2ae8e54b628_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/d415d490eb05_.py` & `edumfa-1.5.0/migrations/versions/d415d490eb05_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/d6b40a745e5_.py` & `edumfa-1.5.0/migrations/versions/d6b40a745e5_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/d756b34061ff_.py` & `edumfa-1.5.0/migrations/versions/d756b34061ff_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/dceb6cd3c41e_.py` & `edumfa-1.5.0/migrations/versions/dceb6cd3c41e_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/e360c56bcf8c_.py` & `edumfa-1.5.0/migrations/versions/e360c56bcf8c_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/e5cbeb7c177_.py` & `edumfa-1.5.0/migrations/versions/e5cbeb7c177_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/ef29ba43e290_.py` & `edumfa-1.5.0/migrations/versions/ef29ba43e290_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/fa07bd604a75.py` & `edumfa-1.5.0/migrations/versions/fa07bd604a75.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/fabcf24d9304_.py` & `edumfa-1.5.0/migrations/versions/fabcf24d9304_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/migrations/versions/ff26585932ec_.py` & `edumfa-1.5.0/migrations/versions/ff26585932ec_.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/requirements.txt` & `edumfa-1.5.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/setup.py` & `edumfa-1.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 import os
 import stat
 import sys
 
-VERSION = "1.4.0"
+VERSION = "1.5.0"
 
 # Taken from kennethreitz/requests/setup.py
 package_directory = os.path.realpath(os.path.dirname(__file__))
 
 
 def get_file_contents(file_path):
     """Get the context of the file using full path name."""
```

### Comparing `edumfa-1.4.0/tests/base.py` & `edumfa-1.5.0/tests/base.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/ldap3mock.py` & `edumfa-1.5.0/tests/ldap3mock.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/mscamock.py` & `edumfa-1.5.0/tests/mscamock.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/pkcs11mock.py` & `edumfa-1.5.0/tests/pkcs11mock.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/queuemock.py` & `edumfa-1.5.0/tests/queuemock.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/radiusmock.py` & `edumfa-1.5.0/tests/radiusmock.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/redismock.py` & `edumfa-1.5.0/tests/redismock.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/requirements.txt` & `edumfa-1.5.0/tests/requirements.txt`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/smppmock.py` & `edumfa-1.5.0/tests/smppmock.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/smtpmock.py` & `edumfa-1.5.0/tests/smtpmock.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_2stepinit.py` & `edumfa-1.5.0/tests/test_api_2stepinit.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_applications.py` & `edumfa-1.5.0/tests/test_api_applications.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_audit.py` & `edumfa-1.5.0/tests/test_api_audit.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_auth.py` & `edumfa-1.5.0/tests/test_api_auth.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_caconnector.py` & `edumfa-1.5.0/tests/test_api_caconnector.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_clienttype.py` & `edumfa-1.5.0/tests/test_api_clienttype.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_edumfaserver.py` & `edumfa-1.5.0/tests/test_api_edumfaserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_events.py` & `edumfa-1.5.0/tests/test_api_events.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_lib_policy.py` & `edumfa-1.5.0/tests/test_api_lib_policy.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_lib_utils.py` & `edumfa-1.5.0/tests/test_api_lib_utils.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_machineresolver.py` & `edumfa-1.5.0/tests/test_api_machineresolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_machines.py` & `edumfa-1.5.0/tests/test_api_machines.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_machines_serviceid.py` & `edumfa-1.5.0/tests/test_api_machines_serviceid.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_monitoring.py` & `edumfa-1.5.0/tests/test_api_monitoring.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_offline_no_token.py` & `edumfa-1.5.0/tests/test_api_offline_no_token.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_periodictask.py` & `edumfa-1.5.0/tests/test_api_periodictask.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_policy.py` & `edumfa-1.5.0/tests/test_api_policy.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_push_validate.py` & `edumfa-1.5.0/tests/test_api_push_validate.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_radiusserver.py` & `edumfa-1.5.0/tests/test_api_radiusserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_register.py` & `edumfa-1.5.0/tests/test_api_register.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_roles.py` & `edumfa-1.5.0/tests/test_api_roles.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_serviceids.py` & `edumfa-1.5.0/tests/test_api_serviceids.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_smsgateway.py` & `edumfa-1.5.0/tests/test_api_smsgateway.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_smtpserver.py` & `edumfa-1.5.0/tests/test_api_smtpserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_system.py` & `edumfa-1.5.0/tests/test_api_system.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_token.py` & `edumfa-1.5.0/tests/test_api_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -2947,15 +2947,15 @@
                                            headers={'Authorization': self.at}):
             res = self.app.full_dispatch_request()
             # check if rollout work as expected with no type set.
             self.assertTrue(res.status_code == 200, res)
 
         delete_policy("require_description")
 
-    def test_43_modify_tokeninfo_bulk(self):
+    def test_51_modify_tokeninfo_bulk(self):
         self._create_temp_token("INF001")
         # Set three tokeninfo values
         with self.app.test_request_context('/token/info/INF001',
                                            method="POST",
                                            data={"info": '{"key1": "value 1", "key2": "value 2", "key3": "value 3"}'},
                                            headers={'Authorization': self.at}):
             res = self.app.full_dispatch_request()
@@ -3030,14 +3030,55 @@
                                            data={"info": '{"key1": "value 1", "key2": "value 2"}'},
                                            headers={'Authorization': self.at}):
             res = self.app.full_dispatch_request()
             self.assertEqual(res.status_code, 404)
             result = res.json.get("result")
             self.assertFalse(result.get("status"))
 
+    def test_52_init_token_with_tokeninfo(self):
+        with self.app.test_request_context('/token/init',
+                                           method='POST',
+                                           data={"type": "HOTP",
+                                                 "otpkey": self.otpkey,
+                                                 "pin": "1234",
+                                                 "user": "cornelius",
+                                                 "realm": self.realm1,
+                                                 "info": '{"key1": "value 1", "key2": "value 2", "key3": "value 3"}'},
+                                           headers={'Authorization': self.at}):
+            res = self.app.full_dispatch_request()
+            data = res.json
+            self.assertTrue(res.status_code == 200, res)
+            result = data.get("result")
+            detail = data.get("detail")
+            self.assertTrue(result.get("status"), result)
+            self.assertTrue(result.get("value"), result)
+            self.assertTrue("value" in detail.get("googleurl"), detail)
+            serial = detail.get("serial")
+            self.assertTrue("OATH" in serial, detail)
+
+        with self.app.test_request_context('/token/',
+                                           method="GET",
+                                           query_string=urlencode(
+                                               {"serial": serial}),
+                                           headers={'Authorization': self.at}):
+            res = self.app.full_dispatch_request()
+            self.assertTrue(res.status_code == 200, res)
+            result = res.json.get("result")
+            value = result.get("value")
+            token = value.get("tokens")[0]
+            self.assertTrue(value.get("count") == 1, result)
+
+            tokeninfo = token.get("info")
+            test_dict = {'key1': 'value 1', 'key2': 'value 2', 'key3' : 'value 3'}
+            try:
+                self.assertTrue(test_dict.viewitems() <= tokeninfo.viewitems())
+            except AttributeError:
+                self.assertTrue(test_dict.items() <= tokeninfo.items())
+
+        remove_token(serial)
 
 
 class API00TokenPerformance(MyApiTestCase):
 
     token_count = 21
 
     def test_00_create_some_tokens(self):
```

### Comparing `edumfa-1.4.0/tests/test_api_tokengroup.py` & `edumfa-1.5.0/tests/test_api_tokengroup.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_ttype.py` & `edumfa-1.5.0/tests/test_api_ttype.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_u2f.py` & `edumfa-1.5.0/tests/test_api_u2f.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_users.py` & `edumfa-1.5.0/tests/test_api_users.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_api_validate.py` & `edumfa-1.5.0/tests/test_api_validate.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_app.py` & `edumfa-1.5.0/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_db_model.py` & `edumfa-1.5.0/tests/test_db_model.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_applications.py` & `edumfa-1.5.0/tests/test_lib_applications.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_apps.py` & `edumfa-1.5.0/tests/test_lib_apps.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_audit.py` & `edumfa-1.5.0/tests/test_lib_audit.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_auth.py` & `edumfa-1.5.0/tests/test_lib_auth.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_authcache.py` & `edumfa-1.5.0/tests/test_lib_authcache.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_caconnector.py` & `edumfa-1.5.0/tests/test_lib_caconnector.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_challenges.py` & `edumfa-1.5.0/tests/test_lib_challenges.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_clientapplication.py` & `edumfa-1.5.0/tests/test_lib_clientapplication.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_config.py` & `edumfa-1.5.0/tests/test_lib_config.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_counter.py` & `edumfa-1.5.0/tests/test_lib_counter.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_crypto.py` & `edumfa-1.5.0/tests/test_lib_crypto.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_edumfaserver.py` & `edumfa-1.5.0/tests/test_lib_edumfaserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_eventhandler_logging.py` & `edumfa-1.5.0/tests/test_lib_eventhandler_logging.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_eventhandler_usernotification.py` & `edumfa-1.5.0/tests/test_lib_eventhandler_usernotification.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_events.py` & `edumfa-1.5.0/tests/test_lib_events.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_framework.py` & `edumfa-1.5.0/tests/test_lib_framework.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_importotp.py` & `edumfa-1.5.0/tests/test_lib_importotp.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_lifecycle.py` & `edumfa-1.5.0/tests/test_lib_lifecycle.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_machine_resolver_ldap.py` & `edumfa-1.5.0/tests/test_lib_machine_resolver_ldap.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_machines.py` & `edumfa-1.5.0/tests/test_lib_machines.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_machinetokens.py` & `edumfa-1.5.0/tests/test_lib_machinetokens.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_monitoringstats.py` & `edumfa-1.5.0/tests/test_lib_monitoringstats.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_periodictask.py` & `edumfa-1.5.0/tests/test_lib_periodictask.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_policy.py` & `edumfa-1.5.0/tests/test_lib_policy.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_policydecorator.py` & `edumfa-1.5.0/tests/test_lib_policydecorator.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_pooling.py` & `edumfa-1.5.0/tests/test_lib_pooling.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_queue.py` & `edumfa-1.5.0/tests/test_lib_queue.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_radiusserver.py` & `edumfa-1.5.0/tests/test_lib_radiusserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_realm.py` & `edumfa-1.5.0/tests/test_lib_realm.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_recovery.py` & `edumfa-1.5.0/tests/test_lib_recovery.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_resolver.py` & `edumfa-1.5.0/tests/test_lib_resolver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_serviceid.py` & `edumfa-1.5.0/tests/test_lib_serviceid.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_smsprovider.py` & `edumfa-1.5.0/tests/test_lib_smsprovider.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_smtpserver.py` & `edumfa-1.5.0/tests/test_lib_smtpserver.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_sqlutils.py` & `edumfa-1.5.0/tests/test_lib_sqlutils.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_subscriptions.py` & `edumfa-1.5.0/tests/test_lib_subscriptions.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_task_eventcounter.py` & `edumfa-1.5.0/tests/test_lib_task_eventcounter.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_task_simplestats.py` & `edumfa-1.5.0/tests/test_lib_task_simplestats.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tasks.py` & `edumfa-1.5.0/tests/test_lib_tasks.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_token.py` & `edumfa-1.5.0/tests/test_lib_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,14 +316,19 @@
         count = get_tokens(count=True)
         self.assertTrue(count == 5, count)
 
         # try to create unknown tokentype
         self.assertRaises(TokenAdminError, init_token, {"otpkey": "1234",
                                                         "type": "never_know"})
 
+        # try to create invalid tokeninfo
+        self.assertRaises(ParameterError, init_token, {"otpkey": "1234",
+                                                        "type": "totp",
+                                                        "info": "[1,2,3,4]"})
+
         # try to create the same token with another type
         self.assertRaises(TokenAdminError, init_token, {"otpkey": "1234",
                                                         "serial": "NEW001",
                                                         "type": "totp"})
 
         # try to update the same token with another user assignment
         self.assertRaises(TokenAdminError, init_token, {"otpkey": "1234",
```

### Comparing `edumfa-1.4.0/tests/test_lib_tokenclass.py` & `edumfa-1.5.0/tests/test_lib_tokenclass.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tokengroup.py` & `edumfa-1.5.0/tests/test_lib_tokengroup.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tokens_certificate.py` & `edumfa-1.5.0/tests/test_lib_tokens_certificate.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tokens_daplug.py` & `edumfa-1.5.0/tests/test_lib_tokens_daplug.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tokens_daypassword.py` & `edumfa-1.5.0/tests/test_lib_tokens_daypassword.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tokens_email.py` & `edumfa-1.5.0/tests/test_lib_tokens_email.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tokens_foureyes.py` & `edumfa-1.5.0/tests/test_lib_tokens_foureyes.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tokens_hotp.py` & `edumfa-1.5.0/tests/test_lib_tokens_hotp.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tokens_indexedsecret.py` & `edumfa-1.5.0/tests/test_lib_tokens_indexedsecret.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tokens_motp.py` & `edumfa-1.5.0/tests/test_lib_tokens_motp.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tokens_paper.py` & `edumfa-1.5.0/tests/test_lib_tokens_paper.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tokens_passwordtoken.py` & `edumfa-1.5.0/tests/test_lib_tokens_passwordtoken.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tokens_push.py` & `edumfa-1.5.0/tests/test_lib_tokens_push.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tokens_questionnaire.py` & `edumfa-1.5.0/tests/test_lib_tokens_questionnaire.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tokens_radius.py` & `edumfa-1.5.0/tests/test_lib_tokens_radius.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tokens_registration.py` & `edumfa-1.5.0/tests/test_lib_tokens_registration.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tokens_remote.py` & `edumfa-1.5.0/tests/test_lib_tokens_remote.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tokens_sms.py` & `edumfa-1.5.0/tests/test_lib_tokens_sms.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tokens_spass.py` & `edumfa-1.5.0/tests/test_lib_tokens_spass.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tokens_ssh.py` & `edumfa-1.5.0/tests/test_lib_tokens_ssh.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tokens_tan.py` & `edumfa-1.5.0/tests/test_lib_tokens_tan.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tokens_tiqr.py` & `edumfa-1.5.0/tests/test_lib_tokens_tiqr.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tokens_totp.py` & `edumfa-1.5.0/tests/test_lib_tokens_totp.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tokens_u2f.py` & `edumfa-1.5.0/tests/test_lib_tokens_u2f.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tokens_vasco.py` & `edumfa-1.5.0/tests/test_lib_tokens_vasco.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tokens_webauthn.py` & `edumfa-1.5.0/tests/test_lib_tokens_webauthn.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tokens_yubico.py` & `edumfa-1.5.0/tests/test_lib_tokens_yubico.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_tokens_yubikey.py` & `edumfa-1.5.0/tests/test_lib_tokens_yubikey.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_user.py` & `edumfa-1.5.0/tests/test_lib_user.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_usercache.py` & `edumfa-1.5.0/tests/test_lib_usercache.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_utils.py` & `edumfa-1.5.0/tests/test_lib_utils.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_lib_utils_compare.py` & `edumfa-1.5.0/tests/test_lib_utils_compare.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_mock_ldap3.py` & `edumfa-1.5.0/tests/test_mock_ldap3.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_resolver_realm.py` & `edumfa-1.5.0/tests/test_resolver_realm.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_scripts.py` & `edumfa-1.5.0/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_ui_certificate.py` & `edumfa-1.5.0/tests/test_ui_certificate.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/test_ui_login.py` & `edumfa-1.5.0/tests/test_ui_login.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/FIDO-U2F-Security-Key-444x444.png` & `edumfa-1.5.0/tests/testdata/FIDO-U2F-Security-Key-444x444.png`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/attestation/yubico.pem` & `edumfa-1.5.0/tests/testdata/attestation/yubico.pem`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/audit.sqlite` & `edumfa-1.5.0/tests/testdata/audit.sqlite`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/ca/cacert.pem` & `edumfa-1.5.0/tests/testdata/ca/cacert.pem`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/ca/cakey.pem` & `edumfa-1.5.0/tests/testdata/ca/cakey.pem`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/ca/index.txt` & `edumfa-1.5.0/tests/testdata/ca/index.txt`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/ca/openssl.cnf` & `edumfa-1.5.0/tests/testdata/ca/openssl.cnf`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/dictionary` & `edumfa-1.5.0/tests/testdata/dictionary`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/firebase-test.json` & `edumfa-1.5.0/tests/testdata/firebase-test.json`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/google-services.json` & `edumfa-1.5.0/tests/testdata/google-services.json`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/gpg/pubring.gpg` & `edumfa-1.5.0/tests/testdata/gpg/pubring.gpg`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/gpg/random_seed` & `edumfa-1.5.0/tests/testdata/gpg/random_seed`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/gpg/secring.gpg` & `edumfa-1.5.0/tests/testdata/gpg/secring.gpg`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/gpg/trustdb.gpg` & `edumfa-1.5.0/tests/testdata/gpg/trustdb.gpg`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/import.oath.asc` & `edumfa-1.5.0/tests/testdata/import.oath.asc`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/jwt_sign.key` & `edumfa-1.5.0/tests/testdata/jwt_sign.key`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/logging.cfg` & `edumfa-1.5.0/tests/testdata/logging.cfg`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/logging.yml` & `edumfa-1.5.0/tests/testdata/logging.yml`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/msca-connector/ca.pem` & `edumfa-1.5.0/tests/testdata/msca-connector/ca.pem`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/msca-connector/privacyidea-encrypted.key` & `edumfa-1.5.0/tests/testdata/msca-connector/privacyidea-encrypted.key`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/msca-connector/privacyidea.key` & `edumfa-1.5.0/tests/testdata/msca-connector/privacyidea.key`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/msca-connector/privacyidea.pem` & `edumfa-1.5.0/tests/testdata/msca-connector/privacyidea.pem`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/passwd` & `edumfa-1.5.0/tests/testdata/passwd`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/passwords` & `edumfa-1.5.0/tests/testdata/passwords`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/private.pem` & `edumfa-1.5.0/tests/testdata/private.pem`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/pskc-aes.xml` & `edumfa-1.5.0/tests/testdata/pskc-aes.xml`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/pskc-password.xml` & `edumfa-1.5.0/tests/testdata/pskc-password.xml`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/test.sub` & `edumfa-1.5.0/tests/testdata/test.sub`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/test2.sub` & `edumfa-1.5.0/tests/testdata/test2.sub`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/testuser-api.sqlite` & `edumfa-1.5.0/tests/testdata/testuser-api.sqlite`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/testuser.sqlite` & `edumfa-1.5.0/tests/testdata/testuser.sqlite`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/testusercache.sqlite` & `edumfa-1.5.0/tests/testdata/testusercache.sqlite`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/trusted_attestation_roots/solokeys_device_attestation_ca.pem` & `edumfa-1.5.0/tests/testdata/trusted_attestation_roots/solokeys_device_attestation_ca.pem`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/trusted_attestation_roots/yubico_u2f_device_attestation_ca.pem` & `edumfa-1.5.0/tests/testdata/trusted_attestation_roots/yubico_u2f_device_attestation_ca.pem`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/yubico-oath-long.csv` & `edumfa-1.5.0/tests/testdata/yubico-oath-long.csv`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tests/testdata/yubico.csv` & `edumfa-1.5.0/tests/testdata/yubico.csv`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/creategoogleauthenticator-file` & `edumfa-1.5.0/tools/creategoogleauthenticator-file`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-authorizedkeys` & `edumfa-1.5.0/tools/edumfa-authorizedkeys`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-convert-base32.py` & `edumfa-1.5.0/tools/edumfa-convert-base32.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-convert-token` & `edumfa-1.5.0/tools/edumfa-convert-token`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-convert-token.1` & `edumfa-1.5.0/tools/edumfa-convert-token.1`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-convert-xml-to-csv` & `edumfa-1.5.0/tools/edumfa-convert-xml-to-csv`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-create-ad-users` & `edumfa-1.5.0/tools/edumfa-create-ad-users`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-create-ad-users.1` & `edumfa-1.5.0/tools/edumfa-create-ad-users.1`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-create-certificate` & `edumfa-1.5.0/tools/edumfa-create-certificate`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-create-certificate.1` & `edumfa-1.5.0/tools/edumfa-create-certificate.1`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-create-pwidresolver-user` & `edumfa-1.5.0/tools/edumfa-create-pwidresolver-user`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-create-pwidresolver-user.1` & `edumfa-1.5.0/tools/edumfa-create-pwidresolver-user.1`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-create-sqlidresolver-user` & `edumfa-1.5.0/tools/edumfa-create-sqlidresolver-user`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-create-sqlidresolver-user.1` & `edumfa-1.5.0/tools/edumfa-create-sqlidresolver-user.1`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-create-userdb` & `edumfa-1.5.0/tools/edumfa-create-userdb`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-create-userdb.1` & `edumfa-1.5.0/tools/edumfa-create-userdb.1`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-cron` & `edumfa-1.5.0/tools/edumfa-cron`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-diag` & `edumfa-1.5.0/tools/edumfa-diag`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-expired-users` & `edumfa-1.5.0/tools/edumfa-expired-users`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-export-edumfa-counter.py` & `edumfa-1.5.0/tools/edumfa-export-edumfa-counter.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-export-linotp-counter.py` & `edumfa-1.5.0/tools/edumfa-export-linotp-counter.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-fetchssh` & `edumfa-1.5.0/tools/edumfa-fetchssh`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-fetchssh.1` & `edumfa-1.5.0/tools/edumfa-fetchssh.1`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-fix-access-rights` & `edumfa-1.5.0/tools/edumfa-fix-access-rights`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-fix-access-rights.1` & `edumfa-1.5.0/tools/edumfa-fix-access-rights.1`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-get-serial` & `edumfa-1.5.0/tools/edumfa-get-serial`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-get-unused-tokens` & `edumfa-1.5.0/tools/edumfa-get-unused-tokens`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-migrate-linotp.py` & `edumfa-1.5.0/tools/edumfa-migrate-linotp.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-pip-update` & `edumfa-1.5.0/tools/edumfa-pip-update`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-pip-update.1` & `edumfa-1.5.0/tools/edumfa-pip-update.1`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-queue-huey` & `edumfa-1.5.0/tools/edumfa-queue-huey`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-schema-upgrade` & `edumfa-1.5.0/tools/edumfa-schema-upgrade`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-standalone` & `edumfa-1.5.0/tools/edumfa-standalone`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-sync-owncloud.py` & `edumfa-1.5.0/tools/edumfa-sync-owncloud.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-token-janitor` & `edumfa-1.5.0/tools/edumfa-token-janitor`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-update-counter.py` & `edumfa-1.5.0/tools/edumfa-update-counter.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-update-linotp-counter.py` & `edumfa-1.5.0/tools/edumfa-update-linotp-counter.py`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-user-action` & `edumfa-1.5.0/tools/edumfa-user-action`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/edumfa-usercache-cleanup` & `edumfa-1.5.0/tools/edumfa-usercache-cleanup`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/getgooglecodes` & `edumfa-1.5.0/tools/getgooglecodes`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/reset-edumfa` & `edumfa-1.5.0/tools/reset-edumfa`

 * *Files identical despite different names*

### Comparing `edumfa-1.4.0/tools/ssha.py` & `edumfa-1.5.0/tools/ssha.py`

 * *Files identical despite different names*

