# Comparing `tmp/ofscraper-3.9.0.dev6.tar.gz` & `tmp/ofscraper-3.9.0.dev7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ofscraper-3.9.0.dev6.tar", max compression
+gzip compressed data, was "ofscraper-3.9.0.dev7.tar", max compression
```

## Comparing `ofscraper-3.9.0.dev6.tar` & `ofscraper-3.9.0.dev7.tar`

### file list

```diff
@@ -1,164 +1,164 @@
--rw-r--r--   0        0        0     1067 2024-03-23 22:44:49.848278 ofscraper-3.9.0.dev6/LICENSE
--rw-r--r--   0        0        0     4067 2024-03-23 22:44:49.848278 ofscraper-3.9.0.dev6/README.md
--rwxr-xr-x   0        0        0      283 2024-03-23 22:44:49.852278 ofscraper-3.9.0.dev6/ofscraper/__main__.py
--rw-r--r--   0        0        0     1064 2024-03-23 22:44:49.852278 ofscraper-3.9.0.dev6/ofscraper/__version__.py
--rw-r--r--   0        0        0      999 2024-03-23 22:44:49.852278 ofscraper-3.9.0.dev6/ofscraper/__version__.pye
--rw-r--r--   0        0        0        1 2024-03-23 22:44:49.852278 ofscraper-3.9.0.dev6/ofscraper/actions/__init__.py
--rw-r--r--   0        0        0     6372 2024-03-23 22:44:49.852278 ofscraper-3.9.0.dev6/ofscraper/actions/like.py
--rw-r--r--   0        0        0     9943 2024-03-23 22:44:49.852278 ofscraper-3.9.0.dev6/ofscraper/actions/process.py
--rw-r--r--   0        0        0    24904 2024-03-23 22:44:49.852278 ofscraper-3.9.0.dev6/ofscraper/actions/scraper.py
--rw-r--r--   0        0        0    13940 2024-03-23 22:44:49.852278 ofscraper-3.9.0.dev6/ofscraper/api/archive.py
--rw-r--r--   0        0        0    21424 2024-03-23 22:44:49.852278 ofscraper-3.9.0.dev6/ofscraper/api/highlights.py
--rw-r--r--   0        0        0     1479 2024-03-23 22:44:49.852278 ofscraper-3.9.0.dev6/ofscraper/api/init.py
--rw-r--r--   0        0        0    13750 2024-03-23 22:44:49.852278 ofscraper-3.9.0.dev6/ofscraper/api/labels.py
--rw-r--r--   0        0        0     4724 2024-03-23 22:44:49.852278 ofscraper-3.9.0.dev6/ofscraper/api/me.py
--rw-r--r--   0        0        0    25141 2024-03-23 22:44:49.852278 ofscraper-3.9.0.dev6/ofscraper/api/messages.py
--rw-r--r--   0        0        0    17526 2024-03-23 22:44:49.852278 ofscraper-3.9.0.dev6/ofscraper/api/paid.py
--rw-r--r--   0        0        0     8246 2024-03-23 22:44:49.852278 ofscraper-3.9.0.dev6/ofscraper/api/pinned.py
--rw-r--r--   0        0        0     8913 2024-03-23 22:44:49.852278 ofscraper-3.9.0.dev6/ofscraper/api/profile.py
--rw-r--r--   0        0        0     3069 2024-03-23 22:44:49.852278 ofscraper-3.9.0.dev6/ofscraper/api/subscriptions/helpers.py
--rw-r--r--   0        0        0     3035 2024-03-23 22:44:49.852278 ofscraper-3.9.0.dev6/ofscraper/api/subscriptions/individual.py
--rw-r--r--   0        0        0    14508 2024-03-23 22:44:49.852278 ofscraper-3.9.0.dev6/ofscraper/api/subscriptions/lists.py
--rw-r--r--   0        0        0    11801 2024-03-23 22:44:49.852278 ofscraper-3.9.0.dev6/ofscraper/api/subscriptions/subscriptions.py
--rw-r--r--   0        0        0    19969 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/api/timeline.py
--rw-r--r--   0        0        0     1413 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/classes/base.py
--rw-r--r--   0        0        0      876 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/classes/labels.py
--rw-r--r--   0        0        0    15247 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/classes/media.py
--rw-r--r--   0        0        0     5892 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/classes/models.py
--rw-r--r--   0        0        0     1771 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/classes/multiprocessprogress.py
--rw-r--r--   0        0        0    20730 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/classes/placeholder.py
--rw-r--r--   0        0        0     4452 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/classes/posts.py
--rw-r--r--   0        0        0      489 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/classes/semaphoreDelayed.py
--rw-r--r--   0        0        0     8226 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/classes/sessionbuilder.py
--rw-r--r--   0        0        0    31963 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/classes/table.py
--rw-r--r--   0        0        0    18318 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/commands/check.py
--rw-r--r--   0        0        0     7479 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/commands/manual.py
--rw-r--r--   0        0        0      430 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/commands/picker.py
--rwxr-xr-x   0        0        0     3915 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/commands/scraper.py
--rw-r--r--   0        0        0       53 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/const/binary.py
--rw-r--r--   0        0        0     1549 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/const/config.py
--rw-r--r--   0        0        0      927 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/const/constants.py
--rw-r--r--   0        0        0       34 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/const/date.py
--rw-r--r--   0        0        0      184 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/const/download.py
--rw-r--r--   0        0        0      204 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/const/files.py
--rw-r--r--   0        0        0     1231 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/const/general.py
--rw-r--r--   0        0        0       93 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/const/logger.py
--rw-r--r--   0        0        0      775 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/const/other_url.py
--rw-r--r--   0        0        0     1876 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/const/prompts.py
--rw-r--r--   0        0        0      615 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/const/req.py
--rw-r--r--   0        0        0   265533 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/const/test_constants.py
--rw-r--r--   0        0        0      213 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/const/time.py
--rw-r--r--   0        0        0     3516 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/const/url.py
--rw-r--r--   0        0        0        1 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/db/__init__.py
--rw-r--r--   0        0        0    20820 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/db/operations.py
--rw-r--r--   0        0        0     5172 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/db/queries.py
--rw-r--r--   0        0        0    14521 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/download/alt_download.py
--rw-r--r--   0        0        0    14694 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/download/alt_downloadbatch.py
--rw-r--r--   0        0        0     5662 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/download/common/common.py
--rw-r--r--   0        0        0     3122 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/download/common/globals.py
--rw-r--r--   0        0        0    12589 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/download/common/keyhelpers.py
--rw-r--r--   0        0        0     2910 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/download/common/log.py
--rw-r--r--   0        0        0      790 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/download/common/message.py
--rw-r--r--   0        0        0     5672 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/download/common/metadata.py
--rw-r--r--   0        0        0     2092 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/download/common/paths.py
--rw-r--r--   0        0        0      453 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/download/common/progress.py
--rw-r--r--   0        0        0     1161 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/download/common/sem.py
--rw-r--r--   0        0        0     1075 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/download/common/text.py
--rw-r--r--   0        0        0     2642 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/download/download.py
--rw-r--r--   0        0        0    16936 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/download/downloadbatch.py
--rw-r--r--   0        0        0     9046 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/download/downloadnormal.py
--rw-r--r--   0        0        0    13069 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/download/main_download.py
--rw-r--r--   0        0        0    13533 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/download/main_downloadbatch.py
--rw-r--r--   0        0        0     5481 2024-03-23 22:44:49.856278 ofscraper-3.9.0.dev6/ofscraper/filters/media/helpers.py
--rw-r--r--   0        0        0    12337 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/filters/media/main.py
--rw-r--r--   0        0        0     2682 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/filters/models/date.py
--rw-r--r--   0        0        0     2532 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/filters/models/flags.py
--rw-r--r--   0        0        0      586 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/filters/models/other.py
--rw-r--r--   0        0        0     6342 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/filters/models/price.py
--rw-r--r--   0        0        0     1415 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/filters/models/sort.py
--rw-r--r--   0        0        0     1122 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/filters/models/subtype.py
--rw-r--r--   0        0        0     3349 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/models/retriver.py
--rw-r--r--   0        0        0     7043 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/models/selector.py
--rw-r--r--   0        0        0     2466 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/prompts/helpers/model_helpers.py
--rw-r--r--   0        0        0    13078 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/prompts/helpers/prompt_helpers.py
--rw-r--r--   0        0        0      846 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/prompts/keybindings.py
--rw-r--r--   0        0        0     7310 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/prompts/promptConvert.py
--rw-r--r--   0        0        0      917 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/prompts/prompt_groups/actions.py
--rw-r--r--   0        0        0     6549 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/prompts/prompt_groups/area.py
--rw-r--r--   0        0        0     8257 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/prompts/prompt_groups/auth.py
--rw-r--r--   0        0        0     4621 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/prompts/prompt_groups/binary.py
--rw-r--r--   0        0        0    27481 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/prompts/prompt_groups/config.py
--rw-r--r--   0        0        0     1878 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/prompts/prompt_groups/menu.py
--rw-r--r--   0        0        0    15703 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/prompts/prompt_groups/model.py
--rw-r--r--   0        0        0     4134 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/prompts/prompt_groups/profile.py
--rw-r--r--   0        0        0     7589 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/prompts/prompt_strings.py
--rw-r--r--   0        0        0    10184 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/prompts/prompt_validators.py
--rw-r--r--   0        0        0     1290 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/prompts/prompts.py
--rw-r--r--   0        0        0      567 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/runner/exit.py
--rw-r--r--   0        0        0     1431 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/runner/load.py
--rw-r--r--   0        0        0     2748 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/runner/run.py
--rw-r--r--   0        0        0        1 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/__init__.py
--rw-r--r--   0        0        0     3806 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/actions.py
--rw-r--r--   0        0        0     1815 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/args/areas.py
--rw-r--r--   0        0        0       12 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/args/globals.py
--rw-r--r--   0        0        0     4914 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/args/helpers.py
--rw-r--r--   0        0        0    27837 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/args/parse.py
--rw-r--r--   0        0        0      383 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/args/quality.py
--rw-r--r--   0        0        0      839 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/args/read.py
--rw-r--r--   0        0        0      552 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/args/user.py
--rw-r--r--   0        0        0      253 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/args/write.py
--rw-r--r--   0        0        0     2148 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/auth/context.py
--rw-r--r--   0        0        0     1680 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/auth/data.py
--rw-r--r--   0        0        0     2131 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/auth/file.py
--rw-r--r--   0        0        0     2843 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/auth/helpers.py
--rw-r--r--   0        0        0     1756 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/auth/make.py
--rw-r--r--   0        0        0     6092 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/auth/request.py
--rw-r--r--   0        0        0      802 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/auth/schema.py
--rw-r--r--   0        0        0     9824 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/binaries.py
--rw-r--r--   0        0        0     1780 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/cache.py
--rw-r--r--   0        0        0     1650 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/checkers.py
--rw-r--r--   0        0        0     2893 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/config/config.py
--rw-r--r--   0        0        0     1090 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/config/context.py
--rw-r--r--   0        0        0      452 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/config/custom.py
--rw-r--r--   0        0        0    23180 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/config/data.py
--rw-r--r--   0        0        0     2110 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/config/file.py
--rw-r--r--   0        0        0     2111 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/config/menu.py
--rw-r--r--   0        0        0     4708 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/config/schema.py
--rw-r--r--   0        0        0      429 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/config/wrapper.py
--rw-r--r--   0        0        0      499 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/console.py
--rw-r--r--   0        0        0      461 2024-03-23 22:44:49.860278 ofscraper-3.9.0.dev6/ofscraper/utils/constants.py
--rw-r--r--   0        0        0     3401 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/context/exit.py
--rw-r--r--   0        0        0     1135 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/context/run_async.py
--rw-r--r--   0        0        0     1014 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/context/stdout.py
--rw-r--r--   0        0        0     2679 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/dates.py
--rw-r--r--   0        0        0     1040 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/encoding.py
--rw-r--r--   0        0        0     1716 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/hash.py
--rw-r--r--   0        0        0     6242 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/logs/classes.py
--rw-r--r--   0        0        0     2588 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/logs/close.py
--rw-r--r--   0        0        0      477 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/logs/globals.py
--rw-r--r--   0        0        0     1551 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/logs/helpers.py
--rw-r--r--   0        0        0     2098 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/logs/logger.py
--rw-r--r--   0        0        0     1672 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/logs/logs.py
--rw-r--r--   0        0        0     5512 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/logs/other.py
--rw-r--r--   0        0        0     3652 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/logs/stdout.py
--rw-r--r--   0        0        0      584 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/manager.py
--rw-r--r--   0        0        0      388 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/me.py
--rw-r--r--   0        0        0     4087 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/menu.py
--rw-r--r--   0        0        0     1732 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/paths/check.py
--rw-r--r--   0        0        0     3105 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/paths/common.py
--rw-r--r--   0        0        0      279 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/paths/manage.py
--rw-r--r--   0        0        0     5061 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/paths/paths.py
--rw-r--r--   0        0        0     1058 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/profiles/data.py
--rw-r--r--   0        0        0     2785 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/profiles/manage.py
--rw-r--r--   0        0        0     1606 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/profiles/tools.py
--rw-r--r--   0        0        0     5084 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/progress.py
--rw-r--r--   0        0        0     4447 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/run.py
--rw-r--r--   0        0        0      255 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/sems.py
--rw-r--r--   0        0        0     1595 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/separate.py
--rw-r--r--   0        0        0     3752 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/settings.py
--rw-r--r--   0        0        0      417 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/system/free.py
--rw-r--r--   0        0        0     3108 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/system/network.py
--rw-r--r--   0        0        0     2448 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/system/system.py
--rw-r--r--   0        0        0     2075 2024-03-23 22:44:49.864278 ofscraper-3.9.0.dev6/ofscraper/utils/text.py
--rw-r--r--   0        0        0     2106 2024-03-23 22:45:14.708390 ofscraper-3.9.0.dev6/pyproject.toml
--rw-r--r--   0        0        0     6190 1970-01-01 00:00:00.000000 ofscraper-3.9.0.dev6/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-02 16:59:06.785275 ofscraper-3.9.0.dev7/LICENSE
+-rw-r--r--   0        0        0     4067 2024-04-02 16:59:06.785275 ofscraper-3.9.0.dev7/README.md
+-rwxr-xr-x   0        0        0      283 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/__main__.py
+-rw-r--r--   0        0        0     1064 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/__version__.py
+-rw-r--r--   0        0        0      999 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/__version__.pye
+-rw-r--r--   0        0        0        1 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/actions/__init__.py
+-rw-r--r--   0        0        0     6372 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/actions/like.py
+-rw-r--r--   0        0        0     9943 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/actions/process.py
+-rw-r--r--   0        0        0    23104 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/actions/scraper.py
+-rw-r--r--   0        0        0    13937 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/archive.py
+-rw-r--r--   0        0        0    21424 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/highlights.py
+-rw-r--r--   0        0        0     1479 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/init.py
+-rw-r--r--   0        0        0    13750 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/labels.py
+-rw-r--r--   0        0        0     4724 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/me.py
+-rw-r--r--   0        0        0    25187 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/messages.py
+-rw-r--r--   0        0        0    17245 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/paid.py
+-rw-r--r--   0        0        0     8246 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/pinned.py
+-rw-r--r--   0        0        0     8913 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/profile.py
+-rw-r--r--   0        0        0     3069 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/subscriptions/helpers.py
+-rw-r--r--   0        0        0     3035 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/subscriptions/individual.py
+-rw-r--r--   0        0        0    14508 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/subscriptions/lists.py
+-rw-r--r--   0        0        0    11801 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/subscriptions/subscriptions.py
+-rw-r--r--   0        0        0    19969 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/api/timeline.py
+-rw-r--r--   0        0        0     1413 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/classes/base.py
+-rw-r--r--   0        0        0      876 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/classes/labels.py
+-rw-r--r--   0        0        0    15247 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/classes/media.py
+-rw-r--r--   0        0        0     5892 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/classes/models.py
+-rw-r--r--   0        0        0     1771 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/classes/multiprocessprogress.py
+-rw-r--r--   0        0        0    20730 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/classes/placeholder.py
+-rw-r--r--   0        0        0     4452 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/classes/posts.py
+-rw-r--r--   0        0        0      489 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/classes/semaphoreDelayed.py
+-rw-r--r--   0        0        0     8226 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/classes/sessionbuilder.py
+-rw-r--r--   0        0        0    31963 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/classes/table.py
+-rw-r--r--   0        0        0    18318 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/commands/check.py
+-rw-r--r--   0        0        0     7479 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/commands/manual.py
+-rw-r--r--   0        0        0      430 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/commands/picker.py
+-rwxr-xr-x   0        0        0     3915 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/commands/scraper.py
+-rw-r--r--   0        0        0       53 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/const/binary.py
+-rw-r--r--   0        0        0     1581 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/const/config.py
+-rw-r--r--   0        0        0      927 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/const/constants.py
+-rw-r--r--   0        0        0       34 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/const/date.py
+-rw-r--r--   0        0        0      184 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/const/download.py
+-rw-r--r--   0        0        0      204 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/const/files.py
+-rw-r--r--   0        0        0     1231 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/const/general.py
+-rw-r--r--   0        0        0       93 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/const/logger.py
+-rw-r--r--   0        0        0      775 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/const/other_url.py
+-rw-r--r--   0        0        0     1876 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/const/prompts.py
+-rw-r--r--   0        0        0      615 2024-04-02 16:59:06.793275 ofscraper-3.9.0.dev7/ofscraper/const/req.py
+-rw-r--r--   0        0        0   265533 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/const/test_constants.py
+-rw-r--r--   0        0        0      212 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/const/time.py
+-rw-r--r--   0        0        0     3516 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/const/url.py
+-rw-r--r--   0        0        0        1 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/db/__init__.py
+-rw-r--r--   0        0        0    44884 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/db/operations.py
+-rw-r--r--   0        0        0     8452 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/db/queries.py
+-rw-r--r--   0        0        0    14959 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/alt_download.py
+-rw-r--r--   0        0        0    15034 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/alt_downloadbatch.py
+-rw-r--r--   0        0        0     6188 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/common/common.py
+-rw-r--r--   0        0        0     3122 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/common/globals.py
+-rw-r--r--   0        0        0    12589 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/common/keyhelpers.py
+-rw-r--r--   0        0        0     2910 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/common/log.py
+-rw-r--r--   0        0        0      790 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/common/message.py
+-rw-r--r--   0        0        0     5678 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/common/metadata.py
+-rw-r--r--   0        0        0     2092 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/common/paths.py
+-rw-r--r--   0        0        0      453 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/common/progress.py
+-rw-r--r--   0        0        0     1161 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/common/sem.py
+-rw-r--r--   0        0        0     1075 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/common/text.py
+-rw-r--r--   0        0        0     2642 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/download.py
+-rw-r--r--   0        0        0    16936 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/downloadbatch.py
+-rw-r--r--   0        0        0     9046 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/downloadnormal.py
+-rw-r--r--   0        0        0    13470 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/main_download.py
+-rw-r--r--   0        0        0    14063 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/download/main_downloadbatch.py
+-rw-r--r--   0        0        0     5481 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/filters/media/helpers.py
+-rw-r--r--   0        0        0    12337 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/filters/media/main.py
+-rw-r--r--   0        0        0     2682 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/filters/models/date.py
+-rw-r--r--   0        0        0     2532 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/filters/models/flags.py
+-rw-r--r--   0        0        0      586 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/filters/models/other.py
+-rw-r--r--   0        0        0     6342 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/filters/models/price.py
+-rw-r--r--   0        0        0     1415 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/filters/models/sort.py
+-rw-r--r--   0        0        0     1122 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/filters/models/subtype.py
+-rw-r--r--   0        0        0     3349 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/models/retriver.py
+-rw-r--r--   0        0        0     7043 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/models/selector.py
+-rw-r--r--   0        0        0     2466 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/helpers/model_helpers.py
+-rw-r--r--   0        0        0    13078 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/helpers/prompt_helpers.py
+-rw-r--r--   0        0        0      846 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/keybindings.py
+-rw-r--r--   0        0        0     7310 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/promptConvert.py
+-rw-r--r--   0        0        0      917 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/actions.py
+-rw-r--r--   0        0        0     6549 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/area.py
+-rw-r--r--   0        0        0     8257 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/auth.py
+-rw-r--r--   0        0        0     4621 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/binary.py
+-rw-r--r--   0        0        0    27481 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/config.py
+-rw-r--r--   0        0        0     1878 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/menu.py
+-rw-r--r--   0        0        0    15703 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/model.py
+-rw-r--r--   0        0        0     4134 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/profile.py
+-rw-r--r--   0        0        0     7589 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_strings.py
+-rw-r--r--   0        0        0    10184 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_validators.py
+-rw-r--r--   0        0        0     1290 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/prompts/prompts.py
+-rw-r--r--   0        0        0      567 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/runner/exit.py
+-rw-r--r--   0        0        0     1431 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/runner/load.py
+-rw-r--r--   0        0        0     2748 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/runner/run.py
+-rw-r--r--   0        0        0        1 2024-04-02 16:59:06.797275 ofscraper-3.9.0.dev7/ofscraper/utils/__init__.py
+-rw-r--r--   0        0        0     3806 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/actions.py
+-rw-r--r--   0        0        0     1815 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/args/areas.py
+-rw-r--r--   0        0        0       12 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/args/globals.py
+-rw-r--r--   0        0        0     4914 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/args/helpers.py
+-rw-r--r--   0        0        0    27837 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/args/parse.py
+-rw-r--r--   0        0        0      383 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/args/quality.py
+-rw-r--r--   0        0        0      839 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/args/read.py
+-rw-r--r--   0        0        0      552 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/args/user.py
+-rw-r--r--   0        0        0      253 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/args/write.py
+-rw-r--r--   0        0        0     2148 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/auth/context.py
+-rw-r--r--   0        0        0     1680 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/auth/data.py
+-rw-r--r--   0        0        0     2131 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/auth/file.py
+-rw-r--r--   0        0        0     2843 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/auth/helpers.py
+-rw-r--r--   0        0        0     1756 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/auth/make.py
+-rw-r--r--   0        0        0     6092 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/auth/request.py
+-rw-r--r--   0        0        0      802 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/auth/schema.py
+-rw-r--r--   0        0        0     9824 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/binaries.py
+-rw-r--r--   0        0        0     1780 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/cache.py
+-rw-r--r--   0        0        0     1650 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/checkers.py
+-rw-r--r--   0        0        0     2893 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/config/config.py
+-rw-r--r--   0        0        0     1090 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/config/context.py
+-rw-r--r--   0        0        0      452 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/config/custom.py
+-rw-r--r--   0        0        0    23180 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/config/data.py
+-rw-r--r--   0        0        0     2110 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/config/file.py
+-rw-r--r--   0        0        0     2111 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/config/menu.py
+-rw-r--r--   0        0        0     4708 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/config/schema.py
+-rw-r--r--   0        0        0      429 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/config/wrapper.py
+-rw-r--r--   0        0        0      499 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/console.py
+-rw-r--r--   0        0        0      461 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/constants.py
+-rw-r--r--   0        0        0     3401 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/context/exit.py
+-rw-r--r--   0        0        0     1135 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/context/run_async.py
+-rw-r--r--   0        0        0     1014 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/context/stdout.py
+-rw-r--r--   0        0        0     2679 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/dates.py
+-rw-r--r--   0        0        0     1040 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/encoding.py
+-rw-r--r--   0        0        0     1716 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/hash.py
+-rw-r--r--   0        0        0     8325 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/logs/classes.py
+-rw-r--r--   0        0        0     2588 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/logs/close.py
+-rw-r--r--   0        0        0      477 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/logs/globals.py
+-rw-r--r--   0        0        0     1551 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/logs/helpers.py
+-rw-r--r--   0        0        0     2098 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/logs/logger.py
+-rw-r--r--   0        0        0     1672 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/logs/logs.py
+-rw-r--r--   0        0        0     5955 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/logs/other.py
+-rw-r--r--   0        0        0     3652 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/logs/stdout.py
+-rw-r--r--   0        0        0      584 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/manager.py
+-rw-r--r--   0        0        0      388 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/me.py
+-rw-r--r--   0        0        0     4087 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/menu.py
+-rw-r--r--   0        0        0     1732 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/paths/check.py
+-rw-r--r--   0        0        0     3105 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/paths/common.py
+-rw-r--r--   0        0        0      279 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/paths/manage.py
+-rw-r--r--   0        0        0     5061 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/paths/paths.py
+-rw-r--r--   0        0        0     1058 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/profiles/data.py
+-rw-r--r--   0        0        0     2785 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/profiles/manage.py
+-rw-r--r--   0        0        0     1606 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/profiles/tools.py
+-rw-r--r--   0        0        0     5615 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/progress.py
+-rw-r--r--   0        0        0     4447 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/run.py
+-rw-r--r--   0        0        0      255 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/sems.py
+-rw-r--r--   0        0        0     1595 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/separate.py
+-rw-r--r--   0        0        0     3752 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/settings.py
+-rw-r--r--   0        0        0      417 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/system/free.py
+-rw-r--r--   0        0        0     3108 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/system/network.py
+-rw-r--r--   0        0        0     2448 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/system/system.py
+-rw-r--r--   0        0        0     2075 2024-04-02 16:59:06.801275 ofscraper-3.9.0.dev7/ofscraper/utils/text.py
+-rw-r--r--   0        0        0     2106 2024-04-02 16:59:36.681179 ofscraper-3.9.0.dev7/pyproject.toml
+-rw-r--r--   0        0        0     6190 1970-01-01 00:00:00.000000 ofscraper-3.9.0.dev7/PKG-INFO
```

### Comparing `ofscraper-3.9.0.dev6/LICENSE` & `ofscraper-3.9.0.dev7/LICENSE`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/README.md` & `ofscraper-3.9.0.dev7/README.md`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/__version__.py` & `ofscraper-3.9.0.dev7/ofscraper/__version__.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/__version__.pye` & `ofscraper-3.9.0.dev7/ofscraper/__version__.pye`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/actions/like.py` & `ofscraper-3.9.0.dev7/ofscraper/actions/like.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/actions/process.py` & `ofscraper-3.9.0.dev7/ofscraper/actions/process.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/actions/scraper.py` & `ofscraper-3.9.0.dev7/ofscraper/actions/scraper.py`

 * *Files 13% similar despite different names*

```diff
@@ -50,20 +50,17 @@
 async def process_messages(model_id, username, c):
     try:
         with stdout.lowstdout():
             messages_ = await messages.get_messages_progress(model_id, username, c=c)
             messages_ = list(
                 map(lambda x: posts_.Post(x, model_id, username), messages_)
             )
-            curr = set(
-                operations.get_all_messages_ids(model_id=model_id, username=username)
-            )
             [
-                operations.write_messages_table(
-                    list(filter(lambda x: x.id not in curr, messages_)),
+                operations.make_messages_table_changes(
+                    messages_,
                     model_id=model_id,
                     username=username,
                 )
             ]
 
             log.debug(
                 f"[bold]Messages media count with locked[/bold] {sum(map(lambda x:len(x.post_media),messages_))}"
@@ -71,15 +68,14 @@
             log.debug("Removing locked messages media")
             output = []
             [output.extend(message.media) for message in messages_]
             log.debug(f"[bold]Messages media count[/bold] {len(output)}")
 
             await operations.batch_mediainsert(
                 output,
-                operations.write_media_table_batch,
                 model_id=model_id,
                 username=username,
                 downloaded=False,
             )
             # Update after database
             cache.set(
                 f"{model_id}_scrape_messages",
@@ -103,30 +99,26 @@
             paid_content = await paid.get_paid_posts_progress(username, model_id, c=c)
             paid_content = list(
                 map(
                     lambda x: posts_.Post(x, model_id, username, responsetype="paid"),
                     paid_content,
                 )
             )
-            curr = set(
-                operations.get_all_post_ids(model_id=model_id, username=username)
-            )
-            operations.write_post_table(
-                list(filter(lambda x: x.id not in curr, paid_content)),
+            operations.make_post_table_changes(
+                paid_content,
                 model_id=model_id,
                 username=username,
             )
 
             output = []
             [output.extend(post.media) for post in paid_content]
             log.debug(f"[bold]Paid media count without locked[/bold] {len(output)}")
 
             await operations.batch_mediainsert(
                 output,
-                operations.write_media_table_batch,
                 model_id=model_id,
                 username=username,
                 downloaded=False,
             )
 
             return (
                 list(filter(lambda x: isinstance(x, media.Media), output)),
@@ -149,31 +141,27 @@
                 map(
                     lambda x: posts_.Post(
                         x, model_id, username, responsetype="stories"
                     ),
                     stories,
                 )
             )
-            curr = set(
-                operations.get_all_stories_ids(model_id=model_id, username=username)
-            )
-            operations.write_stories_table(
-                list(filter(lambda x: x.id not in curr, stories)),
+            operations.make_stories_tables_changes(
+                stories,
                 model_id=model_id,
                 username=username,
             )
 
             log.debug(
                 f"[bold]Story media count[/bold] {sum(map(lambda x:len(x.post_media), stories))}"
             )
             output = []
             [output.extend(stories.media) for stories in stories]
             await operations.batch_mediainsert(
                 output,
-                operations.write_media_table_batch,
                 model_id=model_id,
                 username=username,
                 downloaded=False,
             )
 
             return list(filter(lambda x: isinstance(x, media.Media), output)), stories
     except Exception as E:
@@ -193,31 +181,27 @@
                 map(
                     lambda x: posts_.Post(
                         x, model_id, username, responsetype="highlights"
                     ),
                     highlights_,
                 )
             )
-            curr = set(
-                operations.get_all_stories_ids(model_id=model_id, username=username)
-            )
-            operations.write_stories_table(
-                list(filter(lambda x: x.id not in curr, highlights_)),
+            operations.make_stories_tables_changes(
+                highlights_,
                 model_id=model_id,
                 username=username,
             )
 
             log.debug(
                 f"[bold]highlight media count[/bold] {sum(map(lambda x:len(x.post_media), highlights_))}"
             )
             output = []
             [output.extend(stories.media) for stories in highlights_]
             await operations.batch_mediainsert(
                 output,
-                operations.write_media_table_batch,
                 model_id=model_id,
                 username=username,
                 downloaded=False,
             )
 
             return (
                 list(filter(lambda x: isinstance(x, media.Media), output)),
@@ -240,41 +224,36 @@
             )
             timeline_posts = list(
                 map(
                     lambda x: posts_.Post(x, model_id, username, "timeline"),
                     timeline_posts,
                 )
             )
-
-            curr = set(
-                operations.get_all_post_ids(model_id=model_id, username=username)
-            )
-            operations.write_post_table(
-                list(filter(lambda x: x.id not in curr, timeline_posts)),
+            operations.make_post_table_changes(
+                timeline_posts,
                 model_id=model_id,
                 username=username,
             )
+
             log.debug(
                 f"[bold]Timeline media count with locked[/bold] {sum(map(lambda x:len(x.post_media),timeline_posts))}"
             )
             log.debug("Removing locked timeline media")
             output = []
             [output.extend(post.media) for post in timeline_posts]
             log.debug(f"[bold]Timeline media count without locked[/bold] {len(output)}")
 
             await operations.batch_mediainsert(
                 output,
-                operations.write_media_table_batch,
                 model_id=model_id,
                 username=username,
                 downloaded=False,
             )
             await operations.batch_mediainsert(
                 output,
-                operations.update_response_media_table,
                 model_id=model_id,
                 username=username,
                 downloaded=False,
             )
             cache.set(
                 f"{model_id}_full_timeline_scrape",
                 read_args.retriveArgs().after is not None,
@@ -299,34 +278,30 @@
             archived_posts = list(
                 map(
                     lambda x: posts_.Post(x, model_id, username, "archived"),
                     archived_posts,
                 )
             )
 
-            curr = set(
-                operations.get_all_post_ids(model_id=model_id, username=username)
-            )
-            operations.write_post_table(
-                list(filter(lambda x: x.id not in curr, archived_posts)),
+            operations.make_post_table_changes(
+                archived_posts,
                 model_id=model_id,
                 username=username,
             )
 
             log.debug(
                 f"[bold]Archived media count with locked[/bold] {sum(map(lambda x:len(x.post_media),archived_posts))}"
             )
             log.debug("Removing locked archived media")
             output = []
             [output.extend(post.media) for post in archived_posts]
             log.debug(f"[bold]Archived media count without locked[/bold] {len(output)}")
 
             await operations.batch_mediainsert(
                 output,
-                operations.write_media_table_batch,
                 model_id=model_id,
                 username=username,
                 downloaded=False,
             )
             cache.set(
                 f"{model_id}_full_archived_scrape",
                 read_args.retriveArgs().after is not None,
@@ -349,41 +324,36 @@
         with stdout.lowstdout():
             pinned_posts = await pinned.get_pinned_post(model_id, c=c)
             pinned_posts = list(
                 map(
                     lambda x: posts_.Post(x, model_id, username, "pinned"), pinned_posts
                 )
             )
-            curr = set(
-                operations.get_all_post_ids(model_id=model_id, username=username)
-            )
-            operations.write_post_table(
-                list(filter(lambda x: x.id not in curr, pinned_posts)),
+            operations.make_post_table_changes(
+                pinned_posts,
                 model_id=model_id,
                 username=username,
             )
 
             log.debug(
                 f"[bold]Pinned media count with locked[/bold] {sum(map(lambda x:len(x.post_media),pinned_posts))}"
             )
             log.debug("Removing locked pinned media")
             output = []
             [output.extend(post.media) for post in pinned_posts]
             log.debug(f"[bold]Pinned media count without locked[/bold] {len(output)}")
 
             await operations.batch_mediainsert(
                 output,
-                operations.write_media_table_batch,
                 model_id=model_id,
                 username=username,
                 downloaded=False,
             )
             await operations.batch_mediainsert(
                 output,
-                operations.update_response_media_table,
                 model_id=model_id,
                 username=username,
                 downloaded=False,
             )
 
             return (
                 list(filter(lambda x: isinstance(x, media.Media), output)),
@@ -471,19 +441,16 @@
                     value,
                 )
             )
             new_dict = {}
             for ele in all_posts:
                 new_dict[ele.id] = ele
             new_posts = new_dict.values()
-            curr = set(
-                operations.get_all_post_ids(model_id=model_id, username=username) or []
-            )
-            operations.write_post_table(
-                list(filter(lambda x: x.id not in curr, new_posts)),
+            operations.make_post_table_changes(
+                new_posts,
                 model_id=model_id,
                 username=username,
             )
             temp = []
             [temp.extend(post.media) for post in new_posts]
             output.extend(temp)
             log.debug(
@@ -568,16 +535,15 @@
         else ThreadPoolExecutor()
     )
     try:
         with executor:
             asyncio.get_event_loop().set_default_executor(executor)
             username = ele.name
             output = []
-            group = progress_utils.get_api_progress_Group()
-            with Live(group, console=console_.get_shared_console()):
+            with progress_utils.setup_api_progress_live():
                 medias, posts = await process_task(model_id, username, ele)
                 output.extend(medias)
         return filters.filterMedia(output), filters.filterPost(posts)
     except Exception as E:
         print(E)
         raise E
```

### Comparing `ofscraper-3.9.0.dev6/ofscraper/api/archive.py` & `ofscraper-3.9.0.dev7/ofscraper/api/archive.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,15 @@
         and not read_args.retriveArgs().after
         and not data.get_disable_after()
     ):
         log.info(
             "Used --after previously. Scraping all archived posts required to make sure content is not missing"
         )
         return 0
-    curr = operations.get_archived_postinfo(model_id=model_id, username=username)
+    curr = operations.get_archived_media(model_id=model_id, username=username)
 
     if len(curr) == 0:
         log.debug("Setting date to zero because database is empty")
         return 0
     missing_items = list(filter(lambda x: x[10] != 1, curr))
     missing_items = list(sorted(missing_items, key=lambda x: arrow.get(x[12])))
     if len(missing_items) == 0:
```

### Comparing `ofscraper-3.9.0.dev6/ofscraper/api/highlights.py` & `ofscraper-3.9.0.dev7/ofscraper/api/highlights.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/api/init.py` & `ofscraper-3.9.0.dev7/ofscraper/api/init.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/api/labels.py` & `ofscraper-3.9.0.dev7/ofscraper/api/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/api/me.py` & `ofscraper-3.9.0.dev7/ofscraper/api/me.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/api/messages.py` & `ofscraper-3.9.0.dev7/ofscraper/api/messages.py`

 * *Files 0% similar despite different names*

```diff
@@ -636,15 +636,17 @@
             except Exception as E:
                 await asyncio.sleep(1)
                 log.traceback_(E)
                 log.traceback_(traceback.format_exc())
                 raise E
             finally:
                 sem.release()
-                job_progress.remove_task(task) if job_progress and task else None
+                job_progress.remove_task(
+                    task
+                ) if job_progress and task != None else None
             return messages, new_tasks
 
 
 def get_individual_post(model_id, postid):
     with sessionbuilder.sessionBuilder(
         backend="httpx",
     ) as c:
```

### Comparing `ofscraper-3.9.0.dev6/ofscraper/api/paid.py` & `ofscraper-3.9.0.dev7/ofscraper/api/paid.py`

 * *Files 2% similar despite different names*

```diff
@@ -247,33 +247,28 @@
 
         return media, new_tasks
 
 
 @run
 async def get_all_paid_posts():
     global sem
-    sem = semaphoreDelayed(constants.getattr("MAX_SEMAPHORE"))
+    sem = sems.get_req_sem()
     with ThreadPoolExecutor(
         max_workers=constants.getattr("MAX_REQUEST_WORKERS")
     ) as executor:
         asyncio.get_event_loop().set_default_executor(executor)
-        overall_progress = Progress(
-            SpinnerColumn(style=Style(color="blue")),
-            TextColumn("Getting all paid media...\n{task.description}"),
-        )
-        job_progress = Progress("{task.description}")
-        progress_group = Group(overall_progress, Panel(Group(job_progress)))
 
         output = []
         min_posts = 100
         tasks = []
         page_count = 0
-        with Live(
-            progress_group, refresh_per_second=5, console=console.get_shared_console()
-        ):
+        with progress_utils.setup_all_paid_live():
+            job_progress = progress_utils.all_paid_progress
+            overall_progress = progress_utils.overall_progress
+
             async with sessionbuilder.sessionBuilder() as c:
                 allpaid = cache.get(f"purchased_all", default=[])
                 log.debug(f"[bold]All Paid Cache[/bold] {len(allpaid)} found")
 
                 if len(allpaid) > min_posts:
                     splitArrays = [i for i in range(0, len(allpaid), min_posts)]
                     # use the previous split for timesamp
```

### Comparing `ofscraper-3.9.0.dev6/ofscraper/api/pinned.py` & `ofscraper-3.9.0.dev7/ofscraper/api/pinned.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/api/profile.py` & `ofscraper-3.9.0.dev7/ofscraper/api/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/api/subscriptions/helpers.py` & `ofscraper-3.9.0.dev7/ofscraper/api/subscriptions/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/api/subscriptions/individual.py` & `ofscraper-3.9.0.dev7/ofscraper/api/subscriptions/individual.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/api/subscriptions/lists.py` & `ofscraper-3.9.0.dev7/ofscraper/api/subscriptions/lists.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/api/subscriptions/subscriptions.py` & `ofscraper-3.9.0.dev7/ofscraper/api/subscriptions/subscriptions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/api/timeline.py` & `ofscraper-3.9.0.dev7/ofscraper/api/timeline.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/classes/base.py` & `ofscraper-3.9.0.dev7/ofscraper/classes/base.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/classes/labels.py` & `ofscraper-3.9.0.dev7/ofscraper/classes/labels.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/classes/media.py` & `ofscraper-3.9.0.dev7/ofscraper/classes/media.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/classes/models.py` & `ofscraper-3.9.0.dev7/ofscraper/classes/models.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/classes/multiprocessprogress.py` & `ofscraper-3.9.0.dev7/ofscraper/classes/multiprocessprogress.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/classes/placeholder.py` & `ofscraper-3.9.0.dev7/ofscraper/classes/placeholder.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/classes/posts.py` & `ofscraper-3.9.0.dev7/ofscraper/classes/posts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/classes/sessionbuilder.py` & `ofscraper-3.9.0.dev7/ofscraper/classes/sessionbuilder.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/classes/table.py` & `ofscraper-3.9.0.dev7/ofscraper/classes/table.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/commands/check.py` & `ofscraper-3.9.0.dev7/ofscraper/commands/check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/commands/manual.py` & `ofscraper-3.9.0.dev7/ofscraper/commands/manual.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/commands/scraper.py` & `ofscraper-3.9.0.dev7/ofscraper/commands/scraper.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/const/config.py` & `ofscraper-3.9.0.dev7/ofscraper/const/config.py`

 * *Files 17% similar despite different names*

```diff
@@ -50,7 +50,8 @@
 DISABLE_AFTER_DEFAULT = False
 DEFAULT_USER_LIST = "main"
 DEFAULT_BLACK_LIST = ""
 HASHED_DEFAULT = False
 EMPTY_MEDIA_DEFAULT = {}
 DEFAULT_LOG_LEVEL = "DEBUG"
 INCLUDED_LABELS_ALL = False
+DISCORD_THREAD_OVERRIDE = False
```

### Comparing `ofscraper-3.9.0.dev6/ofscraper/const/constants.py` & `ofscraper-3.9.0.dev7/ofscraper/const/constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/const/general.py` & `ofscraper-3.9.0.dev7/ofscraper/const/general.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/const/other_url.py` & `ofscraper-3.9.0.dev7/ofscraper/const/other_url.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/const/prompts.py` & `ofscraper-3.9.0.dev7/ofscraper/const/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/const/req.py` & `ofscraper-3.9.0.dev7/ofscraper/const/req.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/const/test_constants.py` & `ofscraper-3.9.0.dev7/ofscraper/const/test_constants.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/const/url.py` & `ofscraper-3.9.0.dev7/ofscraper/const/url.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/download/alt_download.py` & `ofscraper-3.9.0.dev7/ofscraper/download/alt_download.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,29 +129,31 @@
             f"{get_medialog(ele)} Attempt to set Date to {arrow.get(newDate).format('YYYY-MM-DD HH:mm')}"
         )
         set_time(sharedPlaceholderObj.trunicated_filepath, newDate)
         common_globals.log.debug(
             f"{get_medialog(ele)} Date set to {arrow.get(sharedPlaceholderObj.trunicated_filepath.stat().st_mtime).format('YYYY-MM-DD HH:mm')}"
         )
     if ele.id:
-        await operations.update_media_table(
+        await operations.download_media_update(
             ele,
             filename=sharedPlaceholderObj.trunicated_filepath,
             model_id=model_id,
             username=username,
             downloaded=True,
-            hash=await common.get_hash(sharedPlaceholderObj, mediatype=ele.mediatype),
+            hashdata=await common.get_hash(
+                sharedPlaceholderObj, mediatype=ele.mediatype
+            ),
         )
     return ele.mediatype, video["total"] + audio["total"]
 
 
 async def media_item_post_process(audio, video, ele, username, model_id):
     if (audio["total"] + video["total"]) == 0:
         if ele.mediatype != "forced_skipped":
-            await operations.update_media_table(
+            await operations.download_media_update(
                 ele,
                 filename=None,
                 model_id=model_id,
                 username=username,
                 downloaded=True,
             )
         return ele.mediatype, 0
@@ -263,70 +265,76 @@
     except OSError as E:
         raise E
     except Exception as E:
         raise E
 
 
 async def send_req_inner(c, ele, item, placeholderObj, job_progress):
-    resume_size = get_resume_size(placeholderObj, mediatype=ele.mediatype)
-    total = item["total"]
-    await update_total(total) if total else None
-    headers = (
-        None
-        if resume_size == 0 or not total
-        else {"Range": f"bytes={resume_size}-{total}"}
-    )
-    params = {
-        "Policy": ele.policy,
-        "Key-Pair-Id": ele.keypair,
-        "Signature": ele.signature,
-    }
-    base_url = re.sub("[0-9a-z]*\.mpd$", "", ele.mpd, re.IGNORECASE)
-    url = f"{base_url}{item['origname']}"
-    async with sem_wrapper(common_globals.req_sem):
-        async with c.requests(url=url, headers=headers, params=params)() as l:
-            if l.ok:
-                await asyncio.get_event_loop().run_in_executor(
-                    common_globals.cache_thread,
-                    partial(
-                        cache.set,
-                        f"{item['name']}_headers",
-                        {
-                            "content-length": l.headers.get("content-length"),
-                            "content-type": l.headers.get("content-type"),
-                        },
-                    ),
-                )
-                new_total = int(l.headers["content-length"])
-                await update_total(new_total) if not item["total"] else None
-                temp_file_logger(placeholderObj, ele)
-                item["total"] = new_total
-                total = item["total"]
-                if await check_forced_skip(ele, total):
-                    item["total"] = 0
-                elif total == resume_size:
-                    None
+    old_total = item["total"]
+    total = old_total
+    try:
+        await common.total_change_helper(None, total)
+        resume_size = get_resume_size(placeholderObj, mediatype=ele.mediatype)
+        headers = (
+            None
+            if resume_size == 0 or not total
+            else {"Range": f"bytes={resume_size}-{total}"}
+        )
+        params = {
+            "Policy": ele.policy,
+            "Key-Pair-Id": ele.keypair,
+            "Signature": ele.signature,
+        }
+        base_url = re.sub("[0-9a-z]*\.mpd$", "", ele.mpd, re.IGNORECASE)
+        url = f"{base_url}{item['origname']}"
+        async with sem_wrapper(common_globals.req_sem):
+            async with c.requests(url=url, headers=headers, params=params)() as l:
+                if l.ok:
+                    await asyncio.get_event_loop().run_in_executor(
+                        common_globals.cache_thread,
+                        partial(
+                            cache.set,
+                            f"{item['name']}_headers",
+                            {
+                                "content-length": l.headers.get("content-length"),
+                                "content-type": l.headers.get("content-type"),
+                            },
+                        ),
+                    )
+                    new_total = int(l.headers["content-length"])
+                    temp_file_logger(placeholderObj, ele)
+                    if await check_forced_skip(ele, new_total):
+                        item["total"] = 0
+                        await common.total_change_helper(None, old_total)
+                    elif total == resume_size:
+                        None
+                    else:
+                        item["total"] = new_total
+                        total = new_total
+                        await common.total_change_helper(old_total, total)
+                        await download_fileobject_writer(
+                            total, l, ele, job_progress, placeholderObj
+                        )
                 else:
-                    await download_fileobject_writer(
-                        total, l, ele, job_progress, placeholderObj
+                    common_globals.log.debug(
+                        f"[bold]  {get_medialog(ele)}  alt download status[/bold]: {l.status}"
                     )
-            else:
-                common_globals.log.debug(
-                    f"[bold]  {get_medialog(ele)}  alt download status[/bold]: {l.status}"
-                )
-                common_globals.log.debug(
-                    f"[bold] {get_medialog(ele)}  alt download text [/bold]: {await l.text_()}"
-                )
-                common_globals.log.debug(
-                    f"[bold]  {get_medialog(ele)} alt download  headers [/bold]: {l.headers}"
-                )
-                l.raise_for_status()
+                    common_globals.log.debug(
+                        f"[bold] {get_medialog(ele)}  alt download text [/bold]: {await l.text_()}"
+                    )
+                    common_globals.log.debug(
+                        f"[bold]  {get_medialog(ele)} alt download  headers [/bold]: {l.headers}"
+                    )
+                    l.raise_for_status()
 
-    await size_checker(placeholderObj.tempfilepath, ele, total)
-    return item
+        await size_checker(placeholderObj.tempfilepath, ele, total)
+        return item
+    except Exception as E:
+        await common.total_change_helper(None, -(total or 0))
+        raise E
 
 
 async def download_fileobject_writer(total, l, ele, job_progress, placeholderObj):
     pathstr = str(placeholderObj.tempfilepath)
 
     downloadprogress = settings.get_download_bars()
 
@@ -358,15 +366,14 @@
                         .absolute()
                         .stat()
                         .st_size,
                     ),
                 )
             (await asyncio.sleep(download_sleep)) if download_sleep else None
     except Exception as E:
-        await update_total(-total)
         raise E
     finally:
         # Close file if needed
         try:
             await fileobject.close()
         except Exception:
             None
```

### Comparing `ofscraper-3.9.0.dev6/ofscraper/download/alt_downloadbatch.py` & `ofscraper-3.9.0.dev7/ofscraper/download/alt_downloadbatch.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,29 +122,31 @@
     if ele.postdate:
         newDate = dates.convert_local_time(ele.postdate)
         set_time(sharedPlaceholderObj.trunicated_filepath, newDate)
         common_globals.innerlog.get().debug(
             f"{get_medialog(ele)} Date set to {arrow.get(sharedPlaceholderObj.trunicated_filepath.stat().st_mtime).format('YYYY-MM-DD HH:mm')}"
         )
     if ele.id:
-        await operations.update_media_table(
+        await operations.download_media_update(
             ele,
             filename=sharedPlaceholderObj.trunicated_filepath,
             model_id=model_id,
             username=username,
             downloaded=True,
-            hash=await common.get_hash(sharedPlaceholderObj, mediatype=ele.mediatype),
+            hashdata=await common.get_hash(
+                sharedPlaceholderObj, mediatype=ele.mediatype
+            ),
         )
     return ele.mediatype, video["total"] + audio["total"]
 
 
 async def media_item_post_process(audio, video, ele, username, model_id):
     if (audio["total"] + video["total"]) == 0:
         if ele.mediatype != "forced_skipped":
-            await operations.update_media_table(
+            await operations.download_media_update(
                 ele,
                 filename=None,
                 model_id=model_id,
                 username=username,
                 downloaded=True,
             )
         return ele.mediatype, 0
@@ -267,74 +269,77 @@
     except OSError as E:
         raise E
     except Exception as E:
         raise E
 
 
 async def send_req_inner(c, ele, item, placeholderObj):
-    resume_size = get_resume_size(placeholderObj, mediatype=ele.mediatype)
-    total = item["total"]
-    await common.send_msg((None, 0, total)) if total else None
-    headers = (
-        None
-        if resume_size == 0 or not total
-        else {"Range": f"bytes={resume_size}-{total}"}
-    )
-    params = {
-        "Policy": ele.policy,
-        "Key-Pair-Id": ele.keypair,
-        "Signature": ele.signature,
-    }
-    base_url = re.sub("[0-9a-z]*\.mpd$", "", ele.mpd, re.IGNORECASE)
-    url = f"{base_url}{item['origname']}"
-    await common.send_msg((None, 0, total)) if total else None
-    async with sem_wrapper(common_globals.req_sem):
-        async with c.requests(url=url, headers=headers, params=params)() as l:
-            if l.ok:
-                await asyncio.get_event_loop().run_in_executor(
-                    common_globals.cache_thread,
-                    partial(
-                        cache.set,
-                        f"{item['name']}_headers",
-                        {
-                            "content-length": l.headers.get("content-length"),
-                            "content-type": l.headers.get("content-type"),
-                        },
-                    ),
-                )
-                new_total = int(l.headers["content-length"])
-                await common.send_msg((None, 0, new_total)) if not total else None
-                temp_file_logger(placeholderObj, ele, common_globals.innerlog.get())
-                item["total"] = new_total
-                total = item["total"]
-                if await check_forced_skip(ele, total) == 0:
-                    item["total"] = 0
-                    return item
-                elif total == resume_size:
-                    None
+    old_total = item["total"]
+    total = old_total
+    try:
+        await common.batch_total_change_helper(None, total)
+        resume_size = get_resume_size(placeholderObj, mediatype=ele.mediatype)
+        headers = (
+            None
+            if resume_size == 0 or not total
+            else {"Range": f"bytes={resume_size}-{total}"}
+        )
+        params = {
+            "Policy": ele.policy,
+            "Key-Pair-Id": ele.keypair,
+            "Signature": ele.signature,
+        }
+        base_url = re.sub("[0-9a-z]*\.mpd$", "", ele.mpd, re.IGNORECASE)
+        url = f"{base_url}{item['origname']}"
+        async with sem_wrapper(common_globals.req_sem):
+            async with c.requests(url=url, headers=headers, params=params)() as l:
+                if l.ok:
+                    await asyncio.get_event_loop().run_in_executor(
+                        common_globals.cache_thread,
+                        partial(
+                            cache.set,
+                            f"{item['name']}_headers",
+                            {
+                                "content-length": l.headers.get("content-length"),
+                                "content-type": l.headers.get("content-type"),
+                            },
+                        ),
+                    )
+                    new_total = int(l.headers["content-length"])
+                    temp_file_logger(placeholderObj, ele, common_globals.innerlog.get())
+                    if await check_forced_skip(ele, new_total) == 0:
+                        item["total"] = 0
+                        await common.batch_total_change_helper(old_total, 0)
+                        return item
+                    elif item["total"] == resume_size:
+                        None
+                    else:
+                        item["total"] = new_total
+                        total = new_total
+                        await common.batch_total_change_helper(old_total, total)
+                        await download_fileobject_writer(total, l, ele, placeholderObj)
                 else:
-                    await download_fileobject_writerr(total, l, ele, placeholderObj)
-
-            else:
-                common_globals.innerlog.get().debug(
-                    f"[bold]  {get_medialog(ele)}  main download data finder status[/bold]: {l.status}"
-                )
-                common_globals.innerlog.get().debug(
-                    f"[bold] {get_medialog(ele)}  main download data finder text [/bold]: {await l.text_()}"
-                )
-                common_globals.innerlog.get().debug(
-                    f"[bold]  {get_medialog(ele)} main download data finder headers [/bold]: {l.headers}"
-                )
-                l.raise_for_status()
-
-    await size_checker(placeholderObj.tempfilepath, ele, total)
-    return item
+                    common_globals.innerlog.get().debug(
+                        f"[bold]  {get_medialog(ele)}  main download data finder status[/bold]: {l.status}"
+                    )
+                    common_globals.innerlog.get().debug(
+                        f"[bold] {get_medialog(ele)}  main download data finder text [/bold]: {await l.text_()}"
+                    )
+                    common_globals.innerlog.get().debug(
+                        f"[bold]  {get_medialog(ele)} main download data finder headers [/bold]: {l.headers}"
+                    )
+                    l.raise_for_status()
+        await size_checker(placeholderObj.tempfilepath, ele, item["total"])
+        return item
+    except Exception as E:
+        await common.batch_total_change_helper(None, -(total or 0))
+        raise E
 
 
-async def download_fileobject_writerr(total, l, ele, placeholderObj):
+async def download_fileobject_writer(total, l, ele, placeholderObj):
     pathstr = str(placeholderObj.tempfilepath)
     try:
         count = 0
         await common.send_msg(
             {
                 "type": "add_task",
                 "args": (
@@ -367,16 +372,14 @@
                             .st_size
                         ),
                     }
                 )
                 count = 0
             (await asyncio.sleep(download_sleep)) if download_sleep else None
     except Exception as E:
-        # reset download data
-        await common.send_msg((None, 0, -total))
         raise E
     finally:
         # Close file if needed
         try:
             await fileobject.close()
         except Exception:
             None
```

### Comparing `ofscraper-3.9.0.dev6/ofscraper/download/common/common.py` & `ofscraper-3.9.0.dev7/ofscraper/download/common/common.py`

 * *Files 7% similar despite different names*

```diff
@@ -139,7 +139,25 @@
     return (
         "mp4"
         if ele.mediatype.lower() == "videos"
         else "jpg"
         if ele.mediatype.lower() == "images"
         else None
     )
+
+
+async def batch_total_change_helper(total, new_total):
+    if not new_total and not new_total:
+        return
+    elif not total:
+        await send_msg((None, 0, new_total))
+    elif total and new_total - total != 0:
+        await send_msg((None, 0, new_total - total))
+
+
+async def total_change_helper(total, new_total):
+    if not new_total and not new_total:
+        return
+    elif not total:
+        await update_total(new_total)
+    elif total and new_total - total != 0:
+        await update_total(new_total - total)
```

### Comparing `ofscraper-3.9.0.dev6/ofscraper/download/common/globals.py` & `ofscraper-3.9.0.dev7/ofscraper/download/common/globals.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/download/common/keyhelpers.py` & `ofscraper-3.9.0.dev7/ofscraper/download/common/keyhelpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/download/common/log.py` & `ofscraper-3.9.0.dev7/ofscraper/download/common/log.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/download/common/message.py` & `ofscraper-3.9.0.dev7/ofscraper/download/common/message.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/download/common/metadata.py` & `ofscraper-3.9.0.dev7/ofscraper/download/common/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     )
     download_data = await asyncio.get_event_loop().run_in_executor(
         common_globals.cache_thread, partial(cache.get, f"{ele.id}_headers")
     )
     for _ in range(2):
         if placeholderObj:
             if ele.id:
-                await operations.update_media_table(
+                await operations.download_media_update(
                     ele,
                     filename=placeholderObj.trunicated_filepath,
                     model_id=model_id,
                     username=username,
                     downloaded=metadata_downloaded_helper(placeholderObj),
                 )
             return (
@@ -39,15 +39,15 @@
                 0,
             )
         elif download_data and download_data.get("content-type"):
             content_type = download_data.get("content-type").split("/")[-1]
             placeholderObj = placeholder.Placeholders(ele)
             await placeholderObj.set_trunicated_filepath(ele, content_type)
             if ele.id:
-                await operations.update_media_table(
+                await operations.download_media_update(
                     ele,
                     filename=placeholderObj.trunicated_filepath,
                     model_id=model_id,
                     username=username,
                     downloaded=metadata_downloaded_helper(placeholderObj),
                 )
             return (
```

### Comparing `ofscraper-3.9.0.dev6/ofscraper/download/common/paths.py` & `ofscraper-3.9.0.dev7/ofscraper/download/common/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/download/common/sem.py` & `ofscraper-3.9.0.dev7/ofscraper/download/common/sem.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/download/common/text.py` & `ofscraper-3.9.0.dev7/ofscraper/download/common/text.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/download/download.py` & `ofscraper-3.9.0.dev7/ofscraper/download/download.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/download/downloadbatch.py` & `ofscraper-3.9.0.dev7/ofscraper/download/downloadbatch.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/download/downloadnormal.py` & `ofscraper-3.9.0.dev7/ofscraper/download/downloadnormal.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/download/main_download.py` & `ofscraper-3.9.0.dev7/ofscraper/download/main_download.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,15 +74,15 @@
         c,
         ele,
         job_progress,
     )
     # special case for zero byte files
     if result[0] == 0:
         if ele.mediatype != "forced_skipped":
-            await operations.update_media_table(
+            await operations.download_media_update(
                 ele,
                 filename=None,
                 model_id=model_id,
                 username=username,
                 downloaded=True,
             )
         return ele.mediatype, 0
@@ -108,21 +108,21 @@
         )
         set_time(path_to_file, newDate)
         common_globals.log.debug(
             f"{get_medialog(ele)} Date set to {arrow.get(path_to_file.stat().st_mtime).format('YYYY-MM-DD HH:mm')}"
         )
 
     if ele.id:
-        await operations.update_media_table(
+        await operations.download_media_update(
             ele,
             filename=path_to_file,
             model_id=model_id,
             username=username,
             downloaded=True,
-            hash=await common.get_hash(path_to_file, mediatype=ele.mediatype),
+            hashdata=await common.get_hash(path_to_file, mediatype=ele.mediatype),
         )
     await set_profile_cache_helper(ele)
     return ele.mediatype, total
 
 
 async def main_download_downloader(c, ele, job_progress):
     downloadspace(mediatype=ele.mediatype)
@@ -237,66 +237,72 @@
     except Exception as E:
         raise E
 
 
 async def send_req_inner(
     c, ele, tempholderObj, job_progress, placeholderObj=None, total=None
 ):
-    resume_size = get_resume_size(tempholderObj, mediatype=ele.mediatype)
-    headers = (
-        None
-        if resume_size == 0 or not total
-        else {"Range": f"bytes={resume_size}-{total}"}
-    )
-    await update_total(total) if total else None
-    async with sem_wrapper(common_globals.req_sem):
-        async with c.requests(url=ele.url, headers=headers)() as r:
-            if r.ok:
-                await asyncio.get_event_loop().run_in_executor(
-                    common_globals.cache_thread,
-                    partial(
-                        cache.set,
-                        f"{ele.id}_headers",
-                        {
-                            "content-length": r.headers.get("content-length"),
-                            "content-type": r.headers.get("content-type"),
-                        },
-                    ),
-                )
-                new_total = int(r.headers["content-length"])
-                await update_total(new_total) if not total else None
-                total = new_total
-                content_type = r.headers.get("content-type").split("/")[-1]
-                content_type = content_type or get_unknown_content_type(ele)
-                if not placeholderObj:
-                    placeholderObj = placeholder.Placeholders(ele, content_type)
-                    await placeholderObj.init()
-                path_to_file_logger(placeholderObj, ele)
-                if await check_forced_skip(ele, total):
-                    total = 0
-                elif total == resume_size:
-                    None
+    old_total = total
+    try:
+        await common.total_change_helper(None, total)
+        resume_size = get_resume_size(tempholderObj, mediatype=ele.mediatype)
+        headers = (
+            None
+            if resume_size == 0 or not total
+            else {"Range": f"bytes={resume_size}-{total}"}
+        )
+        async with sem_wrapper(common_globals.req_sem):
+            async with c.requests(url=ele.url, headers=headers)() as r:
+                if r.ok:
+                    await asyncio.get_event_loop().run_in_executor(
+                        common_globals.cache_thread,
+                        partial(
+                            cache.set,
+                            f"{ele.id}_headers",
+                            {
+                                "content-length": r.headers.get("content-length"),
+                                "content-type": r.headers.get("content-type"),
+                            },
+                        ),
+                    )
+                    new_total = int(r.headers["content-length"])
+                    content_type = r.headers.get("content-type").split("/")[-1]
+                    content_type = content_type or get_unknown_content_type(ele)
+                    if not placeholderObj:
+                        placeholderObj = placeholder.Placeholders(ele, content_type)
+                        await placeholderObj.init()
+                    path_to_file_logger(placeholderObj, ele)
+                    if await check_forced_skip(ele, new_total):
+                        total = 0
+                        await common.total_change_helper(old_total, total)
+                    elif total == resume_size:
+                        None
+                    else:
+                        total = new_total
+                        await common.total_change_helper(old_total, total)
+                        await download_fileobject_writer(
+                            r, job_progress, ele, tempholderObj, placeholderObj, total
+                        )
                 else:
-                    await download_fileobject_writer(
-                        r, job_progress, ele, tempholderObj, placeholderObj, total
+                    common_globals.log.debug(
+                        f"[bold] {get_medialog(ele)} main download response status code [/bold]: {r.status}"
                     )
-            else:
-                common_globals.log.debug(
-                    f"[bold] {get_medialog(ele)} main download response status code [/bold]: {r.status}"
-                )
-                common_globals.log.debug(
-                    f"[bold] {get_medialog(ele)}  main download  response text [/bold]: {await r.text_()}"
-                )
-                common_globals.log.debug(
-                    f"[bold] {get_medialog(ele)}  main download headers [/bold]: {r.headers}"
-                )
-                r.raise_for_status()
+                    common_globals.log.debug(
+                        f"[bold] {get_medialog(ele)}  main download  response text [/bold]: {await r.text_()}"
+                    )
+                    common_globals.log.debug(
+                        f"[bold] {get_medialog(ele)}  main download headers [/bold]: {r.headers}"
+                    )
+                    r.raise_for_status()
 
-    await size_checker(tempholderObj.tempfilepath, ele, total)
-    return (total, tempholderObj.tempfilepath, placeholderObj)
+        await size_checker(tempholderObj.tempfilepath, ele, total)
+        return (total, tempholderObj.tempfilepath, placeholderObj)
+    except Exception as E:
+        await common.total_change_helper(None, -(total or 0))
+        raise E
 
 
 async def download_fileobject_writer(
     r, job_progress, ele, tempholderObj, placeholderObj, total
 ):
     pathstr = str(placeholderObj.trunicated_filepath)
     downloadprogress = settings.get_download_bars()
@@ -328,15 +334,14 @@
                         .absolute()
                         .stat()
                         .st_size,
                     ),
                 )
             (await asyncio.sleep(download_sleep)) if download_sleep else None
     except Exception as E:
-        await update_total(-total)
         raise E
     finally:
         # Close file if needed
         try:
             await fileobject.close()
         except Exception:
             None
```

### Comparing `ofscraper-3.9.0.dev6/ofscraper/download/main_downloadbatch.py` & `ofscraper-3.9.0.dev7/ofscraper/download/main_downloadbatch.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,15 +72,15 @@
             username,
             model_id,
         )
 
     result = list(await main_download_downloader(c, ele))
     if result[0] == 0:
         if ele.mediatype != "forced_skipped":
-            await operations.update_media_table(
+            await operations.download_media_update(
                 ele,
                 filename=None,
                 model_id=model_id,
                 username=username,
                 downloaded=True,
             )
         return ele.mediatype, 0
@@ -105,21 +105,21 @@
             f"{get_medialog(ele)} Attempt to set Date to {arrow.get(newDate).format('YYYY-MM-DD HH:mm')}"
         )
         set_time(path_to_file, newDate)
         common_globals.innerlog.get().debug(
             f"{get_medialog(ele)} Date set to {arrow.get(path_to_file.stat().st_mtime).format('YYYY-MM-DD HH:mm')}"
         )
     if ele.id:
-        await operations.update_media_table(
+        await operations.download_media_update(
             ele,
             filename=path_to_file,
             model_id=model_id,
             username=username,
             downloaded=True,
-            hash=await common.get_hash(path_to_file, mediatype=ele.mediatype),
+            hashdata=await common.get_hash(path_to_file, mediatype=ele.mediatype),
         )
     await set_profile_cache_helper(ele)
     return ele.mediatype, total
 
 
 async def main_download_downloader(c, ele):
     downloadspace(mediatype=ele.mediatype)
@@ -220,66 +220,76 @@
     except OSError as E:
         raise E
     except Exception as E:
         raise E
 
 
 async def send_req_inner(c, ele, tempholderObj, placeholderObj=None, total=None):
-    resume_size = get_resume_size(tempholderObj, mediatype=ele.mediatype)
-    headers = (
-        None
-        if resume_size == 0 or not total
-        else {"Range": f"bytes={resume_size}-{total}"}
-    )
-    await common.send_msg((None, 0, total)) if total else None
-    async with sem_wrapper(common_globals.req_sem):
-        async with c.requests(url=ele.url, headers=headers)() as r:
-            if r.ok:
-                await asyncio.get_event_loop().run_in_executor(
-                    common_globals.cache_thread,
-                    partial(
-                        cache.set,
-                        f"{ele.id}_headers",
-                        {
-                            "content-length": r.headers.get("content-length"),
-                            "content-type": r.headers.get("content-type"),
-                        },
-                    ),
-                )
-                new_total = int(r.headers["content-length"])
-                await common.send_msg((None, 0, new_total)) if not total else None
-                total = new_total
-                content_type = r.headers.get("content-type").split("/")[-1]
-                content_type = get_unknown_content_type(ele)
-                if not placeholderObj:
-                    placeholderObj = placeholder.Placeholders(ele, content_type)
-                    await placeholderObj.init()
-                path_to_file_logger(placeholderObj, ele, common_globals.innerlog.get())
-                if await check_forced_skip(ele, total) == 0:
-                    total = 0
-                elif total == resume_size:
-                    None
+    old_total = total
+    try:
+        await common.batch_total_change_helper(None, total)
+        resume_size = get_resume_size(tempholderObj, mediatype=ele.mediatype)
+        headers = (
+            None
+            if resume_size == 0 or not old_total
+            else {"Range": f"bytes={resume_size}-{total}"}
+        )
+        async with sem_wrapper(common_globals.req_sem):
+            async with c.requests(url=ele.url, headers=headers)() as r:
+                if r.ok:
+                    await asyncio.get_event_loop().run_in_executor(
+                        common_globals.cache_thread,
+                        partial(
+                            cache.set,
+                            f"{ele.id}_headers",
+                            {
+                                "content-length": r.headers.get("content-length"),
+                                "content-type": r.headers.get("content-type"),
+                            },
+                        ),
+                    )
+                    new_total = int(r.headers["content-length"])
+                    content_type = r.headers.get("content-type").split("/")[
+                        -1
+                    ] or get_unknown_content_type(ele)
+                    if not placeholderObj:
+                        placeholderObj = placeholder.Placeholders(ele, content_type)
+                        await placeholderObj.init()
+                    path_to_file_logger(
+                        placeholderObj, ele, common_globals.innerlog.get()
+                    )
+                    if await check_forced_skip(ele, new_total) == 0:
+                        total = 0
+                        await common.batch_total_change_helper(old_total, total)
+                        return (total, tempholderObj.tempfilepath, placeholderObj)
+                    elif total == resume_size:
+                        None
+                    else:
+                        total = new_total
+                        await common.batch_total_change_helper(old_total, total)
+                        await download_fileobject_writer(
+                            r, ele, total, tempholderObj, placeholderObj
+                        )
                 else:
-                    await download_fileobject_writer(
-                        r, ele, total, tempholderObj, placeholderObj
+                    common_globals.innerlog.get().debug(
+                        f"[bold] {get_medialog(ele)} main download response status code [/bold]: {r.status}"
                     )
-            else:
-                common_globals.innerlog.get().debug(
-                    f"[bold] {get_medialog(ele)} main download response status code [/bold]: {r.status}"
-                )
-                common_globals.innerlog.get().debug(
-                    f"[bold] {get_medialog(ele)} main download  response text [/bold]: {await r.text_()}"
-                )
-                common_globals.innerlog.get().debug(
-                    f"[bold] {get_medialog(ele)}main download headers [/bold]: {r.headers}"
-                )
-                r.raise_for_status()
+                    common_globals.innerlog.get().debug(
+                        f"[bold] {get_medialog(ele)} main download  response text [/bold]: {await r.text_()}"
+                    )
+                    common_globals.innerlog.get().debug(
+                        f"[bold] {get_medialog(ele)}main download headers [/bold]: {r.headers}"
+                    )
+                    r.raise_for_status()
 
-    await size_checker(tempholderObj.tempfilepath, ele, total)
-    return (total, tempholderObj.tempfilepath, placeholderObj)
+        await size_checker(tempholderObj.tempfilepath, ele, total)
+        return (total, tempholderObj.tempfilepath, placeholderObj)
+    except Exception as E:
+        await common.batch_total_change_helper(None, -(total or 0))
+        raise E
 
 
 async def download_fileobject_writer(r, ele, total, tempholderObj, placeholderObj):
     pathstr = str(placeholderObj.trunicated_filepath)
     downloadprogress = settings.get_download_bars()
     try:
         count = 0
@@ -320,15 +330,14 @@
                         ),
                     }
                 )
                 count = 0
             (await asyncio.sleep(download_sleep)) if download_sleep else None
     except Exception as E:
         # reset download data
-        await common.send_msg((None, 0, -total))
         raise E
     finally:
         try:
             await common.send_msg({"type": "remove_task", "args": (ele.id,)})
         except:
             None
```

### Comparing `ofscraper-3.9.0.dev6/ofscraper/filters/media/helpers.py` & `ofscraper-3.9.0.dev7/ofscraper/filters/media/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/filters/media/main.py` & `ofscraper-3.9.0.dev7/ofscraper/filters/media/main.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/filters/models/date.py` & `ofscraper-3.9.0.dev7/ofscraper/filters/models/date.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/filters/models/flags.py` & `ofscraper-3.9.0.dev7/ofscraper/filters/models/flags.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/filters/models/other.py` & `ofscraper-3.9.0.dev7/ofscraper/filters/models/other.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/filters/models/price.py` & `ofscraper-3.9.0.dev7/ofscraper/filters/models/price.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/filters/models/sort.py` & `ofscraper-3.9.0.dev7/ofscraper/filters/models/sort.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/filters/models/subtype.py` & `ofscraper-3.9.0.dev7/ofscraper/filters/models/subtype.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/models/retriver.py` & `ofscraper-3.9.0.dev7/ofscraper/models/retriver.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/models/selector.py` & `ofscraper-3.9.0.dev7/ofscraper/models/selector.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/prompts/helpers/model_helpers.py` & `ofscraper-3.9.0.dev7/ofscraper/prompts/helpers/model_helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/prompts/helpers/prompt_helpers.py` & `ofscraper-3.9.0.dev7/ofscraper/prompts/helpers/prompt_helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/prompts/keybindings.py` & `ofscraper-3.9.0.dev7/ofscraper/prompts/keybindings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/prompts/promptConvert.py` & `ofscraper-3.9.0.dev7/ofscraper/prompts/promptConvert.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/prompts/prompt_groups/actions.py` & `ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/actions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/prompts/prompt_groups/area.py` & `ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/area.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/prompts/prompt_groups/auth.py` & `ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/auth.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/prompts/prompt_groups/binary.py` & `ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/binary.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/prompts/prompt_groups/config.py` & `ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/prompts/prompt_groups/menu.py` & `ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/menu.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/prompts/prompt_groups/model.py` & `ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/model.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/prompts/prompt_groups/profile.py` & `ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_groups/profile.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/prompts/prompt_strings.py` & `ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_strings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/prompts/prompt_validators.py` & `ofscraper-3.9.0.dev7/ofscraper/prompts/prompt_validators.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/prompts/prompts.py` & `ofscraper-3.9.0.dev7/ofscraper/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/runner/exit.py` & `ofscraper-3.9.0.dev7/ofscraper/runner/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/runner/load.py` & `ofscraper-3.9.0.dev7/ofscraper/runner/load.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/runner/run.py` & `ofscraper-3.9.0.dev7/ofscraper/runner/run.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/actions.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/actions.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/args/areas.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/args/areas.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/args/helpers.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/args/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/args/parse.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/args/parse.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/args/read.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/args/read.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/args/user.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/args/user.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/auth/context.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/auth/context.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/auth/data.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/auth/data.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/auth/file.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/auth/file.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/auth/helpers.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/auth/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/auth/make.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/auth/make.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/auth/request.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/auth/request.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/auth/schema.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/auth/schema.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/binaries.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/binaries.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/cache.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/cache.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/checkers.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/checkers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/config/config.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/config/config.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/config/context.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/config/context.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/config/data.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/config/data.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/config/file.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/config/file.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/config/menu.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/config/menu.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/config/schema.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/config/schema.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/context/exit.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/context/exit.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/context/run_async.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/context/run_async.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/context/stdout.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/context/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/dates.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/dates.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/encoding.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/hash.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/hash.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/logs/close.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/logs/close.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/logs/helpers.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/logs/helpers.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/logs/logger.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/logs/logger.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/logs/logs.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/logs/logs.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/logs/other.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/logs/other.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,14 +42,21 @@
         for message in messages:
             # set close value
             if event and event.is_set():
                 break
             elif message == "None":
                 count = count + 1
                 continue
+            elif isinstance(message, str):
+                list(
+                    filter(
+                        lambda x: isinstance(x, log_class.DiscordHandler),
+                        log.handlers,
+                    )
+                )[0].handle(message)
             elif isinstance(message, io.TextIOBase):
                 [
                     ele.setStream(message)
                     for ele in filter(
                         lambda x: isinstance(x, logging.StreamHandler),
                         log.handlers,
                     )
@@ -126,23 +133,25 @@
         log_globals.other_log_thread = start_other_thread(
             other_event=log_globals.other_event
         )
 
 
 # updates stream for main process
 def updateOtherLoggerStream():
-    if read_args.retriveArgs().discord == "OFF" and settings.get_log_level() == "OFF":
-        return
-    dates.resetLogDateVManager()
-    stream = open(
-        common_paths.getlogpath(),
-        encoding="utf-8",
-        mode="a",
-    )
-    log_globals.otherqueue_.put_nowait(stream)
+    if settings.get_log_level() and settings.get_log_level() != "OFF":
+        dates.resetLogDateVManager()
+        stream = open(
+            common_paths.getlogpath(),
+            encoding="utf-8",
+            mode="a",
+        )
+        log_globals.otherqueue_.put_nowait(stream)
+    if read_args.retriveArgs().discord and read_args.retriveArgs().discord != "OFF":
+        temp = log_class.DiscordHandler()
+        log_globals.otherqueue_.put_nowait(temp._url)
 
 
 def init_other_logger(name):
     name = name or "ofscraper_other"
     log = logging.getLogger(name)
     log.handlers.clear()
     format = " %(asctime)s:\[%(module)s.%(funcName)s:%(lineno)d]  %(message)s"
```

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/logs/stdout.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/logs/stdout.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/manager.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/manager.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/menu.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/menu.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/paths/check.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/paths/check.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/paths/common.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/paths/common.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/paths/paths.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/paths/paths.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/profiles/data.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/profiles/data.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/profiles/manage.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/profiles/manage.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/profiles/tools.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/profiles/tools.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/progress.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/progress.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from rich.console import Group
 from rich.layout import Layout
+from rich.live import Live
 from rich.panel import Panel
 from rich.progress import (
     BarColumn,
     DownloadColumn,
     Progress,
     SpinnerColumn,
     TaskProgressColumn,
@@ -17,15 +18,30 @@
 
 import ofscraper.utils.args.read as read_args
 import ofscraper.utils.config.data as config_data
 import ofscraper.utils.console as console_
 from ofscraper.classes.multiprocessprogress import MultiprocessProgress as MultiProgress
 
 
-def get_api_progress_Group():
+def setup_all_paid_live():
+    global all_paid_progress
+    global overall_progress
+    all_paid_progress = Progress("{task.description}")
+    overall_progress = Progress(
+        SpinnerColumn(style=Style(color="blue")),
+        TextColumn("{task.description}"),
+    )
+    progress_group = Group(overall_progress, Panel(Group(all_paid_progress)))
+
+    return Live(
+        progress_group, refresh_per_second=5, console=console_.get_shared_console()
+    )
+
+
+def setup_api_progress_live():
     global timeline_layout
     global pinned_layout
     global archived_layout
     global labelled_layout
     global messages_layout
     global paid_layout
     global stories_layout
@@ -47,15 +63,15 @@
         paid_layout,
         stories_layout,
         highlights_layout,
         Layout(name="OF-Scaper", size=0, ratio=0),
     )
 
     progress_group = Group(overall_progress, layout)
-    return progress_group
+    return Live(progress_group, console=console_.get_shared_console())
 
 
 def setup_layout():
     global timeline_progress
     global pinned_progress
     global overall_progress
     global archived_progress
```

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/run.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/run.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/separate.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/separate.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/settings.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/settings.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/system/network.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/system/network.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/system/system.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/system/system.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/ofscraper/utils/text.py` & `ofscraper-3.9.0.dev7/ofscraper/utils/text.py`

 * *Files identical despite different names*

### Comparing `ofscraper-3.9.0.dev6/pyproject.toml` & `ofscraper-3.9.0.dev7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ofscraper"
-version = "3.9.0dev6"
+version = "3.9.0dev7"
 description = "automatically scrape onlyfans"
 authors = ["datawhores <datawhores@riseup.net>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.11,<3.14"
```

### Comparing `ofscraper-3.9.0.dev6/PKG-INFO` & `ofscraper-3.9.0.dev7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ofscraper
-Version: 3.9.0.dev6
+Version: 3.9.0.dev7
 Summary: automatically scrape onlyfans
 Author: datawhores
 Author-email: datawhores@riseup.net
 Requires-Python: >=3.11,<3.14
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ofscraper Version: 3.9.0.dev6 Summary:
+Metadata-Version: 2.1 Name: ofscraper Version: 3.9.0.dev7 Summary:
 automatically scrape onlyfans Author: datawhores Author-email:
 datawhores@riseup.net Requires-Python: >=3.11,<3.14 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Provides-Extra: pyinstaller
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0) Requires-Dist: aiohttp[speedups]
 (>=3.8.5,<4.0.0) Requires-Dist: aioprocessing (>=2.0.1,<3.0.0) Requires-Dist:
 aiosqlite (>=0.20.0,<0.21.0) Requires-Dist: arrow (>=1.3.0,<2.0.0) Requires-
```

