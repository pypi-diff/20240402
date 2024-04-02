# Comparing `tmp/genericsuite-0.1.1.tar.gz` & `tmp/genericsuite-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genericsuite-0.1.1.tar", max compression
+gzip compressed data, was "genericsuite-0.1.2.tar", max compression
```

## Comparing `genericsuite-0.1.1.tar` & `genericsuite-0.1.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1074 2024-03-03 12:08:30.337779 genericsuite-0.1.1/LICENSE
--rw-r--r--   0        0        0    11296 2024-03-18 11:55:18.436429 genericsuite-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-03-03 23:49:07.732831 genericsuite-0.1.1/genericsuite/__init__.py
--rw-r--r--   0        0        0        0 2024-02-21 12:30:14.702977 genericsuite-0.1.1/genericsuite/chalicelib/__init__.py
--rw-r--r--   0        0        0        0 2024-02-23 11:10:05.850616 genericsuite-0.1.1/genericsuite/chalicelib/endpoints/__init__.py
--rw-r--r--   0        0        0     1096 2024-02-24 02:22:20.582188 genericsuite-0.1.1/genericsuite/chalicelib/endpoints/menu_options.py
--rw-r--r--   0        0        0     2125 2024-02-24 02:14:13.742858 genericsuite-0.1.1/genericsuite/chalicelib/endpoints/users.py
--rw-r--r--   0        0        0     1482 2024-02-24 13:33:20.978316 genericsuite-0.1.1/genericsuite/chalicelib/framework_abstraction.py
--rw-r--r--   0        0        0        0 2024-02-21 12:47:25.905045 genericsuite-0.1.1/genericsuite/chalicelib/util/__init__.py
--rw-r--r--   0        0        0     2751 2024-02-26 13:41:07.446923 genericsuite-0.1.1/genericsuite/chalicelib/util/create_app.py
--rw-r--r--   0        0        0     4647 2024-02-25 17:57:02.422438 genericsuite-0.1.1/genericsuite/chalicelib/util/generic_endpoint_builder.py
--rw-r--r--   0        0        0        0 2023-04-09 20:12:57.378538 genericsuite-0.1.1/genericsuite/config/__init__.py
--rw-r--r--   0        0        0     4443 2024-03-01 12:22:13.763424 genericsuite-0.1.1/genericsuite/config/config.py
--rw-r--r--   0        0        0     4683 2024-03-01 00:12:35.189298 genericsuite-0.1.1/genericsuite/config/config_from_db.py
--rw-r--r--   0        0        0      609 2024-02-18 20:15:35.895205 genericsuite-0.1.1/genericsuite/config/logging.conf.yml
--rw-r--r--   0        0        0        0 2024-02-18 20:15:35.895273 genericsuite-0.1.1/genericsuite/constants/__init__.py
--rw-r--r--   0        0        0     1443 2024-02-23 00:45:12.985504 genericsuite-0.1.1/genericsuite/constants/const_tables.py
--rw-r--r--   0        0        0        0 2024-02-21 12:30:32.204369 genericsuite-0.1.1/genericsuite/fastapilib/__init__.py
--rw-r--r--   0        0        0     1455 2024-02-24 13:33:13.552960 genericsuite-0.1.1/genericsuite/fastapilib/framework_abstraction.py
--rw-r--r--   0        0        0        0 2024-02-21 12:47:35.347602 genericsuite-0.1.1/genericsuite/fastapilib/util/__init__.py
--rw-r--r--   0        0        0     1307 2024-02-18 20:15:35.911504 genericsuite-0.1.1/genericsuite/fastapilib/util/generic_endpoint_builder.py
--rw-r--r--   0        0        0        0 2024-02-21 12:30:50.817726 genericsuite-0.1.1/genericsuite/flasklib/__init__.py
--rw-r--r--   0        0        0     1708 2024-02-24 13:34:01.565559 genericsuite-0.1.1/genericsuite/flasklib/framework_abstraction.py
--rw-r--r--   0        0        0        0 2024-02-21 12:47:42.207235 genericsuite-0.1.1/genericsuite/flasklib/util/__init__.py
--rw-r--r--   0        0        0        0 2024-02-18 20:15:35.903766 genericsuite-0.1.1/genericsuite/models/billing/__init__.py
--rw-r--r--   0        0        0     1419 2024-03-03 02:47:22.334682 genericsuite-0.1.1/genericsuite/models/billing/billing_utilities.py
--rw-r--r--   0        0        0        0 2023-07-17 02:15:00.638430 genericsuite-0.1.1/genericsuite/models/menu_options/__init__.py
--rw-r--r--   0        0        0     2840 2024-02-24 02:14:13.741348 genericsuite-0.1.1/genericsuite/models/menu_options/menu_options.py
--rw-r--r--   0        0        0        0 2023-04-09 20:12:57.379886 genericsuite-0.1.1/genericsuite/models/users/__init__.py
--rw-r--r--   0        0        0     8650 2024-02-25 16:04:51.338589 genericsuite-0.1.1/genericsuite/models/users/users.py
--rw-r--r--   0        0        0        0 2023-04-09 20:12:57.380476 genericsuite-0.1.1/genericsuite/util/__init__.py
--rw-r--r--   0        0        0     5898 2024-02-29 11:32:04.042270 genericsuite-0.1.1/genericsuite/util/app_context.py
--rw-r--r--   0        0        0     1608 2024-02-23 01:37:50.489847 genericsuite-0.1.1/genericsuite/util/app_logger.py
--rw-r--r--   0        0        0     7160 2024-02-23 00:45:13.028977 genericsuite-0.1.1/genericsuite/util/aws.py
--rw-r--r--   0        0        0     4319 2024-02-23 00:45:12.989787 genericsuite-0.1.1/genericsuite/util/blueprint_one.py
--rw-r--r--   0        0        0     1797 2024-02-23 10:56:31.242663 genericsuite-0.1.1/genericsuite/util/config_dbdef_helpers.py
--rw-r--r--   0        0        0     1387 2024-02-27 16:04:59.642735 genericsuite-0.1.1/genericsuite/util/current_user_data.py
--rw-r--r--   0        0        0     4972 2024-03-02 04:46:29.973118 genericsuite-0.1.1/genericsuite/util/datetime_utilities.py
--rw-r--r--   0        0        0    35651 2024-02-25 15:25:41.529780 genericsuite-0.1.1/genericsuite/util/db_abstractor.py
--rw-r--r--   0        0        0      807 2024-02-21 16:28:35.421102 genericsuite-0.1.1/genericsuite/util/exceptions.py
--rw-r--r--   0        0        0     2287 2024-02-24 13:40:02.416560 genericsuite-0.1.1/genericsuite/util/framework_abs_layer.py
--rw-r--r--   0        0        0    47797 2024-02-25 17:57:22.042814 genericsuite-0.1.1/genericsuite/util/generic_db_helpers.py
--rw-r--r--   0        0        0     5889 2024-02-25 12:47:46.514099 genericsuite-0.1.1/genericsuite/util/generic_db_middleware.py
--rw-r--r--   0        0        0    10325 2024-02-27 16:04:16.316160 genericsuite-0.1.1/genericsuite/util/generic_endpoint_helpers.py
--rw-r--r--   0        0        0     5372 2024-02-26 14:01:45.304576 genericsuite-0.1.1/genericsuite/util/jwt.py
--rw-r--r--   0        0        0     3216 2024-02-23 00:45:13.032873 genericsuite-0.1.1/genericsuite/util/nav_helpers.py
--rw-r--r--   0        0        0     4421 2024-02-23 00:45:13.039348 genericsuite-0.1.1/genericsuite/util/parse_multipart.py
--rw-r--r--   0        0        0     1818 2024-02-23 01:37:50.488701 genericsuite-0.1.1/genericsuite/util/passwords.py
--rw-r--r--   0        0        0      585 2024-02-18 20:15:35.910549 genericsuite-0.1.1/genericsuite/util/request_handler.py
--rw-r--r--   0        0        0     6568 2024-02-23 00:45:13.032854 genericsuite-0.1.1/genericsuite/util/security.py
--rw-r--r--   0        0        0     3318 2024-02-25 11:52:22.059881 genericsuite-0.1.1/genericsuite/util/send_email.py
--rw-r--r--   0        0        0    16009 2024-03-02 15:00:06.343708 genericsuite-0.1.1/genericsuite/util/utilities.py
--rw-r--r--   0        0        0     1429 2024-03-19 13:05:50.502989 genericsuite-0.1.1/pyproject.toml
--rw-r--r--   0        0        0    12493 1970-01-01 00:00:00.000000 genericsuite-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      747 2024-03-31 23:36:29.408323 genericsuite-0.1.2/LICENSE
+-rw-r--r--   0        0        0    12258 2024-03-31 23:43:26.985724 genericsuite-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-03-03 23:49:07.732831 genericsuite-0.1.2/genericsuite/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-21 12:30:14.702977 genericsuite-0.1.2/genericsuite/chalicelib/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-23 11:10:05.850616 genericsuite-0.1.2/genericsuite/chalicelib/endpoints/__init__.py
+-rw-r--r--   0        0        0     1096 2024-02-24 02:22:20.582188 genericsuite-0.1.2/genericsuite/chalicelib/endpoints/menu_options.py
+-rw-r--r--   0        0        0     2125 2024-02-24 02:14:13.742858 genericsuite-0.1.2/genericsuite/chalicelib/endpoints/users.py
+-rw-r--r--   0        0        0     1482 2024-02-24 13:33:20.978316 genericsuite-0.1.2/genericsuite/chalicelib/framework_abstraction.py
+-rw-r--r--   0        0        0        0 2024-02-21 12:47:25.905045 genericsuite-0.1.2/genericsuite/chalicelib/util/__init__.py
+-rw-r--r--   0        0        0     2751 2024-02-26 13:41:07.446923 genericsuite-0.1.2/genericsuite/chalicelib/util/create_app.py
+-rw-r--r--   0        0        0     4647 2024-02-25 17:57:02.422438 genericsuite-0.1.2/genericsuite/chalicelib/util/generic_endpoint_builder.py
+-rw-r--r--   0        0        0        0 2023-04-09 20:12:57.378538 genericsuite-0.1.2/genericsuite/config/__init__.py
+-rw-r--r--   0        0        0     4443 2024-03-01 12:22:13.763424 genericsuite-0.1.2/genericsuite/config/config.py
+-rw-r--r--   0        0        0     4683 2024-03-01 00:12:35.189298 genericsuite-0.1.2/genericsuite/config/config_from_db.py
+-rw-r--r--   0        0        0      609 2024-02-18 20:15:35.895205 genericsuite-0.1.2/genericsuite/config/logging.conf.yml
+-rw-r--r--   0        0        0        0 2024-02-18 20:15:35.895273 genericsuite-0.1.2/genericsuite/constants/__init__.py
+-rw-r--r--   0        0        0     1443 2024-02-23 00:45:12.985504 genericsuite-0.1.2/genericsuite/constants/const_tables.py
+-rw-r--r--   0        0        0        0 2024-02-21 12:30:32.204369 genericsuite-0.1.2/genericsuite/fastapilib/__init__.py
+-rw-r--r--   0        0        0     1455 2024-02-24 13:33:13.552960 genericsuite-0.1.2/genericsuite/fastapilib/framework_abstraction.py
+-rw-r--r--   0        0        0        0 2024-02-21 12:47:35.347602 genericsuite-0.1.2/genericsuite/fastapilib/util/__init__.py
+-rw-r--r--   0        0        0     1307 2024-02-18 20:15:35.911504 genericsuite-0.1.2/genericsuite/fastapilib/util/generic_endpoint_builder.py
+-rw-r--r--   0        0        0        0 2024-02-21 12:30:50.817726 genericsuite-0.1.2/genericsuite/flasklib/__init__.py
+-rw-r--r--   0        0        0     1708 2024-02-24 13:34:01.565559 genericsuite-0.1.2/genericsuite/flasklib/framework_abstraction.py
+-rw-r--r--   0        0        0        0 2024-02-21 12:47:42.207235 genericsuite-0.1.2/genericsuite/flasklib/util/__init__.py
+-rw-r--r--   0        0        0        0 2024-02-18 20:15:35.903766 genericsuite-0.1.2/genericsuite/models/billing/__init__.py
+-rw-r--r--   0        0        0     1419 2024-03-03 02:47:22.334682 genericsuite-0.1.2/genericsuite/models/billing/billing_utilities.py
+-rw-r--r--   0        0        0        0 2023-07-17 02:15:00.638430 genericsuite-0.1.2/genericsuite/models/menu_options/__init__.py
+-rw-r--r--   0        0        0     2840 2024-02-24 02:14:13.741348 genericsuite-0.1.2/genericsuite/models/menu_options/menu_options.py
+-rw-r--r--   0        0        0        0 2023-04-09 20:12:57.379886 genericsuite-0.1.2/genericsuite/models/users/__init__.py
+-rw-r--r--   0        0        0     8650 2024-02-25 16:04:51.338589 genericsuite-0.1.2/genericsuite/models/users/users.py
+-rw-r--r--   0        0        0        0 2023-04-09 20:12:57.380476 genericsuite-0.1.2/genericsuite/util/__init__.py
+-rw-r--r--   0        0        0     5898 2024-02-29 11:32:04.042270 genericsuite-0.1.2/genericsuite/util/app_context.py
+-rw-r--r--   0        0        0     1608 2024-02-23 01:37:50.489847 genericsuite-0.1.2/genericsuite/util/app_logger.py
+-rw-r--r--   0        0        0     7160 2024-02-23 00:45:13.028977 genericsuite-0.1.2/genericsuite/util/aws.py
+-rw-r--r--   0        0        0     4319 2024-02-23 00:45:12.989787 genericsuite-0.1.2/genericsuite/util/blueprint_one.py
+-rw-r--r--   0        0        0     1797 2024-02-23 10:56:31.242663 genericsuite-0.1.2/genericsuite/util/config_dbdef_helpers.py
+-rw-r--r--   0        0        0     1387 2024-02-27 16:04:59.642735 genericsuite-0.1.2/genericsuite/util/current_user_data.py
+-rw-r--r--   0        0        0     4972 2024-03-02 04:46:29.973118 genericsuite-0.1.2/genericsuite/util/datetime_utilities.py
+-rw-r--r--   0        0        0    35651 2024-02-25 15:25:41.529780 genericsuite-0.1.2/genericsuite/util/db_abstractor.py
+-rw-r--r--   0        0        0      807 2024-02-21 16:28:35.421102 genericsuite-0.1.2/genericsuite/util/exceptions.py
+-rw-r--r--   0        0        0     2287 2024-02-24 13:40:02.416560 genericsuite-0.1.2/genericsuite/util/framework_abs_layer.py
+-rw-r--r--   0        0        0    47797 2024-02-25 17:57:22.042814 genericsuite-0.1.2/genericsuite/util/generic_db_helpers.py
+-rw-r--r--   0        0        0     5889 2024-02-25 12:47:46.514099 genericsuite-0.1.2/genericsuite/util/generic_db_middleware.py
+-rw-r--r--   0        0        0    10325 2024-02-27 16:04:16.316160 genericsuite-0.1.2/genericsuite/util/generic_endpoint_helpers.py
+-rw-r--r--   0        0        0     5372 2024-02-26 14:01:45.304576 genericsuite-0.1.2/genericsuite/util/jwt.py
+-rw-r--r--   0        0        0     3216 2024-02-23 00:45:13.032873 genericsuite-0.1.2/genericsuite/util/nav_helpers.py
+-rw-r--r--   0        0        0     4421 2024-02-23 00:45:13.039348 genericsuite-0.1.2/genericsuite/util/parse_multipart.py
+-rw-r--r--   0        0        0     1818 2024-02-23 01:37:50.488701 genericsuite-0.1.2/genericsuite/util/passwords.py
+-rw-r--r--   0        0        0      585 2024-02-18 20:15:35.910549 genericsuite-0.1.2/genericsuite/util/request_handler.py
+-rw-r--r--   0        0        0     6568 2024-02-23 00:45:13.032854 genericsuite-0.1.2/genericsuite/util/security.py
+-rw-r--r--   0        0        0     3318 2024-02-25 11:52:22.059881 genericsuite-0.1.2/genericsuite/util/send_email.py
+-rw-r--r--   0        0        0    16009 2024-03-02 15:00:06.343708 genericsuite-0.1.2/genericsuite/util/utilities.py
+-rw-r--r--   0        0        0     1429 2024-04-02 13:49:21.876653 genericsuite-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0    13455 1970-01-01 00:00:00.000000 genericsuite-0.1.2/PKG-INFO
```

### Comparing `genericsuite-0.1.1/README.md` & `genericsuite-0.1.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 - **Menu Options**: Functionality to manage and retrieve authorized menu options based on user roles.
 
 ## Pre-requisites
 
 - [Python](https://www.python.org/downloads/) >= 3.9 and < 4.0
 - [Git](https://www.atlassian.com/git/tutorials/install-git)
 - Make: [Mac](https://formulae.brew.sh/formula/make) | [Windows](https://stackoverflow.com/questions/32127524/how-to-install-and-use-make-in-windows)
+- Node version 18+, installed via [NVM (Node Package Manager)](https://nodejs.org/en/download/package-manager) or [NPM and Node](https://nodejs.org/en/download) install.
 
 ### AWS account and credentials
 
 If you plan to deploy the App in the AWS Cloud:
 
 * AWS account, see [free tier](https://aws.amazon.com/free).
 * AWS Token, see [Access Keys](https://us-east-1.console.aws.amazon.com/iamv2/home?region=us-east-1#/security_credentials?section=IAM_credentials).
@@ -34,17 +35,14 @@
 To get started with GenericSuite, follow these steps:
 
 ### Initiate your project
 
 To create the project directory for the App's backend API. E.g. `exampleapp_backend`, instrctions will depend on the dependency management of your preference:
 
 ```bash
-```
-
-```bash
 # Pip
 mkdir -p exampleapp_backend/exampleapp_backend
 cd exampleapp_backend
 python3 -m venv venv
 source venv/bin/activate
 ```
 
@@ -97,26 +95,53 @@
 ```
 
 #### Poetry
 ```bash
 poetry add git+https://github.com/tomkat-cr/genericsuite-be@branch_x
 ```
 
-## Usage
+### Test dependencies
+
+To execute the unit and integration test, install `pytest` and `coverage`:
+
+#### Pip
+```bash
+pip install pytest coverage
+```
+
+#### Pipenv
+```bash
+pipenv install --dev pytest coverage
+```
+
+#### Poetry
+```bash
+poetry add --dev pytest coverage
+```
+
+### Development scripts installation
+
+[The GenericSuite backend development scripts](https://github.com/tomkat-cr/genericsuite-be-scripts?tab=readme-ov-file#the-genericsuite-scripts-backend-version) contains utilities to build and deploy APIs made by The GenericSuite.
+
+```bash
+npm install -D genericsuite-be-scripts
+```
+
+## Features
 
 1. **Select Your Framework**: Depending on your project, choose between [Chalice](https://aws.github.io/chalice/quickstart.html), [FastAPI](https://fastapi.tiangolo.com/), or [Flask](https://flask.palletsprojects.com/).
 2. **Select Your Database of choice**: Implement database operations using the provided abstracted functions for [MongoDB](https://www.mongodb.com/) and [DynamoDB](https://aws.amazon.com/pm/dynamodb/).
 3. **Included Authentication**: Your endpoints will be secured with [JWT](https://jwt.io/libraries)-based authentication.
 4. **Define Endpoints**: Utilize the dynamic endpoint creation feature by defining your endpoints in a JSON configuration file. Visit the [Generic Suite Configuration Guide](https://github.com/tomkat-cr/genericsuite-fe/tree/main/src/configs) for more information.
 2. **Define Menu Options**: Utilize the dynamic menu creation feature by defining your muenu and option access security in a JSON configuration file. Visit the [Generic Suite Configuration Guide](https://github.com/tomkat-cr/genericsuite-fe/tree/main/src/configs) for guidance.
 2. **Define Table structures**: Utilize the dynamic table creation feature by defining your CRUD editors in JSON configuration files. Visit the [Generic Suite Configuration Guide](https://github.com/tomkat-cr/genericsuite-fe/tree/main/src/configs) for sample code and files.
 
 ## Configuration
 
-Configure your application by setting up the necessary environment variables. Refer to the [.env.example](https://github.com/tomkat-cr/genericsuite-be/blob/main/.env-example) file for the required variables.
+Configure your application by setting up the necessary environment variables. Refer to the [.env.example](https://github.com/tomkat-cr/genericsuite-be/blob/main/.env.example) and [config.py](https://github.com/tomkat-cr/genericsuite-be/blob/main/genericsuite/config/config.py) files for the available options.
 
 1. Aplicacion name
 ```
 APP_NAME=ExampleApp
 ```
 2. Aplicacion domain
 ```
@@ -168,14 +193,20 @@
 ```
 ```
 # PROD: AWS DynamoDB
 APP_DB_ENGINE_PROD=DYNAMO_DB
 APP_DB_NAME_PROD=
 APP_DB_URI_PROD=
 ```
+```
+# # DEMO: AWS DynamoDB
+# APP_DB_ENGINE_DEMO=DYNAMO_DB
+# APP_DB_NAME_DEMO=
+# APP_DB_URI_DEMO=
+```
 - For MongoDB
 ```
 # DEV: Docker container
 APP_DB_ENGINE_DEV=MONGO_DB
 APP_DB_NAME_DEV=mongo
 APP_DB_URI_DEV=mongodb://root:example@app.exampleapp.local:27017/
 ```
@@ -193,14 +224,20 @@
 ```
 ```
 # PROD: MongoDB Atlas
 APP_DB_ENGINE_PROD=MONGO_DB
 APP_DB_NAME_PROD=xxxx
 APP_DB_URI_PROD=mongodb+srv://<user>:<password>@<cluster>.mongodb.net
 ```
+```
+# DEMO: MongoDB Atlas
+APP_DB_ENGINE_DEMO=MONGO_DB
+APP_DB_NAME_DEMO=xxxx
+APP_DB_URI_DEMO=mongodb+srv://<user>:<password>@<cluster>.mongodb.net
+```
 8. CORS origin
 ```
 # DEV
 APP_CORS_ORIGIN_DEV=*
 APP_FRONTEND_AUDIENCE_DEV=
 ```
 ```
@@ -208,22 +245,27 @@
 APP_CORS_ORIGIN_QA=*
 APP_CORS_ORIGIN_QA_CLOUD=https://app-qa.exampleapp.com
 APP_CORS_ORIGIN_QA_LOCAL=http://localhost:3000
 APP_FRONTEND_AUDIENCE_QA=
 ```
 ```
 # Staging
-APP_CORS_ORIGIN_STAGING=*
+APP_CORS_ORIGIN_STAGING=https://app-qa.exampleapp.com
 APP_FRONTEND_AUDIENCE_STAGING=
 ```
 ```
 # PROD
-APP_CORS_ORIGIN_PROD=*
+APP_CORS_ORIGIN_PROD=https://app.exampleapp.com
 APP_FRONTEND_AUDIENCE_PROD=
 ```
+```
+# DEMO
+APP_CORS_ORIGIN_DEMO=https://app-demo.exampleapp.com
+APP_FRONTEND_AUDIENCE_DEMO=
+```
 9. Current framework options: chalice, flask, fastapi
 ```
 CURRENT_FRAMEWORK=chalice
 ```
 10. JSON configuration files location and git URL
 ```
 GIT_SUBMODULE_LOCAL_PATH=lib/config_dbdef
@@ -274,25 +316,14 @@
 # Testing enndpoint
 TEST_APP_URL=http://app.exampleapp.local:5002
 ```
 19. Flask configuration
 ```
 FLASK_APP=index.py
 ```
-20. For GenricSuite AI only
-```
-# Aplicacion AI assistant name
-AI_ASSISTANT_NAME=ExampleBot
-
-# AWS configuration
-AWS_S3_CHATBOT_ATTACHMENTS_BUCKET_DEV=aws-s3-bucket-name
-AWS_S3_CHATBOT_ATTACHMENTS_BUCKET_QA=aws-s3-bucket-name
-AWS_S3_CHATBOT_ATTACHMENTS_BUCKET_STAGING=aws-s3-bucket-name
-AWS_S3_CHATBOT_ATTACHMENTS_BUCKET_PROD=aws-s3-bucket-name
-```
 
 ## App structure
 
 This is a suggested App development repository structure for a Chalice project:
 
 ```
 .
@@ -306,15 +337,15 @@
 │   ├── deployment
 │   │   ├── deployment.zip
 │   │   └── sam.json
 │   ├── deployments
 │   ├── dynamodb_cf_template.yaml
 │   └── policy-qa.json
 ├── .env
-├── .env-example
+├── .env.example
 ├── .gitignore
 ├── CHANGELOG.md
 ├── LICENSE
 ├── Makefile
 ├── Pipfile
 ├── Pipfile.lock
 ├── README.md
@@ -356,18 +387,22 @@
 
 ```
 
 ## Code examples and JSON configuration files
 
 The main menu, API endpoints and CRUD editor configurations are defined in the JSON configuration files.
 
-You can find examples about configurations and how to code an App [here](https://github.com/tomkat-cr/genericsuite-fe/blob/main/src/configs/README.md) and the different JSON files in the [src/configs/frontend](https://github.com/tomkat-cr/genericsuite-fe/blob/main/src/configs/frontend) and [src/configs/backend](https://github.com/tomkat-cr/genericsuite-fe/blob/main/src/configs/backend) directories.
+You can find examples about configurations and how to code an App in the [GenericSuite App Creation and Configuration guide](https://github.com/tomkat-cr/genericsuite-fe/blob/main/src/configs/README.md).
+
+## Usage
+
+Check the [The GenericSuite backend development scripts](https://github.com/tomkat-cr/genericsuite-be-scripts?tab=readme-ov-file#the-genericsuite-scripts-backend-version) for more details.
 
 ## License
 
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+This project is licensed under the ISC License - see the [LICENSE](https://github.com/tomkat-cr/genericsuite-be/blob/main/LICENSE) file for details.
 
 ## Credits
 
 This project is developed and maintained by Carlos J. Ramirez. For more information or to contribute to the project, visit [GenericSuite on GitHub](https://github.com/tomkat-cr/genericsuite-be).
 
-Happy Coding!
+Happy Coding!
```

### Comparing `genericsuite-0.1.1/genericsuite/chalicelib/endpoints/menu_options.py` & `genericsuite-0.1.2/genericsuite/chalicelib/endpoints/menu_options.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/chalicelib/endpoints/users.py` & `genericsuite-0.1.2/genericsuite/chalicelib/endpoints/users.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/chalicelib/framework_abstraction.py` & `genericsuite-0.1.2/genericsuite/chalicelib/framework_abstraction.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/chalicelib/util/create_app.py` & `genericsuite-0.1.2/genericsuite/chalicelib/util/create_app.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/chalicelib/util/generic_endpoint_builder.py` & `genericsuite-0.1.2/genericsuite/chalicelib/util/generic_endpoint_builder.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/config/config.py` & `genericsuite-0.1.2/genericsuite/config/config.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/config/config_from_db.py` & `genericsuite-0.1.2/genericsuite/config/config_from_db.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/config/logging.conf.yml` & `genericsuite-0.1.2/genericsuite/config/logging.conf.yml`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/constants/const_tables.py` & `genericsuite-0.1.2/genericsuite/constants/const_tables.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/fastapilib/framework_abstraction.py` & `genericsuite-0.1.2/genericsuite/fastapilib/framework_abstraction.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/fastapilib/util/generic_endpoint_builder.py` & `genericsuite-0.1.2/genericsuite/fastapilib/util/generic_endpoint_builder.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/flasklib/framework_abstraction.py` & `genericsuite-0.1.2/genericsuite/flasklib/framework_abstraction.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/models/billing/billing_utilities.py` & `genericsuite-0.1.2/genericsuite/models/billing/billing_utilities.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/models/menu_options/menu_options.py` & `genericsuite-0.1.2/genericsuite/models/menu_options/menu_options.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/models/users/users.py` & `genericsuite-0.1.2/genericsuite/models/users/users.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/util/app_context.py` & `genericsuite-0.1.2/genericsuite/util/app_context.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/util/app_logger.py` & `genericsuite-0.1.2/genericsuite/util/app_logger.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/util/aws.py` & `genericsuite-0.1.2/genericsuite/util/aws.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/util/blueprint_one.py` & `genericsuite-0.1.2/genericsuite/util/blueprint_one.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/util/config_dbdef_helpers.py` & `genericsuite-0.1.2/genericsuite/util/config_dbdef_helpers.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/util/current_user_data.py` & `genericsuite-0.1.2/genericsuite/util/current_user_data.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/util/datetime_utilities.py` & `genericsuite-0.1.2/genericsuite/util/datetime_utilities.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/util/db_abstractor.py` & `genericsuite-0.1.2/genericsuite/util/db_abstractor.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/util/exceptions.py` & `genericsuite-0.1.2/genericsuite/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/util/framework_abs_layer.py` & `genericsuite-0.1.2/genericsuite/util/framework_abs_layer.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/util/generic_db_helpers.py` & `genericsuite-0.1.2/genericsuite/util/generic_db_helpers.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/util/generic_db_middleware.py` & `genericsuite-0.1.2/genericsuite/util/generic_db_middleware.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/util/generic_endpoint_helpers.py` & `genericsuite-0.1.2/genericsuite/util/generic_endpoint_helpers.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/util/jwt.py` & `genericsuite-0.1.2/genericsuite/util/jwt.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/util/nav_helpers.py` & `genericsuite-0.1.2/genericsuite/util/nav_helpers.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/util/parse_multipart.py` & `genericsuite-0.1.2/genericsuite/util/parse_multipart.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/util/passwords.py` & `genericsuite-0.1.2/genericsuite/util/passwords.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/util/request_handler.py` & `genericsuite-0.1.2/genericsuite/util/request_handler.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/util/security.py` & `genericsuite-0.1.2/genericsuite/util/security.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/util/send_email.py` & `genericsuite-0.1.2/genericsuite/util/send_email.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/genericsuite/util/utilities.py` & `genericsuite-0.1.2/genericsuite/util/utilities.py`

 * *Files identical despite different names*

### Comparing `genericsuite-0.1.1/pyproject.toml` & `genericsuite-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "genericsuite"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     { name="Carlos J. Ramirez", email="<tomkat_cr@yahoo.com>" }
 ]
 description = "The GenericSuite for Python (backend version)"
 readme = "README.md"
 requires-python = ">=3.9,<4.0"
 classifiers = [
@@ -15,15 +15,15 @@
 
 [project.urls]
 Homepage = "https://github.com/tomkat-cr/genericsuite-be"
 Issues = "https://github.com/tomkat-cr/genericsuite-be/issues"
 
 [tool.poetry]
 name = "genericsuite"
-version = "0.1.1"
+version = "0.1.2"
 description = "The GenericSuite for Python (backend version)"
 authors = ["Carlos J. Ramirez <tomkat_cr@yahoo.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/tomkat-cr/genericsuite-be.git"
 packages = [
     { include = "genericsuite" }
```

### Comparing `genericsuite-0.1.1/PKG-INFO` & `genericsuite-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genericsuite
-Version: 0.1.1
+Version: 0.1.2
 Summary: The GenericSuite for Python (backend version)
 Home-page: https://github.com/tomkat-cr/genericsuite-be.git
 License: MIT
 Author: Carlos J. Ramirez
 Author-email: tomkat_cr@yahoo.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -45,14 +45,15 @@
 - **Menu Options**: Functionality to manage and retrieve authorized menu options based on user roles.
 
 ## Pre-requisites
 
 - [Python](https://www.python.org/downloads/) >= 3.9 and < 4.0
 - [Git](https://www.atlassian.com/git/tutorials/install-git)
 - Make: [Mac](https://formulae.brew.sh/formula/make) | [Windows](https://stackoverflow.com/questions/32127524/how-to-install-and-use-make-in-windows)
+- Node version 18+, installed via [NVM (Node Package Manager)](https://nodejs.org/en/download/package-manager) or [NPM and Node](https://nodejs.org/en/download) install.
 
 ### AWS account and credentials
 
 If you plan to deploy the App in the AWS Cloud:
 
 * AWS account, see [free tier](https://aws.amazon.com/free).
 * AWS Token, see [Access Keys](https://us-east-1.console.aws.amazon.com/iamv2/home?region=us-east-1#/security_credentials?section=IAM_credentials).
@@ -64,17 +65,14 @@
 To get started with GenericSuite, follow these steps:
 
 ### Initiate your project
 
 To create the project directory for the App's backend API. E.g. `exampleapp_backend`, instrctions will depend on the dependency management of your preference:
 
 ```bash
-```
-
-```bash
 # Pip
 mkdir -p exampleapp_backend/exampleapp_backend
 cd exampleapp_backend
 python3 -m venv venv
 source venv/bin/activate
 ```
 
@@ -127,26 +125,53 @@
 ```
 
 #### Poetry
 ```bash
 poetry add git+https://github.com/tomkat-cr/genericsuite-be@branch_x
 ```
 
-## Usage
+### Test dependencies
+
+To execute the unit and integration test, install `pytest` and `coverage`:
+
+#### Pip
+```bash
+pip install pytest coverage
+```
+
+#### Pipenv
+```bash
+pipenv install --dev pytest coverage
+```
+
+#### Poetry
+```bash
+poetry add --dev pytest coverage
+```
+
+### Development scripts installation
+
+[The GenericSuite backend development scripts](https://github.com/tomkat-cr/genericsuite-be-scripts?tab=readme-ov-file#the-genericsuite-scripts-backend-version) contains utilities to build and deploy APIs made by The GenericSuite.
+
+```bash
+npm install -D genericsuite-be-scripts
+```
+
+## Features
 
 1. **Select Your Framework**: Depending on your project, choose between [Chalice](https://aws.github.io/chalice/quickstart.html), [FastAPI](https://fastapi.tiangolo.com/), or [Flask](https://flask.palletsprojects.com/).
 2. **Select Your Database of choice**: Implement database operations using the provided abstracted functions for [MongoDB](https://www.mongodb.com/) and [DynamoDB](https://aws.amazon.com/pm/dynamodb/).
 3. **Included Authentication**: Your endpoints will be secured with [JWT](https://jwt.io/libraries)-based authentication.
 4. **Define Endpoints**: Utilize the dynamic endpoint creation feature by defining your endpoints in a JSON configuration file. Visit the [Generic Suite Configuration Guide](https://github.com/tomkat-cr/genericsuite-fe/tree/main/src/configs) for more information.
 2. **Define Menu Options**: Utilize the dynamic menu creation feature by defining your muenu and option access security in a JSON configuration file. Visit the [Generic Suite Configuration Guide](https://github.com/tomkat-cr/genericsuite-fe/tree/main/src/configs) for guidance.
 2. **Define Table structures**: Utilize the dynamic table creation feature by defining your CRUD editors in JSON configuration files. Visit the [Generic Suite Configuration Guide](https://github.com/tomkat-cr/genericsuite-fe/tree/main/src/configs) for sample code and files.
 
 ## Configuration
 
-Configure your application by setting up the necessary environment variables. Refer to the [.env.example](https://github.com/tomkat-cr/genericsuite-be/blob/main/.env-example) file for the required variables.
+Configure your application by setting up the necessary environment variables. Refer to the [.env.example](https://github.com/tomkat-cr/genericsuite-be/blob/main/.env.example) and [config.py](https://github.com/tomkat-cr/genericsuite-be/blob/main/genericsuite/config/config.py) files for the available options.
 
 1. Aplicacion name
 ```
 APP_NAME=ExampleApp
 ```
 2. Aplicacion domain
 ```
@@ -198,14 +223,20 @@
 ```
 ```
 # PROD: AWS DynamoDB
 APP_DB_ENGINE_PROD=DYNAMO_DB
 APP_DB_NAME_PROD=
 APP_DB_URI_PROD=
 ```
+```
+# # DEMO: AWS DynamoDB
+# APP_DB_ENGINE_DEMO=DYNAMO_DB
+# APP_DB_NAME_DEMO=
+# APP_DB_URI_DEMO=
+```
 - For MongoDB
 ```
 # DEV: Docker container
 APP_DB_ENGINE_DEV=MONGO_DB
 APP_DB_NAME_DEV=mongo
 APP_DB_URI_DEV=mongodb://root:example@app.exampleapp.local:27017/
 ```
@@ -223,14 +254,20 @@
 ```
 ```
 # PROD: MongoDB Atlas
 APP_DB_ENGINE_PROD=MONGO_DB
 APP_DB_NAME_PROD=xxxx
 APP_DB_URI_PROD=mongodb+srv://<user>:<password>@<cluster>.mongodb.net
 ```
+```
+# DEMO: MongoDB Atlas
+APP_DB_ENGINE_DEMO=MONGO_DB
+APP_DB_NAME_DEMO=xxxx
+APP_DB_URI_DEMO=mongodb+srv://<user>:<password>@<cluster>.mongodb.net
+```
 8. CORS origin
 ```
 # DEV
 APP_CORS_ORIGIN_DEV=*
 APP_FRONTEND_AUDIENCE_DEV=
 ```
 ```
@@ -238,22 +275,27 @@
 APP_CORS_ORIGIN_QA=*
 APP_CORS_ORIGIN_QA_CLOUD=https://app-qa.exampleapp.com
 APP_CORS_ORIGIN_QA_LOCAL=http://localhost:3000
 APP_FRONTEND_AUDIENCE_QA=
 ```
 ```
 # Staging
-APP_CORS_ORIGIN_STAGING=*
+APP_CORS_ORIGIN_STAGING=https://app-qa.exampleapp.com
 APP_FRONTEND_AUDIENCE_STAGING=
 ```
 ```
 # PROD
-APP_CORS_ORIGIN_PROD=*
+APP_CORS_ORIGIN_PROD=https://app.exampleapp.com
 APP_FRONTEND_AUDIENCE_PROD=
 ```
+```
+# DEMO
+APP_CORS_ORIGIN_DEMO=https://app-demo.exampleapp.com
+APP_FRONTEND_AUDIENCE_DEMO=
+```
 9. Current framework options: chalice, flask, fastapi
 ```
 CURRENT_FRAMEWORK=chalice
 ```
 10. JSON configuration files location and git URL
 ```
 GIT_SUBMODULE_LOCAL_PATH=lib/config_dbdef
@@ -304,25 +346,14 @@
 # Testing enndpoint
 TEST_APP_URL=http://app.exampleapp.local:5002
 ```
 19. Flask configuration
 ```
 FLASK_APP=index.py
 ```
-20. For GenricSuite AI only
-```
-# Aplicacion AI assistant name
-AI_ASSISTANT_NAME=ExampleBot
-
-# AWS configuration
-AWS_S3_CHATBOT_ATTACHMENTS_BUCKET_DEV=aws-s3-bucket-name
-AWS_S3_CHATBOT_ATTACHMENTS_BUCKET_QA=aws-s3-bucket-name
-AWS_S3_CHATBOT_ATTACHMENTS_BUCKET_STAGING=aws-s3-bucket-name
-AWS_S3_CHATBOT_ATTACHMENTS_BUCKET_PROD=aws-s3-bucket-name
-```
 
 ## App structure
 
 This is a suggested App development repository structure for a Chalice project:
 
 ```
 .
@@ -336,15 +367,15 @@
 │   ├── deployment
 │   │   ├── deployment.zip
 │   │   └── sam.json
 │   ├── deployments
 │   ├── dynamodb_cf_template.yaml
 │   └── policy-qa.json
 ├── .env
-├── .env-example
+├── .env.example
 ├── .gitignore
 ├── CHANGELOG.md
 ├── LICENSE
 ├── Makefile
 ├── Pipfile
 ├── Pipfile.lock
 ├── README.md
@@ -386,18 +417,23 @@
 
 ```
 
 ## Code examples and JSON configuration files
 
 The main menu, API endpoints and CRUD editor configurations are defined in the JSON configuration files.
 
-You can find examples about configurations and how to code an App [here](https://github.com/tomkat-cr/genericsuite-fe/blob/main/src/configs/README.md) and the different JSON files in the [src/configs/frontend](https://github.com/tomkat-cr/genericsuite-fe/blob/main/src/configs/frontend) and [src/configs/backend](https://github.com/tomkat-cr/genericsuite-fe/blob/main/src/configs/backend) directories.
+You can find examples about configurations and how to code an App in the [GenericSuite App Creation and Configuration guide](https://github.com/tomkat-cr/genericsuite-fe/blob/main/src/configs/README.md).
+
+## Usage
+
+Check the [The GenericSuite backend development scripts](https://github.com/tomkat-cr/genericsuite-be-scripts?tab=readme-ov-file#the-genericsuite-scripts-backend-version) for more details.
 
 ## License
 
-This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
+This project is licensed under the ISC License - see the [LICENSE](https://github.com/tomkat-cr/genericsuite-be/blob/main/LICENSE) file for details.
 
 ## Credits
 
 This project is developed and maintained by Carlos J. Ramirez. For more information or to contribute to the project, visit [GenericSuite on GitHub](https://github.com/tomkat-cr/genericsuite-be).
 
 Happy Coding!
+
```

