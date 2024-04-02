# Comparing `tmp/keri-1.1.8.tar.gz` & `tmp/keri-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "keri-1.1.8.tar", last modified: Sun Mar 17 23:25:00 2024, max compression
+gzip compressed data, was "keri-1.1.9.tar", last modified: Wed Mar 27 01:43:02 2024, max compression
```

## Comparing `keri-1.1.8.tar` & `keri-1.1.9.tar`

### file list

```diff
@@ -1,199 +1,199 @@
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.259031 keri-1.1.8/
--rw-r--r--   0 pfeairheller   (501) staff       (20)    11357 2023-03-20 02:45:25.000000 keri-1.1.8/LICENSE
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1527 2024-03-17 23:25:00.258847 keri-1.1.8/PKG-INFO
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2203 2024-03-15 13:00:30.000000 keri-1.1.8/README.md
--rw-r--r--   0 pfeairheller   (501) staff       (20)       38 2024-03-17 23:25:00.259078 keri-1.1.8/setup.cfg
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3783 2024-03-17 23:15:50.000000 keri-1.1.8/setup.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.232973 keri-1.1.8/src/
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.235519 keri-1.1.8/src/keri/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       78 2024-03-17 23:15:50.000000 keri-1.1.8/src/keri/__init__.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.240273 keri-1.1.8/src/keri/app/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       58 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    36847 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/app/agenting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2780 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/apping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1648 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/challenging.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.240566 keri-1.1.8/src/keri/app/cli/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       62 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/__init__.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.243636 keri-1.1.8/src/keri/app/cli/commands/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/__init__.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.244165 keri-1.1.8/src/keri/app/cli/commands/challenge/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/challenge/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1529 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/challenge/generate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4353 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/challenge/respond.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5565 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/challenge/verify.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.244381 keri-1.1.8/src/keri/app/cli/commands/contacts/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/contacts/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2281 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/contacts/list.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.244779 keri-1.1.8/src/keri/app/cli/commands/delegate/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/delegate/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9345 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/app/cli/commands/delegate/confirm.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4082 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/app/cli/commands/delegate/request.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.244998 keri-1.1.8/src/keri/app/cli/commands/did/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/did/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3450 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/did/generate.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.245477 keri-1.1.8/src/keri/app/cli/commands/ends/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/ends/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4679 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/ends/add.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2873 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/ends/export.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2566 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/ends/list.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6291 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/escrow.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3774 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/export.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     7160 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/app/cli/commands/incept.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5419 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/app/cli/commands/init.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3855 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/interact.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.246746 keri-1.1.8/src/keri/app/cli/commands/ipex/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/ipex/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6651 2024-03-17 23:09:21.000000 keri-1.1.8/src/keri/app/cli/commands/ipex/admit.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      529 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/ipex/agree.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      470 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/ipex/apply.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6996 2024-03-17 23:09:21.000000 keri-1.1.8/src/keri/app/cli/commands/ipex/grant.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9834 2024-03-17 23:09:21.000000 keri-1.1.8/src/keri/app/cli/commands/ipex/join.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9870 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/ipex/list.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      564 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/ipex/offer.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5584 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/ipex/spurn.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3371 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/kevers.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1402 2023-11-27 19:46:40.000000 keri-1.1.8/src/keri/app/cli/commands/list.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.246958 keri-1.1.8/src/keri/app/cli/commands/local/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/local/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9105 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/local/watch.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.247327 keri-1.1.8/src/keri/app/cli/commands/mailbox/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/mailbox/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4555 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/mailbox/debug.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2554 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/mailbox/update.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5900 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/migrate.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.248649 keri-1.1.8/src/keri/app/cli/commands/multisig/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/multisig/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3048 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/app/cli/commands/multisig/continue.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      735 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/multisig/demo.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6701 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/app/cli/commands/multisig/incept.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5619 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/multisig/interact.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    30794 2024-03-17 23:09:21.000000 keri-1.1.8/src/keri/app/cli/commands/multisig/join.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5227 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/app/cli/commands/multisig/notice.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    10193 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/app/cli/commands/multisig/rotate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9500 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/multisig/shell.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4898 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/multisig/update.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      440 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/nonce.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.249211 keri-1.1.8/src/keri/app/cli/commands/oobi/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/oobi/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1975 2023-11-27 19:46:40.000000 keri-1.1.8/src/keri/app/cli/commands/oobi/clean.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3120 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/oobi/generate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3716 2023-11-15 20:54:14.000000 keri-1.1.8/src/keri/app/cli/commands/oobi/resolve.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.249822 keri-1.1.8/src/keri/app/cli/commands/passcode/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/passcode/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      662 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/passcode/generate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1521 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/passcode/remove.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2475 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/passcode/set.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3559 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/query.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1860 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/app/cli/commands/rename.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4044 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/rollback.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     8454 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/app/cli/commands/rotate.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1051 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/saidify.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      528 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/salt.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2140 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/sign.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.250040 keri-1.1.8/src/keri/app/cli/commands/ssh/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/ssh/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3392 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/ssh/export.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2284 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/status.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      414 2024-03-17 23:09:21.000000 keri-1.1.8/src/keri/app/cli/commands/time.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.250622 keri-1.1.8/src/keri/app/cli/commands/vc/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/vc/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    10784 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/vc/create.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5966 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/vc/export.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     6251 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/vc/list.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.251047 keri-1.1.8/src/keri/app/cli/commands/vc/registry/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/vc/registry/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     7267 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/app/cli/commands/vc/registry/incept.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1764 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/vc/registry/list.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3683 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/vc/registry/status.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     7026 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/vc/revoke.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2928 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/verify.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      429 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/version.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.251492 keri-1.1.8/src/keri/app/cli/commands/watcher/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/watcher/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1002 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/app/cli/commands/watcher/list.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2877 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/watcher/start.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2471 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/app/cli/commands/watcher/update.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.251918 keri-1.1.8/src/keri/app/cli/commands/witness/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/witness/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3059 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/witness/demo.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4618 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/commands/witness/start.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3624 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/commands/witness/submit.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.252761 keri-1.1.8/src/keri/app/cli/common/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/common/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2877 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/common/config.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3893 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/app/cli/common/displaying.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3264 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/app/cli/common/existing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1783 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/common/incepting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1208 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/common/rotating.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      415 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/cli/common/terming.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      728 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/cli/kli.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     7485 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/app/configing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     7632 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/connecting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    10218 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/app/delegating.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    24656 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/app/directing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    18772 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/app/forwarding.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    26582 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/app/grouping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)   124547 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/app/habbing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     8565 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/app/httping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    41620 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/app/indirecting.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    73666 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/keeping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/kiwiing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    13938 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/notifying.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    23097 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/oobiing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     4471 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/querying.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     8400 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/signaling.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5908 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/app/signing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1837 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/app/specing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9669 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/app/storing.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.253994 keri-1.1.8/src/keri/core/
--rw-r--r--   0 pfeairheller   (501) staff       (20)      114 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/core/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)   240644 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/core/coring.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)   276895 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/core/eventing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    58260 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/core/parsing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    26300 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/core/routing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    12848 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/core/scheming.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    63844 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/core/serdering.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.255008 keri-1.1.8/src/keri/db/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       55 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/db/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)   120727 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/db/basing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    75451 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/db/dbing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     9322 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/db/escrowing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    30476 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/db/koming.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    59260 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/db/subing.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.256220 keri-1.1.8/src/keri/demo/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       59 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/demo/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2794 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/demo/demo_bob.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2811 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/demo/demo_eve.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)      932 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/demo/demo_kev.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2836 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/demo/demo_sam.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    16437 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/demo/demoing.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.256671 keri-1.1.8/src/keri/end/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       73 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/end/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    24878 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/end/ending.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1322 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/end/priming.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.256919 keri-1.1.8/src/keri/help/
--rw-r--r--   0 pfeairheller   (501) staff       (20)      557 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/help/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     8211 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/help/helping.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    18567 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/kering.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.257171 keri-1.1.8/src/keri/peer/
--rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/peer/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    19487 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/peer/exchanging.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.257713 keri-1.1.8/src/keri/vc/
--rw-r--r--   0 pfeairheller   (501) staff       (20)       56 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/vc/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    10278 2024-03-17 23:09:21.000000 keri-1.1.8/src/keri/vc/protocoling.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     2505 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/vc/proving.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)     3749 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/vc/walleting.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.258426 keri-1.1.8/src/keri/vdr/
--rw-r--r--   0 pfeairheller   (501) staff       (20)      120 2023-03-20 02:45:25.000000 keri-1.1.8/src/keri/vdr/__init__.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    34269 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/vdr/credentialing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    84543 2024-03-15 13:00:30.000000 keri-1.1.8/src/keri/vdr/eventing.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    14342 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/vdr/verifying.py
--rw-r--r--   0 pfeairheller   (501) staff       (20)    35871 2024-03-12 23:12:35.000000 keri-1.1.8/src/keri/vdr/viring.py
-drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-17 23:25:00.258598 keri-1.1.8/src/keri.egg-info/
--rw-r--r--   0 pfeairheller   (501) staff       (20)     1527 2024-03-17 23:25:00.000000 keri-1.1.8/src/keri.egg-info/PKG-INFO
--rw-r--r--   0 pfeairheller   (501) staff       (20)     5641 2024-03-17 23:25:00.000000 keri-1.1.8/src/keri.egg-info/SOURCES.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2024-03-17 23:25:00.000000 keri-1.1.8/src/keri.egg-info/dependency_links.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)      181 2024-03-17 23:25:00.000000 keri-1.1.8/src/keri.egg-info/entry_points.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2023-03-20 03:44:29.000000 keri-1.1.8/src/keri.egg-info/not-zip-safe
--rw-r--r--   0 pfeairheller   (501) staff       (20)      282 2024-03-17 23:25:00.000000 keri-1.1.8/src/keri.egg-info/requires.txt
--rw-r--r--   0 pfeairheller   (501) staff       (20)        5 2024-03-17 23:25:00.000000 keri-1.1.8/src/keri.egg-info/top_level.txt
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.248848 keri-1.1.9/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    11357 2023-03-20 02:45:25.000000 keri-1.1.9/LICENSE
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1527 2024-03-27 01:43:02.248636 keri-1.1.9/PKG-INFO
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2456 2024-03-27 00:38:35.000000 keri-1.1.9/README.md
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       38 2024-03-27 01:43:02.248888 keri-1.1.9/setup.cfg
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3783 2024-03-27 00:38:35.000000 keri-1.1.9/setup.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.218186 keri-1.1.9/src/
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.220522 keri-1.1.9/src/keri/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       78 2024-03-27 00:38:35.000000 keri-1.1.9/src/keri/__init__.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.226283 keri-1.1.9/src/keri/app/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       58 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    36847 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/agenting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2780 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/apping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1648 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/challenging.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.226744 keri-1.1.9/src/keri/app/cli/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       62 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/__init__.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.230853 keri-1.1.9/src/keri/app/cli/commands/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/__init__.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.231577 keri-1.1.9/src/keri/app/cli/commands/challenge/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/challenge/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1529 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/challenge/generate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4353 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/challenge/respond.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5565 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/challenge/verify.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.231976 keri-1.1.9/src/keri/app/cli/commands/contacts/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/contacts/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2281 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/contacts/list.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.232392 keri-1.1.9/src/keri/app/cli/commands/delegate/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/delegate/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9345 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/delegate/confirm.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4082 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/delegate/request.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.232601 keri-1.1.9/src/keri/app/cli/commands/did/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/did/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3450 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/did/generate.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.233286 keri-1.1.9/src/keri/app/cli/commands/ends/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/ends/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4679 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/ends/add.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2873 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/ends/export.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2566 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/ends/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6291 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/escrow.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3774 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/export.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     7160 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/incept.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5419 2024-03-26 19:38:12.000000 keri-1.1.9/src/keri/app/cli/commands/init.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3855 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/interact.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.234799 keri-1.1.9/src/keri/app/cli/commands/ipex/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/ipex/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6651 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/ipex/admit.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      529 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/ipex/agree.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      470 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/ipex/apply.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6996 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/ipex/grant.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9834 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/ipex/join.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9870 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/ipex/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      564 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/ipex/offer.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5584 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/ipex/spurn.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3371 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/kevers.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1402 2023-11-27 19:46:40.000000 keri-1.1.9/src/keri/app/cli/commands/list.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.235058 keri-1.1.9/src/keri/app/cli/commands/local/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/local/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9105 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/local/watch.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.235705 keri-1.1.9/src/keri/app/cli/commands/mailbox/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/mailbox/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4555 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/mailbox/debug.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2554 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/mailbox/update.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5900 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/migrate.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.237139 keri-1.1.9/src/keri/app/cli/commands/multisig/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/multisig/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3048 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/multisig/continue.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      735 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/multisig/demo.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6701 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/multisig/incept.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5619 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/multisig/interact.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    30794 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/multisig/join.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5227 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/multisig/notice.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    10193 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/multisig/rotate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9500 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/multisig/shell.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4898 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/multisig/update.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      440 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/nonce.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.237681 keri-1.1.9/src/keri/app/cli/commands/oobi/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/oobi/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1975 2023-11-27 19:46:40.000000 keri-1.1.9/src/keri/app/cli/commands/oobi/clean.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3120 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/oobi/generate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3716 2023-11-15 20:54:14.000000 keri-1.1.9/src/keri/app/cli/commands/oobi/resolve.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.238233 keri-1.1.9/src/keri/app/cli/commands/passcode/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/passcode/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      662 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/passcode/generate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1521 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/passcode/remove.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2475 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/passcode/set.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3559 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/query.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1860 2024-03-26 19:38:12.000000 keri-1.1.9/src/keri/app/cli/commands/rename.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4044 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/rollback.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     8454 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/rotate.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1051 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/saidify.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      528 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/salt.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2140 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/sign.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.238424 keri-1.1.9/src/keri/app/cli/commands/ssh/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/ssh/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3392 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/ssh/export.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2284 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/status.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      414 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/time.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.239298 keri-1.1.9/src/keri/app/cli/commands/vc/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/vc/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    10784 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/vc/create.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5966 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/vc/export.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     6251 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/vc/list.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.239861 keri-1.1.9/src/keri/app/cli/commands/vc/registry/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/vc/registry/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     7267 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/vc/registry/incept.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1764 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/vc/registry/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3683 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/vc/registry/status.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     7517 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/vc/revoke.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2928 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/verify.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      429 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/version.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.240410 keri-1.1.9/src/keri/app/cli/commands/watcher/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/watcher/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1002 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/watcher/list.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2877 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/watcher/start.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2471 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/commands/watcher/update.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.240827 keri-1.1.9/src/keri/app/cli/commands/witness/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/witness/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3059 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/witness/demo.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4618 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/commands/witness/start.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3624 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/commands/witness/submit.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.241854 keri-1.1.9/src/keri/app/cli/common/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/common/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2877 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/common/config.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3893 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/cli/common/displaying.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3264 2024-03-26 19:38:12.000000 keri-1.1.9/src/keri/app/cli/common/existing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1783 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/common/incepting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1208 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/common/rotating.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      415 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/cli/common/terming.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      728 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/cli/kli.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     7485 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/configing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     7632 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/connecting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    10218 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/delegating.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    24656 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/directing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    18772 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/forwarding.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    26582 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/grouping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)   124547 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/habbing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     8565 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/httping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    41620 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/indirecting.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    73666 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/keeping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/kiwiing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    13938 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/notifying.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    23097 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/oobiing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     4471 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/querying.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     8400 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/signaling.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5908 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/app/signing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1837 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/app/specing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9669 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/app/storing.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.243529 keri-1.1.9/src/keri/core/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      114 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/core/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)   240644 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/core/coring.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)   276895 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/core/eventing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    58260 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/core/parsing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    26300 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/core/routing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    12848 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/core/scheming.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    63844 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/core/serdering.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.245101 keri-1.1.9/src/keri/db/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       55 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/db/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)   120727 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/db/basing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    75451 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/db/dbing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     9322 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/db/escrowing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    30476 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/db/koming.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    59260 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/db/subing.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.245942 keri-1.1.9/src/keri/demo/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       59 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/demo/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2794 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/demo/demo_bob.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2811 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/demo/demo_eve.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      932 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/demo/demo_kev.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2836 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/demo/demo_sam.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    16437 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/demo/demoing.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.246353 keri-1.1.9/src/keri/end/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       73 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/end/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    24878 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/end/ending.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1322 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/end/priming.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.246729 keri-1.1.9/src/keri/help/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      557 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/help/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     8211 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/help/helping.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    18567 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/kering.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.246963 keri-1.1.9/src/keri/peer/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        0 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/peer/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    19487 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/peer/exchanging.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.247459 keri-1.1.9/src/keri/vc/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)       56 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/vc/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    10278 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/vc/protocoling.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     2505 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/vc/proving.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     3749 2024-03-12 23:12:35.000000 keri-1.1.9/src/keri/vc/walleting.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.248191 keri-1.1.9/src/keri/vdr/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      120 2023-03-20 02:45:25.000000 keri-1.1.9/src/keri/vdr/__init__.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    34269 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/vdr/credentialing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    84543 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/vdr/eventing.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    14342 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/vdr/verifying.py
+-rw-r--r--   0 pfeairheller   (501) staff       (20)    35871 2024-03-26 23:29:19.000000 keri-1.1.9/src/keri/vdr/viring.py
+drwxr-xr-x   0 pfeairheller   (501) staff       (20)        0 2024-03-27 01:43:02.248381 keri-1.1.9/src/keri.egg-info/
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     1527 2024-03-27 01:43:02.000000 keri-1.1.9/src/keri.egg-info/PKG-INFO
+-rw-r--r--   0 pfeairheller   (501) staff       (20)     5641 2024-03-27 01:43:02.000000 keri-1.1.9/src/keri.egg-info/SOURCES.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2024-03-27 01:43:02.000000 keri-1.1.9/src/keri.egg-info/dependency_links.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      181 2024-03-27 01:43:02.000000 keri-1.1.9/src/keri.egg-info/entry_points.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        1 2023-03-20 03:44:29.000000 keri-1.1.9/src/keri.egg-info/not-zip-safe
+-rw-r--r--   0 pfeairheller   (501) staff       (20)      282 2024-03-27 01:43:02.000000 keri-1.1.9/src/keri.egg-info/requires.txt
+-rw-r--r--   0 pfeairheller   (501) staff       (20)        5 2024-03-27 01:43:02.000000 keri-1.1.9/src/keri.egg-info/top_level.txt
```

### Comparing `keri-1.1.8/LICENSE` & `keri-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/PKG-INFO` & `keri-1.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keri
-Version: 1.1.8
+Version: 1.1.9
 Summary: Key Event Receipt Infrastructure
 Home-page: https://github.com/WebOfTrust/keripy
 Author: Samuel M. Smith
 Author-email: smith.samuel.m@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://keri.readthedocs.io/
 Project-URL: Changelog, https://keri.readthedocs.io/en/latest/changelog.html
```

### Comparing `keri-1.1.8/README.md` & `keri-1.1.9/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -22,15 +22,18 @@
 to get a version string similar to the following: 
 
 `1.0.0`
 
 ### Local installation - Docker build
 Run `make build-keri` to build your docker image.
 
-Then run `docker run -it gleif/keri /bin/bash` and you can run `kli version` from within the running container to play with KERIpy.
+Then run `docker run --pull=never -it --entrypoint /bin/bash weboftrust/keri:1.1.9` and you can run `kli version` from within the running container to play with KERIpy.
+
+Make sure the image tag matches the version used in the `Makefile`.
+We use `--pull=never` to ensure that docker does not implicitly pull a remote image and relies on the local image tagged during `make build-keri`.
 
 ### Dependencies
 #### Binaries
 
 python 3.10.4+
 libsodium 1.0.18+
```

### Comparing `keri-1.1.8/setup.py` & `keri-1.1.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 from glob import glob
 from os.path import basename
 from os.path import splitext
 
 from setuptools import find_packages, setup
 setup(
     name='keri',
-    version='1.1.8',  # also change in src/keri/__init__.py
+    version='1.1.9',  # also change in src/keri/__init__.py
     license='Apache Software License 2.0',
     description='Key Event Receipt Infrastructure',
     long_description="KERI Decentralized Key Management Infrastructure",
     author='Samuel M. Smith',
     author_email='smith.samuel.m@gmail.com',
     url='https://github.com/WebOfTrust/keripy',
     packages=find_packages('src'),
```

### Comparing `keri-1.1.8/src/keri/app/agenting.py` & `keri-1.1.9/src/keri/app/agenting.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/apping.py` & `keri-1.1.9/src/keri/app/apping.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/challenging.py` & `keri-1.1.9/src/keri/app/challenging.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/challenge/generate.py` & `keri-1.1.9/src/keri/app/cli/commands/challenge/generate.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/challenge/respond.py` & `keri-1.1.9/src/keri/app/cli/commands/challenge/respond.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/challenge/verify.py` & `keri-1.1.9/src/keri/app/cli/commands/challenge/verify.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/contacts/list.py` & `keri-1.1.9/src/keri/app/cli/commands/contacts/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/delegate/confirm.py` & `keri-1.1.9/src/keri/app/cli/commands/delegate/confirm.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/delegate/request.py` & `keri-1.1.9/src/keri/app/cli/commands/delegate/request.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/did/generate.py` & `keri-1.1.9/src/keri/app/cli/commands/did/generate.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/ends/add.py` & `keri-1.1.9/src/keri/app/cli/commands/ends/add.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/ends/export.py` & `keri-1.1.9/src/keri/app/cli/commands/ends/export.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/ends/list.py` & `keri-1.1.9/src/keri/app/cli/commands/ends/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/escrow.py` & `keri-1.1.9/src/keri/app/cli/commands/escrow.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/export.py` & `keri-1.1.9/src/keri/app/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/incept.py` & `keri-1.1.9/src/keri/app/cli/commands/incept.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/init.py` & `keri-1.1.9/src/keri/app/cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/interact.py` & `keri-1.1.9/src/keri/app/cli/commands/interact.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/ipex/admit.py` & `keri-1.1.9/src/keri/app/cli/commands/ipex/admit.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/ipex/agree.py` & `keri-1.1.9/src/keri/app/cli/commands/ipex/agree.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/ipex/grant.py` & `keri-1.1.9/src/keri/app/cli/commands/ipex/grant.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/ipex/join.py` & `keri-1.1.9/src/keri/app/cli/commands/ipex/join.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/ipex/list.py` & `keri-1.1.9/src/keri/app/cli/commands/ipex/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/ipex/offer.py` & `keri-1.1.9/src/keri/app/cli/commands/ipex/offer.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/ipex/spurn.py` & `keri-1.1.9/src/keri/app/cli/commands/ipex/spurn.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/kevers.py` & `keri-1.1.9/src/keri/app/cli/commands/kevers.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/list.py` & `keri-1.1.9/src/keri/app/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/local/watch.py` & `keri-1.1.9/src/keri/app/cli/commands/local/watch.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/mailbox/debug.py` & `keri-1.1.9/src/keri/app/cli/commands/mailbox/debug.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/mailbox/update.py` & `keri-1.1.9/src/keri/app/cli/commands/mailbox/update.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/migrate.py` & `keri-1.1.9/src/keri/app/cli/commands/migrate.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/multisig/continue.py` & `keri-1.1.9/src/keri/app/cli/commands/multisig/continue.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/multisig/demo.py` & `keri-1.1.9/src/keri/app/cli/commands/multisig/demo.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/multisig/incept.py` & `keri-1.1.9/src/keri/app/cli/commands/multisig/incept.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/multisig/interact.py` & `keri-1.1.9/src/keri/app/cli/commands/multisig/interact.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/multisig/join.py` & `keri-1.1.9/src/keri/app/cli/commands/multisig/join.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/multisig/notice.py` & `keri-1.1.9/src/keri/app/cli/commands/multisig/notice.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/multisig/rotate.py` & `keri-1.1.9/src/keri/app/cli/commands/multisig/rotate.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/multisig/shell.py` & `keri-1.1.9/src/keri/app/cli/commands/multisig/shell.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/multisig/update.py` & `keri-1.1.9/src/keri/app/cli/commands/multisig/update.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/oobi/clean.py` & `keri-1.1.9/src/keri/app/cli/commands/oobi/clean.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/oobi/generate.py` & `keri-1.1.9/src/keri/app/cli/commands/oobi/generate.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/oobi/resolve.py` & `keri-1.1.9/src/keri/app/cli/commands/oobi/resolve.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/passcode/generate.py` & `keri-1.1.9/src/keri/app/cli/commands/passcode/generate.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/passcode/remove.py` & `keri-1.1.9/src/keri/app/cli/commands/passcode/remove.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/passcode/set.py` & `keri-1.1.9/src/keri/app/cli/commands/passcode/set.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/query.py` & `keri-1.1.9/src/keri/app/cli/commands/query.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/rename.py` & `keri-1.1.9/src/keri/app/cli/commands/rename.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/rollback.py` & `keri-1.1.9/src/keri/app/cli/commands/rollback.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/rotate.py` & `keri-1.1.9/src/keri/app/cli/commands/rotate.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/saidify.py` & `keri-1.1.9/src/keri/app/cli/commands/saidify.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/salt.py` & `keri-1.1.9/src/keri/app/cli/commands/salt.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/sign.py` & `keri-1.1.9/src/keri/app/cli/commands/sign.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/ssh/export.py` & `keri-1.1.9/src/keri/app/cli/commands/ssh/export.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/status.py` & `keri-1.1.9/src/keri/app/cli/commands/status.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/vc/create.py` & `keri-1.1.9/src/keri/app/cli/commands/vc/create.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/vc/export.py` & `keri-1.1.9/src/keri/app/cli/commands/vc/export.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/vc/list.py` & `keri-1.1.9/src/keri/app/cli/commands/vc/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/vc/registry/incept.py` & `keri-1.1.9/src/keri/app/cli/commands/vc/registry/incept.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/vc/registry/list.py` & `keri-1.1.9/src/keri/app/cli/commands/vc/registry/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/vc/registry/status.py` & `keri-1.1.9/src/keri/app/cli/commands/vc/registry/status.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/vc/revoke.py` & `keri-1.1.9/src/keri/app/cli/commands/vc/revoke.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,48 +118,60 @@
                 anc = hab.rotate(data=[rseal])
             else:
                 anc = hab.interact(data=[rseal])
 
             aserder = serdering.SerderKERI(raw=bytes(anc))
             self.registrar.revoke(creder, rserder, aserder)
 
-            senderHab = self.hab
             if isinstance(self.hab, GroupHab):
-                senderHab = self.hab.mhab
                 smids = self.hab.db.signingMembers(pre=self.hab.pre)
                 smids.remove(self.hab.mhab.pre)
 
                 for recp in smids:  # this goes to other participants only as a signaling mechanism
                     exn, atc = grouping.multisigRevokeExn(ghab=self.hab, said=creder.said, rev=rserder.raw, anc=anc)
                     self.postman.send(src=self.hab.mhab.pre,
                                       dest=recp,
                                       topic="multisig",
                                       serder=exn,
                                       attachment=atc)
 
             while not self.registrar.complete(creder.said, sn=1):
                 yield self.tock
 
-            if self.hab.witnesser() and 'i' in creder.attrib:
-                recp = creder.attrib['i']
+            recps = [creder.attrib['i']] if 'i' in creder.attrib else []
+            if self.send is not None:
+                recps.extend(self.send)
+
+            senderHab = self.hab.mhab if isinstance(self.hab, GroupHab) else self.hab
+
+            if len(recps) > 0:
                 msgs = []
                 for msg in self.hby.db.clonePreIter(pre=creder.issuer):
                     serder = serdering.SerderKERI(raw=msg)
                     atc = msg[serder.size:]
                     msgs.append((serder, atc))
                 for msg in self.rgy.reger.clonePreIter(pre=creder.said):
                     serder = serdering.SerderKERI(raw=msg)
                     atc = msg[serder.size:]
                     msgs.append((serder, atc))
 
-                for (serder, atc) in msgs:
-                    self.postman.send(src=senderHab.pre, dest=recp, topic="credential", serder=serder,
-                                      attachment=atc)
+                sent = 0
+                for send in recps:
+                    if send in self.hby.kevers:
+                        recp = send
+                    else:
+                        recp = self.org.find("alias", send)
+                        if len(recp) != 1:
+                            raise ValueError(f"invalid recipient {send}")
+                        recp = recp[0]['id']
+                    for (serder, atc) in msgs:
+                        self.postman.send(src=senderHab.pre, dest=recp, topic="credential", serder=serder,
+                                          attachment=atc)
+                        sent += 1
 
-                last = msgs[-1][0]
-                while not self.postman.sent(said=last.said):
+                while not len(self.postman.cues) == sent:
                     yield self.tock
 
         except kering.ValidationError as ex:
             raise ex
 
         self.remove(self.toRemove)
```

### Comparing `keri-1.1.8/src/keri/app/cli/commands/verify.py` & `keri-1.1.9/src/keri/app/cli/commands/verify.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/watcher/list.py` & `keri-1.1.9/src/keri/app/cli/commands/watcher/list.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/watcher/start.py` & `keri-1.1.9/src/keri/app/cli/commands/watcher/start.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/watcher/update.py` & `keri-1.1.9/src/keri/app/cli/commands/watcher/update.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/witness/demo.py` & `keri-1.1.9/src/keri/app/cli/commands/witness/demo.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/witness/start.py` & `keri-1.1.9/src/keri/app/cli/commands/witness/start.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/commands/witness/submit.py` & `keri-1.1.9/src/keri/app/cli/commands/witness/submit.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/common/config.py` & `keri-1.1.9/src/keri/app/cli/common/config.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/common/displaying.py` & `keri-1.1.9/src/keri/app/cli/common/displaying.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/common/existing.py` & `keri-1.1.9/src/keri/app/cli/common/existing.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/common/incepting.py` & `keri-1.1.9/src/keri/app/cli/common/incepting.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/common/rotating.py` & `keri-1.1.9/src/keri/app/cli/common/rotating.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/cli/kli.py` & `keri-1.1.9/src/keri/app/cli/kli.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/configing.py` & `keri-1.1.9/src/keri/app/configing.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/connecting.py` & `keri-1.1.9/src/keri/app/connecting.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/delegating.py` & `keri-1.1.9/src/keri/app/delegating.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/directing.py` & `keri-1.1.9/src/keri/app/directing.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/forwarding.py` & `keri-1.1.9/src/keri/app/forwarding.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/grouping.py` & `keri-1.1.9/src/keri/app/grouping.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/habbing.py` & `keri-1.1.9/src/keri/app/habbing.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/httping.py` & `keri-1.1.9/src/keri/app/httping.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/indirecting.py` & `keri-1.1.9/src/keri/app/indirecting.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/keeping.py` & `keri-1.1.9/src/keri/app/keeping.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/notifying.py` & `keri-1.1.9/src/keri/app/notifying.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/oobiing.py` & `keri-1.1.9/src/keri/app/oobiing.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/querying.py` & `keri-1.1.9/src/keri/app/querying.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/signaling.py` & `keri-1.1.9/src/keri/app/signaling.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/signing.py` & `keri-1.1.9/src/keri/app/signing.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/specing.py` & `keri-1.1.9/src/keri/app/specing.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/app/storing.py` & `keri-1.1.9/src/keri/app/storing.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/core/coring.py` & `keri-1.1.9/src/keri/core/coring.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/core/eventing.py` & `keri-1.1.9/src/keri/core/eventing.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/core/parsing.py` & `keri-1.1.9/src/keri/core/parsing.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/core/routing.py` & `keri-1.1.9/src/keri/core/routing.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/core/scheming.py` & `keri-1.1.9/src/keri/core/scheming.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/core/serdering.py` & `keri-1.1.9/src/keri/core/serdering.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/db/basing.py` & `keri-1.1.9/src/keri/db/basing.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/db/dbing.py` & `keri-1.1.9/src/keri/db/dbing.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/db/escrowing.py` & `keri-1.1.9/src/keri/db/escrowing.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/db/koming.py` & `keri-1.1.9/src/keri/db/koming.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/db/subing.py` & `keri-1.1.9/src/keri/db/subing.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/demo/demo_bob.py` & `keri-1.1.9/src/keri/demo/demo_bob.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/demo/demo_eve.py` & `keri-1.1.9/src/keri/demo/demo_eve.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/demo/demo_kev.py` & `keri-1.1.9/src/keri/demo/demo_kev.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/demo/demo_sam.py` & `keri-1.1.9/src/keri/demo/demo_sam.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/demo/demoing.py` & `keri-1.1.9/src/keri/demo/demoing.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/end/ending.py` & `keri-1.1.9/src/keri/end/ending.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/end/priming.py` & `keri-1.1.9/src/keri/end/priming.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/help/__init__.py` & `keri-1.1.9/src/keri/help/__init__.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/help/helping.py` & `keri-1.1.9/src/keri/help/helping.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/kering.py` & `keri-1.1.9/src/keri/kering.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/peer/exchanging.py` & `keri-1.1.9/src/keri/peer/exchanging.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/vc/protocoling.py` & `keri-1.1.9/src/keri/vc/protocoling.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/vc/proving.py` & `keri-1.1.9/src/keri/vc/proving.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/vc/walleting.py` & `keri-1.1.9/src/keri/vc/walleting.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/vdr/credentialing.py` & `keri-1.1.9/src/keri/vdr/credentialing.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/vdr/eventing.py` & `keri-1.1.9/src/keri/vdr/eventing.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/vdr/verifying.py` & `keri-1.1.9/src/keri/vdr/verifying.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri/vdr/viring.py` & `keri-1.1.9/src/keri/vdr/viring.py`

 * *Files identical despite different names*

### Comparing `keri-1.1.8/src/keri.egg-info/PKG-INFO` & `keri-1.1.9/src/keri.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: keri
-Version: 1.1.8
+Version: 1.1.9
 Summary: Key Event Receipt Infrastructure
 Home-page: https://github.com/WebOfTrust/keripy
 Author: Samuel M. Smith
 Author-email: smith.samuel.m@gmail.com
 License: Apache Software License 2.0
 Project-URL: Documentation, https://keri.readthedocs.io/
 Project-URL: Changelog, https://keri.readthedocs.io/en/latest/changelog.html
```

### Comparing `keri-1.1.8/src/keri.egg-info/SOURCES.txt` & `keri-1.1.9/src/keri.egg-info/SOURCES.txt`

 * *Files identical despite different names*

