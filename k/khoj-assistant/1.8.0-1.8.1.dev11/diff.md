# Comparing `tmp/khoj_assistant-1.8.0.tar.gz` & `tmp/khoj_assistant-1.8.1.dev11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sat Mar 30 18:36:15 2024, max compression
+gzip compressed data, last modified: Tue Apr  2 10:19:42 2024, max compression
```

## Comparing `khoj_assistant-1.8.0.tar` & `khoj_assistant-1.8.1.dev11.tar`

### file list

```diff
@@ -1,181 +1,182 @@
--rw-r--r--   0        0        0        0 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/__init__.py
--rw-r--r--   0        0        0    14822 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/configure.py
--rw-r--r--   0        0        0     5330 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/main.py
--rwxr-xr-x   0        0        0      664 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/manage.py
--rw-r--r--   0        0        0     2832 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/app/README.md
--rw-r--r--   0        0        0        0 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/app/__init__.py
--rw-r--r--   0        0        0     4534 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/app/settings.py
--rw-r--r--   0        0        0      869 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/app/urls.py
--rw-r--r--   0        0        0      388 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/app/wsgi.py
--rw-r--r--   0        0        0        0 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/__init__.py
--rw-r--r--   0        0        0     5419 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/admin.py
--rw-r--r--   0        0        0      153 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/apps.py
--rw-r--r--   0        0        0       60 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/tests.py
--rw-r--r--   0        0        0    33265 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/adapters/__init__.py
--rw-r--r--   0        0        0     4077 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0001_khojuser.py
--rw-r--r--   0        0        0     1195 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0002_googleuser.py
--rw-r--r--   0        0        0      224 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0003_vector_extension.py
--rw-r--r--   0        0        0     8202 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0004_content_types_and_more.py
--rw-r--r--   0        0        0      429 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0005_embeddings_corpus_id.py
--rw-r--r--   0        0        0     1131 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0006_embeddingsdates.py
--rw-r--r--   0        0        0      917 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0007_add_conversation.py
--rw-r--r--   0        0        0      399 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0008_alter_conversation_conversation_log.py
--rw-r--r--   0        0        0      876 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0009_khojapiuser.py
--rw-r--r--   0        0        0     3347 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0010_chatmodeloptions_and_more.py
--rw-r--r--   0        0        0      773 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0010_rename_embeddings_entry_and_more.py
--rw-r--r--   0        0        0      331 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0011_merge_20231102_0138.py
--rw-r--r--   0        0        0      552 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0012_entry_file_source.py
--rw-r--r--   0        0        0     1311 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0013_subscription.py
--rw-r--r--   0        0        0      411 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0014_alter_googleuser_picture.py
--rw-r--r--   0        0        0      584 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0015_alter_subscription_user.py
--rw-r--r--   0        0        0      429 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0016_alter_subscription_renewal_date.py
--rw-r--r--   0        0        0     1219 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0017_searchmodel.py
--rw-r--r--   0        0        0     1152 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0018_searchmodelconfig_delete_searchmodel.py
--rw-r--r--   0        0        0      843 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0019_alter_googleuser_family_name_and_more.py
--rw-r--r--   0        0        0     1190 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0020_reflectivequestion.py
--rw-r--r--   0        0        0     1504 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0021_speechtotextmodeloptions_and_more.py
--rw-r--r--   0        0        0      904 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0022_texttoimagemodelconfig.py
--rw-r--r--   0        0        0     1122 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0023_usersearchmodelconfig.py
--rw-r--r--   0        0        0      405 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0024_alter_entry_embeddings.py
--rw-r--r--   0        0        0     1573 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0025_clientapplication_khojuser_phone_number_and_more.py
--rw-r--r--   0        0        0      691 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0025_searchmodelconfig_embeddings_inference_endpoint_and_more.py
--rw-r--r--   0        0        0      731 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0026_searchmodelconfig_cross_encoder_inference_endpoint_and_more.py
--rw-r--r--   0        0        0      375 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0027_merge_20240118_1324.py
--rw-r--r--   0        0        0      405 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0028_khojuser_verified_phone_number.py
--rw-r--r--   0        0        0      934 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0029_userrequests.py
--rw-r--r--   0        0        0     1252 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0030_conversation_slug_and_title.py
--rw-r--r--   0        0        0     2033 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0031_agent_conversation_agent.py
--rw-r--r--   0        0        0      812 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0031_alter_googleuser_locale.py
--rw-r--r--   0        0        0      317 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0032_merge_20240322_0427.py
--rw-r--r--   0        0        0      369 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/0033_rename_tuning_agent_personality.py
--rw-r--r--   0        0        0        0 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/migrations/__init__.py
--rw-r--r--   0        0        0    11122 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/database/models/__init__.py
--rw-r--r--   0        0        0     1651 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/404.html
--rw-r--r--   0        0        0     8953 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/agent.html
--rw-r--r--   0        0        0     6672 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/agents.html
--rw-r--r--   0        0        0    11089 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/base_config.html
--rw-r--r--   0        0        0      657 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/base_processor_integration.html
--rw-r--r--   0        0        0   100892 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/chat.html
--rw-r--r--   0        0        0    37581 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/config.html
--rw-r--r--   0        0        0     5367 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/content_source_computer_input.html
--rw-r--r--   0        0        0     7225 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/content_source_github_input.html
--rw-r--r--   0        0        0     3655 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/content_source_notion_input.html
--rw-r--r--   0        0        0     1628 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/khoj.webmanifest
--rw-r--r--   0        0        0     4218 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/login.html
--rw-r--r--   0        0        0     2910 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/processor_conversation_input.html
--rw-r--r--   0        0        0    18326 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/search.html
--rw-r--r--   0        0        0     2168 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/utils.html
--rw-r--r--   0        0        0     5160 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/khoj.css
--rw-r--r--   0        0        0   275822 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/markdown-it.min.js
--rw-r--r--   0        0        0    58643 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/org.min.js
--rw-r--r--   0        0        0    73396 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/pico.min.css
--rw-r--r--   0        0        0     1222 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/utils.js
--rw-r--r--   0        0        0    51584 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/chat.svg
--rw-r--r--   0        0        0    10517 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/computer.png
--rw-r--r--   0        0        0      549 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/confirm-icon.svg
--rw-r--r--   0        0        0      503 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/copy-solid.svg
--rw-r--r--   0        0        0      746 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/copy_button.svg
--rw-r--r--   0        0        0    19662 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/credit-card.png
--rw-r--r--   0        0        0   205167 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/favicon-128x128.ico
--rw-r--r--   0        0        0    12518 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/favicon-128x128.png
--rw-r--r--   0        0        0    30234 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/favicon-256x256.png
--rw-r--r--   0        0        0    31531 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/favicon.icns
--rw-r--r--   0        0        0      964 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/github.svg
--rw-r--r--   0        0        0     1100 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/key.svg
--rw-r--r--   0        0        0    13011 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
--rw-r--r--   0        0        0    29856 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/khoj-logo-sideways-500.png
--rw-r--r--   0        0        0  1301428 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
--rw-r--r--   0        0        0     4031 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/logotype.svg
--rw-r--r--   0        0        0      283 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/markdown.svg
--rw-r--r--   0        0        0      616 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/microphone-solid.svg
--rw-r--r--   0        0        0     1578 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/notion.svg
--rw-r--r--   0        0        0     1736 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/openai-logomark.svg
--rw-r--r--   0        0        0     7946 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/org.svg
--rw-r--r--   0        0        0     2504 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/pdf.svg
--rw-r--r--   0        0        0     2945 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/plaintext.svg
--rw-r--r--   0        0        0     1877 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/question-mark-icon.svg
--rw-r--r--   0        0        0     1319 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/stop-solid.svg
--rw-r--r--   0        0        0      503 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/trash-solid.svg
--rw-r--r--   0        0        0     2233 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/user-silhouette.svg
--rw-r--r--   0        0        0      951 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/web.svg
--rw-r--r--   0        0        0     2417 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/whatsapp.svg
--rw-r--r--   0        0        0   591182 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/samples/desktop-browse-draw-sample.png
--rw-r--r--   0        0        0   197173 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/samples/desktop-plain-chat-sample.png
--rw-r--r--   0        0        0   268309 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/samples/desktop-remember-plan-sample.png
--rw-r--r--   0        0        0   406179 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/samples/phone-browse-draw-sample.png
--rw-r--r--   0        0        0    82985 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/samples/phone-plain-chat-sample.png
--rw-r--r--   0        0        0   236285 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/interface/web/assets/samples/phone-remember-plan-sample.png
--rw-r--r--   0        0        0        0 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/migrations/__init__.py
--rw-r--r--   0        0        0     1928 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/migrations/migrate_offline_chat_default_model.py
--rw-r--r--   0        0        0     2510 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/migrations/migrate_offline_chat_schema.py
--rw-r--r--   0        0        0      975 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/migrations/migrate_offline_model.py
--rw-r--r--   0        0        0     2025 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/migrations/migrate_processor_config_openai.py
--rw-r--r--   0        0        0     5132 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/migrations/migrate_server_pg.py
--rw-r--r--   0        0        0      569 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/migrations/migrate_version.py
--rw-r--r--   0        0        0        0 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/__init__.py
--rw-r--r--   0        0        0     4715 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/embeddings.py
--rw-r--r--   0        0        0        0 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/content/__init__.py
--rw-r--r--   0        0        0    12604 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/content/text_to_entries.py
--rw-r--r--   0        0        0        0 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/content/github/__init__.py
--rw-r--r--   0        0        0    13721 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/content/github/github_to_entries.py
--rw-r--r--   0        0        0        0 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/content/markdown/__init__.py
--rw-r--r--   0        0        0     5690 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/content/markdown/markdown_to_entries.py
--rw-r--r--   0        0        0     9871 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/content/notion/notion_to_entries.py
--rw-r--r--   0        0        0        0 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/content/org_mode/__init__.py
--rw-r--r--   0        0        0     6377 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/content/org_mode/org_to_entries.py
--rw-r--r--   0        0        0    18246 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/content/org_mode/orgnode.py
--rw-r--r--   0        0        0        0 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/content/pdf/__init__.py
--rw-r--r--   0        0        0     4660 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/content/pdf/pdf_to_entries.py
--rw-r--r--   0        0        0        0 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/content/plaintext/__init__.py
--rw-r--r--   0        0        0     3717 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/content/plaintext/plaintext_to_entries.py
--rw-r--r--   0        0        0        0 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/conversation/__init__.py
--rw-r--r--   0        0        0    21750 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/conversation/prompts.py
--rw-r--r--   0        0        0     9619 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/conversation/utils.py
--rw-r--r--   0        0        0        0 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/conversation/offline/__init__.py
--rw-r--r--   0        0        0    10729 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/conversation/offline/chat_model.py
--rw-r--r--   0        0        0     1548 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/conversation/offline/utils.py
--rw-r--r--   0        0        0      470 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/conversation/offline/whisper.py
--rw-r--r--   0        0        0        0 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/conversation/openai/__init__.py
--rw-r--r--   0        0        0     6854 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/conversation/openai/gpt.py
--rw-r--r--   0        0        0     3433 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/conversation/openai/utils.py
--rw-r--r--   0        0        0      432 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/conversation/openai/whisper.py
--rw-r--r--   0        0        0        0 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/tools/__init__.py
--rw-r--r--   0        0        0     5929 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/processor/tools/online_search.py
--rw-r--r--   0        0        0        0 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/routers/__init__.py
--rw-r--r--   0        0        0    14566 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/routers/api.py
--rw-r--r--   0        0        0     1443 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/routers/api_agents.py
--rw-r--r--   0        0        0    14988 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/routers/api_chat.py
--rw-r--r--   0        0        0    10614 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/routers/api_config.py
--rw-r--r--   0        0        0     2208 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/routers/api_phone.py
--rw-r--r--   0        0        0     4569 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/routers/auth.py
--rw-r--r--   0        0        0    28123 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/routers/helpers.py
--rw-r--r--   0        0        0    12706 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/routers/indexer.py
--rw-r--r--   0        0        0     1151 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/routers/storage.py
--rw-r--r--   0        0        0     4285 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/routers/subscription.py
--rw-r--r--   0        0        0     1081 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/routers/twilio.py
--rw-r--r--   0        0        0    13166 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/routers/web_client.py
--rw-r--r--   0        0        0        0 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/search_filter/__init__.py
--rw-r--r--   0        0        0      358 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/search_filter/base_filter.py
--rw-r--r--   0        0        0     6438 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/search_filter/date_filter.py
--rw-r--r--   0        0        0      939 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/search_filter/file_filter.py
--rw-r--r--   0        0        0     1005 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/search_filter/word_filter.py
--rw-r--r--   0        0        0        0 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/search_type/__init__.py
--rw-r--r--   0        0        0    11451 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/search_type/image_search.py
--rw-r--r--   0        0        0     8916 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/search_type/text_search.py
--rw-r--r--   0        0        0        0 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/utils/__init__.py
--rw-r--r--   0        0        0     3466 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/utils/cli.py
--rw-r--r--   0        0        0     1874 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/utils/config.py
--rw-r--r--   0        0        0      784 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/utils/constants.py
--rw-r--r--   0        0        0     9519 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/utils/fs_syncer.py
--rw-r--r--   0        0        0    12034 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/utils/helpers.py
--rw-r--r--   0        0        0     7415 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/utils/initialization.py
--rw-r--r--   0        0        0     1192 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/utils/jsonl.py
--rw-r--r--   0        0        0     2009 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/utils/models.py
--rw-r--r--   0        0        0     4021 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/utils/rawconfig.py
--rw-r--r--   0        0        0     1341 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/utils/state.py
--rw-r--r--   0        0        0     1430 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/src/khoj/utils/yaml.py
--rw-r--r--   0        0        0      565 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/.gitignore
--rw-r--r--   0        0        0    34523 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/LICENSE
--rw-r--r--   0        0        0     2007 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/README.md
--rw-r--r--   0        0        0     3566 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/pyproject.toml
--rw-r--r--   0        0        0     5363 2024-03-30 18:36:15.000000 khoj_assistant-1.8.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/__init__.py
+-rw-r--r--   0        0        0    14822 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/configure.py
+-rw-r--r--   0        0        0     5330 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/main.py
+-rwxr-xr-x   0        0        0      664 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/manage.py
+-rw-r--r--   0        0        0     2832 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/app/README.md
+-rw-r--r--   0        0        0        0 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/app/__init__.py
+-rw-r--r--   0        0        0     4534 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/app/settings.py
+-rw-r--r--   0        0        0      869 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/app/urls.py
+-rw-r--r--   0        0        0      388 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/app/wsgi.py
+-rw-r--r--   0        0        0        0 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/__init__.py
+-rw-r--r--   0        0        0     5419 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/admin.py
+-rw-r--r--   0        0        0      153 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/apps.py
+-rw-r--r--   0        0        0       60 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/tests.py
+-rw-r--r--   0        0        0    33288 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/adapters/__init__.py
+-rw-r--r--   0        0        0     4077 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0001_khojuser.py
+-rw-r--r--   0        0        0     1195 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0002_googleuser.py
+-rw-r--r--   0        0        0      224 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0003_vector_extension.py
+-rw-r--r--   0        0        0     8202 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0004_content_types_and_more.py
+-rw-r--r--   0        0        0      429 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0005_embeddings_corpus_id.py
+-rw-r--r--   0        0        0     1131 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0006_embeddingsdates.py
+-rw-r--r--   0        0        0      917 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0007_add_conversation.py
+-rw-r--r--   0        0        0      399 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0008_alter_conversation_conversation_log.py
+-rw-r--r--   0        0        0      876 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0009_khojapiuser.py
+-rw-r--r--   0        0        0     3347 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0010_chatmodeloptions_and_more.py
+-rw-r--r--   0        0        0      773 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0010_rename_embeddings_entry_and_more.py
+-rw-r--r--   0        0        0      331 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0011_merge_20231102_0138.py
+-rw-r--r--   0        0        0      552 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0012_entry_file_source.py
+-rw-r--r--   0        0        0     1311 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0013_subscription.py
+-rw-r--r--   0        0        0      411 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0014_alter_googleuser_picture.py
+-rw-r--r--   0        0        0      584 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0015_alter_subscription_user.py
+-rw-r--r--   0        0        0      429 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0016_alter_subscription_renewal_date.py
+-rw-r--r--   0        0        0     1219 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0017_searchmodel.py
+-rw-r--r--   0        0        0     1152 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0018_searchmodelconfig_delete_searchmodel.py
+-rw-r--r--   0        0        0      843 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0019_alter_googleuser_family_name_and_more.py
+-rw-r--r--   0        0        0     1190 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0020_reflectivequestion.py
+-rw-r--r--   0        0        0     1504 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0021_speechtotextmodeloptions_and_more.py
+-rw-r--r--   0        0        0      904 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0022_texttoimagemodelconfig.py
+-rw-r--r--   0        0        0     1122 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0023_usersearchmodelconfig.py
+-rw-r--r--   0        0        0      405 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0024_alter_entry_embeddings.py
+-rw-r--r--   0        0        0     1573 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0025_clientapplication_khojuser_phone_number_and_more.py
+-rw-r--r--   0        0        0      691 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0025_searchmodelconfig_embeddings_inference_endpoint_and_more.py
+-rw-r--r--   0        0        0      731 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0026_searchmodelconfig_cross_encoder_inference_endpoint_and_more.py
+-rw-r--r--   0        0        0      375 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0027_merge_20240118_1324.py
+-rw-r--r--   0        0        0      405 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0028_khojuser_verified_phone_number.py
+-rw-r--r--   0        0        0      934 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0029_userrequests.py
+-rw-r--r--   0        0        0     1252 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0030_conversation_slug_and_title.py
+-rw-r--r--   0        0        0     2033 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0031_agent_conversation_agent.py
+-rw-r--r--   0        0        0      812 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0031_alter_googleuser_locale.py
+-rw-r--r--   0        0        0      317 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0032_merge_20240322_0427.py
+-rw-r--r--   0        0        0      369 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0033_rename_tuning_agent_personality.py
+-rw-r--r--   0        0        0        0 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/__init__.py
+-rw-r--r--   0        0        0    11129 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/database/models/__init__.py
+-rw-r--r--   0        0        0     1651 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/404.html
+-rw-r--r--   0        0        0     8953 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/agent.html
+-rw-r--r--   0        0        0     6672 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/agents.html
+-rw-r--r--   0        0        0    11089 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/base_config.html
+-rw-r--r--   0        0        0      657 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/base_processor_integration.html
+-rw-r--r--   0        0        0   100892 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/chat.html
+-rw-r--r--   0        0        0    37581 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/config.html
+-rw-r--r--   0        0        0     5367 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/content_source_computer_input.html
+-rw-r--r--   0        0        0     7225 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/content_source_github_input.html
+-rw-r--r--   0        0        0     3655 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/content_source_notion_input.html
+-rw-r--r--   0        0        0     1628 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/khoj.webmanifest
+-rw-r--r--   0        0        0     4218 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/login.html
+-rw-r--r--   0        0        0     2910 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/processor_conversation_input.html
+-rw-r--r--   0        0        0    18326 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/search.html
+-rw-r--r--   0        0        0     2168 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/utils.html
+-rw-r--r--   0        0        0     5160 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/khoj.css
+-rw-r--r--   0        0        0   275822 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/markdown-it.min.js
+-rw-r--r--   0        0        0    58643 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/org.min.js
+-rw-r--r--   0        0        0    73396 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/pico.min.css
+-rw-r--r--   0        0        0     1222 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/utils.js
+-rw-r--r--   0        0        0    51584 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/chat.svg
+-rw-r--r--   0        0        0    10517 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/computer.png
+-rw-r--r--   0        0        0      549 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/confirm-icon.svg
+-rw-r--r--   0        0        0      503 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/copy-solid.svg
+-rw-r--r--   0        0        0      746 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/copy_button.svg
+-rw-r--r--   0        0        0    19662 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/credit-card.png
+-rw-r--r--   0        0        0   205167 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/favicon-128x128.ico
+-rw-r--r--   0        0        0    12518 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/favicon-128x128.png
+-rw-r--r--   0        0        0    30234 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/favicon-256x256.png
+-rw-r--r--   0        0        0    31531 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/favicon.icns
+-rw-r--r--   0        0        0      964 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/github.svg
+-rw-r--r--   0        0        0     1100 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/key.svg
+-rw-r--r--   0        0        0    13011 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png
+-rw-r--r--   0        0        0    29856 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/khoj-logo-sideways-500.png
+-rw-r--r--   0        0        0  1301428 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg
+-rw-r--r--   0        0        0     4031 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/logotype.svg
+-rw-r--r--   0        0        0      283 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/markdown.svg
+-rw-r--r--   0        0        0      616 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/microphone-solid.svg
+-rw-r--r--   0        0        0     1578 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/notion.svg
+-rw-r--r--   0        0        0     1736 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/openai-logomark.svg
+-rw-r--r--   0        0        0     7946 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/org.svg
+-rw-r--r--   0        0        0     2504 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/pdf.svg
+-rw-r--r--   0        0        0     2945 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/plaintext.svg
+-rw-r--r--   0        0        0     1877 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/question-mark-icon.svg
+-rw-r--r--   0        0        0     1319 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/stop-solid.svg
+-rw-r--r--   0        0        0      503 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/trash-solid.svg
+-rw-r--r--   0        0        0     2233 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/user-silhouette.svg
+-rw-r--r--   0        0        0      951 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/web.svg
+-rw-r--r--   0        0        0     2417 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/whatsapp.svg
+-rw-r--r--   0        0        0   591182 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/samples/desktop-browse-draw-sample.png
+-rw-r--r--   0        0        0   197173 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/samples/desktop-plain-chat-sample.png
+-rw-r--r--   0        0        0   268309 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/samples/desktop-remember-plan-sample.png
+-rw-r--r--   0        0        0   406179 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/samples/phone-browse-draw-sample.png
+-rw-r--r--   0        0        0    82985 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/samples/phone-plain-chat-sample.png
+-rw-r--r--   0        0        0   236285 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/samples/phone-remember-plan-sample.png
+-rw-r--r--   0        0        0        0 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/migrations/__init__.py
+-rw-r--r--   0        0        0     1928 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/migrations/migrate_offline_chat_default_model.py
+-rw-r--r--   0        0        0     2034 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/migrations/migrate_offline_chat_default_model_2.py
+-rw-r--r--   0        0        0     2510 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/migrations/migrate_offline_chat_schema.py
+-rw-r--r--   0        0        0      975 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/migrations/migrate_offline_model.py
+-rw-r--r--   0        0        0     2025 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/migrations/migrate_processor_config_openai.py
+-rw-r--r--   0        0        0     5132 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/migrations/migrate_server_pg.py
+-rw-r--r--   0        0        0      569 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/migrations/migrate_version.py
+-rw-r--r--   0        0        0        0 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/__init__.py
+-rw-r--r--   0        0        0     4715 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/embeddings.py
+-rw-r--r--   0        0        0        0 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/content/__init__.py
+-rw-r--r--   0        0        0    12604 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/content/text_to_entries.py
+-rw-r--r--   0        0        0        0 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/content/github/__init__.py
+-rw-r--r--   0        0        0    13721 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/content/github/github_to_entries.py
+-rw-r--r--   0        0        0        0 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/content/markdown/__init__.py
+-rw-r--r--   0        0        0     5690 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/content/markdown/markdown_to_entries.py
+-rw-r--r--   0        0        0     9871 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/content/notion/notion_to_entries.py
+-rw-r--r--   0        0        0        0 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/content/org_mode/__init__.py
+-rw-r--r--   0        0        0     6377 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/content/org_mode/org_to_entries.py
+-rw-r--r--   0        0        0    18246 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/content/org_mode/orgnode.py
+-rw-r--r--   0        0        0        0 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/content/pdf/__init__.py
+-rw-r--r--   0        0        0     4660 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/content/pdf/pdf_to_entries.py
+-rw-r--r--   0        0        0        0 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/content/plaintext/__init__.py
+-rw-r--r--   0        0        0     3717 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/content/plaintext/plaintext_to_entries.py
+-rw-r--r--   0        0        0        0 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/conversation/__init__.py
+-rw-r--r--   0        0        0    20895 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/conversation/prompts.py
+-rw-r--r--   0        0        0    10226 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/conversation/utils.py
+-rw-r--r--   0        0        0        0 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/conversation/offline/__init__.py
+-rw-r--r--   0        0        0     8615 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/conversation/offline/chat_model.py
+-rw-r--r--   0        0        0     1793 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/conversation/offline/utils.py
+-rw-r--r--   0        0        0      470 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/conversation/offline/whisper.py
+-rw-r--r--   0        0        0        0 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/conversation/openai/__init__.py
+-rw-r--r--   0        0        0     6854 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/conversation/openai/gpt.py
+-rw-r--r--   0        0        0     3284 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/conversation/openai/utils.py
+-rw-r--r--   0        0        0      432 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/conversation/openai/whisper.py
+-rw-r--r--   0        0        0        0 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/tools/__init__.py
+-rw-r--r--   0        0        0     5929 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/processor/tools/online_search.py
+-rw-r--r--   0        0        0        0 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/routers/__init__.py
+-rw-r--r--   0        0        0    14588 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/routers/api.py
+-rw-r--r--   0        0        0     1443 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/routers/api_agents.py
+-rw-r--r--   0        0        0    14988 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/routers/api_chat.py
+-rw-r--r--   0        0        0    10614 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/routers/api_config.py
+-rw-r--r--   0        0        0     2208 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/routers/api_phone.py
+-rw-r--r--   0        0        0     4569 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/routers/auth.py
+-rw-r--r--   0        0        0    28306 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/routers/helpers.py
+-rw-r--r--   0        0        0    12706 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/routers/indexer.py
+-rw-r--r--   0        0        0     1151 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/routers/storage.py
+-rw-r--r--   0        0        0     4285 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/routers/subscription.py
+-rw-r--r--   0        0        0     1081 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/routers/twilio.py
+-rw-r--r--   0        0        0    13166 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/routers/web_client.py
+-rw-r--r--   0        0        0        0 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/search_filter/__init__.py
+-rw-r--r--   0        0        0      358 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/search_filter/base_filter.py
+-rw-r--r--   0        0        0     6438 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/search_filter/date_filter.py
+-rw-r--r--   0        0        0      939 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/search_filter/file_filter.py
+-rw-r--r--   0        0        0     1005 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/search_filter/word_filter.py
+-rw-r--r--   0        0        0        0 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/search_type/__init__.py
+-rw-r--r--   0        0        0    11451 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/search_type/image_search.py
+-rw-r--r--   0        0        0     8916 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/search_type/text_search.py
+-rw-r--r--   0        0        0        0 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/utils/__init__.py
+-rw-r--r--   0        0        0     3466 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/utils/cli.py
+-rw-r--r--   0        0        0     1866 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/utils/config.py
+-rw-r--r--   0        0        0      791 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/utils/constants.py
+-rw-r--r--   0        0        0     9519 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/utils/fs_syncer.py
+-rw-r--r--   0        0        0    12034 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/utils/helpers.py
+-rw-r--r--   0        0        0     7245 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/utils/initialization.py
+-rw-r--r--   0        0        0     1192 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/utils/jsonl.py
+-rw-r--r--   0        0        0     2009 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/utils/models.py
+-rw-r--r--   0        0        0     4028 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/utils/rawconfig.py
+-rw-r--r--   0        0        0     1354 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/utils/state.py
+-rw-r--r--   0        0        0     1430 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/src/khoj/utils/yaml.py
+-rw-r--r--   0        0        0      565 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/.gitignore
+-rw-r--r--   0        0        0    34523 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/LICENSE
+-rw-r--r--   0        0        0     2007 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/README.md
+-rw-r--r--   0        0        0     3430 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/pyproject.toml
+-rw-r--r--   0        0        0     5227 2024-04-02 10:19:42.000000 khoj_assistant-1.8.1.dev11/PKG-INFO
```

### Comparing `khoj_assistant-1.8.0/src/khoj/configure.py` & `khoj_assistant-1.8.1.dev11/src/khoj/configure.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/main.py` & `khoj_assistant-1.8.1.dev11/src/khoj/main.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/manage.py` & `khoj_assistant-1.8.1.dev11/src/khoj/manage.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/app/README.md` & `khoj_assistant-1.8.1.dev11/src/khoj/app/README.md`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/app/settings.py` & `khoj_assistant-1.8.1.dev11/src/khoj/app/settings.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/app/urls.py` & `khoj_assistant-1.8.1.dev11/src/khoj/app/urls.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/database/admin.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/admin.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/database/adapters/__init__.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/adapters/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     UserSearchModelConfig,
 )
 from khoj.processor.conversation import prompts
 from khoj.search_filter.date_filter import DateFilter
 from khoj.search_filter.file_filter import FileFilter
 from khoj.search_filter.word_filter import WordFilter
 from khoj.utils import state
-from khoj.utils.config import GPT4AllProcessorModel
+from khoj.utils.config import OfflineChatProcessorModel
 from khoj.utils.helpers import generate_random_name, is_none_or_empty
 
 
 class SubscriptionState(Enum):
     TRIAL = "trial"
     SUBSCRIBED = "subscribed"
     UNSUBSCRIBED = "unsubscribed"
@@ -701,16 +701,16 @@
         else:
             conversation_config = ConversationAdapters.get_conversation_config(user)
 
         if conversation_config is None:
             conversation_config = ConversationAdapters.get_default_conversation_config()
 
         if offline_chat_config and offline_chat_config.enabled and conversation_config.model_type == "offline":
-            if state.gpt4all_processor_config is None or state.gpt4all_processor_config.loaded_model is None:
-                state.gpt4all_processor_config = GPT4AllProcessorModel(conversation_config.chat_model)
+            if state.offline_chat_processor_config is None or state.offline_chat_processor_config.loaded_model is None:
+                state.offline_chat_processor_config = OfflineChatProcessorModel(conversation_config.chat_model)
 
             return conversation_config
 
         openai_chat_config = ConversationAdapters.get_openai_conversation_config()
         if openai_chat_config and conversation_config.model_type == "openai":
             return conversation_config
```

### Comparing `khoj_assistant-1.8.0/src/khoj/database/migrations/0001_khojuser.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0001_khojuser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/database/migrations/0002_googleuser.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0002_googleuser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/database/migrations/0004_content_types_and_more.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0004_content_types_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/database/migrations/0006_embeddingsdates.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0006_embeddingsdates.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/database/migrations/0007_add_conversation.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0007_add_conversation.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/database/migrations/0009_khojapiuser.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0009_khojapiuser.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/database/migrations/0010_chatmodeloptions_and_more.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0010_chatmodeloptions_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/database/migrations/0010_rename_embeddings_entry_and_more.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0010_rename_embeddings_entry_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/database/migrations/0012_entry_file_source.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0012_entry_file_source.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/database/migrations/0013_subscription.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0013_subscription.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/database/migrations/0015_alter_subscription_user.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0015_alter_subscription_user.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/database/migrations/0017_searchmodel.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0017_searchmodel.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/database/migrations/0018_searchmodelconfig_delete_searchmodel.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0018_searchmodelconfig_delete_searchmodel.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/database/migrations/0019_alter_googleuser_family_name_and_more.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0019_alter_googleuser_family_name_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/database/migrations/0020_reflectivequestion.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0020_reflectivequestion.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/database/migrations/0021_speechtotextmodeloptions_and_more.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0021_speechtotextmodeloptions_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/database/migrations/0022_texttoimagemodelconfig.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0022_texttoimagemodelconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/database/migrations/0023_usersearchmodelconfig.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0023_usersearchmodelconfig.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/database/migrations/0025_clientapplication_khojuser_phone_number_and_more.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0025_clientapplication_khojuser_phone_number_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/database/migrations/0025_searchmodelconfig_embeddings_inference_endpoint_and_more.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0025_searchmodelconfig_embeddings_inference_endpoint_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/database/migrations/0026_searchmodelconfig_cross_encoder_inference_endpoint_and_more.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0026_searchmodelconfig_cross_encoder_inference_endpoint_and_more.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/database/migrations/0029_userrequests.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0029_userrequests.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/database/migrations/0030_conversation_slug_and_title.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0030_conversation_slug_and_title.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/database/migrations/0031_agent_conversation_agent.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0031_agent_conversation_agent.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/database/migrations/0031_alter_googleuser_locale.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/migrations/0031_alter_googleuser_locale.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/database/models/__init__.py` & `khoj_assistant-1.8.1.dev11/src/khoj/database/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 class ChatModelOptions(BaseModel):
     class ModelType(models.TextChoices):
         OPENAI = "openai"
         OFFLINE = "offline"
 
     max_prompt_size = models.IntegerField(default=None, null=True, blank=True)
     tokenizer = models.CharField(max_length=200, default=None, null=True, blank=True)
-    chat_model = models.CharField(max_length=200, default="mistral-7b-instruct-v0.1.Q4_0.gguf")
+    chat_model = models.CharField(max_length=200, default="NousResearch/Hermes-2-Pro-Mistral-7B-GGUF")
     model_type = models.CharField(max_length=200, choices=ModelType.choices, default=ModelType.OFFLINE)
 
 
 class Agent(BaseModel):
     creator = models.ForeignKey(
         KhojUser, on_delete=models.CASCADE, default=None, null=True, blank=True
     )  # Creator will only be null when the agents are managed by admin
```

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/404.html` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/404.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/agent.html` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/agent.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/agents.html` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/agents.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/base_config.html` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/base_config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/base_processor_integration.html` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/base_processor_integration.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/chat.html` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/chat.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/config.html` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/config.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/content_source_computer_input.html` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/content_source_computer_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/content_source_github_input.html` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/content_source_github_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/content_source_notion_input.html` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/content_source_notion_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/khoj.webmanifest` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/khoj.webmanifest`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/login.html` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/login.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/processor_conversation_input.html` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/processor_conversation_input.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/search.html` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/search.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/utils.html` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/utils.html`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/khoj.css` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/khoj.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/markdown-it.min.js` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/markdown-it.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/org.min.js` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/org.min.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/pico.min.css` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/pico.min.css`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/utils.js` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/utils.js`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/chat.svg` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/chat.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/computer.png` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/computer.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/confirm-icon.svg` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/confirm-icon.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/copy_button.svg` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/copy_button.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/credit-card.png` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/credit-card.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/favicon-128x128.ico` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/favicon-128x128.ico`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/favicon-128x128.png` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/favicon-256x256.png` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/favicon-256x256.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/favicon.icns` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/favicon.icns`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/github.svg` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/github.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/key.svg` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/key.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/khoj-logo-sideways-200.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/khoj-logo-sideways-500.png` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/khoj-logo-sideways-500.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/khoj-logo-sideways.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/logotype.svg` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/logotype.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/microphone-solid.svg` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/microphone-solid.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/notion.svg` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/notion.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/openai-logomark.svg` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/openai-logomark.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/org.svg` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/org.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/pdf.svg` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/pdf.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/plaintext.svg` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/plaintext.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/question-mark-icon.svg` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/question-mark-icon.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/stop-solid.svg` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/stop-solid.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/user-silhouette.svg` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/user-silhouette.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/web.svg` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/web.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/icons/whatsapp.svg` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/icons/whatsapp.svg`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/samples/desktop-browse-draw-sample.png` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/samples/desktop-browse-draw-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/samples/desktop-plain-chat-sample.png` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/samples/desktop-plain-chat-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/samples/desktop-remember-plan-sample.png` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/samples/desktop-remember-plan-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/samples/phone-browse-draw-sample.png` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/samples/phone-browse-draw-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/samples/phone-plain-chat-sample.png` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/samples/phone-plain-chat-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/interface/web/assets/samples/phone-remember-plan-sample.png` & `khoj_assistant-1.8.1.dev11/src/khoj/interface/web/assets/samples/phone-remember-plan-sample.png`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/migrations/migrate_offline_chat_default_model.py` & `khoj_assistant-1.8.1.dev11/src/khoj/migrations/migrate_offline_chat_default_model.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/migrations/migrate_offline_chat_schema.py` & `khoj_assistant-1.8.1.dev11/src/khoj/migrations/migrate_offline_chat_schema.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/migrations/migrate_offline_model.py` & `khoj_assistant-1.8.1.dev11/src/khoj/migrations/migrate_offline_model.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/migrations/migrate_processor_config_openai.py` & `khoj_assistant-1.8.1.dev11/src/khoj/migrations/migrate_processor_config_openai.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/migrations/migrate_server_pg.py` & `khoj_assistant-1.8.1.dev11/src/khoj/migrations/migrate_server_pg.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/migrations/migrate_version.py` & `khoj_assistant-1.8.1.dev11/src/khoj/migrations/migrate_version.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/processor/embeddings.py` & `khoj_assistant-1.8.1.dev11/src/khoj/processor/embeddings.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/processor/content/text_to_entries.py` & `khoj_assistant-1.8.1.dev11/src/khoj/processor/content/text_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/processor/content/github/github_to_entries.py` & `khoj_assistant-1.8.1.dev11/src/khoj/processor/content/github/github_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/processor/content/markdown/markdown_to_entries.py` & `khoj_assistant-1.8.1.dev11/src/khoj/processor/content/markdown/markdown_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/processor/content/notion/notion_to_entries.py` & `khoj_assistant-1.8.1.dev11/src/khoj/processor/content/notion/notion_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/processor/content/org_mode/org_to_entries.py` & `khoj_assistant-1.8.1.dev11/src/khoj/processor/content/org_mode/org_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/processor/content/org_mode/orgnode.py` & `khoj_assistant-1.8.1.dev11/src/khoj/processor/content/org_mode/orgnode.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/processor/content/pdf/pdf_to_entries.py` & `khoj_assistant-1.8.1.dev11/src/khoj/processor/content/pdf/pdf_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/processor/content/plaintext/plaintext_to_entries.py` & `khoj_assistant-1.8.1.dev11/src/khoj/processor/content/plaintext/plaintext_to_entries.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/processor/conversation/prompts.py` & `khoj_assistant-1.8.1.dev11/src/khoj/processor/conversation/prompts.py`

 * *Files 15% similar despite different names*

```diff
@@ -61,89 +61,55 @@
 
 no_entries_found = PromptTemplate.from_template(
     """
     It looks like you haven't added any notes yet. No worries, you can fix that by downloading the Khoj app from <a href=https://khoj.dev/downloads>here</a>.
 """.strip()
 )
 
-## Conversation Prompts for GPT4All Models
+## Conversation Prompts for Offline Chat Models
 ## --
-system_prompt_message_gpt4all = PromptTemplate.from_template(
+system_prompt_offline_chat = PromptTemplate.from_template(
     """
 You are Khoj, a smart, inquisitive and helpful personal assistant.
 - Use your general knowledge and past conversation with the user as context to inform your responses.
 - If you do not know the answer, say 'I don't know.'
 - Think step-by-step and ask questions to get the necessary information to answer the user's question.
 - Do not print verbatim Notes unless necessary.
 
 Today is {current_date} in UTC.
     """.strip()
 )
 
-custom_system_prompt_message_gpt4all = PromptTemplate.from_template(
+custom_system_prompt_offline_chat = PromptTemplate.from_template(
     """
 You are {name}, a personal agent on Khoj.
 - Use your general knowledge and past conversation with the user as context to inform your responses.
 - If you do not know the answer, say 'I don't know.'
 - Think step-by-step and ask questions to get the necessary information to answer the user's question.
 - Do not print verbatim Notes unless necessary.
 
 Today is {current_date} in UTC.
 
 Instructions:\n{bio}
     """.strip()
 )
 
-system_prompt_message_extract_questions_gpt4all = f"""You are Khoj, a kind and intelligent personal assistant. When the user asks you a question, you ask follow-up questions to clarify the necessary information you need in order to answer from the user's perspective.
-- Write the question as if you can search for the answer on the user's personal notes.
-- Try to be as specific as possible. Instead of saying "they" or "it" or "he", use the name of the person or thing you are referring to. For example, instead of saying "Which store did they go to?", say "Which store did Alice and Bob go to?".
-- Add as much context from the previous questions and notes as required into your search queries.
-- Provide search queries as a list of questions
-What follow-up questions, if any, will you need to ask to answer the user's question?
-"""
-
-system_prompt_gpt4all = PromptTemplate.from_template(
-    """
-<s>[INST] <<SYS>>
-{message}
-<</SYS>>Hi there! [/INST] Hello! How can I help you today? </s>"""
-)
-
-system_prompt_extract_questions_gpt4all = PromptTemplate.from_template(
-    """
-<s>[INST] <<SYS>>
-{message}
-<</SYS>>[/INST]</s>"""
-)
-
-user_message_gpt4all = PromptTemplate.from_template(
-    """
-<s>[INST] {message} [/INST]
-""".strip()
-)
-
-khoj_message_gpt4all = PromptTemplate.from_template(
-    """
-{message}</s>
-""".strip()
-)
-
 ## Notes Conversation
 ## --
 notes_conversation = PromptTemplate.from_template(
     """
 Use my personal notes and our past conversations to inform your response.
 Ask crisp follow-up questions to get additional context, when a helpful response cannot be provided from the provided notes or past conversations.
 
 Notes:
 {references}
 """.strip()
 )
 
-notes_conversation_gpt4all = PromptTemplate.from_template(
+notes_conversation_offline = PromptTemplate.from_template(
     """
 User's Notes:
 {references}
 """.strip()
 )
 
 ## Image Generation
@@ -187,66 +153,58 @@
 ## --
 query_prompt = PromptTemplate.from_template(
     """
 Query: {query}""".strip()
 )
 
 
-## Summarize Notes
+## Extract Questions
 ## --
-summarize_notes = PromptTemplate.from_template(
+extract_questions_offline = PromptTemplate.from_template(
     """
-Summarize the below notes about {user_query}:
+You are Khoj, an extremely smart and helpful search assistant with the ability to retrieve information from the user's notes. Construct search queries to retrieve relevant information to answer the user's question.
+- You will be provided past questions(Q) and answers(A) for context.
+- Try to be as specific as possible. Instead of saying "they" or "it" or "he", use proper nouns like name of the person or thing you are referring to.
+- Add as much context from the previous questions and answers as required into your search queries.
+- Break messages into multiple search queries when required to retrieve the relevant information.
+- Add date filters to your search queries from questions and answers when required to retrieve the relevant information.
 
-{text}
+Current Date: {current_date}
+User's Location: {location}
 
-Summarize the notes in second person perspective:"""
-)
+Examples:
+Q: How was my trip to Cambodia?
+Khoj: ["How was my trip to Cambodia?"]
 
+Q: Who did I visit the temple with on that trip?
+Khoj: ["Who did I visit the temple with in Cambodia?"]
 
-## Answer
-## --
-answer = PromptTemplate.from_template(
-    """
-You are a friendly, helpful personal assistant.
-Using the users notes below, answer their following question. If the answer is not contained within the notes, say "I don't know."
+Q: Which of them is older?
+Khoj: ["When was Alice born?", "What is Bob's age?"]
 
-Notes:
-{text}
+Q: Where did John say he was? He mentioned it in our call last week.
+Khoj: ["Where is John? dt>='{last_year}-12-25' dt<'{last_year}-12-26'", "John's location in call notes"]
 
-Question: {user_query}
+Q: How can you help me?
+Khoj: ["Social relationships", "Physical and mental health", "Education and career", "Personal life goals and habits"]
 
-Answer (in second person):"""
-)
+Q: What did I do for Christmas last year?
+Khoj: ["What did I do for Christmas {last_year} dt>='{last_year}-12-25' dt<'{last_year}-12-26'"]
 
+Q: How should I take care of my plants?
+Khoj: ["What kind of plants do I have?", "What issues do my plants have?"]
 
-## Extract Questions
-## --
-extract_questions_gpt4all_sample = PromptTemplate.from_template(
-    """
-<s>[INST] <<SYS>>Current Date: {current_date}. User's Location: {location}<</SYS>> [/INST]</s>
-<s>[INST] How was my trip to Cambodia? [/INST]
-How was my trip to Cambodia?</s>
-<s>[INST] Who did I visit the temple with on that trip? [/INST]
-Who did I visit the temple with in Cambodia?</s>
-<s>[INST] How should I take care of my plants? [/INST]
-What kind of plants do I have? What issues do my plants have?</s>
-<s>[INST] How many tennis balls fit in the back of a 2002 Honda Civic? [/INST]
-What is the size of a tennis ball? What is the trunk size of a 2002 Honda Civic?</s>
-<s>[INST] What did I do for Christmas last year? [/INST]
-What did I do for Christmas {last_year} dt>='{last_christmas_date}' dt<'{next_christmas_date}'</s>
-<s>[INST] How are you feeling today? [/INST]</s>
-<s>[INST] Is Alice older than Bob? [/INST]
-When was Alice born? What is Bob's age?</s>
-<s>[INST] <<SYS>>
-Use these notes from the user's previous conversations to provide a response:
+Q: Who all did I meet here yesterday?
+Khoj: ["Met in {location} on {yesterday_date} dt>='{yesterday_date}' dt<'{current_date}'"]
+
+Chat History:
 {chat_history}
-<</SYS>> [/INST]</s>
-<s>[INST] {query} [/INST]
-"""
+What searches will you perform to answer the following question, using the chat history as reference? Respond with relevant search queries as list of strings.
+Q: {query}
+""".strip()
 )
 
 
 extract_questions = PromptTemplate.from_template(
     """
 You are Khoj, an extremely smart and helpful search assistant with the ability to retrieve information from the user's notes. Construct search queries to retrieve relevant information to answer the user's question.
 - You will be provided past questions(Q) and answers(A) for context.
@@ -256,15 +214,15 @@
 
 What searches will you perform to answer the users question? Respond with search queries as list of strings in a JSON object.
 Current Date: {day_of_week}, {current_date}
 User's Location: {location}
 
 Q: How was my trip to Cambodia?
 Khoj: {{"queries": ["How was my trip to Cambodia?"]}}
-A: The trip was amazing. I went to the Angkor Wat temple and it was beautiful.
+A: The trip was amazing. You went to the Angkor Wat temple and it was beautiful.
 
 Q: Who did i visit that temple with?
 Khoj: {{"queries": ["Who did I visit the Angkor Wat Temple in Cambodia with?"]}}
 A: You visited the Angkor Wat Temple in Cambodia with Pablo, Namita and Xi.
 
 Q: What national parks did I go to last year?
 Khoj: {{"queries": ["National park I visited in {last_new_year} dt>='{last_new_year_date}' dt<'{current_new_year_date}'"]}}
@@ -282,16 +240,16 @@
 Khoj: {{"queries": ["When was Bob born?", "What is Tom's age?"]}}
 A: Yes, Bob is older than Tom. As Bob was born on 1984-01-01 and Tom is 30 years old.
 
 Q: What is their age difference?
 Khoj: {{"queries": ["What is Bob's age?", "What is Tom's age?"]}}
 A: Bob is {bob_tom_age_difference} years older than Tom. As Bob is {bob_age} years old and Tom is 30 years old.
 
-Q: What does yesterday's note say?
-Khoj: {{"queries": ["Note from {yesterday_date} dt>='{yesterday_date}' dt<'{current_date}'"]}}
+Q: Who all did I meet here yesterday?
+Khoj: {{"queries": ["Met in {location} on {yesterday_date} dt>='{yesterday_date}' dt<'{current_date}'"]}}
 A: Yesterday's note mentions your visit to your local beach with Ram and Shyam.
 
 {chat_history}
 Q: {text}
 Khoj:
 """.strip()
 )
@@ -539,15 +497,14 @@
 - **/notes**: Chat using the information in your knowledge base.
 - **/general**: Chat using just Khoj's general knowledge. This will not search against your notes.
 - **/default**: Chat using your knowledge base and Khoj's general knowledge for context.
 - **/online**: Chat using the internet as a source of information.
 - **/image**: Generate an image based on your message.
 - **/help**: Show this help message.
 
-
 You are using the **{model}** model on the **{device}**.
 **version**: {version}
 """.strip()
 )
 
 # Personalization to the user
 # --
```

#### html2text {}

```diff
@@ -33,182 +33,173 @@
 ( """ {query} """.strip() ) no_notes_found = PromptTemplate.from_template( """
 I'm sorry, I couldn't find any relevant notes to respond to your message.
 """.strip() ) no_online_results_found = PromptTemplate.from_template( """ I'm
 sorry, I couldn't find any relevant information from the internet to respond to
 your message. """.strip() ) no_entries_found = PromptTemplate.from_template
 ( """ It looks like you haven't added any notes yet. No worries, you can fix
 that by downloading the Khoj app from _h_e_r_e. """.strip() ) ## Conversation
-Prompts for GPT4All Models ## -- system_prompt_message_gpt4all =
+Prompts for Offline Chat Models ## -- system_prompt_offline_chat =
 PromptTemplate.from_template( """ You are Khoj, a smart, inquisitive and
 helpful personal assistant. - Use your general knowledge and past conversation
 with the user as context to inform your responses. - If you do not know the
 answer, say 'I don't know.' - Think step-by-step and ask questions to get the
 necessary information to answer the user's question. - Do not print verbatim
 Notes unless necessary. Today is {current_date} in UTC. """.strip() )
-custom_system_prompt_message_gpt4all = PromptTemplate.from_template( """ You
-are {name}, a personal agent on Khoj. - Use your general knowledge and past
+custom_system_prompt_offline_chat = PromptTemplate.from_template( """ You are
+{name}, a personal agent on Khoj. - Use your general knowledge and past
 conversation with the user as context to inform your responses. - If you do not
 know the answer, say 'I don't know.' - Think step-by-step and ask questions to
 get the necessary information to answer the user's question. - Do not print
 verbatim Notes unless necessary. Today is {current_date} in UTC. Instructions:
-\n{bio} """.strip() ) system_prompt_message_extract_questions_gpt4all = f"""You
-are Khoj, a kind and intelligent personal assistant. When the user asks you a
-question, you ask follow-up questions to clarify the necessary information you
-need in order to answer from the user's perspective. - Write the question as if
-you can search for the answer on the user's personal notes. - Try to be as
-specific as possible. Instead of saying "they" or "it" or "he", use the name of
-the person or thing you are referring to. For example, instead of saying "Which
-store did they go to?", say "Which store did Alice and Bob go to?". - Add as
-much context from the previous questions and notes as required into your search
-queries. - Provide search queries as a list of questions What follow-up
-questions, if any, will you need to ask to answer the user's question? """
-system_prompt_gpt4all = PromptTemplate.from_template( """ [INST] <> {message}
-<>Hi there! [/INST] Hello! How can I help you today? """ )
-system_prompt_extract_questions_gpt4all = PromptTemplate.from_template( """
-[INST] <> {message} <>[/INST]""" ) user_message_gpt4all =
-PromptTemplate.from_template( """ [INST] {message} [/INST] """.strip() )
-khoj_message_gpt4all = PromptTemplate.from_template( """ {message} """.strip()
-) ## Notes Conversation ## -- notes_conversation = PromptTemplate.from_template
-( """ Use my personal notes and our past conversations to inform your response.
-Ask crisp follow-up questions to get additional context, when a helpful
-response cannot be provided from the provided notes or past conversations.
-Notes: {references} """.strip() ) notes_conversation_gpt4all =
-PromptTemplate.from_template( """ User's Notes: {references} """.strip() ) ##
-Image Generation ## -- image_generation_improve_prompt =
-PromptTemplate.from_template( """ You are a talented creator. Generate a
-detailed prompt to generate an image based on the following description. Update
-the query below to improve the image generation. Add additional context to the
-query to improve the image generation. Make sure to retain any important
-information originally from the query. You are provided with the following
-information to help you generate the prompt: Today's Date: {current_date}
-User's Location: {location} User's Notes: {references} Online References:
-{online_results} Conversation Log: {chat_history} Query: {query} Remember, now
-you are generating a prompt to improve the image generation. Add additional
-context to the query to improve the image generation. Make sure to retain any
-important information originally from the query. Use the additional context
-from the user's notes, online references and conversation log to improve the
-image generation. Improved Query:""" ) ## Online Search Conversation ## -
-- online_search_conversation = PromptTemplate.from_template( """ Use this up-
-to-date information from the internet to inform your response. Ask crisp
-follow-up questions to get additional context, when a helpful response cannot
-be provided from the online data or past conversations. Information from the
-internet: {online_results} """.strip() ) ## Query prompt ## -- query_prompt =
-PromptTemplate.from_template( """ Query: {query}""".strip() ) ## Summarize
-Notes ## -- summarize_notes = PromptTemplate.from_template( """ Summarize the
-below notes about {user_query}: {text} Summarize the notes in second person
-perspective:""" ) ## Answer ## -- answer = PromptTemplate.from_template( """
-You are a friendly, helpful personal assistant. Using the users notes below,
-answer their following question. If the answer is not contained within the
-notes, say "I don't know." Notes: {text} Question: {user_query} Answer (in
-second person):""" ) ## Extract Questions ## -
-- extract_questions_gpt4all_sample = PromptTemplate.from_template( """ [INST]
-<>Current Date: {current_date}. User's Location: {location}<> [/INST] [INST]
-How was my trip to Cambodia? [/INST] How was my trip to Cambodia? [INST] Who
-did I visit the temple with on that trip? [/INST] Who did I visit the temple
-with in Cambodia? [INST] How should I take care of my plants? [/INST] What kind
-of plants do I have? What issues do my plants have? [INST] How many tennis
-balls fit in the back of a 2002 Honda Civic? [/INST] What is the size of a
-tennis ball? What is the trunk size of a 2002 Honda Civic? [INST] What did I do
-for Christmas last year? [/INST] What did I do for Christmas {last_year} dt>='
-{last_christmas_date}' dt<'{next_christmas_date}' [INST] How are you feeling
-today? [/INST] [INST] Is Alice older than Bob? [/INST] When was Alice born?
-What is Bob's age? [INST] <> Use these notes from the user's previous
-conversations to provide a response: {chat_history} <> [/INST] [INST] {query}
-[/INST] """ ) extract_questions = PromptTemplate.from_template( """ You are
-Khoj, an extremely smart and helpful search assistant with the ability to
-retrieve information from the user's notes. Construct search queries to
-retrieve relevant information to answer the user's question. - You will be
-provided past questions(Q) and answers(A) for context. - Add as much context
-from the previous questions and answers as required into your search queries. -
-Break messages into multiple search queries when required to retrieve the
-relevant information. - Add date filters to your search queries from questions
-and answers when required to retrieve the relevant information. What searches
-will you perform to answer the users question? Respond with search queries as
-list of strings in a JSON object. Current Date: {day_of_week}, {current_date}
-User's Location: {location} Q: How was my trip to Cambodia? Khoj: {{"queries":
-["How was my trip to Cambodia?"]}} A: The trip was amazing. I went to the
-Angkor Wat temple and it was beautiful. Q: Who did i visit that temple with?
-Khoj: {{"queries": ["Who did I visit the Angkor Wat Temple in Cambodia
-with?"]}} A: You visited the Angkor Wat Temple in Cambodia with Pablo, Namita
-and Xi. Q: What national parks did I go to last year? Khoj: {{"queries":
-["National park I visited in {last_new_year} dt>='{last_new_year_date}' dt<'
-{current_new_year_date}'"]}} A: You visited the Grand Canyon and Yellowstone
-National Park in {last_new_year}. Q: How can you help me? Khoj: {{"queries":
-["Social relationships", "Physical and mental health", "Education and career",
-"Personal life goals and habits"]}} A: I can help you live healthier and
-happier across work and personal life Q: How many tennis balls fit in the back
-of a 2002 Honda Civic? Khoj: {{"queries": ["What is the size of a tennis
-ball?", "What is the trunk size of a 2002 Honda Civic?"]}} A: 1085 tennis balls
-will fit in the trunk of a Honda Civic Q: Is Bob older than Tom? Khoj: {
-{"queries": ["When was Bob born?", "What is Tom's age?"]}} A: Yes, Bob is older
-than Tom. As Bob was born on 1984-01-01 and Tom is 30 years old. Q: What is
-their age difference? Khoj: {{"queries": ["What is Bob's age?", "What is Tom's
-age?"]}} A: Bob is {bob_tom_age_difference} years older than Tom. As Bob is
-{bob_age} years old and Tom is 30 years old. Q: What does yesterday's note say?
-Khoj: {{"queries": ["Note from {yesterday_date} dt>='{yesterday_date}' dt<'
-{current_date}'"]}} A: Yesterday's note mentions your visit to your local beach
-with Ram and Shyam. {chat_history} Q: {text} Khoj: """.strip() )
-system_prompt_extract_relevant_information = """As a professional analyst,
-create a comprehensive report of the most relevant information from a web page
-in response to a user's query. The text provided is directly from within the
-web page. The report you create should be multiple paragraphs, and it should
-represent the content of the website. Tell the user exactly what the website
-says in response to their query, while adhering to these guidelines: 1. Answer
-the user's query as specifically as possible. Include many supporting details
-from the website. 2. Craft a report that is detailed, thorough, in-depth, and
-complex, while maintaining clarity. 3. Rely strictly on the provided text,
-without including external information. 4. Format the report in multiple
-paragraphs with a clear structure. 5. Be as specific as possible in your answer
-to the user's query. 6. Reproduce as much of the provided text as possible,
-while maintaining readability. """.strip() extract_relevant_information =
-PromptTemplate.from_template( """ Target Query: {query} Web Pages: {corpus}
-Collate only relevant information from the website to answer the target query.
-""".strip() ) pick_relevant_output_mode = PromptTemplate.from_template( """ You
-are Khoj, an excellent analyst for selecting the correct way to respond to a
-user's query. You have access to a limited set of modes for your response. You
-can only use one of these modes. {modes} Here are some example responses:
-Example: Chat History: User: I just visited Jerusalem for the first time. Pull
-up my notes from the trip. AI: You mention visiting Masjid Al-Aqsa and the
-Western Wall. You also mention trying the local cuisine and visiting the Dead
-Sea. Q: Draw a picture of my trip to Jerusalem. Khoj: image Example: Chat
-History: User: I'm having trouble deciding which laptop to get. I want
-something with at least 16 GB of RAM and a 1 TB SSD. AI: I can help with that.
-I see online that there is a new model of the Dell XPS 15 that meets your
-requirements. Q: What are the specs of the new Dell XPS 15? Khoj: default Now
-it's your turn to pick the mode you would like to use to answer the user's
-question. Provide your response as a string. Chat History: {chat_history} Q:
-{query} Khoj: """.strip() ) pick_relevant_information_collection_tools =
+\n{bio} """.strip() ) ## Notes Conversation ## -- notes_conversation =
+PromptTemplate.from_template( """ Use my personal notes and our past
+conversations to inform your response. Ask crisp follow-up questions to get
+additional context, when a helpful response cannot be provided from the
+provided notes or past conversations. Notes: {references} """.strip() )
+notes_conversation_offline = PromptTemplate.from_template( """ User's Notes:
+{references} """.strip() ) ## Image Generation ## -
+- image_generation_improve_prompt = PromptTemplate.from_template( """ You are a
+talented creator. Generate a detailed prompt to generate an image based on the
+following description. Update the query below to improve the image generation.
+Add additional context to the query to improve the image generation. Make sure
+to retain any important information originally from the query. You are provided
+with the following information to help you generate the prompt: Today's Date:
+{current_date} User's Location: {location} User's Notes: {references} Online
+References: {online_results} Conversation Log: {chat_history} Query: {query}
+Remember, now you are generating a prompt to improve the image generation. Add
+additional context to the query to improve the image generation. Make sure to
+retain any important information originally from the query. Use the additional
+context from the user's notes, online references and conversation log to
+improve the image generation. Improved Query:""" ) ## Online Search
+Conversation ## -- online_search_conversation = PromptTemplate.from_template
+( """ Use this up-to-date information from the internet to inform your
+response. Ask crisp follow-up questions to get additional context, when a
+helpful response cannot be provided from the online data or past conversations.
+Information from the internet: {online_results} """.strip() ) ## Query prompt
+## -- query_prompt = PromptTemplate.from_template( """ Query: {query}""".strip
+() ) ## Extract Questions ## -- extract_questions_offline =
 PromptTemplate.from_template( """ You are Khoj, an extremely smart and helpful
-search assistant. - You have access to a variety of data sources to help you
-answer the user's question - You can use the data sources listed below to
-collect more relevant information - You can use any combination of these data
-sources to answer the user's question Which of the data sources listed below
-you would use to answer the user's question? {tools} Here are some example
-responses: Example: Chat History: User: I'm thinking of moving to a new city.
-I'm trying to decide between New York and San Francisco. AI: Moving to a new
-city can be challenging. Both New York and San Francisco are great cities to
-live in. New York is known for its diverse culture and San Francisco is known
-for its tech scene. Q: What is the population of each of those cities? Khoj: {
-{"source": ["online"]}} Example: Chat History: User: I'm thinking of my next
-vacation idea. Ideally, I want to see something new and exciting. AI:
-Excellent! Taking a vacation is a great way to relax and recharge. Q: Where did
-Grandma grow up? Khoj: {{"source": ["notes"]}} Example: Chat History: Q: What
-can you do for me? Khoj: {{"source": ["notes", "online"]}} Example: Chat
-History: User: Good morning AI: Good morning! How can I help you today? Q: How
-can I share my files with Khoj? Khoj: {{"source": ["default", "online"]}}
-Example: Chat History: User: What is the first element in the periodic table?
-AI: The first element in the periodic table is Hydrogen. Q: Summarize this
-article https://en.wikipedia.org/wiki/Hydrogen Khoj: {{"source": ["webpage"]}}
-Example: Chat History: User: I want to start a new hobby. I'm thinking of
-learning to play the guitar. AI: Learning to play the guitar is a great hobby.
-It can be a lot of fun and a great way to express yourself. Q: What is the
-first element of the periodic table? Khoj: {{"source": ["general"]}} Now it's
-your turn to pick the data sources you would like to use to answer the user's
-question. Respond with data sources as a list of strings in a JSON object. Chat
-History: {chat_history} Q: {query} Khoj: """.strip() ) infer_webpages_to_read =
+search assistant with the ability to retrieve information from the user's
+notes. Construct search queries to retrieve relevant information to answer the
+user's question. - You will be provided past questions(Q) and answers(A) for
+context. - Try to be as specific as possible. Instead of saying "they" or "it"
+or "he", use proper nouns like name of the person or thing you are referring
+to. - Add as much context from the previous questions and answers as required
+into your search queries. - Break messages into multiple search queries when
+required to retrieve the relevant information. - Add date filters to your
+search queries from questions and answers when required to retrieve the
+relevant information. Current Date: {current_date} User's Location: {location}
+Examples: Q: How was my trip to Cambodia? Khoj: ["How was my trip to
+Cambodia?"] Q: Who did I visit the temple with on that trip? Khoj: ["Who did I
+visit the temple with in Cambodia?"] Q: Which of them is older? Khoj: ["When
+was Alice born?", "What is Bob's age?"] Q: Where did John say he was? He
+mentioned it in our call last week. Khoj: ["Where is John? dt>='{last_year}-12-
+25' dt<'{last_year}-12-26'", "John's location in call notes"] Q: How can you
+help me? Khoj: ["Social relationships", "Physical and mental health",
+"Education and career", "Personal life goals and habits"] Q: What did I do for
+Christmas last year? Khoj: ["What did I do for Christmas {last_year} dt>='
+{last_year}-12-25' dt<'{last_year}-12-26'"] Q: How should I take care of my
+plants? Khoj: ["What kind of plants do I have?", "What issues do my plants
+have?"] Q: Who all did I meet here yesterday? Khoj: ["Met in {location} on
+{yesterday_date} dt>='{yesterday_date}' dt<'{current_date}'"] Chat History:
+{chat_history} What searches will you perform to answer the following question,
+using the chat history as reference? Respond with relevant search queries as
+list of strings. Q: {query} """.strip() ) extract_questions =
+PromptTemplate.from_template( """ You are Khoj, an extremely smart and helpful
+search assistant with the ability to retrieve information from the user's
+notes. Construct search queries to retrieve relevant information to answer the
+user's question. - You will be provided past questions(Q) and answers(A) for
+context. - Add as much context from the previous questions and answers as
+required into your search queries. - Break messages into multiple search
+queries when required to retrieve the relevant information. - Add date filters
+to your search queries from questions and answers when required to retrieve the
+relevant information. What searches will you perform to answer the users
+question? Respond with search queries as list of strings in a JSON object.
+Current Date: {day_of_week}, {current_date} User's Location: {location} Q: How
+was my trip to Cambodia? Khoj: {{"queries": ["How was my trip to Cambodia?"]}}
+A: The trip was amazing. You went to the Angkor Wat temple and it was
+beautiful. Q: Who did i visit that temple with? Khoj: {{"queries": ["Who did I
+visit the Angkor Wat Temple in Cambodia with?"]}} A: You visited the Angkor Wat
+Temple in Cambodia with Pablo, Namita and Xi. Q: What national parks did I go
+to last year? Khoj: {{"queries": ["National park I visited in {last_new_year}
+dt>='{last_new_year_date}' dt<'{current_new_year_date}'"]}} A: You visited the
+Grand Canyon and Yellowstone National Park in {last_new_year}. Q: How can you
+help me? Khoj: {{"queries": ["Social relationships", "Physical and mental
+health", "Education and career", "Personal life goals and habits"]}} A: I can
+help you live healthier and happier across work and personal life Q: How many
+tennis balls fit in the back of a 2002 Honda Civic? Khoj: {{"queries": ["What
+is the size of a tennis ball?", "What is the trunk size of a 2002 Honda
+Civic?"]}} A: 1085 tennis balls will fit in the trunk of a Honda Civic Q: Is
+Bob older than Tom? Khoj: {{"queries": ["When was Bob born?", "What is Tom's
+age?"]}} A: Yes, Bob is older than Tom. As Bob was born on 1984-01-01 and Tom
+is 30 years old. Q: What is their age difference? Khoj: {{"queries": ["What is
+Bob's age?", "What is Tom's age?"]}} A: Bob is {bob_tom_age_difference} years
+older than Tom. As Bob is {bob_age} years old and Tom is 30 years old. Q: Who
+all did I meet here yesterday? Khoj: {{"queries": ["Met in {location} on
+{yesterday_date} dt>='{yesterday_date}' dt<'{current_date}'"]}} A: Yesterday's
+note mentions your visit to your local beach with Ram and Shyam. {chat_history}
+Q: {text} Khoj: """.strip() ) system_prompt_extract_relevant_information =
+"""As a professional analyst, create a comprehensive report of the most
+relevant information from a web page in response to a user's query. The text
+provided is directly from within the web page. The report you create should be
+multiple paragraphs, and it should represent the content of the website. Tell
+the user exactly what the website says in response to their query, while
+adhering to these guidelines: 1. Answer the user's query as specifically as
+possible. Include many supporting details from the website. 2. Craft a report
+that is detailed, thorough, in-depth, and complex, while maintaining clarity.
+3. Rely strictly on the provided text, without including external information.
+4. Format the report in multiple paragraphs with a clear structure. 5. Be as
+specific as possible in your answer to the user's query. 6. Reproduce as much
+of the provided text as possible, while maintaining readability. """.strip()
+extract_relevant_information = PromptTemplate.from_template( """ Target Query:
+{query} Web Pages: {corpus} Collate only relevant information from the website
+to answer the target query. """.strip() ) pick_relevant_output_mode =
+PromptTemplate.from_template( """ You are Khoj, an excellent analyst for
+selecting the correct way to respond to a user's query. You have access to a
+limited set of modes for your response. You can only use one of these modes.
+{modes} Here are some example responses: Example: Chat History: User: I just
+visited Jerusalem for the first time. Pull up my notes from the trip. AI: You
+mention visiting Masjid Al-Aqsa and the Western Wall. You also mention trying
+the local cuisine and visiting the Dead Sea. Q: Draw a picture of my trip to
+Jerusalem. Khoj: image Example: Chat History: User: I'm having trouble deciding
+which laptop to get. I want something with at least 16 GB of RAM and a 1 TB
+SSD. AI: I can help with that. I see online that there is a new model of the
+Dell XPS 15 that meets your requirements. Q: What are the specs of the new Dell
+XPS 15? Khoj: default Now it's your turn to pick the mode you would like to use
+to answer the user's question. Provide your response as a string. Chat History:
+{chat_history} Q: {query} Khoj: """.strip() )
+pick_relevant_information_collection_tools = PromptTemplate.from_template( """
+You are Khoj, an extremely smart and helpful search assistant. - You have
+access to a variety of data sources to help you answer the user's question -
+You can use the data sources listed below to collect more relevant information
+- You can use any combination of these data sources to answer the user's
+question Which of the data sources listed below you would use to answer the
+user's question? {tools} Here are some example responses: Example: Chat
+History: User: I'm thinking of moving to a new city. I'm trying to decide
+between New York and San Francisco. AI: Moving to a new city can be
+challenging. Both New York and San Francisco are great cities to live in. New
+York is known for its diverse culture and San Francisco is known for its tech
+scene. Q: What is the population of each of those cities? Khoj: {{"source":
+["online"]}} Example: Chat History: User: I'm thinking of my next vacation
+idea. Ideally, I want to see something new and exciting. AI: Excellent! Taking
+a vacation is a great way to relax and recharge. Q: Where did Grandma grow up?
+Khoj: {{"source": ["notes"]}} Example: Chat History: Q: What can you do for me?
+Khoj: {{"source": ["notes", "online"]}} Example: Chat History: User: Good
+morning AI: Good morning! How can I help you today? Q: How can I share my files
+with Khoj? Khoj: {{"source": ["default", "online"]}} Example: Chat History:
+User: What is the first element in the periodic table? AI: The first element in
+the periodic table is Hydrogen. Q: Summarize this article https://
+en.wikipedia.org/wiki/Hydrogen Khoj: {{"source": ["webpage"]}} Example: Chat
+History: User: I want to start a new hobby. I'm thinking of learning to play
+the guitar. AI: Learning to play the guitar is a great hobby. It can be a lot
+of fun and a great way to express yourself. Q: What is the first element of the
+periodic table? Khoj: {{"source": ["general"]}} Now it's your turn to pick the
+data sources you would like to use to answer the user's question. Respond with
+data sources as a list of strings in a JSON object. Chat History:
+{chat_history} Q: {query} Khoj: """.strip() ) infer_webpages_to_read =
 PromptTemplate.from_template( """ You are Khoj, an advanced web page reading
 assistant. You are to construct **up to three, valid** webpage urls to read
 before answering the user's question. - You will receive the conversation
 history as context. - Add as much context from the previous questions and
 answers as required to construct the webpage urls. - Use multiple web page urls
 if required to retrieve the relevant information. - You have access to the the
 whole internet to retrieve information. Which webpages will you need to read to
```

### Comparing `khoj_assistant-1.8.0/src/khoj/processor/conversation/utils.py` & `khoj_assistant-1.8.1.dev11/src/khoj/processor/conversation/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 import json
 import logging
 import queue
 from datetime import datetime
 from time import perf_counter
-from typing import Any, Dict, List
+from typing import Any, Dict, List, Optional
 
 import tiktoken
 from langchain.schema import ChatMessage
+from llama_cpp.llama import Llama
 from transformers import AutoTokenizer
 
 from khoj.database.adapters import ConversationAdapters
 from khoj.database.models import ClientApplication, KhojUser
+from khoj.processor.conversation.offline.utils import download_model
 from khoj.utils.helpers import is_none_or_empty, merge_dicts
 
 logger = logging.getLogger(__name__)
 model_to_prompt_size = {
-    "gpt-3.5-turbo": 3000,
-    "gpt-3.5-turbo-0125": 3000,
-    "gpt-4-0125-preview": 7000,
-    "gpt-4-turbo-preview": 7000,
-    "llama-2-7b-chat.ggmlv3.q4_0.bin": 1548,
-    "mistral-7b-instruct-v0.1.Q4_0.gguf": 1548,
-}
-model_to_tokenizer = {
-    "llama-2-7b-chat.ggmlv3.q4_0.bin": "hf-internal-testing/llama-tokenizer",
-    "mistral-7b-instruct-v0.1.Q4_0.gguf": "mistralai/Mistral-7B-Instruct-v0.1",
+    "gpt-3.5-turbo": 12000,
+    "gpt-3.5-turbo-0125": 12000,
+    "gpt-4-0125-preview": 20000,
+    "gpt-4-turbo-preview": 20000,
+    "TheBloke/Mistral-7B-Instruct-v0.2-GGUF": 3500,
+    "NousResearch/Hermes-2-Pro-Mistral-7B-GGUF": 3500,
 }
+model_to_tokenizer: Dict[str, str] = {}
 
 
 class ThreadedGenerator:
     def __init__(self, compiled_references, online_results, completion_func=None):
         self.queue = queue.Queue()
         self.compiled_references = compiled_references
         self.online_results = online_results
@@ -130,17 +129,18 @@
 Khoj: "{inferred_queries if ("text-to-image" in intent_type) else chat_response}"
 """.strip()
     )
 
 
 def generate_chatml_messages_with_context(
     user_message,
-    system_message,
+    system_message=None,
     conversation_log={},
     model_name="gpt-3.5-turbo",
+    loaded_model: Optional[Llama] = None,
     max_prompt_size=None,
     tokenizer_name=None,
 ):
     """Generate messages for ChatGPT with context from previous conversation"""
     # Set max prompt size from user config, pre-configured for model or to default prompt size
     try:
         max_prompt_size = max_prompt_size or model_to_prompt_size[model_name]
@@ -155,15 +155,15 @@
 
     # Extract Chat History for Context
     chat_logs = []
     for chat in conversation_log.get("chat", []):
         chat_notes = f'\n\n Notes:\n{chat.get("context")}' if chat.get("context") else "\n"
         chat_logs += [chat["message"] + chat_notes]
 
-    rest_backnforths = []
+    rest_backnforths: List[ChatMessage] = []
     # Extract in reverse chronological order
     for user_msg, assistant_msg in zip(chat_logs[-2::-2], chat_logs[::-2]):
         if len(rest_backnforths) >= 2 * lookback_turns:
             break
         rest_backnforths += reciprocal_conversation_to_chatml([user_msg, assistant_msg])[::-1]
 
     # Format user and system messages to chatml format
@@ -172,30 +172,39 @@
         messages.append(ChatMessage(content=user_message, role="user"))
     if len(rest_backnforths) > 0:
         messages += rest_backnforths
     if not is_none_or_empty(system_message):
         messages.append(ChatMessage(content=system_message, role="system"))
 
     # Truncate oldest messages from conversation history until under max supported prompt size by model
-    messages = truncate_messages(messages, max_prompt_size, model_name, tokenizer_name)
+    messages = truncate_messages(messages, max_prompt_size, model_name, loaded_model, tokenizer_name)
 
     # Return message in chronological order
     return messages[::-1]
 
 
 def truncate_messages(
-    messages: list[ChatMessage], max_prompt_size, model_name: str, tokenizer_name=None
+    messages: list[ChatMessage],
+    max_prompt_size,
+    model_name: str,
+    loaded_model: Optional[Llama] = None,
+    tokenizer_name=None,
 ) -> list[ChatMessage]:
     """Truncate messages to fit within max prompt size supported by model"""
 
     try:
-        if model_name.startswith("gpt-"):
+        if loaded_model:
+            encoder = loaded_model.tokenizer()
+        elif model_name.startswith("gpt-"):
             encoder = tiktoken.encoding_for_model(model_name)
         else:
-            encoder = AutoTokenizer.from_pretrained(tokenizer_name or model_to_tokenizer[model_name])
+            try:
+                encoder = download_model(model_name).tokenizer()
+            except:
+                encoder = AutoTokenizer.from_pretrained(tokenizer_name or model_to_tokenizer[model_name])
     except:
         default_tokenizer = "hf-internal-testing/llama-tokenizer"
         encoder = AutoTokenizer.from_pretrained(default_tokenizer)
         logger.warning(
             f"Fallback to default chat model tokenizer: {default_tokenizer}.\nConfigure tokenizer for unsupported model: {model_name} in Khoj settings to improve context stuffing."
         )
 
@@ -219,20 +228,25 @@
 
     # Truncate current message if still over max supported prompt size by model
     if (tokens + system_message_tokens) > max_prompt_size:
         current_message = "\n".join(messages[0].content.split("\n")[:-1]) if type(messages[0].content) == str else ""
         original_question = "\n".join(messages[0].content.split("\n")[-1:]) if type(messages[0].content) == str else ""
         original_question = f"\n{original_question}"
         original_question_tokens = len(encoder.encode(original_question))
-        remaining_tokens = max_prompt_size - original_question_tokens - system_message_tokens
-        truncated_message = encoder.decode(encoder.encode(current_message)[:remaining_tokens]).strip()
+        remaining_tokens = max_prompt_size - system_message_tokens
+        if remaining_tokens > original_question_tokens:
+            remaining_tokens -= original_question_tokens
+            truncated_message = encoder.decode(encoder.encode(current_message)[:remaining_tokens]).strip()
+            messages = [ChatMessage(content=truncated_message + original_question, role=messages[0].role)]
+        else:
+            truncated_message = encoder.decode(encoder.encode(original_question)[:remaining_tokens]).strip()
+            messages = [ChatMessage(content=truncated_message, role=messages[0].role)]
         logger.debug(
             f"Truncate current message to fit within max prompt size of {max_prompt_size} supported by {model_name} model:\n {truncated_message}"
         )
-        messages = [ChatMessage(content=truncated_message + original_question, role=messages[0].role)]
 
     return messages + [system_message] if system_message else messages
 
 
 def reciprocal_conversation_to_chatml(message_pair):
     """Convert a single back and forth between user and assistant to chatml format"""
     return [ChatMessage(content=message, role=role) for message, role in zip(message_pair, ["user", "assistant"])]
```

### Comparing `khoj_assistant-1.8.0/src/khoj/processor/conversation/offline/chat_model.py` & `khoj_assistant-1.8.1.dev11/src/khoj/processor/conversation/offline/chat_model.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,108 +1,98 @@
+import json
 import logging
-from collections import deque
-from datetime import datetime
+from datetime import datetime, timedelta
 from threading import Thread
 from typing import Any, Iterator, List, Union
 
 from langchain.schema import ChatMessage
+from llama_cpp import Llama
 
 from khoj.database.models import Agent
 from khoj.processor.conversation import prompts
+from khoj.processor.conversation.offline.utils import download_model
 from khoj.processor.conversation.utils import (
     ThreadedGenerator,
     generate_chatml_messages_with_context,
 )
 from khoj.utils import state
 from khoj.utils.constants import empty_escape_sequences
 from khoj.utils.helpers import ConversationCommand, is_none_or_empty
 from khoj.utils.rawconfig import LocationData
 
 logger = logging.getLogger(__name__)
 
 
 def extract_questions_offline(
     text: str,
-    model: str = "mistral-7b-instruct-v0.1.Q4_0.gguf",
+    model: str = "NousResearch/Hermes-2-Pro-Mistral-7B-GGUF",
     loaded_model: Union[Any, None] = None,
     conversation_log={},
     use_history: bool = True,
     should_extract_questions: bool = True,
     location_data: LocationData = None,
 ) -> List[str]:
     """
     Infer search queries to retrieve relevant notes to answer user query
     """
-    try:
-        from gpt4all import GPT4All
-    except ModuleNotFoundError as e:
-        logger.info("There was an error importing GPT4All. Please run pip install gpt4all in order to install it.")
-        raise e
-
-    # Assert that loaded_model is either None or of type GPT4All
-    assert loaded_model is None or isinstance(loaded_model, GPT4All), "loaded_model must be of type GPT4All or None"
-
     all_questions = text.split("? ")
     all_questions = [q + "?" for q in all_questions[:-1]] + [all_questions[-1]]
 
     if not should_extract_questions:
         return all_questions
 
-    gpt4all_model = loaded_model or GPT4All(model)
+    assert loaded_model is None or isinstance(loaded_model, Llama), "loaded_model must be of type Llama, if configured"
+    offline_chat_model = loaded_model or download_model(model)
 
     location = f"{location_data.city}, {location_data.region}, {location_data.country}" if location_data else "Unknown"
 
     # Extract Past User Message and Inferred Questions from Conversation Log
     chat_history = ""
 
     if use_history:
         for chat in conversation_log.get("chat", [])[-4:]:
-            if chat["by"] == "khoj" and chat["intent"].get("type") != "text-to-image":
+            if chat["by"] == "khoj" and "text-to-image" not in chat["intent"].get("type"):
                 chat_history += f"Q: {chat['intent']['query']}\n"
-                chat_history += f"A: {chat['message']}\n"
+                chat_history += f"Khoj: {chat['message']}\n\n"
 
-    current_date = datetime.now().strftime("%Y-%m-%d")
-    last_year = datetime.now().year - 1
-    last_christmas_date = f"{last_year}-12-25"
-    next_christmas_date = f"{datetime.now().year}-12-25"
-    system_prompt = prompts.system_prompt_extract_questions_gpt4all.format(
-        message=(prompts.system_prompt_message_extract_questions_gpt4all)
-    )
-    example_questions = prompts.extract_questions_gpt4all_sample.format(
+    today = datetime.today()
+    yesterday = (today - timedelta(days=1)).strftime("%Y-%m-%d")
+    last_year = today.year - 1
+    example_questions = prompts.extract_questions_offline.format(
         query=text,
         chat_history=chat_history,
-        current_date=current_date,
+        current_date=today.strftime("%Y-%m-%d"),
+        yesterday_date=yesterday,
         last_year=last_year,
-        last_christmas_date=last_christmas_date,
-        next_christmas_date=next_christmas_date,
+        this_year=today.year,
         location=location,
     )
-    message = system_prompt + example_questions
+    messages = generate_chatml_messages_with_context(
+        example_questions, model_name=model, loaded_model=offline_chat_model
+    )
+
     state.chat_lock.acquire()
     try:
-        response = gpt4all_model.generate(message, max_tokens=200, top_k=2, temp=0, n_batch=512)
+        response = send_message_to_model_offline(messages, loaded_model=offline_chat_model)
     finally:
         state.chat_lock.release()
 
     # Extract, Clean Message from GPT's Response
     try:
         # This will expect to be a list with a single string with a list of questions
-        questions = (
+        questions_str = (
             str(response)
             .strip(empty_escape_sequences)
             .replace("['", '["')
             .replace("<s>", "")
             .replace("</s>", "")
             .replace("']", '"]')
             .replace("', '", '", "')
-            .replace('["', "")
-            .replace('"]', "")
-            .split("? ")
         )
-        questions = [q + "?" for q in questions[:-1]] + [questions[-1]]
+        questions: List[str] = json.loads(questions_str)
         questions = filter_questions(questions)
     except:
         logger.warning(f"Llama returned invalid JSON. Falling back to using user message as search query.\n{response}")
         return all_questions
     logger.debug(f"Extracted Questions by Llama: {questions}")
     questions.extend(all_questions)
     return questions
@@ -117,59 +107,53 @@
         "can't",
         "cannot",
         "don't know",
         "don't understand",
         "do not know",
         "do not understand",
     ]
-    filtered_questions = []
+    filtered_questions = set()
     for q in questions:
         if not any([word in q.lower() for word in hint_words]) and not is_none_or_empty(q):
-            filtered_questions.append(q)
+            filtered_questions.add(q)
 
-    return filtered_questions
+    return list(filtered_questions)
 
 
 def converse_offline(
     user_query,
     references=[],
     online_results=[],
     conversation_log={},
-    model: str = "mistral-7b-instruct-v0.1.Q4_0.gguf",
+    model: str = "NousResearch/Hermes-2-Pro-Mistral-7B-GGUF",
     loaded_model: Union[Any, None] = None,
     completion_func=None,
     conversation_commands=[ConversationCommand.Default],
     max_prompt_size=None,
     tokenizer_name=None,
     location_data: LocationData = None,
     user_name: str = None,
     agent: Agent = None,
 ) -> Union[ThreadedGenerator, Iterator[str]]:
     """
     Converse with user using Llama
     """
-    try:
-        from gpt4all import GPT4All
-    except ModuleNotFoundError as e:
-        logger.info("There was an error importing GPT4All. Please run pip install gpt4all in order to install it.")
-        raise e
-
-    assert loaded_model is None or isinstance(loaded_model, GPT4All), "loaded_model must be of type GPT4All or None"
-    gpt4all_model = loaded_model or GPT4All(model)
     # Initialize Variables
+    assert loaded_model is None or isinstance(loaded_model, Llama), "loaded_model must be of type Llama, if configured"
+    offline_chat_model = loaded_model or download_model(model)
     compiled_references_message = "\n\n".join({f"{item}" for item in references})
 
     current_date = datetime.now().strftime("%Y-%m-%d")
 
     if agent and agent.personality:
-        system_prompt = prompts.custom_system_prompt_message_gpt4all.format(
+        system_prompt = prompts.custom_system_prompt_offline_chat.format(
             name=agent.name, bio=agent.personality, current_date=current_date
         )
     else:
-        system_prompt = prompts.system_prompt_message_gpt4all.format(current_date=current_date)
+        system_prompt = prompts.system_prompt_offline_chat.format(current_date=current_date)
 
     conversation_primer = prompts.query_prompt.format(query=user_query)
 
     if location_data:
         location = f"{location_data.city}, {location_data.region}, {location_data.country}"
         location_prompt = prompts.user_location.format(location=location)
         conversation_primer = f"{location_prompt}\n{conversation_primer}"
@@ -189,84 +173,56 @@
         simplified_online_results = online_results.copy()
         for result in online_results:
             if online_results[result].get("webpages"):
                 simplified_online_results[result] = online_results[result]["webpages"]
 
         conversation_primer = f"{prompts.online_search_conversation.format(online_results=str(simplified_online_results))}\n{conversation_primer}"
     if not is_none_or_empty(compiled_references_message):
-        conversation_primer = f"{prompts.notes_conversation_gpt4all.format(references=compiled_references_message)}\n{conversation_primer}"
+        conversation_primer = f"{prompts.notes_conversation_offline.format(references=compiled_references_message)}\n{conversation_primer}"
 
     # Setup Prompt with Primer or Conversation History
     messages = generate_chatml_messages_with_context(
         conversation_primer,
         system_prompt,
         conversation_log,
         model_name=model,
+        loaded_model=offline_chat_model,
         max_prompt_size=max_prompt_size,
         tokenizer_name=tokenizer_name,
     )
 
     g = ThreadedGenerator(references, online_results, completion_func=completion_func)
-    t = Thread(target=llm_thread, args=(g, messages, gpt4all_model))
+    t = Thread(target=llm_thread, args=(g, messages, offline_chat_model))
     t.start()
     return g
 
 
 def llm_thread(g, messages: List[ChatMessage], model: Any):
-    user_message = messages[-1]
-    system_message = messages[0]
-    conversation_history = messages[1:-1]
-
-    formatted_messages = [
-        prompts.khoj_message_gpt4all.format(message=message.content)
-        if message.role == "assistant"
-        else prompts.user_message_gpt4all.format(message=message.content)
-        for message in conversation_history
-    ]
-
     stop_phrases = ["<s>", "INST]", "Notes:"]
-    chat_history = "".join(formatted_messages)
-    templated_system_message = prompts.system_prompt_gpt4all.format(message=system_message.content)
-    templated_user_message = prompts.user_message_gpt4all.format(message=user_message.content)
-    prompted_message = templated_system_message + chat_history + templated_user_message
-    response_queue: deque[str] = deque(maxlen=3)  # Create a response queue with a maximum length of 3
-    hit_stop_phrase = False
 
     state.chat_lock.acquire()
-    response_iterator = send_message_to_model_offline(prompted_message, loaded_model=model, streaming=True)
     try:
+        response_iterator = send_message_to_model_offline(
+            messages, loaded_model=model, stop=stop_phrases, streaming=True
+        )
         for response in response_iterator:
-            response_queue.append(response)
-            hit_stop_phrase = any(stop_phrase in "".join(response_queue) for stop_phrase in stop_phrases)
-            if hit_stop_phrase:
-                logger.debug(f"Stop response as hit stop phrase: {''.join(response_queue)}")
-                break
-            # Start streaming the response at a lag once the queue is full
-            # This allows stop word testing before sending the response
-            if len(response_queue) == response_queue.maxlen:
-                g.send(response_queue[0])
+            g.send(response["choices"][0]["delta"].get("content", ""))
     finally:
-        if not hit_stop_phrase:
-            if len(response_queue) == response_queue.maxlen:
-                # remove already sent reponse chunk
-                response_queue.popleft()
-            # send the remaining response
-            g.send("".join(response_queue))
         state.chat_lock.release()
     g.close()
 
 
 def send_message_to_model_offline(
-    message, loaded_model=None, model="mistral-7b-instruct-v0.1.Q4_0.gguf", streaming=False, system_message=""
-) -> str:
-    try:
-        from gpt4all import GPT4All
-    except ModuleNotFoundError as e:
-        logger.info("There was an error importing GPT4All. Please run pip install gpt4all in order to install it.")
-        raise e
-
-    assert loaded_model is None or isinstance(loaded_model, GPT4All), "loaded_model must be of type GPT4All or None"
-    gpt4all_model = loaded_model or GPT4All(model)
-
-    return gpt4all_model.generate(
-        system_message + message, max_tokens=200, top_k=2, temp=0, n_batch=512, streaming=streaming
-    )
+    messages: List[ChatMessage],
+    loaded_model=None,
+    model="NousResearch/Hermes-2-Pro-Mistral-7B-GGUF",
+    streaming=False,
+    stop=[],
+):
+    assert loaded_model is None or isinstance(loaded_model, Llama), "loaded_model must be of type Llama, if configured"
+    offline_chat_model = loaded_model or download_model(model)
+    messages_dict = [{"role": message.role, "content": message.content} for message in messages]
+    response = offline_chat_model.create_chat_completion(messages_dict, stop=stop, stream=streaming)
+    if streaming:
+        return response
+    else:
+        return response["choices"][0]["message"].get("content", "")
```

### Comparing `khoj_assistant-1.8.0/src/khoj/processor/conversation/openai/gpt.py` & `khoj_assistant-1.8.1.dev11/src/khoj/processor/conversation/openai/gpt.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/processor/conversation/openai/utils.py` & `khoj_assistant-1.8.1.dev11/src/khoj/processor/conversation/openai/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -97,12 +97,7 @@
         max_retries=1,
         client=None,
     )
 
     chat(messages=messages)
 
     g.close()
-
-
-def extract_summaries(metadata):
-    """Extract summaries from metadata"""
-    return "".join([f'\n{session["summary"]}' for session in metadata])
```

### Comparing `khoj_assistant-1.8.0/src/khoj/processor/tools/online_search.py` & `khoj_assistant-1.8.1.dev11/src/khoj/processor/tools/online_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/routers/api.py` & `khoj_assistant-1.8.1.dev11/src/khoj/routers/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     update_telemetry_state,
 )
 from khoj.search_filter.date_filter import DateFilter
 from khoj.search_filter.file_filter import FileFilter
 from khoj.search_filter.word_filter import WordFilter
 from khoj.search_type import image_search, text_search
 from khoj.utils import constants, state
-from khoj.utils.config import GPT4AllProcessorModel
+from khoj.utils.config import OfflineChatProcessorModel
 from khoj.utils.helpers import ConversationCommand, timer
 from khoj.utils.rawconfig import LocationData, SearchResponse
 from khoj.utils.state import SearchType
 
 # Initialize Router
 api = APIRouter()
 logger = logging.getLogger(__name__)
@@ -314,24 +314,24 @@
             offline_chat_config
             and offline_chat_config.enabled
             and conversation_config.model_type == ChatModelOptions.ModelType.OFFLINE
         ):
             using_offline_chat = True
             default_offline_llm = await ConversationAdapters.get_default_offline_llm()
             chat_model = default_offline_llm.chat_model
-            if state.gpt4all_processor_config is None:
-                state.gpt4all_processor_config = GPT4AllProcessorModel(chat_model=chat_model)
+            if state.offline_chat_processor_config is None:
+                state.offline_chat_processor_config = OfflineChatProcessorModel(chat_model=chat_model)
 
-            loaded_model = state.gpt4all_processor_config.loaded_model
+            loaded_model = state.offline_chat_processor_config.loaded_model
 
             inferred_queries = extract_questions_offline(
                 defiltered_query,
                 loaded_model=loaded_model,
                 conversation_log=meta_log,
-                should_extract_questions=False,
+                should_extract_questions=True,
                 location_data=location_data,
             )
         elif conversation_config and conversation_config.model_type == ChatModelOptions.ModelType.OPENAI:
             openai_chat_config = await ConversationAdapters.get_openai_chat_config()
             default_openai_llm = await ConversationAdapters.aget_default_openai_llm()
             api_key = openai_chat_config.api_key
             chat_model = default_openai_llm.chat_model
```

### Comparing `khoj_assistant-1.8.0/src/khoj/routers/api_agents.py` & `khoj_assistant-1.8.1.dev11/src/khoj/routers/api_agents.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/routers/api_chat.py` & `khoj_assistant-1.8.1.dev11/src/khoj/routers/api_chat.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/routers/api_config.py` & `khoj_assistant-1.8.1.dev11/src/khoj/routers/api_config.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/routers/api_phone.py` & `khoj_assistant-1.8.1.dev11/src/khoj/routers/api_phone.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/routers/auth.py` & `khoj_assistant-1.8.1.dev11/src/khoj/routers/auth.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/routers/helpers.py` & `khoj_assistant-1.8.1.dev11/src/khoj/routers/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from khoj.processor.conversation.utils import (
     ThreadedGenerator,
     generate_chatml_messages_with_context,
     save_to_conversation_log,
 )
 from khoj.routers.storage import upload_image
 from khoj.utils import state
-from khoj.utils.config import GPT4AllProcessorModel
+from khoj.utils.config import OfflineChatProcessorModel
 from khoj.utils.helpers import (
     ConversationCommand,
     is_none_or_empty,
     is_valid_url,
     log_telemetry,
     mode_descriptions_for_llm,
     timer,
@@ -65,17 +65,17 @@
 async def is_ready_to_chat(user: KhojUser):
     has_offline_config = await ConversationAdapters.ahas_offline_chat()
     has_openai_config = await ConversationAdapters.has_openai_chat()
     user_conversation_config = await ConversationAdapters.aget_user_conversation_config(user)
 
     if has_offline_config and user_conversation_config and user_conversation_config.model_type == "offline":
         chat_model = user_conversation_config.chat_model
-        if state.gpt4all_processor_config is None:
+        if state.offline_chat_processor_config is None:
             logger.info("Loading Offline Chat Model...")
-            state.gpt4all_processor_config = GPT4AllProcessorModel(chat_model=chat_model)
+            state.offline_chat_processor_config = OfflineChatProcessorModel(chat_model=chat_model)
         return True
 
     ready = has_openai_config or has_offline_config
 
     if not ready:
         raise HTTPException(status_code=500, detail="Set your OpenAI API key or enable Local LLM via Khoj settings.")
 
@@ -323,18 +323,21 @@
     note_references: List[str],
     online_results: Optional[dict] = None,
 ) -> str:
     """
     Generate a better image prompt from the given query
     """
 
-    location = f"{location_data.city}, {location_data.region}, {location_data.country}" if location_data else "Unknown"
     today_date = datetime.now(tz=timezone.utc).strftime("%Y-%m-%d")
 
-    location_prompt = prompts.user_location.format(location=location)
+    if location_data:
+        location = f"{location_data.city}, {location_data.region}, {location_data.country}"
+        location_prompt = prompts.user_location.format(location=location)
+    else:
+        location_prompt = "Unknown"
 
     user_references = "\n\n".join([f"# {item}" for item in note_references])
 
     simplified_online_results = {}
 
     if online_results:
         for result in online_results:
@@ -364,35 +367,39 @@
     response_type: str = "text",
 ):
     conversation_config: ChatModelOptions = await ConversationAdapters.aget_default_conversation_config()
 
     if conversation_config is None:
         raise HTTPException(status_code=500, detail="Contact the server administrator to set a default chat model.")
 
-    truncated_messages = generate_chatml_messages_with_context(
-        user_message=message, system_message=system_message, model_name=conversation_config.chat_model
-    )
+    chat_model = conversation_config.chat_model
 
     if conversation_config.model_type == "offline":
-        if state.gpt4all_processor_config is None or state.gpt4all_processor_config.loaded_model is None:
-            state.gpt4all_processor_config = GPT4AllProcessorModel(conversation_config.chat_model)
+        if state.offline_chat_processor_config is None or state.offline_chat_processor_config.loaded_model is None:
+            state.offline_chat_processor_config = OfflineChatProcessorModel(chat_model)
+
+        loaded_model = state.offline_chat_processor_config.loaded_model
+        truncated_messages = generate_chatml_messages_with_context(
+            user_message=message, system_message=system_message, model_name=chat_model, loaded_model=loaded_model
+        )
 
-        loaded_model = state.gpt4all_processor_config.loaded_model
         return send_message_to_model_offline(
-            message=truncated_messages[-1].content,
+            messages=truncated_messages,
             loaded_model=loaded_model,
-            model=conversation_config.chat_model,
+            model=chat_model,
             streaming=False,
-            system_message=truncated_messages[0].content,
         )
 
     elif conversation_config.model_type == "openai":
         openai_chat_config = await ConversationAdapters.aget_openai_conversation_config()
         api_key = openai_chat_config.api_key
-        chat_model = conversation_config.chat_model
+        truncated_messages = generate_chatml_messages_with_context(
+            user_message=message, system_message=system_message, model_name=chat_model
+        )
+
         openai_response = send_message_to_model(
             messages=truncated_messages, api_key=api_key, model=chat_model, response_type=response_type
         )
 
         return openai_response
     else:
         raise HTTPException(status_code=500, detail="Invalid conversation config")
@@ -430,18 +437,18 @@
             inferred_queries=inferred_queries,
             client_application=client_application,
             conversation_id=conversation_id,
         )
 
         conversation_config = ConversationAdapters.get_valid_conversation_config(user, conversation)
         if conversation_config.model_type == "offline":
-            if state.gpt4all_processor_config is None or state.gpt4all_processor_config.loaded_model is None:
-                state.gpt4all_processor_config = GPT4AllProcessorModel(conversation_config.chat_model)
+            if state.offline_chat_processor_config is None or state.offline_chat_processor_config.loaded_model is None:
+                state.offline_chat_processor_config = OfflineChatProcessorModel(conversation_config.chat_model)
 
-            loaded_model = state.gpt4all_processor_config.loaded_model
+            loaded_model = state.offline_chat_processor_config.loaded_model
             chat_response = converse_offline(
                 references=compiled_references,
                 online_results=online_results,
                 user_query=q,
                 loaded_model=loaded_model,
                 conversation_log=meta_log,
                 completion_func=partial_completion,
```

### Comparing `khoj_assistant-1.8.0/src/khoj/routers/indexer.py` & `khoj_assistant-1.8.1.dev11/src/khoj/routers/indexer.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/routers/storage.py` & `khoj_assistant-1.8.1.dev11/src/khoj/routers/storage.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/routers/subscription.py` & `khoj_assistant-1.8.1.dev11/src/khoj/routers/subscription.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/routers/twilio.py` & `khoj_assistant-1.8.1.dev11/src/khoj/routers/twilio.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/routers/web_client.py` & `khoj_assistant-1.8.1.dev11/src/khoj/routers/web_client.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/search_filter/date_filter.py` & `khoj_assistant-1.8.1.dev11/src/khoj/search_filter/date_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/search_filter/file_filter.py` & `khoj_assistant-1.8.1.dev11/src/khoj/search_filter/file_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/search_filter/word_filter.py` & `khoj_assistant-1.8.1.dev11/src/khoj/search_filter/word_filter.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/search_type/image_search.py` & `khoj_assistant-1.8.1.dev11/src/khoj/search_type/image_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/search_type/text_search.py` & `khoj_assistant-1.8.1.dev11/src/khoj/search_type/text_search.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/utils/cli.py` & `khoj_assistant-1.8.1.dev11/src/khoj/utils/cli.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/utils/config.py` & `khoj_assistant-1.8.1.dev11/src/khoj/utils/config.py`

 * *Files 16% similar despite different names*

```diff
@@ -66,23 +66,20 @@
 @dataclass
 class SearchModels:
     text_search: Optional[TextSearchModel] = None
     image_search: Optional[ImageSearchModel] = None
 
 
 @dataclass
-class GPT4AllProcessorConfig:
+class OfflineChatProcessorConfig:
     loaded_model: Union[Any, None] = None
 
 
-class GPT4AllProcessorModel:
-    def __init__(
-        self,
-        chat_model: str = "mistral-7b-instruct-v0.1.Q4_0.gguf",
-    ):
+class OfflineChatProcessorModel:
+    def __init__(self, chat_model: str = "NousResearch/Hermes-2-Pro-Mistral-7B-GGUF"):
         self.chat_model = chat_model
         self.loaded_model = None
         try:
             self.loaded_model = download_model(self.chat_model)
         except ValueError as e:
             self.loaded_model = None
             logger.error(f"Error while loading offline chat model: {e}", exc_info=True)
```

### Comparing `khoj_assistant-1.8.0/src/khoj/utils/constants.py` & `khoj_assistant-1.8.1.dev11/src/khoj/utils/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 app_root_directory = Path(__file__).parent.parent.parent
 web_directory = app_root_directory / "khoj/interface/web/"
 empty_escape_sequences = "\n|\r|\t| "
 app_env_filepath = "~/.khoj/env"
 telemetry_server = "https://khoj.beta.haletic.com/v1/telemetry"
 content_directory = "~/.khoj/content/"
-default_offline_chat_model = "mistral-7b-instruct-v0.1.Q4_0.gguf"
+default_offline_chat_model = "NousResearch/Hermes-2-Pro-Mistral-7B-GGUF"
 default_online_chat_model = "gpt-4-turbo-preview"
 
 empty_config = {
     "search-type": {
         "image": {"encoder": "sentence-transformers/clip-ViT-B-32", "model_directory": "~/.khoj/search/image/"},
     },
 }
```

### Comparing `khoj_assistant-1.8.0/src/khoj/utils/fs_syncer.py` & `khoj_assistant-1.8.1.dev11/src/khoj/utils/fs_syncer.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/utils/helpers.py` & `khoj_assistant-1.8.1.dev11/src/khoj/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/utils/initialization.py` & `khoj_assistant-1.8.1.dev11/src/khoj/utils/initialization.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,25 +28,21 @@
 
     def _create_chat_configuration():
         logger.info(
             "🗣️  Configure chat models available to your server. You can always update these at /server/admin using the credentials of your admin account"
         )
 
         try:
-            # Note: gpt4all package is not available on all devices.
-            # So ensure gpt4all package is installed before continuing this step.
-            import gpt4all
-
             use_offline_model = input("Use offline chat model? (y/n): ")
             if use_offline_model == "y":
                 logger.info("🗣️ Setting up offline chat model")
                 OfflineChatProcessorConversationConfig.objects.create(enabled=True)
 
                 offline_chat_model = input(
-                    f"Enter the offline chat model you want to use, See GPT4All for supported models (default: {default_offline_chat_model}): "
+                    f"Enter the offline chat model you want to use. See HuggingFace for available GGUF models (default: {default_offline_chat_model}): "
                 )
                 if offline_chat_model == "":
                     ChatModelOptions.objects.create(
                         chat_model=default_offline_chat_model, model_type=ChatModelOptions.ModelType.OFFLINE
                     )
                 else:
                     default_max_tokens = model_to_prompt_size.get(offline_chat_model, 2000)
```

### Comparing `khoj_assistant-1.8.0/src/khoj/utils/jsonl.py` & `khoj_assistant-1.8.1.dev11/src/khoj/utils/jsonl.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/utils/models.py` & `khoj_assistant-1.8.1.dev11/src/khoj/utils/models.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/src/khoj/utils/rawconfig.py` & `khoj_assistant-1.8.1.dev11/src/khoj/utils/rawconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 class OpenAIProcessorConfig(ConfigBase):
     api_key: str
     chat_model: Optional[str] = "gpt-3.5-turbo"
 
 
 class OfflineChatProcessorConfig(ConfigBase):
     enable_offline_chat: Optional[bool] = False
-    chat_model: Optional[str] = "mistral-7b-instruct-v0.1.Q4_0.gguf"
+    chat_model: Optional[str] = "NousResearch/Hermes-2-Pro-Mistral-7B-GGUF"
 
 
 class ConversationProcessorConfig(ConfigBase):
     openai: Optional[OpenAIProcessorConfig] = None
     offline_chat: Optional[OfflineChatProcessorConfig] = None
     max_prompt_size: Optional[int] = None
     tokenizer: Optional[str] = None
```

### Comparing `khoj_assistant-1.8.0/src/khoj/utils/state.py` & `khoj_assistant-1.8.1.dev11/src/khoj/utils/state.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 from typing import Dict, List
 
 from openai import OpenAI
 from whisper import Whisper
 
 from khoj.processor.embeddings import CrossEncoderModel, EmbeddingsModel
 from khoj.utils import config as utils_config
-from khoj.utils.config import ContentIndex, GPT4AllProcessorModel, SearchModels
+from khoj.utils.config import ContentIndex, OfflineChatProcessorModel, SearchModels
 from khoj.utils.helpers import LRU, get_device
 from khoj.utils.rawconfig import FullConfig
 
 # Application Global State
 config = FullConfig()
 search_models = SearchModels()
 embeddings_model: Dict[str, EmbeddingsModel] = None
 cross_encoder_model: Dict[str, CrossEncoderModel] = None
 content_index = ContentIndex()
 openai_client: OpenAI = None
-gpt4all_processor_config: GPT4AllProcessorModel = None
+offline_chat_processor_config: OfflineChatProcessorModel = None
 whisper_model: Whisper = None
 config_file: Path = None
 verbose: int = 0
 host: str = None
 port: int = None
 cli_args: List[str] = None
 query_cache: Dict[str, LRU] = defaultdict(LRU)
```

### Comparing `khoj_assistant-1.8.0/src/khoj/utils/yaml.py` & `khoj_assistant-1.8.1.dev11/src/khoj/utils/yaml.py`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/.gitignore` & `khoj_assistant-1.8.1.dev11/.gitignore`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/LICENSE` & `khoj_assistant-1.8.1.dev11/LICENSE`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/README.md` & `khoj_assistant-1.8.1.dev11/README.md`

 * *Files identical despite different names*

### Comparing `khoj_assistant-1.8.0/pyproject.toml` & `khoj_assistant-1.8.1.dev11/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -58,16 +58,15 @@
     "langchain <= 0.2.0",
     "langchain-openai >= 0.0.5",
     "requests >= 2.26.0",
     "anyio == 3.7.1",
     "pymupdf >= 1.23.5",
     "django == 4.2.10",
     "authlib == 1.2.1",
-    "gpt4all == 2.1.0; platform_system == 'Linux' and platform_machine == 'x86_64'",
-    "gpt4all == 2.1.0; platform_system == 'Windows' or platform_system == 'Darwin'",
+    "llama-cpp-python == 0.2.56",
     "itsdangerous == 2.1.2",
     "httpx == 0.25.0",
     "pgvector == 0.2.4",
     "psycopg2-binary == 2.9.9",
     "gunicorn == 21.2.0",
     "lxml == 4.9.3",
     "tzdata == 2023.3",
```

### Comparing `khoj_assistant-1.8.0/PKG-INFO` & `khoj_assistant-1.8.1.dev11/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: khoj-assistant
-Version: 1.8.0
+Version: 1.8.1.dev11
 Summary: An AI copilot for your Second Brain
 Project-URL: Homepage, https://khoj.dev
 Project-URL: Documentation, https://docs.khoj.dev
 Project-URL: Code, https://github.com/khoj-ai/khoj
 Author: Debanjum Singh Solanky, Saba Imran
 License-Expression: AGPL-3.0-or-later
 License-File: LICENSE
@@ -26,22 +26,21 @@
 Requires-Dist: authlib==1.2.1
 Requires-Dist: beautifulsoup4~=4.12.3
 Requires-Dist: dateparser>=1.1.1
 Requires-Dist: defusedxml==0.7.1
 Requires-Dist: django-phonenumber-field==7.3.0
 Requires-Dist: django==4.2.10
 Requires-Dist: fastapi>=0.104.1
-Requires-Dist: gpt4all==2.1.0; platform_system == 'Linux' and platform_machine == 'x86_64'
-Requires-Dist: gpt4all==2.1.0; platform_system == 'Windows' or platform_system == 'Darwin'
 Requires-Dist: gunicorn==21.2.0
 Requires-Dist: httpx==0.25.0
 Requires-Dist: itsdangerous==2.1.2
 Requires-Dist: jinja2==3.1.3
 Requires-Dist: langchain-openai>=0.0.5
 Requires-Dist: langchain<=0.2.0
+Requires-Dist: llama-cpp-python==0.2.56
 Requires-Dist: lxml==4.9.3
 Requires-Dist: markdownify~=0.11.6
 Requires-Dist: openai-whisper>=20231117
 Requires-Dist: openai>=1.0.0
 Requires-Dist: pgvector==0.2.4
 Requires-Dist: phonenumbers==8.13.27
 Requires-Dist: pillow~=9.5.0
```

