# Comparing `tmp/lumacli-0.0.9.tar.gz` & `tmp/lumacli-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumacli-0.0.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lumacli-0.1.0.tar", max compression
```

## Comparing `lumacli-0.0.9.tar` & `lumacli-0.1.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0      821 2023-08-10 09:26:14.173602 lumacli-0.0.9/.github/workflows/publish_to_pypi.yml
--rw-r--r--   0        0        0     3166 2023-08-10 09:26:14.173602 lumacli-0.0.9/.gitignore
--rw-r--r--   0        0        0     1064 2023-08-10 09:26:14.173602 lumacli-0.0.9/LICENSE
--rw-r--r--   0        0        0     4331 2023-08-10 09:26:14.173602 lumacli-0.0.9/README.md
--rw-r--r--   0        0        0      502 2023-08-10 09:26:14.173602 lumacli-0.0.9/lumaCLI/__init__.py
--rw-r--r--   0        0        0     3319 2023-08-10 09:26:14.173602 lumacli-0.0.9/lumaCLI/common.py
--rw-r--r--   0        0        0     1094 2023-08-10 09:26:14.173602 lumacli-0.0.9/lumaCLI/config.py
--rw-r--r--   0        0        0     4868 2023-08-10 09:26:14.173602 lumacli-0.0.9/lumaCLI/dbt.py
--rw-r--r--   0        0        0     1030 2023-08-10 09:26:14.173602 lumacli-0.0.9/lumaCLI/luma.py
--rw-r--r--   0        0        0       98 2023-08-10 09:26:14.173602 lumacli-0.0.9/lumaCLI/models/__init__.py
--rw-r--r--   0        0        0     6818 2023-08-10 09:26:14.173602 lumacli-0.0.9/lumaCLI/models/config_info.py
--rw-r--r--   0        0        0      942 2023-08-10 09:26:14.173602 lumacli-0.0.9/lumaCLI/models/request_info.py
--rw-r--r--   0        0        0     1905 2023-08-10 09:26:14.173602 lumacli-0.0.9/lumaCLI/postgres.py
--rw-r--r--   0        0        0        0 2023-08-10 09:26:14.173602 lumacli-0.0.9/lumaCLI/tests/__init__.py
--rw-r--r--   0        0        0     6531 2023-08-10 09:26:14.173602 lumacli-0.0.9/lumaCLI/tests/conftest.py
--rw-r--r--   0        0        0     8087 2023-08-10 09:26:14.173602 lumacli-0.0.9/lumaCLI/tests/metadata_dir/catalog.json
--rw-r--r--   0        0        0        0 2023-08-10 09:26:14.173602 lumacli-0.0.9/lumaCLI/tests/metadata_dir/file.txt
--rw-r--r--   0        0        0      260 2023-08-10 09:26:14.173602 lumacli-0.0.9/lumaCLI/tests/metadata_dir/invalid_json.json
--rw-r--r--   0        0        0   173474 2023-08-10 09:26:14.177602 lumacli-0.0.9/lumaCLI/tests/metadata_dir/manifest.json
--rw-r--r--   0        0        0     5109 2023-08-10 09:26:14.177602 lumacli-0.0.9/lumaCLI/tests/metadata_dir/postgres_dump_file.sql
--rw-r--r--   0        0        0    10271 2023-08-10 09:26:14.177602 lumacli-0.0.9/lumaCLI/tests/metadata_dir/run_results.json
--rw-r--r--   0        0        0     9716 2023-08-10 09:26:14.177602 lumacli-0.0.9/lumaCLI/tests/metadata_dir/sources.json
--rw-r--r--   0        0        0       90 2023-08-10 09:26:14.177602 lumacli-0.0.9/lumaCLI/tests/requirements.txt
--rw-r--r--   0        0        0     1904 2023-08-10 09:26:14.177602 lumacli-0.0.9/lumaCLI/tests/test_config.py
--rw-r--r--   0        0        0      743 2023-08-10 09:26:14.177602 lumacli-0.0.9/lumaCLI/tests/test_dbt.py
--rw-r--r--   0        0        0      695 2023-08-10 09:26:14.177602 lumacli-0.0.9/lumaCLI/tests/test_postgres.py
--rw-r--r--   0        0        0     3002 2023-08-10 09:26:14.177602 lumacli-0.0.9/lumaCLI/tests/test_postgres_utils.py
--rw-r--r--   0        0        0      526 2023-08-10 09:26:14.177602 lumacli-0.0.9/lumaCLI/tests/utils.py
--rw-r--r--   0        0        0      421 2023-08-10 09:26:14.177602 lumacli-0.0.9/lumaCLI/utils/__init__.py
--rw-r--r--   0        0        0     1644 2023-08-10 09:26:14.177602 lumacli-0.0.9/lumaCLI/utils/dbt_utils.py
--rw-r--r--   0        0        0     6031 2023-08-10 09:26:14.177602 lumacli-0.0.9/lumaCLI/utils/luma_utils.py
--rw-r--r--   0        0        0     7945 2023-08-10 09:26:14.177602 lumacli-0.0.9/lumaCLI/utils/postgres_utils.py
--rw-r--r--   0        0        0     1372 2023-08-10 09:26:14.177602 lumacli-0.0.9/playground.py
--rw-r--r--   0        0        0     1072 2023-08-10 09:26:14.177602 lumacli-0.0.9/pyproject.toml
--rw-r--r--   0        0        0     5119 1970-01-01 00:00:00.000000 lumacli-0.0.9/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-02 09:33:57.828337 lumacli-0.1.0/LICENSE
+-rw-r--r--   0        0        0      399 2024-04-02 09:33:57.828337 lumacli-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2024-04-02 09:33:57.832337 lumacli-0.1.0/lumaCLI/__init__.py
+-rw-r--r--   0        0        0     2618 2024-04-02 09:33:57.832337 lumacli-0.1.0/lumaCLI/commands/config.py
+-rw-r--r--   0        0        0     6352 2024-04-02 09:33:57.832337 lumacli-0.1.0/lumaCLI/commands/dbt.py
+-rw-r--r--   0        0        0     2177 2024-04-02 09:33:57.832337 lumacli-0.1.0/lumaCLI/commands/postgres.py
+-rw-r--r--   0        0        0     2505 2024-04-02 09:33:57.832337 lumacli-0.1.0/lumaCLI/main.py
+-rw-r--r--   0        0        0       98 2024-04-02 09:33:57.832337 lumacli-0.1.0/lumaCLI/models/__init__.py
+-rw-r--r--   0        0        0     8892 2024-04-02 09:33:57.832337 lumacli-0.1.0/lumaCLI/models/config_info.py
+-rw-r--r--   0        0        0     7922 2024-04-02 09:33:57.832337 lumacli-0.1.0/lumaCLI/models/dbt.py
+-rw-r--r--   0        0        0     2047 2024-04-02 09:33:57.832337 lumacli-0.1.0/lumaCLI/models/request_info.py
+-rw-r--r--   0        0        0        0 2024-04-02 09:33:57.832337 lumacli-0.1.0/lumaCLI/tests/__init__.py
+-rw-r--r--   0        0        0     8087 2024-04-02 09:33:57.832337 lumacli-0.1.0/lumaCLI/tests/assets/dbt_v1.3/catalog.json
+-rw-r--r--   0        0        0      260 2024-04-02 09:33:57.832337 lumacli-0.1.0/lumaCLI/tests/assets/dbt_v1.3/invalid_json.json
+-rw-r--r--   0        0        0   173474 2024-04-02 09:33:57.832337 lumacli-0.1.0/lumaCLI/tests/assets/dbt_v1.3/manifest.json
+-rw-r--r--   0        0        0    10271 2024-04-02 09:33:57.832337 lumacli-0.1.0/lumaCLI/tests/assets/dbt_v1.3/run_results.json
+-rw-r--r--   0        0        0     9716 2024-04-02 09:33:57.832337 lumacli-0.1.0/lumaCLI/tests/assets/dbt_v1.3/sources.json
+-rw-r--r--   0        0        0        0 2024-04-02 09:33:57.832337 lumacli-0.1.0/lumaCLI/tests/assets/dbt_v1.3/test_non_json_file.txt
+-rw-r--r--   0        0        0     6277 2024-04-02 09:33:57.832337 lumacli-0.1.0/lumaCLI/tests/assets/dbt_v1.7/model_metadata/catalog.json
+-rw-r--r--   0        0        0  1063666 2024-04-02 09:33:57.836337 lumacli-0.1.0/lumaCLI/tests/assets/dbt_v1.7/model_metadata/manifest.json
+-rw-r--r--   0        0        0     2002 2024-04-02 09:33:57.836337 lumacli-0.1.0/lumaCLI/tests/assets/dbt_v1.7/model_run_metadata/run_results.json
+-rw-r--r--   0        0        0     6811 2024-04-02 09:33:57.836337 lumacli-0.1.0/lumaCLI/tests/conftest.py
+-rw-r--r--   0        0        0      441 2024-04-02 09:33:57.836337 lumacli-0.1.0/lumaCLI/tests/integration/test_dbt.py
+-rw-r--r--   0        0        0      319 2024-04-02 09:33:57.836337 lumacli-0.1.0/lumaCLI/tests/integration/test_luma.py
+-rw-r--r--   0        0        0     5109 2024-04-02 09:33:57.836337 lumacli-0.1.0/lumaCLI/tests/postgres_dump_file.sql
+-rw-r--r--   0        0        0       90 2024-04-02 09:33:57.836337 lumacli-0.1.0/lumaCLI/tests/requirements.txt
+-rw-r--r--   0        0        0     2524 2024-04-02 09:33:57.836337 lumacli-0.1.0/lumaCLI/tests/unit/test_config.py
+-rw-r--r--   0        0        0     3752 2024-04-02 09:33:57.836337 lumacli-0.1.0/lumaCLI/tests/unit/test_dbt.py
+-rw-r--r--   0        0        0     1208 2024-04-02 09:33:57.836337 lumacli-0.1.0/lumaCLI/tests/unit/test_postgres.py
+-rw-r--r--   0        0        0     4258 2024-04-02 09:33:57.836337 lumacli-0.1.0/lumaCLI/tests/unit/test_postgres_utils.py
+-rw-r--r--   0        0        0      478 2024-04-02 09:33:57.836337 lumacli-0.1.0/lumaCLI/utils/__init__.py
+-rw-r--r--   0        0        0    15023 2024-04-02 09:33:57.836337 lumacli-0.1.0/lumaCLI/utils/luma_utils.py
+-rw-r--r--   0        0        0     4177 2024-04-02 09:33:57.836337 lumacli-0.1.0/lumaCLI/utils/options.py
+-rw-r--r--   0        0        0    10546 2024-04-02 09:33:57.836337 lumacli-0.1.0/lumaCLI/utils/postgres_utils.py
+-rw-r--r--   0        0        0     1606 2024-04-02 09:33:57.836337 lumacli-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1397 1970-01-01 00:00:00.000000 lumacli-0.1.0/PKG-INFO
```

### Comparing `lumacli-0.0.9/LICENSE` & `lumacli-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.9/lumaCLI/common.py` & `lumacli-0.1.0/lumaCLI/utils/options.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,97 +1,128 @@
-import typer
 import os
+from importlib.metadata import version
 from pathlib import Path
-from rich.panel import Panel
+
+import typer
 from rich import print
-from importlib.metadata import version
+from rich.panel import Panel
+from typing_extensions import Annotated
 
 CLI_NAME = "luma"
-# Get version
 __version__ = version("lumaCLI")
 
 
 # Utility functions
 def get_current_working_directory(metadata_dir, ctx: typer.Context) -> Path:
+    """
+    Returns the current working directory if 'metadata_dir' is not specified.
+    If 'metadata_dir' is provided, it returns the specified directory.
+
+    Args:
+    - metadata_dir: Path to the metadata directory.
+    - ctx: Context of the current Typer command execution.
+
+    Returns:
+    - Path: The current working directory or the specified metadata directory.
+    """
     # Returns current working directory if metadata_dir is not specified
     if ctx.resilient_parsing:
         return
     if metadata_dir is not None:
         return metadata_dir
     cwd = Path(os.getcwd())
     print(
         Panel(
             f"[yellow]'metadata_dir' not specified, using current working directory {cwd}[/yellow]"
         )
     )
     return cwd
 
 
-def get_config_dir(config_dir, ctx: typer.Context) -> Path:
-    if ctx.resilient_parsing:
-        return
-    if config_dir is not None:
-        return config_dir
-
-    config_dir = Path(typer.get_app_dir(CLI_NAME, force_posix=True))
-    return config_dir
-
-
 # Callback functions
 def require_if_not_dry_run(value, param: typer.CallbackParam, ctx: typer.Context):
+    """
+    Ensures that the given value is required if the 'dry_run' flag is not set.
+
+    Args:
+    - value: The value to be checked.
+    - param: The parameter associated with the value.
+    - ctx: Context of the current Typer command execution.
+
+    Returns:
+    - str: The validated value if the conditions are met.
+
+    Raises:
+    - typer.BadParameter: If the value is missing and 'dry_run' is not enabled.
+    """
     if ctx.resilient_parsing:
         return
     dry_run = ctx.params.get("dry_run", False)
 
     if value or dry_run:
         return value
 
     # Raise a typer.BadParameter exception to simulate the same error as missing 'endpoint'
     raise typer.BadParameter(f"Missing argument '{param.name.upper()}'")
 
 
-# Create command line optionss
+# Command Line Options
+
 MetadataDir: Path = typer.Option(
     None,
     "--metadata-dir",
     "-m",
     help="Specify the directory with dbt metadata files. Defaults to current working directory if not provided.",
     callback=get_current_working_directory,
     exists=True,
     dir_okay=True,
     resolve_path=True,
 )
 ConfigDir: Path = typer.Option(
-    None,
+    "./.luma",
     "--config-dir",
     "-c",
-    help="Specify the directory with the config files. Defaults to ~/.luma",
-    callback=get_config_dir,
-    exists=True,
+    help="Specify the directory with the config files. Defaults to ./.luma",
+    envvar="LUMA_CONFIG_DIR",
     dir_okay=True,
     resolve_path=True,
 )
+Force: bool = typer.Option(
+    False,
+    "--force",
+    "-f",
+    help="Force the operation.",
+)
 
 DryRun: bool = typer.Option(
     False,
     "--dry-run",
     "-D",
+    is_flag=True,
     help="Perform a dry run. Print the payload but do not send it.",
 )
+
 NoConfig: bool = typer.Option(
     False,
     "--no-config",
     "-n",
     help="Set this flag to prevent sending configuration data along with the request.",
 )
+
+Follow: bool = typer.Option(
+    False, "--follow", help="Follow the ingestion process until it's completed."
+)
+
+IngestionId = Annotated[str, typer.Argument(help="Ingestion UUID.")]
+
 LumaURL: str = typer.Option(
     None,
     "--luma-url",
     "-l",
-    help="URL of the luma instance",
+    help="URL of the luma instance.",
     envvar="LUMA_URL",
     callback=require_if_not_dry_run,
 )
 PostgresUsername: str = typer.Option(
     ...,
     "--username",
     "-u",
```

### Comparing `lumacli-0.0.9/lumaCLI/models/config_info.py` & `lumacli-0.1.0/lumaCLI/models/config_info.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from typing import List, Optional
+
 from pydantic import BaseModel, EmailStr, root_validator, validator
 
+
 allowed_icons = (
     "AcademicCap",
     "AdjustmentsHorizontal",
     "AdjustmentsVertical",
     "ArchiveBox",
     "ArchiveBoxArrowDown",
     "ArchiveBoxXMark",
@@ -294,40 +296,102 @@
     "WrenchScrewdriver",
     "XCircle",
     "XMark",
 )
 
 
 class Group(BaseModel):
+    """Represents a group with metadata, slug, labels, and an optional icon.
+
+    Attributes:
+        meta_key (str): A key for metadata associated with the group.
+        slug (str): A slug for the group, used in URLs or as an identifier.
+        label_plural (str): The plural label for the group.
+        label_singular (str): The singular label for the group.
+        icon (Optional[str]): An optional icon for the group. Must be one of the allowed
+            icons.
+        in_sidebar (bool, optional): Whether the group should be displayed in the
+            sidebar.
+
+    Methods:
+        icon_validator: Validates that the provided icon (if any) is in the allowed set.
+    """
+
     meta_key: str
     slug: str
     label_plural: str
     label_singular: str
     icon: Optional[str]
+    in_sidebar: Optional[bool] = True
 
     @validator("icon")
     def icon_validator(cls, v):
+        """Validates the icon attribute.
+
+        Ensures that if an icon is provided, it is one of the pre-approved icons.
+
+        Args:
+            v (str): The icon to validate.
+
+        Returns:
+            str: The validated icon.
+
+        Raises:
+            ValueError: If the icon is not in the allowed set.
+        """
         if v is not None and v not in allowed_icons:
             raise ValueError("Icon is not one of the allowed options")
         return v
 
 
 class Owner(BaseModel):
+    """Represents an owner with email, name, and title.
+
+    Attributes:
+        email (EmailStr): The email address of the owner.
+        first_name (str): The first name of the owner.
+        last_name (str): The last name of the owner.
+        title (str): The title of the owner.
+    """
+
     email: EmailStr
     first_name: str
     last_name: str
     title: str
 
 
 class Config(BaseModel):
+    """Configuration model holding information about groups and owners.
+
+    Attributes:
+        groups (Optional[List[Group]]): A list of Group objects. Ensures uniqueness of
+            meta_keys and slugs among groups.
+        owners (Optional[List[Owner]]): A list of Owner objects.
+
+    Methods:
+        validate_unique: Validates the uniqueness of meta_keys and slugs within the
+            groups.
+    """
+
     groups: Optional[List[Group]]
     owners: Optional[List[Owner]]
 
     @root_validator
     def validate_unique(cls, values):
+        """Validates the uniqueness of 'meta_key' and 'slug' for each group.
+
+        Args:
+            values (dict): The values to validate.
+
+        Returns:
+            dict: The validated values.
+
+        Raises:
+            ValueError: If 'meta_key' or 'slug' is not unique across all groups.
+        """
         groups = values.get("groups")
         if groups:
             # Check for unique meta_key
             meta_keys = {group.meta_key for group in groups}
             if len(meta_keys) != len(groups):
                 raise ValueError("meta_key must be unique for each group")
```

### Comparing `lumacli-0.0.9/lumaCLI/models/request_info.py` & `lumacli-0.1.0/lumaCLI/models/request_info.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,35 +1,68 @@
 from enum import Enum
 from typing import Dict, Optional, Tuple, Union
 
 from pydantic import AnyHttpUrl, BaseModel, validator
 
 
 class HttpMethod(str, Enum):
+    """
+    Enumeration for HTTP methods.
+    """
     GET = "GET"
     POST = "POST"
     PUT = "PUT"
     DELETE = "DELETE"
     HEAD = "HEAD"
     OPTIONS = "OPTIONS"
     PATCH = "PATCH"
 
 
 class RequestInfo(BaseModel):
+    """
+    Information about an HTTP request.
+
+    Attributes:
+        url (AnyHttpUrl): The URL for the request.
+        payload (Optional[Union[Dict, list]]): The payload for the request, if any.
+        verify (bool): Whether to verify the server's TLS certificate.
+        method (HttpMethod): The HTTP method for the request. Defaults to POST.
+        timeout (Optional[Union[float, Tuple[float, float], Tuple[float, None]]]): The timeout for the request.
+        headers (Optional[Dict[str, str]]): Headers to be sent with the request.
+        params (Optional[Dict[str, Union[str, int, float]]]): URL parameters for the request.
+    """
     url: AnyHttpUrl
     payload: Optional[Union[Dict, list]]
     verify: bool = True
     method: HttpMethod = HttpMethod.POST
     timeout: Optional[Union[float, Tuple[float, float], Tuple[float, None]]] = (
-        3.05,
+        20,
         60 * 30,
     )
     headers: Optional[Dict[str, str]] = None
     params: Optional[Dict[str, Union[str, int, float]]] = None
 
     @validator("headers", pre=True, always=True)
     def set_default_headers(cls, v):
+        """
+        Ensures that default headers are set if none are provided.
+
+        Args:
+            v: The value of the headers.
+
+        Returns:
+            The headers with a default if none were provided.
+        """
         return v or {"Content-Type": "application/json"}
 
     @validator("method", pre=True)
     def uppercase_method(cls, v):
+        """
+        Ensures that the HTTP method is in uppercase.
+
+        Args:
+            v: The HTTP method.
+
+        Returns:
+            The HTTP method in uppercase.
+        """
         return v.upper() if isinstance(v, str) else v
```

### Comparing `lumacli-0.0.9/lumaCLI/postgres.py` & `lumacli-0.1.0/lumaCLI/commands/postgres.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,52 +1,60 @@
-import typer
+from pathlib import Path
 from typing import Dict, List
 
+import typer
 from rich import print
+from rich.panel import Panel
 
 from lumaCLI.models import Config, RequestInfo
-from lumaCLI.utils import (
-    get_db_metadata,
-    get_config,
-    send_config,
-    send_request_info,
-)
-from lumaCLI.common import (
-    LumaURL,
+from lumaCLI.utils import get_config, get_db_metadata, send_config, perform_request
+from lumaCLI.utils.options import (
+    ConfigDir,
     DryRun,
+    LumaURL,
     NoConfig,
-    PostgresUsername,
     PostgresDatabase,
     PostgresHost,
-    PostgresPort,
     PostgresPassword,
+    PostgresPort,
+    PostgresUsername,
 )
 
 app = typer.Typer(no_args_is_help=True, pretty_exceptions_show_locals=False)
 
 
 @app.command()
 def ingest(
     luma_url: str = LumaURL,
     username: str = PostgresUsername,
     database: str = PostgresDatabase,
     host: str = PostgresHost,
     port: str = PostgresPort,
     password: str = PostgresPassword,
     dry_run: bool = DryRun,
+    config_dir: Path = ConfigDir,
     no_config: bool = NoConfig,
 ) -> RequestInfo:
     """
-    Sends metadata from a PostgreSQL database to a Luma ingestion endpoint.
-    If 'endpoint' is not specified, it will auto-generate from the '.luma/config.yaml' file.
+    Ingests metadata from a PostgreSQL database and sends it to a specified Luma ingestion endpoint.
     """
 
-    # get_config
-    config: Config = get_config()
     should_send_config = not no_config
+    config = None
+    # get_config
+
+    if should_send_config:
+        try:
+            config: Config = get_config(config_dir=config_dir)
+        except FileNotFoundError:
+            print(
+                Panel(
+                    f"[blue]No config files found. Continuing with the operation...[/blue]"
+                )
+            )
 
     # Retrieve database metadata
     db_metadata: Dict[str, List[Dict]] = get_db_metadata(
         username=username, database=database, host=host, port=port, password=password
     )
 
     # In dry run mode, print the database metadata and exit
@@ -58,20 +66,19 @@
 
     # Create the request info object to return
     request_info = RequestInfo(
         url=endpoint,
         method="POST",
         payload=db_metadata,
         verify=False,
-        timeout=(3.05, 60 * 30),
     )
     if config and should_send_config:
         config_response = send_config(config=config, luma_url=luma_url)
 
-    response = send_request_info(request_info)
+    response = perform_request(request_info)
     if not response.ok:
         raise typer.Exit(1)
 
     return response
 
 
 if __name__ == "__main__":
```

### Comparing `lumacli-0.0.9/lumaCLI/tests/conftest.py` & `lumacli-0.1.0/lumaCLI/tests/conftest.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-### CLIENT
 import socket
-import uvicorn
-import multiprocessing
-import pytest
-from fastapi import FastAPI, HTTPException
 from pathlib import Path
 from time import sleep
-from lumaCLI.tests.utils import LUMA_CONFIG_DIR, INVALID_SCHEMA_LUMA_CONFIG_DIR
 
-## Create FastAPI app to make requests to
+import multiprocess
+import psycopg2
+import pytest
+import uvicorn
+from fastapi import FastAPI, HTTPException
+from pytest_postgresql import factories
+
 app = FastAPI()
 
 
 @app.post("/api/v1/dbt")
 async def dbt(body: dict):
     if body is None:
         raise HTTPException(400)
@@ -45,56 +45,53 @@
         s.bind(("", 0))
         return s.getsockname()[1]
 
 
 @pytest.fixture(scope="module")
 def test_server():
     port = find_free_port()
-    server = multiprocessing.Process(
+    server = multiprocess.Process(
         target=uvicorn.run,
         args=(app,),
         kwargs={"host": "0.0.0.0", "port": port},
         daemon=True,
     )
     server.start()
     sleep(1)  # Time to wait while the server starts up
     yield f"http://0.0.0.0:{port}"
     server.terminate()
 
 
 @pytest.fixture(scope="module")
-def config_dir():
+def config_dir(LUMA_CONFIG_DIR):
     config_dir = Path(LUMA_CONFIG_DIR)
     config_path = config_dir / "config.yaml"
     owners_path = config_dir / "owners.yaml"
 
     config_dir.mkdir(exist_ok=True)
     config_path.touch()
     with config_path.open("w") as f:
         f.write(
             """groups:
   - meta_key: "domain"
     slug: "domains"
     label_plural: "Domains"
     label_singular: "Domain"
     icon: "Cube"
+    in_sidebar: true
   - meta_key: "true_source"
     slug: "sources"
     label_plural: "Sources"
     label_singular: "Source"
     icon: "Cloud"
-colors:
-  - name: "red"
-    emotion: "anger"
-  - name: "purple"
-    emotion: "sadness"
+    in_sidebar: false
 """
         )
     owners_path.touch()
-    with config_path.open("w") as f:
+    with owners_path.open("w") as f:
         f.write(
             """owners:
 - email: "some@one.com"
   first_name: "Dave"
   last_name: "Smith"
   title: "Director"
 - email: "other@person.com"
@@ -111,15 +108,15 @@
 
     config_path.unlink()
     owners_path.unlink()
     config_dir.rmdir()
 
 
 @pytest.fixture(scope="module")
-def config_dir_invalid_schema():
+def config_dir_invalid_schema(INVALID_SCHEMA_LUMA_CONFIG_DIR):
     config_dir = Path(INVALID_SCHEMA_LUMA_CONFIG_DIR)
     config_path = config_dir / "config.yaml"
     owners_path = config_dir / "owners.yaml"
 
     config_dir.mkdir(exist_ok=True)
     config_path.touch()
     with config_path.open("w") as f:
@@ -131,19 +128,14 @@
     label_singular: "Domain"
     icon: "Cube"
   - meta_key: ["true_source"]
     slug: "sources"
     label_plural: "Sources"
     label_singular: "Source"
     icon: "Cloud"
-colors:
-  - name: ["red"]
-    emotion: "anger"
-  - name: "purple"
-    emotion: "sadness"
 """
         )
     owners_path.touch()
     with config_path.open("w") as f:
         f.write(
             """owners:
 - email: "some@one.com"
@@ -162,19 +154,14 @@
         )
     yield config_dir
     config_path.unlink()
     owners_path.unlink()
     config_dir.rmdir()
 
 
-### DATABASE
-import psycopg2
-import pytest
-from pytest_postgresql import factories
-
 # This fixture creates a Postgres database
 postgresql_proc = factories.postgresql_proc(port=find_free_port())
 postgresql = factories.postgresql("postgresql_proc")
 
 
 @pytest.fixture(scope="function")
 def setup_db(postgresql):
@@ -256,7 +243,32 @@
 
     # Closing connection
     conn.commit()
     cur.close()
     conn.close()
 
     return postgresql
+
+
+@pytest.fixture(scope="module")
+def TESTS_DIR():
+    return Path(__file__).parent
+
+
+@pytest.fixture(scope="module")
+def METADATA_DIR_V1_3(TESTS_DIR):
+    return TESTS_DIR / "assets" / "dbt_v1.3"
+
+
+@pytest.fixture(scope="module")
+def METADATA_DIR_V1_7(TESTS_DIR):
+    return TESTS_DIR / "assets" / "dbt_v1.7"
+
+
+@pytest.fixture(scope="module")
+def INVALID_SCHEMA_LUMA_CONFIG_DIR(TESTS_DIR):
+    return TESTS_DIR / ".invalid_schema_luma"
+
+
+@pytest.fixture(scope="module")
+def LUMA_CONFIG_DIR(TESTS_DIR):
+    return TESTS_DIR / ".luma"
```

### Comparing `lumacli-0.0.9/lumaCLI/tests/metadata_dir/catalog.json` & `lumacli-0.1.0/lumaCLI/tests/assets/dbt_v1.3/catalog.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.9/lumaCLI/tests/metadata_dir/manifest.json` & `lumacli-0.1.0/lumaCLI/tests/assets/dbt_v1.3/manifest.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.9/lumaCLI/tests/metadata_dir/postgres_dump_file.sql` & `lumacli-0.1.0/lumaCLI/tests/postgres_dump_file.sql`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.9/lumaCLI/tests/metadata_dir/run_results.json` & `lumacli-0.1.0/lumaCLI/tests/assets/dbt_v1.3/run_results.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.9/lumaCLI/tests/metadata_dir/sources.json` & `lumacli-0.1.0/lumaCLI/tests/assets/dbt_v1.3/sources.json`

 * *Files identical despite different names*

### Comparing `lumacli-0.0.9/lumaCLI/tests/test_config.py` & `lumacli-0.1.0/lumaCLI/tests/unit/test_config.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,31 @@
-from lumaCLI import app
+import click
+from rich.console import Console
 from typer.testing import CliRunner
+
+from lumaCLI.main import app
 from lumaCLI.utils.luma_utils import get_config
-from rich.console import Console
-import yaml
-import click
 
 runner = CliRunner()
 
 
 def test_get_config(config_dir):
+    """
+    Test if the configuration is correctly retrieved from a given directory.
+    """
     config = get_config(config_dir=config_dir)
     assert config
+    assert config.groups is not None
+    assert config.owners is not None
 
 
 def test_show(config_dir):
+    """
+    Test if the 'show' command correctly displays the configuration.
+    """
     result = runner.invoke(
         app,
         [
             "config",
             "show",
             "--config-dir",
             config_dir,
@@ -29,33 +37,42 @@
     console = Console(record=True)
     console.print(config)
     text = console.export_text()
     assert text in result.output
 
 
 def test_send(config_dir, test_server):
+    """
+    Test if the 'send' command successfully sends the configuration.
+    """
     result = runner.invoke(
         app,
         ["config", "send", "--config-dir", config_dir, "--luma-url", test_server],
     )
 
     assert result.exit_code == 0
     assert "The request was successful!" in result.output
 
 
 # Invalid schema tests
 def test_get_config_invalid_schema(config_dir_invalid_schema):
+    """
+    Test if the configuration retrieval correctly handles an invalid schema.
+    """
     try:
         config = get_config(config_dir=config_dir_invalid_schema)
         assert config is None
     except click.exceptions.Abort:
         pass
 
 
 def test_show_invalid_schema(config_dir_invalid_schema):
+    """
+    Test if the 'show' command correctly handles an invalid configuration schema.
+    """
     result = runner.invoke(
         app,
         [
             "config",
             "show",
             "--config-dir",
             config_dir_invalid_schema,
@@ -63,14 +80,17 @@
     )
 
     assert result.exit_code == 1
     assert "Error parsing YAML file" in result.output
 
 
 def test_send_invalid_schema(config_dir_invalid_schema, test_server):
+    """
+    Test if the 'send' command correctly handles an invalid configuration schema.
+    """
     result = runner.invoke(
         app,
         [
             "config",
             "send",
             "--config-dir",
             config_dir_invalid_schema,
```

### Comparing `lumacli-0.0.9/lumaCLI/utils/postgres_utils.py` & `lumacli-0.1.0/lumaCLI/utils/postgres_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,76 @@
 import os
-import psycopg2
 import re
 from typing import Dict, List
 
+import psycopg2
 from rich.console import Console
 
 from lumaCLI.utils import run_command
 
-
 console = Console()
 
 
 def create_conn(username, password, host, port, database):
+    """
+    Create and return a new database connection using the given credentials.
+
+    Args:
+        username (str): Username for the database.
+        password (str): Password for the database.
+        host (str): Host address of the database.
+        port (str): Port number for the database connection.
+        database (str): Name of the database to connect to.
+
+    Returns:
+        psycopg2.extensions.connection: A new database connection.
+    """
     return psycopg2.connect(
         user=username, password=password, host=host, port=port, dbname=database
     )
 
 
 def generate_pg_dump_content(
     username: str,
     database: str,
     password: str,
     host: str = "localhost",
     port: str = "5432",
 ) -> str:
     """
-    Dump the specified PostgreSQL database schema information, table names,
-    column information, row counts, and other details to a dump file.
+    Generate a string dump of the PostgreSQL database schema, tables, and other details.
+
+    Args:
+        username (str): The username for the database.
+        database (str): The name of the database.
+        password (str): The password for the database.
+        host (str, optional): The host of the database. Defaults to "localhost".
+        port (str, optional): The port of the database. Defaults to "5432".
+
+    Returns:
+        str: The result of the pg_dump command as a string.
     """
     original_pgpassword_env = os.getenv("PGPASSWORD")
     os.environ["PGPASSWORD"] = password
     command = f"pg_dump -h {host} -p {port} -U {username} -d {database} --column-inserts --rows-per-insert=1 --no-password"
     result = run_command(command, capture_output=True)
     os.environ["PGPASSWORD"] = original_pgpassword_env
     return result
 
 
-def get_pg_dump_tables_info(content) -> List[Dict]:
+def get_pg_dump_tables_info(content: str) -> List[Dict]:
+    """
+    Extract table information from a PostgreSQL database dump content.
+
+    Args:
+        content (str): PostgreSQL database dump content as a string.
+
+    Returns:
+        List[Dict]: A list of dictionaries, each containing information about a table in the database.
+    """
     # Find table creation statements
     table_creations = re.findall(
         r"CREATE TABLE (.*?)\.(.*?) \((.*?)\);", content, re.DOTALL
     )
 
     # Find row counts and table sizes
     row_counts = re.findall(
@@ -130,15 +160,25 @@
                 "foreign_keys": foreign_keys_list,
             }
         )
 
     return tables_list
 
 
-def get_pg_dump_views_info(content) -> List[Dict]:
+def get_pg_dump_views_info(content: str) -> List[Dict]:
+    """
+    Extract view information from a PostgreSQL database dump content.
+
+    Args:
+        content (str): PostgreSQL database dump content as a string.
+
+    Returns:
+        List[Dict]: A list of dictionaries, each containing information about a view in the database.
+    """
+
     # Find view creation statements
     view_creations = re.findall(
         r"CREATE VIEW (.*?)\.(.*?) AS(.*?);", content, re.DOTALL
     )
 
     # Initialize the list for storing view information
     views_list = []
@@ -164,25 +204,28 @@
                 "columns": columns_dict,
             }
         )
 
     return views_list
 
 
-def get_tables_size_info(
-    username: str,
-    database: str,
-    password: str,
-    host: str = "localhost",
-    port: str = "5432",
-):
-    """
-    Get size information of the specified PostgreSQL database, tables, and indexes.
+def get_tables_size_info(username: str, database: str, password: str, host: str = "localhost", port: str = "5432") -> Dict:
     """
+    Retrieve size information for all tables in the specified PostgreSQL database.
 
+    Args:
+        username (str): Database username.
+        database (str): Database name.
+        password (str): Database password.
+        host (str, optional): Database host. Defaults to "localhost".
+        port (str, optional): Database port. Defaults to "5432".
+
+    Returns:
+        Dict: A dictionary where keys are table names and values are their respective sizes.
+    """
     conn = create_conn(username, password, host, port, database)
     cur = conn.cursor()
     cur.execute(
         """
         SELECT table_schema, 
                table_name,
                pg_size_pretty(pg_total_relation_size(('"' || table_schema || '"."' || table_name || '"'))) AS table_size
@@ -195,23 +238,27 @@
     table_size_dict = {}
 
     for table_schema, table_name, table_size in rows:
         table_size_dict[(table_schema, table_name)] = table_size
     return table_size_dict
 
 
-def get_tables_row_counts(
-    username: str,
-    database: str,
-    password: str,
-    host: str = "localhost",
-    port: str = "5432",
-):
+def get_tables_row_counts(username: str, database: str, password: str, host: str = "localhost", port: str = "5432") -> Dict:
     """
-    Get row counts for all tables in the specified PostgreSQL database.
+    Retrieve row counts for all tables in a specified PostgreSQL database.
+
+    Args:
+        username (str): Database username.
+        database (str): Database name.
+        password (str): Database password.
+        host (str, optional): Database host. Defaults to "localhost".
+        port (str, optional): Database port. Defaults to "5432".
+
+    Returns:
+        Dict: A dictionary where keys are table names and values are the number of rows in each table.
     """
     conn = create_conn(username, password, host, port, database)
     cur = conn.cursor()
     cur.execute(
         """
         SELECT schemaname,relname,n_live_tup 
         FROM pg_stat_user_tables 
@@ -222,21 +269,28 @@
     row_count_dict = {}
 
     for table_schema, table_name, row_count in rows:
         row_count_dict[(table_schema, table_name)] = row_count
     return row_count_dict
 
 
-def get_db_metadata(
-    username: str,
-    database: str,
-    password: str,
-    host: str = "localhost",
-    port: str = "5432",
-) -> Dict[str, List[Dict]]:
+def get_db_metadata(username: str, database: str, password: str, host: str = "localhost", port: str = "5432") -> Dict[str, List[Dict]]:
+    """
+    Gather comprehensive metadata about the specified PostgreSQL database, including tables and views.
+
+    Args:
+        username (str): Database username.
+        database (str): Database name.
+        password (str): Database password.
+        host (str, optional): Database host. Defaults to "localhost".
+        port (str, optional): Database port. Defaults to "5432".
+
+    Returns:
+        Dict[str, List[Dict]]: A dictionary containing metadata about tables and views in the database.
+    """
     dump_content: str = generate_pg_dump_content(
         username=username, database=database, host=host, port=port, password=password
     )
     # Transform SQL dump to dictionary
     tables_info: List[Dict] = get_pg_dump_tables_info(dump_content)
 
     # Get row count information
```

