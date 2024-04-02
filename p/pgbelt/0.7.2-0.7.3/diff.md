# Comparing `tmp/pgbelt-0.7.2.tar.gz` & `tmp/pgbelt-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgbelt-0.7.2.tar", max compression
+gzip compressed data, was "pgbelt-0.7.3.tar", max compression
```

## Comparing `pgbelt-0.7.2.tar` & `pgbelt-0.7.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    10758 2024-03-19 18:01:12.978157 pgbelt-0.7.2/LICENSE
--rw-r--r--   0        0        0     2185 2024-03-19 18:01:12.978157 pgbelt-0.7.2/README.md
--rw-r--r--   0        0        0      137 2024-03-19 18:01:12.978157 pgbelt-0.7.2/pgbelt/__init__.py
--rw-r--r--   0        0        0      462 2024-03-19 18:01:12.978157 pgbelt-0.7.2/pgbelt/cmd/__init__.py
--rw-r--r--   0        0        0     5857 2024-03-19 18:01:12.978157 pgbelt-0.7.2/pgbelt/cmd/convenience.py
--rw-r--r--   0        0        0     5292 2024-03-19 18:01:12.978157 pgbelt-0.7.2/pgbelt/cmd/helpers.py
--rw-r--r--   0        0        0     3043 2024-03-19 18:01:12.978157 pgbelt-0.7.2/pgbelt/cmd/login.py
--rw-r--r--   0        0        0    20676 2024-03-19 18:01:12.978157 pgbelt-0.7.2/pgbelt/cmd/preflight.py
--rw-r--r--   0        0        0     4760 2024-03-19 18:01:12.978157 pgbelt-0.7.2/pgbelt/cmd/schema.py
--rw-r--r--   0        0        0     7015 2024-03-19 18:01:12.978157 pgbelt-0.7.2/pgbelt/cmd/setup.py
--rw-r--r--   0        0        0     4905 2024-03-19 18:01:12.978157 pgbelt-0.7.2/pgbelt/cmd/status.py
--rw-r--r--   0        0        0     9415 2024-03-19 18:01:12.978157 pgbelt-0.7.2/pgbelt/cmd/sync.py
--rw-r--r--   0        0        0     3526 2024-03-19 18:01:12.978157 pgbelt-0.7.2/pgbelt/cmd/teardown.py
--rw-r--r--   0        0        0       35 2024-03-19 18:01:12.982157 pgbelt-0.7.2/pgbelt/config/__init__.py
--rw-r--r--   0        0        0     3817 2024-03-19 18:01:12.982157 pgbelt-0.7.2/pgbelt/config/config.py
--rw-r--r--   0        0        0     5830 2024-03-19 18:01:12.982157 pgbelt-0.7.2/pgbelt/config/models.py
--rw-r--r--   0        0        0     5297 2024-03-19 18:01:12.982157 pgbelt-0.7.2/pgbelt/config/remote.py
--rw-r--r--   0        0        0      186 2024-03-19 18:01:12.982157 pgbelt-0.7.2/pgbelt/main.py
--rw-r--r--   0        0        0       40 2024-03-19 18:01:12.982157 pgbelt-0.7.2/pgbelt/util/__init__.py
--rw-r--r--   0        0        0      583 2024-03-19 18:01:12.982157 pgbelt-0.7.2/pgbelt/util/asyncfuncs.py
--rw-r--r--   0        0        0    14715 2024-03-19 18:01:12.982157 pgbelt-0.7.2/pgbelt/util/dump.py
--rw-r--r--   0        0        0     1699 2024-03-19 18:01:12.982157 pgbelt-0.7.2/pgbelt/util/logs.py
--rw-r--r--   0        0        0    13611 2024-03-19 18:01:12.982157 pgbelt-0.7.2/pgbelt/util/pglogical.py
--rw-r--r--   0        0        0    19819 2024-03-19 18:01:12.982157 pgbelt-0.7.2/pgbelt/util/postgres.py
--rw-r--r--   0        0        0     1229 2024-03-19 18:01:12.982157 pgbelt-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     2964 1970-01-01 00:00:00.000000 pgbelt-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    10758 2024-04-02 06:31:48.565441 pgbelt-0.7.3/LICENSE
+-rw-r--r--   0        0        0     2185 2024-04-02 06:31:48.565441 pgbelt-0.7.3/README.md
+-rw-r--r--   0        0        0      137 2024-04-02 06:31:48.565441 pgbelt-0.7.3/pgbelt/__init__.py
+-rw-r--r--   0        0        0      462 2024-04-02 06:31:48.565441 pgbelt-0.7.3/pgbelt/cmd/__init__.py
+-rw-r--r--   0        0        0     5857 2024-04-02 06:31:48.565441 pgbelt-0.7.3/pgbelt/cmd/convenience.py
+-rw-r--r--   0        0        0     5292 2024-04-02 06:31:48.565441 pgbelt-0.7.3/pgbelt/cmd/helpers.py
+-rw-r--r--   0        0        0     3043 2024-04-02 06:31:48.565441 pgbelt-0.7.3/pgbelt/cmd/login.py
+-rw-r--r--   0        0        0    20676 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/cmd/preflight.py
+-rw-r--r--   0        0        0     4760 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/cmd/schema.py
+-rw-r--r--   0        0        0     6627 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/cmd/setup.py
+-rw-r--r--   0        0        0     4730 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/cmd/status.py
+-rw-r--r--   0        0        0     9027 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/cmd/sync.py
+-rw-r--r--   0        0        0     3526 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/cmd/teardown.py
+-rw-r--r--   0        0        0       35 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/config/__init__.py
+-rw-r--r--   0        0        0     3817 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/config/config.py
+-rw-r--r--   0        0        0     5816 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/config/models.py
+-rw-r--r--   0        0        0     5307 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/config/remote.py
+-rw-r--r--   0        0        0      186 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/main.py
+-rw-r--r--   0        0        0       40 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/util/__init__.py
+-rw-r--r--   0        0        0      583 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/util/asyncfuncs.py
+-rw-r--r--   0        0        0    14715 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/util/dump.py
+-rw-r--r--   0        0        0     1699 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/util/logs.py
+-rw-r--r--   0        0        0    13613 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/util/pglogical.py
+-rw-r--r--   0        0        0    19270 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pgbelt/util/postgres.py
+-rw-r--r--   0        0        0     1234 2024-04-02 06:31:48.569441 pgbelt-0.7.3/pyproject.toml
+-rw-r--r--   0        0        0     2960 1970-01-01 00:00:00.000000 pgbelt-0.7.3/PKG-INFO
```

### Comparing `pgbelt-0.7.2/LICENSE` & `pgbelt-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.2/README.md` & `pgbelt-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.2/pgbelt/cmd/convenience.py` & `pgbelt-0.7.3/pgbelt/cmd/convenience.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.2/pgbelt/cmd/helpers.py` & `pgbelt-0.7.3/pgbelt/cmd/helpers.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.2/pgbelt/cmd/login.py` & `pgbelt-0.7.3/pgbelt/cmd/login.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.2/pgbelt/cmd/preflight.py` & `pgbelt-0.7.3/pgbelt/cmd/preflight.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.2/pgbelt/cmd/schema.py` & `pgbelt-0.7.3/pgbelt/cmd/schema.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.2/pgbelt/cmd/setup.py` & `pgbelt-0.7.3/pgbelt/cmd/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,22 +37,15 @@
     async with create_pool(conf.src.pglogical_uri, min_size=1) as src_pglogical_pool:
         pkey_tables, _, _ = await analyze_table_pkeys(
             src_pglogical_pool, conf.schema_name, src_logger
         )
 
     pglogical_tables = pkey_tables
     if conf.tables:
-        pglogical_tables = [
-            t
-            for t in pkey_tables
-            if t
-            in list(
-                map(str.lower, conf.tables)
-            )  # Postgres returns table names in lowercase (in analyze_table_pkeys)
-        ]
+        pglogical_tables = [t for t in pkey_tables if t in conf.tables]
 
     # Intentionally throw an error if no tables are found, so that the user can correct their config.
     # When reported by a certain user, errors showed when running the status command, but it was ignored,
     # then the user ran setup and since that DIDN'T throw an error, they assumed everything was fine.
 
     if not pglogical_tables:
         raise ValueError(
@@ -157,22 +150,15 @@
         pkeys, _, _ = await analyze_table_pkeys(
             src_pglogical_pool, conf.schema_name, src_logger
         )
         dst_logger = get_logger(conf.db, conf.dc, "setup.src")
 
         pglogical_tables = pkeys
         if conf.tables:
-            pglogical_tables = [
-                t
-                for t in pkeys
-                if t
-                in list(
-                    map(str.lower, conf.tables)
-                )  # Postgres returns table names in lowercase (in analyze_table_pkeys)
-            ]
+            pglogical_tables = [t for t in pkeys if t in conf.tables]
 
         await configure_replication_set(
             dst_root_pool, pglogical_tables, conf.schema_name, dst_logger
         )
         await configure_subscription(
             src_root_pool, "pg2_pg1", conf.dst.pglogical_dsn, src_logger
         )
```

### Comparing `pgbelt-0.7.2/pgbelt/cmd/status.py` & `pgbelt-0.7.3/pgbelt/cmd/status.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,22 +88,15 @@
     # Get the list of targeted tables by first getting all tables, then filtering whatever is in the config.
     pkey_tables, non_pkey_tables, _ = await analyze_table_pkeys(
         src_pool, conf.schema_name, src_logger
     )
     all_tables = pkey_tables + non_pkey_tables
     target_tables = all_tables
     if conf.tables:
-        target_tables = [
-            t
-            for t in all_tables
-            if t
-            in list(
-                map(str.lower, conf.tables)
-            )  # Postgres gave us lowercase table names in analyze_table_pkeys
-        ]
+        target_tables = [t for t in all_tables if t in conf.tables]
 
     if not target_tables:
         raise ValueError(
             f"Targeted tables not found in the source database. Please check your config's schema and tables. DB: {conf.db} DC: {conf.dc}, SCHEMA: {conf.schema_name} TABLES: {conf.tables}."
         )
 
     try:
```

### Comparing `pgbelt-0.7.2/pgbelt/cmd/sync.py` & `pgbelt-0.7.3/pgbelt/cmd/sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,22 +73,15 @@
     if tables:
         tables = tables.split(",")
     else:
         async with create_pool(conf.src.pglogical_uri, min_size=1) as src_pool:
             _, tables, _ = await analyze_table_pkeys(src_pool, conf.schema_name, logger)
 
         if conf.tables:
-            tables = [
-                t
-                for t in tables
-                if t
-                in list(
-                    map(str.lower, conf.tables)
-                )  # Postgres returns table names in lowercase (in analyze_table_pkeys)
-            ]
+            tables = [t for t in tables if t in conf.tables]
 
     await dump_source_tables(conf, tables, logger)
 
 
 @run_with_configs(skip_src=True)
 async def load_tables(
     config_future: Awaitable[DbupgradeConfig],
@@ -188,22 +181,15 @@
 
 
 async def _dump_and_load_all_tables(
     conf: DbupgradeConfig, src_pool: Pool, src_logger: Logger, dst_logger: Logger
 ) -> None:
     _, tables, _ = await analyze_table_pkeys(src_pool, conf.schema_name, src_logger)
     if conf.tables:
-        tables = [
-            t
-            for t in tables
-            if t
-            in list(
-                map(str.lower, conf.tables)
-            )  # Postgres returns table names in lowercase (in analyze_table_pkeys)
-        ]
+        tables = [t for t in tables if t in conf.tables]
     await dump_source_tables(conf, tables, src_logger)
     await load_dumped_tables(conf, tables, dst_logger)
 
 
 @run_with_configs
 async def sync(
     config_future: Awaitable[DbupgradeConfig], no_schema: bool = False
```

### Comparing `pgbelt-0.7.2/pgbelt/cmd/teardown.py` & `pgbelt-0.7.3/pgbelt/cmd/teardown.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.2/pgbelt/config/config.py` & `pgbelt-0.7.3/pgbelt/config/config.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.2/pgbelt/config/models.py` & `pgbelt-0.7.3/pgbelt/config/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from aiofiles import open as aopen
 from aiofiles.os import remove
 from pgbelt.util import get_logger
 from pgbelt.util.asyncfuncs import makedirs
 from pydantic import BaseModel
 from pydantic import ValidationError
-from pydantic import validator
+from pydantic import field_validator
 
 
 def config_dir(db: str, dc: str) -> str:
     return f"configs/{dc}/{db}"
 
 
 def config_file(db: str, dc: str) -> str:
@@ -33,15 +33,15 @@
     name: str The user name.
     pw: str The user's password. Only required for users pgbelt needs to log in as.
     """
 
     name: str
     pw: Optional[str] = None
 
-    _not_empty = validator("name", "pw", allow_reuse=True)(not_empty)
+    _not_empty = field_validator("name", "pw")(not_empty)
 
 
 class DbConfig(BaseModel):
     """
     Represents a postgres db instance.
 
     host: str The hostname of this instance.
@@ -60,17 +60,17 @@
     db: str
     port: str
     root_user: User
     owner_user: User
     pglogical_user: User
     other_users: Optional[list[User]] = None
 
-    _not_empty = validator("host", "ip", "db", "port", allow_reuse=True)(not_empty)
+    _not_empty = field_validator("host", "ip", "db", "port")(not_empty)
 
-    @validator("root_user", "owner_user", "pglogical_user")
+    @field_validator("root_user", "owner_user", "pglogical_user")
     def has_password(cls, v) -> User:  # noqa: N805
         if not v.pw:
             raise ValueError
         return v
 
     @property
     def root_dsn(self) -> str:
@@ -114,15 +114,15 @@
     dc: str
     src: Optional[DbConfig] = None
     dst: Optional[DbConfig] = None
     tables: Optional[list[str]] = None
     sequences: Optional[list[str]] = None
     schema_name: Optional[str] = "public"
 
-    _not_empty = validator("db", "dc", allow_reuse=True)(not_empty)
+    _not_empty = field_validator("db", "dc")(not_empty)
 
     @property
     def file(self) -> str:
         return config_file(self.db, self.dc)
 
     @property
     def dir(self) -> str:
@@ -163,15 +163,15 @@
             async with aopen(config_file(db, dc), "r") as f:
                 raw = await f.read()
         except FileNotFoundError:
             logger.info("No cached config available")
             return None
 
         try:
-            out = cls.parse_raw(raw)
+            out = cls.model_validate_json(raw)
         except ValidationError:
             logger.info("Cached config was not a valid DbupgradeConfig")
             return None
 
         logger.info("Found cached config.")
 
         return out
```

### Comparing `pgbelt-0.7.2/pgbelt/config/remote.py` & `pgbelt-0.7.3/pgbelt/config/remote.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     config_file: str, logger: Logger
 ) -> Optional[RemoteConfigDefinition]:
     try:
         logger.debug(f"Reading remote config definition from file {config_file}")
         async with aopen(config_file, mode="r") as f:
             raw_json = await f.read()
 
-        return RemoteConfigDefinition.parse_raw(raw_json)
+        return RemoteConfigDefinition.model_validate_json(raw_json)
     except FileNotFoundError:
         logger.error(f"No remote config definition exists at {config_file}")
     except JSONDecodeError:
         logger.error(f"Remote config definition in {config_file} was malformed JSON.")
     except ValidationError:
         logger.error(f"Remote config definition in {config_file} was not valid.")
```

### Comparing `pgbelt-0.7.2/pgbelt/util/asyncfuncs.py` & `pgbelt-0.7.3/pgbelt/util/asyncfuncs.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.2/pgbelt/util/dump.py` & `pgbelt-0.7.3/pgbelt/util/dump.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.2/pgbelt/util/logs.py` & `pgbelt-0.7.3/pgbelt/util/logs.py`

 * *Files identical despite different names*

### Comparing `pgbelt-0.7.2/pgbelt/util/pglogical.py` & `pgbelt-0.7.3/pgbelt/util/pglogical.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     and grant to each individually. Then we can call this for every known dsn and we won't miss
     any grants to pglogical because of weird ownership stuff.
     """
     logger.info("Granting data permissions to pglogical...")
     async with pool.acquire() as conn:
         async with conn.transaction():
             if tables:
-                tables_with_schema = [f"{schema}.{table}" for table in tables]
+                tables_with_schema = [f'{schema}."{table}"' for table in tables]
                 await conn.execute(
                     f"GRANT ALL ON TABLE {','.join(tables_with_schema)} TO pglogical;"
                 )
             else:
                 await conn.execute(
                     f"GRANT ALL ON ALL TABLES IN SCHEMA {schema} TO pglogical;"
                 )
```

### Comparing `pgbelt-0.7.2/pgbelt/util/postgres.py` & `pgbelt-0.7.3/pgbelt/util/postgres.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,22 +96,20 @@
 
     dst_old_extra_float_digits = await dst_pool.fetchval("SHOW extra_float_digits;")
     await dst_pool.execute("SET extra_float_digits TO 0;")
 
     has_run = False
     for table in set(pkeys):
         # If specific table list is defined and the iterated table is not in that list, skip.
-        # Note that the pkeys tables returned from Postgres are all lowercased, so we need to
-        # map the passed conf tables to lowercase.
-        if tables and (table not in list(map(str.lower, tables))):
+        if tables and (table not in tables):
             continue
 
         has_run = True  # If this runs, we have at least one table to compare. We will use this flag to throw an error if no tables are found.
 
-        full_table_name = f"{schema}.{table}"
+        full_table_name = f'{schema}."{table}"'
 
         logger.debug(f"Validating table {full_table_name}...")
         order_by_pkeys = ",".join(pkeys_dict[table])
 
         src_rows = await src_pool.fetch(
             query.format(table=full_table_name, order_by_pkeys=order_by_pkeys)
         )
@@ -383,23 +381,17 @@
               AND n.nspname !~ '^pg_toast'
               AND n.nspname <> 'information_schema'
               AND n.nspname <> 'pglogical'
         ORDER BY 1,2;"""
     )
 
     # We filter the table list if the user has specified a list of tables to target.
-    # Note, from issue #420, the above query will return the table names in lowercase,
-    # so we need to map the target_tables to lowercase.
     if target_tables:
 
-        result["tables"] = [
-            t
-            for t in result["tables"]
-            if t["Name"] in list(map(str.lower, target_tables))
-        ]
+        result["tables"] = [t for t in result["tables"] if t["Name"] in target_tables]
 
         # We will not recapitalize the table names in the result["tables"] list,
         # to preserve how Postgres sees those tables in its system catalog. Easy
         # rabbit hole later if we keep patching the table names to match the user's
         # input.
 
     result["sequences"] = await pool.fetch(
@@ -415,22 +407,18 @@
               AND n.nspname !~ '^pg_toast'
               AND n.nspname <> 'information_schema'
               AND n.nspname <> 'pglogical'
         ORDER BY 1,2;"""
     )
 
     # We filter the table list if the user has specified a list of tables to target.
-    # Note, from issue #420, the above query will return the table names in lowercase,
-    # so we need to map the target_tables to lowercase.
     if target_sequences:
 
         result["sequences"] = [
-            t
-            for t in result["sequences"]
-            if t["Name"] in list(map(str.lower, target_sequences))
+            t for t in result["sequences"] if t["Name"] in target_sequences
         ]
 
         # We will not recapitalize the table names in the result["tables"] list,
         # to preserve how Postgres sees those tables in its system catalog. Easy
         # rabbit hole later if we keep patching the table names to match the user's
         # input.
 
@@ -481,26 +469,26 @@
     logger.info("Getting the targeted dataset size...")
 
     # Tables string must be of form "'table1', 'table2', ..."
     tables_string = ", ".join([f"'{t}'" for t in tables])
 
     query = f"""
     SELECT
-        sum(pg_total_relation_size(schemaname || '.' || tablename)) AS total_relation_size
+        sum(pg_total_relation_size(schemaname || '."' || tablename || '"')) AS total_relation_size
     FROM
         pg_tables
     WHERE
         schemaname = '{schema}'
     AND tablename IN ({tables_string});
     """
 
     # Yes it's a duplicate, but it's a pretty one. Rather let Postgres do this than Python.
     pretty_query = f"""
     SELECT
-        pg_size_pretty(sum(pg_total_relation_size(schemaname || '.' || tablename))) AS total_relation_size
+        pg_size_pretty(sum(pg_total_relation_size(schemaname || '."' || tablename || '"'))) AS total_relation_size
     FROM
         pg_tables
     WHERE
         schemaname = '{schema}'
     AND tablename IN ({tables_string});
     """
```

### Comparing `pgbelt-0.7.2/pyproject.toml` & `pgbelt-0.7.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,48 +1,48 @@
 [tool.poetry]
 name = "pgbelt"
-version = "0.7.2"
+version = "0.7.3"
 description = "A CLI tool used to manage Postgres data migrations from beginning to end, for a single database or a fleet, leveraging pglogical replication."
 authors = ["Varjitt Jeeva <varjitt.jeeva@autodesk.com>"]
 readme = "README.md"
 
 packages = [
     { include = "pgbelt", from = "./" },
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 aiofiles = ">=0.8,<23.3"
 asyncpg = ">=0.27,<0.30"
 pydantic = ">=2.0,<3.0"
 tabulate = "^0.9.0"
-typer = "^0.9.0"
+typer = ">=0.9,<0.13"
 
 [tool.poetry.dev-dependencies]
 black = "~24.3.0"
-pre-commit = "~3.6.2"
+pre-commit = "~3.7.0"
 flake8 = "^7.0.0"
-pytest-cov = "~4.1.0"
+pytest-cov = "~5.0.0"
 pytest = "^8.1.1"
 coverage = {extras = ["toml"], version = "^7.4"}
-safety = "^2.3.1"
+safety = "^3.1.0"
 mypy = "^1.9"
 xdoctest = {extras = ["colors"], version = "^1.1.3"}
 flake8-bandit = "~4.1.1"
 flake8-bugbear = ">=21.9.2"
 flake8-docstrings = "^1.6.0"
 flake8-rst-docstrings = "^0.3.0"
 pep8-naming = "^0.13.2"
 darglint = "^1.8.1"
 reorder-python-imports = "^3.9.0"
 pre-commit-hooks = "^4.5.0"
 Pygments = "^2.17.2"
-pyupgrade = "^3.15.1"
+pyupgrade = "^3.15.2"
 pylint = "^3.1.0"
-pytest-asyncio = "~0.23.5"
+pytest-asyncio = "~0.23.6"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "setuptools"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 belt = "pgbelt.main:app"
```

### Comparing `pgbelt-0.7.2/PKG-INFO` & `pgbelt-0.7.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: pgbelt
-Version: 0.7.2
+Version: 0.7.3
 Summary: A CLI tool used to manage Postgres data migrations from beginning to end, for a single database or a fleet, leveraging pglogical replication.
 Author: Varjitt Jeeva
 Author-email: varjitt.jeeva@autodesk.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiofiles (>=0.8,<23.3)
 Requires-Dist: asyncpg (>=0.27,<0.30)
 Requires-Dist: pydantic (>=2.0,<3.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
-Requires-Dist: typer (>=0.9.0,<0.10.0)
+Requires-Dist: typer (>=0.9,<0.13)
 Description-Content-Type: text/markdown
 
 # Pgbelt
 
 <p align="center">
     <img src="https://github.com/Autodesk/pgbelt/blob/main/pgbelt.png?raw=true" width="400">
 </p>
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: pgbelt Version: 0.7.2 Summary: A CLI tool used to
+Metadata-Version: 2.1 Name: pgbelt Version: 0.7.3 Summary: A CLI tool used to
 manage Postgres data migrations from beginning to end, for a single database or
 a fleet, leveraging pglogical replication. Author: Varjitt Jeeva Author-email:
 varjitt.jeeva@autodesk.com Requires-Python: >=3.9,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiofiles (>=0.8,<23.3) Requires-Dist: asyncpg (>=0.27,<0.30)
 Requires-Dist: pydantic (>=2.0,<3.0) Requires-Dist: tabulate (>=0.9.0,<0.10.0)
-Requires-Dist: typer (>=0.9.0,<0.10.0) Description-Content-Type: text/markdown
-# Pgbelt
+Requires-Dist: typer (>=0.9,<0.13) Description-Content-Type: text/markdown #
+Pgbelt
       [https://github.com/Autodesk/pgbelt/blob/main/pgbelt.png?raw=true]
  _[_L_a_t_e_s_t_ _C_o_m_m_i_t_][https://github.com/Autodesk/pgbelt/actions/workflows/ci.yml/
        badge.svg]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_l_i_c_e_n_s_e_/_A_u_t_o_d_e_s_k_/_p_g_b_e_l_t_]
 PgBelt is a CLI tool used to manage Postgres data migrations from beginning to
 end, for a single database or a fleet, leveraging pglogical replication. It was
 built to assist in migrating data between postgres databases with as little
 application downtime as possible. It works in databases running different
```

