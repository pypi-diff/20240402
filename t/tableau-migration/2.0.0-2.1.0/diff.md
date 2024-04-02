# Comparing `tmp/tableau_migration-2.0.0.tar.gz` & `tmp/tableau_migration-2.1.0.tar.gz`

## Comparing `tableau_migration-2.0.0.tar` & `tableau_migration-2.1.0.tar`

### file list

```diff
@@ -1,65 +1,65 @@
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/requirements.txt
--rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/__init__.py
--rw-r--r--   0        0        0     8648 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/migration.py
--rw-r--r--   0        0        0    18376 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/migration_engine.py
--rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/migration_engine_hooks.py
--rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/migration_engine_hooks_filters.py
--rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/migration_engine_hooks_mappings.py
--rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/migration_engine_hooks_transformers.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/migration_engine_migrators.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/migration_engine_options.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/migration_logger.py
--rw-r--r--   0        0        0    19104 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Bcl.AsyncInterfaces.dll
--rw-r--r--   0        0        0    32432 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Bcl.TimeProvider.dll
--rw-r--r--   0        0        0    34848 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.AmbientMetadata.Application.dll
--rw-r--r--   0        0        0    40488 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Compliance.Abstractions.dll
--rw-r--r--   0        0        0    29448 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.Abstractions.dll
--rw-r--r--   0        0        0    44808 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.Binder.dll
--rw-r--r--   0        0        0    23312 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.EnvironmentVariables.dll
--rw-r--r--   0        0        0    45328 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.dll
--rw-r--r--   0        0        0    63264 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.Abstractions.dll
--rw-r--r--   0        0        0    34224 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.AutoActivation.dll
--rw-r--r--   0        0        0    93984 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.dll
--rw-r--r--   0        0        0    41376 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.DiagnosticAdapter.dll
--rw-r--r--   0        0        0    32008 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.Abstractions.dll
--rw-r--r--   0        0        0    31152 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.ExceptionSummarization.dll
--rw-r--r--   0        0        0    37144 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.dll
--rw-r--r--   0        0        0    23728 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.FileProviders.Abstractions.dll
--rw-r--r--   0        0        0    53000 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Hosting.Abstractions.dll
--rw-r--r--   0        0        0   115248 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Http.Diagnostics.dll
--rw-r--r--   0        0        0   129056 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Http.Resilience.dll
--rw-r--r--   0        0        0    89368 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Http.dll
--rw-r--r--   0        0        0    21680 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Localization.Abstractions.dll
--rw-r--r--   0        0        0    33968 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Localization.dll
--rw-r--r--   0        0        0    66336 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Logging.Abstractions.dll
--rw-r--r--   0        0        0    29968 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Logging.Configuration.dll
--rw-r--r--   0        0        0    52496 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Logging.dll
--rw-r--r--   0        0        0    25264 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.ObjectPool.dll
--rw-r--r--   0        0        0    24336 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Options.ConfigurationExtensions.dll
--rw-r--r--   0        0        0    66312 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Options.dll
--rw-r--r--   0        0        0    45336 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Primitives.dll
--rw-r--r--   0        0        0    37936 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Resilience.dll
--rw-r--r--   0        0        0    55344 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Telemetry.Abstractions.dll
--rw-r--r--   0        0        0   116768 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Telemetry.dll
--rw-r--r--   0        0        0    65568 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.IO.RecyclableMemoryStream.dll
--rw-r--r--   0        0        0   242976 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Polly.Core.dll
--rw-r--r--   0        0        0    56736 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Polly.Extensions.dll
--rw-r--r--   0        0        0    29600 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Polly.RateLimiting.dll
--rw-r--r--   0        0        0   247584 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/System.Collections.Immutable.dll
--rw-r--r--   0        0        0   164616 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/System.Diagnostics.DiagnosticSource.dll
--rw-r--r--   0        0        0     6656 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/System.IO.Abstractions.dll
--rw-r--r--   0        0        0    71440 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/System.Text.Encodings.Web.dll
--rw-r--r--   0        0        0   579848 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/System.Text.Json.dll
--rw-r--r--   0        0        0    70416 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/System.Threading.RateLimiting.dll
--rw-r--r--   0        0        0    37426 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Tableau.Migration.deps.json
--rw-r--r--   0        0        0   980992 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Tableau.Migration.dll
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Tableau.Migration.runtimeconfig.json
--rw-r--r--   0        0        0  1071823 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/Tableau.Migration.xml
--rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/TestableIO.System.IO.Abstractions.Wrappers.dll
--rw-r--r--   0        0        0    29184 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/TestableIO.System.IO.Abstractions.dll
--rw-r--r--   0        0        0    71448 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/src/tableau_migration/bin/runtimes/browser/lib/net6.0/System.Text.Encodings.Web.dll
--rw-r--r--   0        0        0     3551 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/.gitignore
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/LICENSE
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/README.md
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 tableau_migration-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/requirements.txt
+-rw-r--r--   0        0        0     2247 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/__init__.py
+-rw-r--r--   0        0        0     8648 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/migration.py
+-rw-r--r--   0        0        0    18376 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/migration_engine.py
+-rw-r--r--   0        0        0     4275 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/migration_engine_hooks.py
+-rw-r--r--   0        0        0     3784 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/migration_engine_hooks_filters.py
+-rw-r--r--   0        0        0     3670 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/migration_engine_hooks_mappings.py
+-rw-r--r--   0        0        0     3713 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/migration_engine_hooks_transformers.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/migration_engine_migrators.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/migration_engine_options.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/migration_logger.py
+-rw-r--r--   0        0        0    19104 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Bcl.AsyncInterfaces.dll
+-rw-r--r--   0        0        0    32432 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Bcl.TimeProvider.dll
+-rw-r--r--   0        0        0    34848 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.AmbientMetadata.Application.dll
+-rw-r--r--   0        0        0    40488 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Compliance.Abstractions.dll
+-rw-r--r--   0        0        0    29448 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.Abstractions.dll
+-rw-r--r--   0        0        0    44808 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.Binder.dll
+-rw-r--r--   0        0        0    23312 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.EnvironmentVariables.dll
+-rw-r--r--   0        0        0    45328 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.dll
+-rw-r--r--   0        0        0    63264 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.Abstractions.dll
+-rw-r--r--   0        0        0    34224 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.AutoActivation.dll
+-rw-r--r--   0        0        0    93984 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.dll
+-rw-r--r--   0        0        0    41376 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.DiagnosticAdapter.dll
+-rw-r--r--   0        0        0    32008 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.Abstractions.dll
+-rw-r--r--   0        0        0    31152 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.ExceptionSummarization.dll
+-rw-r--r--   0        0        0    37144 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.dll
+-rw-r--r--   0        0        0    23728 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.FileProviders.Abstractions.dll
+-rw-r--r--   0        0        0    53000 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Hosting.Abstractions.dll
+-rw-r--r--   0        0        0   115248 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Http.Diagnostics.dll
+-rw-r--r--   0        0        0   129056 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Http.Resilience.dll
+-rw-r--r--   0        0        0    89368 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Http.dll
+-rw-r--r--   0        0        0    21680 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Localization.Abstractions.dll
+-rw-r--r--   0        0        0    33968 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Localization.dll
+-rw-r--r--   0        0        0    66336 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Logging.Abstractions.dll
+-rw-r--r--   0        0        0    29968 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Logging.Configuration.dll
+-rw-r--r--   0        0        0    52496 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Logging.dll
+-rw-r--r--   0        0        0    25264 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.ObjectPool.dll
+-rw-r--r--   0        0        0    24336 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Options.ConfigurationExtensions.dll
+-rw-r--r--   0        0        0    66312 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Options.dll
+-rw-r--r--   0        0        0    45336 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Primitives.dll
+-rw-r--r--   0        0        0    37936 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Resilience.dll
+-rw-r--r--   0        0        0    55344 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Telemetry.Abstractions.dll
+-rw-r--r--   0        0        0   116768 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Telemetry.dll
+-rw-r--r--   0        0        0    65568 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.IO.RecyclableMemoryStream.dll
+-rw-r--r--   0        0        0   242976 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Polly.Core.dll
+-rw-r--r--   0        0        0    56736 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Polly.Extensions.dll
+-rw-r--r--   0        0        0    29600 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Polly.RateLimiting.dll
+-rw-r--r--   0        0        0   247584 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/System.Collections.Immutable.dll
+-rw-r--r--   0        0        0   164616 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/System.Diagnostics.DiagnosticSource.dll
+-rw-r--r--   0        0        0     6656 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/System.IO.Abstractions.dll
+-rw-r--r--   0        0        0    71440 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/System.Text.Encodings.Web.dll
+-rw-r--r--   0        0        0   579848 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/System.Text.Json.dll
+-rw-r--r--   0        0        0    70416 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/System.Threading.RateLimiting.dll
+-rw-r--r--   0        0        0    37426 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Tableau.Migration.deps.json
+-rw-r--r--   0        0        0   985600 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Tableau.Migration.dll
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Tableau.Migration.runtimeconfig.json
+-rw-r--r--   0        0        0  1074636 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/Tableau.Migration.xml
+-rw-r--r--   0        0        0    53248 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/TestableIO.System.IO.Abstractions.Wrappers.dll
+-rw-r--r--   0        0        0    29184 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/TestableIO.System.IO.Abstractions.dll
+-rw-r--r--   0        0        0    71448 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/src/tableau_migration/bin/runtimes/browser/lib/net6.0/System.Text.Encodings.Web.dll
+-rw-r--r--   0        0        0     3583 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/.gitignore
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/LICENSE
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/README.md
+-rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 tableau_migration-2.1.0/PKG-INFO
```

### Comparing `tableau_migration-2.0.0/src/tableau_migration/__init__.py` & `tableau_migration-2.1.0/src/tableau_migration/__init__.py`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/migration.py` & `tableau_migration-2.1.0/src/tableau_migration/migration.py`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/migration_engine.py` & `tableau_migration-2.1.0/src/tableau_migration/migration_engine.py`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/migration_engine_hooks.py` & `tableau_migration-2.1.0/src/tableau_migration/migration_engine_hooks.py`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/migration_engine_hooks_filters.py` & `tableau_migration-2.1.0/src/tableau_migration/migration_engine_hooks_filters.py`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/migration_engine_hooks_mappings.py` & `tableau_migration-2.1.0/src/tableau_migration/migration_engine_hooks_mappings.py`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/migration_engine_hooks_transformers.py` & `tableau_migration-2.1.0/src/tableau_migration/migration_engine_hooks_transformers.py`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/migration_engine_migrators.py` & `tableau_migration-2.1.0/src/tableau_migration/migration_engine_migrators.py`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/migration_engine_options.py` & `tableau_migration-2.1.0/src/tableau_migration/migration_engine_options.py`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/migration_logger.py` & `tableau_migration-2.1.0/src/tableau_migration/migration_logger.py`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Bcl.AsyncInterfaces.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Bcl.AsyncInterfaces.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Bcl.TimeProvider.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Bcl.TimeProvider.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.AmbientMetadata.Application.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.AmbientMetadata.Application.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Compliance.Abstractions.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Compliance.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.Abstractions.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.Binder.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.Binder.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.EnvironmentVariables.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.EnvironmentVariables.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Configuration.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.Abstractions.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.AutoActivation.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.AutoActivation.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.DependencyInjection.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.DiagnosticAdapter.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.DiagnosticAdapter.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.Abstractions.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.ExceptionSummarization.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.ExceptionSummarization.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Diagnostics.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.FileProviders.Abstractions.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.FileProviders.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Hosting.Abstractions.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Hosting.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Http.Diagnostics.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Http.Diagnostics.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Http.Resilience.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Http.Resilience.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Http.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Http.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Localization.Abstractions.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Localization.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Localization.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Localization.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Logging.Abstractions.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Logging.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Logging.Configuration.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Logging.Configuration.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Logging.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Logging.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.ObjectPool.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.ObjectPool.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Options.ConfigurationExtensions.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Options.ConfigurationExtensions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Options.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Options.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Primitives.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Primitives.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Resilience.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Resilience.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Telemetry.Abstractions.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Telemetry.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.Extensions.Telemetry.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.Extensions.Telemetry.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Microsoft.IO.RecyclableMemoryStream.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Microsoft.IO.RecyclableMemoryStream.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Polly.Core.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Polly.Core.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Polly.Extensions.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Polly.Extensions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Polly.RateLimiting.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Polly.RateLimiting.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/System.Collections.Immutable.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/System.Collections.Immutable.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/System.Diagnostics.DiagnosticSource.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/System.Diagnostics.DiagnosticSource.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/System.IO.Abstractions.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/System.IO.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/System.Text.Encodings.Web.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/System.Text.Encodings.Web.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/System.Text.Json.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/System.Text.Json.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/System.Threading.RateLimiting.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/System.Threading.RateLimiting.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Tableau.Migration.deps.json` & `tableau_migration-2.1.0/src/tableau_migration/bin/Tableau.Migration.deps.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9921875%*

 * *Differences: {"'libraries'": "{'Tableau.Migration/2.1.0': OrderedDict([('type', 'project'), ('serviceable', "*

 * *                "False), ('sha512', '')]), delete: ['Tableau.Migration/2.0.0']}",*

 * * "'targets'": "{'.NETCoreApp,Version=v6.0': {'Tableau.Migration/2.1.0': "*

 * *              "OrderedDict([('dependencies', "*

 * *              "OrderedDict([('Microsoft.Extensions.Configuration.EnvironmentVariables', '8.0.0'), "*

 * *              "('Microsoft.Extensions.Http', '8.0.0'), ('Microsoft.Extensions.Http.Resilience', "*

 * *               […]*

```diff
@@ -305,15 +305,15 @@
         "System.Threading.RateLimiting/8.0.0": {
             "hashPath": "system.threading.ratelimiting.8.0.0.nupkg.sha512",
             "path": "system.threading.ratelimiting/8.0.0",
             "serviceable": true,
             "sha512": "sha512-7mu9v0QDv66ar3DpGSZHg9NuNcxDaaAcnMULuZlaTpP9+hwXhrxNGsF5GmLkSHxFdb5bBc1TzeujsRgTrPWi+Q==",
             "type": "package"
         },
-        "Tableau.Migration/2.0.0": {
+        "Tableau.Migration/2.1.0": {
             "serviceable": false,
             "sha512": "",
             "type": "project"
         },
         "TestableIO.System.IO.Abstractions.Wrappers/20.0.15": {
             "hashPath": "testableio.system.io.abstractions.wrappers.20.0.15.nupkg.sha512",
             "path": "testableio.system.io.abstractions.wrappers/20.0.15",
@@ -859,15 +859,15 @@
                 "runtime": {
                     "lib/net6.0/System.Threading.RateLimiting.dll": {
                         "assemblyVersion": "8.0.0.0",
                         "fileVersion": "8.0.23.53103"
                     }
                 }
             },
-            "Tableau.Migration/2.0.0": {
+            "Tableau.Migration/2.1.0": {
                 "dependencies": {
                     "Microsoft.Extensions.Configuration.EnvironmentVariables": "8.0.0",
                     "Microsoft.Extensions.Http": "8.0.0",
                     "Microsoft.Extensions.Http.Resilience": "8.2.0",
                     "Microsoft.Extensions.Localization": "8.0.2",
                     "Microsoft.Extensions.Options.ConfigurationExtensions": "8.0.0",
                     "Microsoft.IO.RecyclableMemoryStream": "3.0.0",
```

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Tableau.Migration.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/Tableau.Migration.dll`

 * *Files 26% similar despite different names*

#### pedump {}

```diff
@@ -1,25 +1,25 @@
 
 COFF Header:
 	                Machine: 0x014c
 	               Sections: 0x0003
-	             Time stamp: 0x883a29ca
+	             Time stamp: 0x8ce8f25f
 	Pointer to Symbol Table: 0x00000000
 	   	   Symbol Count: 0x00000000
 	   Optional Header Size: 0x00e0
 	   	Characteristics: 0x2022
 
 PE Header:
 	         Magic (0x010b): 0x010b
 	             LMajor (6): 0x30
 	             LMinor (0): 0x00
-	              Code Size: 0x000ee800
+	              Code Size: 0x000efa00
 	  Initialized Data Size: 0x00000e00
 	Uninitialized Data Size: 0x00000000
-	        Entry Point RVA: 0x000f0746
+	        Entry Point RVA: 0x000f19ca
 	 	  Code Base RVA: 0x00002000
 		  Data Base RVA: 0x000f2000
 
 
 NT Header:
 	   Image Base (0x400000): 0x10000000
 	Section Alignment (8192): 0x00002000
@@ -41,106 +41,106 @@
 	  Heap Reserve Size (1M): 0x00100000
 	 Heap Commit Size (4096): 0x00001000
 	      Loader flags (0x1): 0x00000000
 	   Data Directories (16): 0x00000010
 
 Data directories:
 	     Export Table: 0x00000000 [0x00000000]
-	     Import Table: 0x000f06f4 [0x0000004f]
+	     Import Table: 0x000f1978 [0x0000004f]
 	   Resource Table: 0x000f2000 [0x00000a7c]
 	  Exception Table: 0x00000000 [0x00000000]
 	Certificate Table: 0x00000000 [0x00000000]
 	      Reloc Table: 0x000f4000 [0x0000000c]
-	            Debug: 0x000f05f4 [0x00000054]
+	            Debug: 0x000f1878 [0x00000054]
 	        Copyright: 0x00000000 [0x00000000]
 	       Global Ptr: 0x00000000 [0x00000000]
 	        TLS Table: 0x00000000 [0x00000000]
 	Load Config Table: 0x00000000 [0x00000000]
 	     Bound Import: 0x00000000 [0x00000000]
 	              IAT: 0x00002000 [0x00000008]
 	Delay Import Desc: 0x00000000 [0x00000000]
 	       CLI Header: 0x00002008 [0x00000048]
 
 	Name: .text
-	   Virtual Size: 0x000ee74c
+	   Virtual Size: 0x000ef9d0
 	Virtual Address: 0x00002000
-	  Raw Data Size: 0x000ee800
+	  Raw Data Size: 0x000efa00
 	   Raw Data Ptr: 0x00000200
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: code, exec, read, 
 
 	Name: .rsrc
 	   Virtual Size: 0x00000a7c
 	Virtual Address: 0x000f2000
 	  Raw Data Size: 0x00000c00
-	   Raw Data Ptr: 0x000eea00
+	   Raw Data Ptr: 0x000efc00
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, read, 
 
 	Name: .reloc
 	   Virtual Size: 0x0000000c
 	Virtual Address: 0x000f4000
 	  Raw Data Size: 0x00000200
-	   Raw Data Ptr: 0x000ef600
+	   Raw Data Ptr: 0x000f0800
 	      Reloc Ptr: 0x00000000
 	     LineNo Ptr: 0x00000000
 	    Reloc Count: 0x0000
 	     Line Count: 0x0000
 	Flags: data, discard, read, 
 
           CLI header size: 72
          Runtime required: 2.5
                     Flags: ilonly, 32/64, no-trackdebug, notsigned
-	         Metadata: 0x0004375c [0x000ab158]
+	         Metadata: 0x00043dbc [0x000abce4]
 	Entry Point Token: 0x00000000
-	     Resources at: 0x000ee8b4 [0x00001d40]
+	     Resources at: 0x000efaa0 [0x00001dd8]
 	   Strong Name at: 0x00000000 [0x00000000]
 	  Code Manager at: 0x00000000 [0x00000000]
 	  VTableFixups at: 0x00000000 [0x00000000]
 	     EAT jumps at: 0x00000000 [0x00000000]
 
 Strong name: none
 
 Public key: none
 
 Metadata header:
            Version: 1.1
     Version string: v4.0.30319
 
 Metadata pointers:
-	Tables (#~): 0x0000006c - 0x0007029c [459312 == 0x00070230]
-	    Strings: 0x0007029c - 0x00087fd8 [97596 == 0x00017d3c]
-	       Blob: 0x0008d700 - 0x000ab158 [121432 == 0x0001da58]
-	User string: 0x00087fd8 - 0x0008d6f0 [22296 == 0x00005718]
-	       GUID: 0x0008d6f0 - 0x0008d700 [16 == 0x00000010]
+	Tables (#~): 0x0000006c - 0x000709a4 [461112 == 0x00070938]
+	    Strings: 0x000709a4 - 0x00088874 [98000 == 0x00017ed0]
+	       Blob: 0x0008e010 - 0x000abce4 [122068 == 0x0001dcd4]
+	User string: 0x00088874 - 0x0008e000 [22412 == 0x0000578c]
+	       GUID: 0x0008e000 - 0x0008e010 [16 == 0x00000010]
 Rows:
-Table Module: 1 records (12 bytes, at 41a44)
-Table TypeRef: 405 records (10 bytes, at 41a50)
-Table TypeDef: 1457 records (18 bytes, at 42a22)
-Table Field: 4250 records (10 bytes, at 49094)
-Table Method: 6096 records (18 bytes, at 53698)
-Table Param: 5446 records (8 bytes, at 6e338)
-Table InterfaceImpl: 1326 records (4 bytes, at 78d68)
-Table MemberRef: 4523 records (10 bytes, at 7a220)
-Table Constant: 419 records (8 bytes, at 852ce)
-Table CustomAttribute: 11141 records (10 bytes, at 85fe6)
-Table StandaloneSig: 849 records (4 bytes, at a1318)
-Table EventMap: 2 records (4 bytes, at a205c)
-Table Event: 2 records (8 bytes, at a2064)
-Table PropertyMap: 483 records (4 bytes, at a2074)
-Table Property: 1519 records (10 bytes, at a2800)
-Table MethodSemantics: 2339 records (6 bytes, at a6356)
-Table MethodImpl: 698 records (6 bytes, at a9a28)
-Table TypeSpec: 1660 records (4 bytes, at aaa84)
-Table Assembly: 1 records (28 bytes, at ac474)
-Table AssemblyRef: 46 records (28 bytes, at ac490)
-Table ManifestResource: 3 records (14 bytes, at ac998)
-Table NestedClass: 680 records (4 bytes, at ac9c2)
-Table GenericParam: 734 records (10 bytes, at ad462)
-Table MethodSpec: 1515 records (6 bytes, at af10e)
-Table GenericParamConstraint: 473 records (4 bytes, at b1490)
+Table Module: 1 records (12 bytes, at 420a4)
+Table TypeRef: 405 records (10 bytes, at 420b0)
+Table TypeDef: 1462 records (18 bytes, at 43082)
+Table Field: 4280 records (10 bytes, at 4974e)
+Table Method: 6118 records (18 bytes, at 53e7e)
+Table Param: 5469 records (8 bytes, at 6ecaa)
+Table InterfaceImpl: 1329 records (4 bytes, at 79792)
+Table MemberRef: 4529 records (10 bytes, at 7ac56)
+Table Constant: 420 records (8 bytes, at 85d40)
+Table CustomAttribute: 11187 records (10 bytes, at 86a60)
+Table StandaloneSig: 856 records (4 bytes, at a1f5e)
+Table EventMap: 2 records (4 bytes, at a2cbe)
+Table Event: 2 records (8 bytes, at a2cc6)
+Table PropertyMap: 483 records (4 bytes, at a2cd6)
+Table Property: 1526 records (10 bytes, at a3462)
+Table MethodSemantics: 2346 records (6 bytes, at a6ffe)
+Table MethodImpl: 705 records (6 bytes, at aa6fa)
+Table TypeSpec: 1662 records (4 bytes, at ab780)
+Table Assembly: 1 records (28 bytes, at ad178)
+Table AssemblyRef: 46 records (28 bytes, at ad194)
+Table ManifestResource: 3 records (14 bytes, at ad69c)
+Table NestedClass: 685 records (4 bytes, at ad6c6)
+Table GenericParam: 735 records (10 bytes, at ae17a)
+Table MethodSpec: 1527 records (6 bytes, at afe30)
+Table GenericParamConstraint: 473 records (4 bytes, at b21fa)
```

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Tableau.Migration.xml` & `tableau_migration-2.1.0/src/tableau_migration/bin/Tableau.Migration.xml`

 * *Files 0% similar despite different names*

#### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/Tableau.Migration.xml` & `tableau_migration-2.1.0/src/tableau_migration/bin/Tableau.Migration.xml`

```diff
@@ -140,14 +140,17 @@
     </member>
     <member name="M:Tableau.Migration.Api.GroupsApiClient.AddUserToGroupAsync(System.Guid,System.Guid,System.Threading.CancellationToken)">
       <inheritdoc/>
     </member>
     <member name="M:Tableau.Migration.Api.GroupsApiClient.RemoveUserFromGroupAsync(System.Guid,System.Guid,System.Threading.CancellationToken)">
       <inheritdoc/>
     </member>
+    <member name="M:Tableau.Migration.Api.GroupsApiClient.DeleteGroupAsync(System.Guid,System.Threading.CancellationToken)">
+      <inheritdoc/>
+    </member>
     <member name="T:Tableau.Migration.Api.IApiClient">
       <summary>Interface for unauthenticated API clients.</summary>
     </member>
     <member name="M:Tableau.Migration.Api.IApiClient.SignInAsync(System.Threading.CancellationToken)">
       <summary>Signs into Tableau Server.</summary>
       <param name="cancel">The cancellation token.</param>
       <returns>
@@ -430,14 +433,20 @@
     <member name="M:Tableau.Migration.Api.IGroupsApiClient.RemoveUserFromGroupAsync(System.Guid,System.Guid,System.Threading.CancellationToken)">
       <summary>Removes a user from a group.</summary>
       <param name="groupId">The id of the group the user belongs to.</param>
       <param name="userId">The user-id.</param>
       <param name="cancel">The cancellation token.</param>
       <returns>The operation result.</returns>
     </member>
+    <member name="M:Tableau.Migration.Api.IGroupsApiClient.DeleteGroupAsync(System.Guid,System.Threading.CancellationToken)">
+      <summary>Deletes a group.</summary>
+      <param name="groupId">The id of the group to delete.</param>
+      <param name="cancel">The cancellation token.</param>
+      <returns/>
+    </member>
     <member name="T:Tableau.Migration.Api.IHttpRequestBuilderExtensions">
       <summary>
         Static class containing extension methods for
         <see cref="T:Tableau.Migration.Net.IHttpRequestBuilder"/>
         objects.
       </summary>
     </member>
@@ -519,14 +528,19 @@
       </param>
       <param name="newContentPermissions">The new content permission mode of the project, or null to not update the mode.</param>
       <param name="newControllingPermissionsProjectId">The ID of the new controlling permissions project,
             or null to not update the controlling permissions project.</param>
       <param name="newOwnerId">The ID of the new owner of the project, or null to not update the owner.</param>
       <returns>The update result.</returns>
     </member>
+    <member name="M:Tableau.Migration.Api.IProjectsApiClient.DeleteProjectAsync(System.Guid,System.Threading.CancellationToken)">
+      <summary>Deletes a project.</summary>
+      <param name="projectId">The ID for the project to delete.</param>
+      <param name="cancel">A cancellation token to obey.</param>
+    </member>
     <member name="T:Tableau.Migration.Api.IPublishApiClient`2">
       <summary>Interface for a content typed API client that can publish items.</summary>
       <typeparam name="TPublish">The content publish type.</typeparam>
       <typeparam name="TPublishResult">The publish result type.</typeparam>
     </member>
     <member name="M:Tableau.Migration.Api.IPublishApiClient`2.PublishAsync(`0,System.Threading.CancellationToken)">
       <summary>Publishes a content item.</summary>
@@ -816,14 +830,20 @@
       <param name="cancel">The cancellation token.</param>
       <param name="newfullName">(Optional) The new Full Name for the user.</param>
       <param name="newEmail">(Optional) The new email address for the user.</param>
       <param name="newPassword">(Optional) The new password for the user.</param>
       <param name="newAuthSetting">(Optional) The new email Auth Setting for the user.</param>
       <returns/>
     </member>
+    <member name="M:Tableau.Migration.Api.IUsersApiClient.DeleteUserAsync(System.Guid,System.Threading.CancellationToken)">
+      <summary>Deletes a user.</summary>
+      <param name="userId">The user's ID.</param>
+      <param name="cancel">The cancellation token.</param>
+      <returns/>
+    </member>
     <member name="T:Tableau.Migration.Api.IViewsApiClient">
       <summary>Interface for an API client that modifies workbook views</summary>
     </member>
     <member name="T:Tableau.Migration.Api.IViewsApiClientFactory">
       <summary>
         Interface for an object that can create
         <see cref="T:Tableau.Migration.Api.IViewsApiClient"/>
@@ -834,15 +854,15 @@
       <summary/>
       <returns/>
     </member>
     <member name="T:Tableau.Migration.Api.IWorkbooksApiClient">
       <summary>Interface for API client workbook operations.</summary>
     </member>
     <member name="M:Tableau.Migration.Api.IWorkbooksApiClient.GetAllWorkbooksAsync(System.Int32,System.Int32,System.Threading.CancellationToken)">
-      <summary>Gets all workbook in the current site.</summary>
+      <summary>Gets all workbooks in the current site except the ones in the Personal Space.</summary>
       <param name="pageNumber">The 1-indexed page number.</param>
       <param name="pageSize">The size of the page.</param>
       <param name="cancel">A cancellation token to obey.</param>
       <returns>A list of a page of workbooks in the current site.</returns>
     </member>
     <member name="M:Tableau.Migration.Api.IWorkbooksApiClient.GetWorkbookAsync(System.Guid,System.Threading.CancellationToken)">
       <summary>Gets a workbook by the given ID.</summary>
@@ -1205,14 +1225,17 @@
     </member>
     <member name="P:Tableau.Migration.Api.Models.IPublishWorkbookOptions.ThumbnailsUserId">
       <summary>Gets the ID of the user to generate thumbnails as.</summary>
     </member>
     <member name="P:Tableau.Migration.Api.Models.IPublishWorkbookOptions.ProjectId">
       <summary>Gets the ID of the project to publish to.</summary>
     </member>
+    <member name="P:Tableau.Migration.Api.Models.IPublishWorkbookOptions.HiddenViewNames">
+      <summary>Gets the names of the views that should be hidden.</summary>
+    </member>
     <member name="T:Tableau.Migration.Api.Models.IServerInfo">
       <summary>Interface for an API client server information model.</summary>
     </member>
     <member name="P:Tableau.Migration.Api.Models.IServerInfo.RestApiVersion">
       <summary>Gets the REST API version of the server.</summary>
     </member>
     <member name="P:Tableau.Migration.Api.Models.IServerInfo.ProductVersion">
@@ -1544,14 +1567,17 @@
     </member>
     <member name="P:Tableau.Migration.Api.Models.PublishWorkbookOptions.FileName">
       <inheritdoc/>
     </member>
     <member name="P:Tableau.Migration.Api.Models.PublishWorkbookOptions.FileType">
       <inheritdoc/>
     </member>
+    <member name="P:Tableau.Migration.Api.Models.PublishWorkbookOptions.HiddenViewNames">
+      <inheritdoc/>
+    </member>
     <member name="M:Tableau.Migration.Api.Models.PublishWorkbookOptions.#ctor(Tableau.Migration.Content.IPublishableWorkbook,System.IO.Stream,System.String)">
       <summary>
         Creates a new
         <see cref="T:Tableau.Migration.Api.Models.PublishWorkbookOptions"/>
         instance.
       </summary>
       <param name="workbook">The publishable workbook information.</param>
@@ -7283,14 +7309,17 @@
     </member>
     <member name="M:Tableau.Migration.Api.UsersApiClient.AddUserAsync(System.String,System.String,System.String,System.Threading.CancellationToken)">
       <inheritdoc/>
     </member>
     <member name="M:Tableau.Migration.Api.UsersApiClient.UpdateUserAsync(System.Guid,System.String,System.Threading.CancellationToken,System.String,System.String,System.String,System.String)">
       <inheritdoc/>
     </member>
+    <member name="M:Tableau.Migration.Api.UsersApiClient.DeleteUserAsync(System.Guid,System.Threading.CancellationToken)">
+      <inheritdoc/>
+    </member>
     <member name="M:Tableau.Migration.Api.UsersApiClient.GetPager(System.Int32)">
       <inheritdoc/>
     </member>
     <member name="M:Tableau.Migration.Api.UsersApiClient.PublishBatchAsync(System.Collections.Generic.IEnumerable{Tableau.Migration.Content.IUser},System.Threading.CancellationToken)">
       <inheritdoc/>
     </member>
     <member name="M:Tableau.Migration.Api.UsersApiClient.GetPageAsync(System.Int32,System.Int32,System.Threading.CancellationToken)">
@@ -9021,23 +9050,26 @@
       <summary>Interface for a group content item with users.</summary>
     </member>
     <member name="P:Tableau.Migration.Content.IPublishableGroup.Users">
       <summary>Gets or sets the users assigned to the group.</summary>
     </member>
     <member name="T:Tableau.Migration.Content.IPublishableWorkbook">
       <summary>
-        Intreface for a
+        Interface for an
         <see cref="T:Tableau.Migration.Content.IWorkbook"/>
         that has been downloaded
             and has full information necessary for re-publishing.
       </summary>
     </member>
     <member name="P:Tableau.Migration.Content.IPublishableWorkbook.ThumbnailsUserId">
       <summary>Gets the ID of the user to generate thumbnails as.</summary>
     </member>
+    <member name="P:Tableau.Migration.Content.IPublishableWorkbook.HiddenViewNames">
+      <summary>Gets the names of the views that should be hidden.</summary>
+    </member>
     <member name="T:Tableau.Migration.Content.IPublishedContent">
       <summary>Interface for a content item that has metadata around publishing information.</summary>
     </member>
     <member name="P:Tableau.Migration.Content.IPublishedContent.CreatedAt">
       <summary>Gets the created timestamp.</summary>
     </member>
     <member name="P:Tableau.Migration.Content.IPublishedContent.UpdatedAt">
@@ -9494,14 +9526,17 @@
     </member>
     <member name="P:Tableau.Migration.Content.PublishableWorkbook.File">
       <inheritdoc/>
     </member>
     <member name="P:Tableau.Migration.Content.PublishableWorkbook.Connections">
       <inheritdoc/>
     </member>
+    <member name="P:Tableau.Migration.Content.PublishableWorkbook.HiddenViewNames">
+      <inheritdoc/>
+    </member>
     <member name="M:Tableau.Migration.Content.PublishableWorkbook.DisposeAsync">
       <summary>Performs application-defined tasks associated with freeing, releasing, or resetting
             unmanaged resources asynchronously.</summary>
       <returns>A task that represents the asynchronous dispose operation.</returns>
     </member>
     <member name="T:Tableau.Migration.Content.Search.CachedContentReferenceFinder`1">
       <summary>
@@ -17476,14 +17511,17 @@
     </member>
     <member name="P:Tableau.Migration.Paging.IPageInfo.PageSize">
       <summary>Gets the expected maximum size of the page.</summary>
     </member>
     <member name="P:Tableau.Migration.Paging.IPageInfo.TotalCount">
       <summary>Gets the total unpaged item count.</summary>
     </member>
+    <member name="P:Tableau.Migration.Paging.IPageInfo.FetchedAllPages">
+      <summary>Indicates whether the SDK has already fetched all pages or not.</summary>
+    </member>
     <member name="T:Tableau.Migration.Paging.IPager`1">
       <summary>Interface for an object that can retrieve pages of content.</summary>
       <typeparam name="TContent">The content type.</typeparam>
     </member>
     <member name="M:Tableau.Migration.Paging.IPager`1.NextPageAsync(System.Threading.CancellationToken)">
       <summary>Gets a page of content.</summary>
       <param name="cancel">A cancellation token to obey.</param>
@@ -17497,46 +17535,51 @@
       <returns>The combined results.</returns>
     </member>
     <member name="M:Tableau.Migration.Paging.IPager`1.GetAllPagesAsync(System.Threading.CancellationToken)">
       <summary>Combines all pages of content.</summary>
       <param name="cancel">A cancellation token to obey.</param>
       <returns>The combined results.</returns>
     </member>
-    <member name="M:Tableau.Migration.Paging.PagedResult`1.#ctor(System.Boolean,System.Collections.Immutable.IImmutableList{`0},System.Int32,System.Int32,System.Int32,System.Exception[])">
+    <member name="M:Tableau.Migration.Paging.PagedResult`1.#ctor(System.Boolean,System.Collections.Immutable.IImmutableList{`0},System.Int32,System.Int32,System.Int32,System.Boolean,System.Exception[])">
       <summary>
         Creates a new
         <see cref="T:Tableau.Migration.Paging.PagedResult`1"/>
         object.
       </summary>
       <param name="success">True if the operation is successful, false otherwise.</param>
       <param name="value">The paged result of the operation.</param>
       <param name="pageNumber">The current 1-indexed page number.</param>
       <param name="pageSize">The page size.</param>
       <param name="totalCount">The total unpaged available item count.</param>
+      <param name="fetchedAllPages">Whether the SDK has already fetched all pages or not.</param>
       <param name="errors">The errors encountered during the operation, if any.</param>
     </member>
     <member name="P:Tableau.Migration.Paging.PagedResult`1.PageNumber">
       <inheritdoc/>
     </member>
     <member name="P:Tableau.Migration.Paging.PagedResult`1.PageSize">
       <inheritdoc/>
     </member>
     <member name="P:Tableau.Migration.Paging.PagedResult`1.TotalCount">
       <inheritdoc/>
     </member>
-    <member name="M:Tableau.Migration.Paging.PagedResult`1.Succeeded(System.Collections.Immutable.IImmutableList{`0},System.Int32,System.Int32,System.Int32)">
+    <member name="P:Tableau.Migration.Paging.PagedResult`1.FetchedAllPages">
+      <inheritdoc/>
+    </member>
+    <member name="M:Tableau.Migration.Paging.PagedResult`1.Succeeded(System.Collections.Immutable.IImmutableList{`0},System.Int32,System.Int32,System.Int32,System.Boolean)">
       <summary>
         Creates a new
         <see cref="T:Tableau.Migration.Paging.PagedResult`1"/>
         instance for successful paged operations.
       </summary>
       <param name="value">The result of the operation.</param>
       <param name="pageNumber">The current 1-indexed page number.</param>
       <param name="pageSize">The page size.</param>
       <param name="totalCount">The total unpaged available item count.</param>
+      <param name="fetchedAllPages">Whether the SDK has already fetched all pages or not.</param>
       <returns>
         A new
         <see cref="T:Tableau.Migration.Paging.PagedResult`1"/>
         instance.
       </returns>
     </member>
     <member name="M:Tableau.Migration.Paging.PagedResult`1.Failed(System.Exception)">
```

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/TestableIO.System.IO.Abstractions.Wrappers.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/TestableIO.System.IO.Abstractions.Wrappers.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/TestableIO.System.IO.Abstractions.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/TestableIO.System.IO.Abstractions.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/src/tableau_migration/bin/runtimes/browser/lib/net6.0/System.Text.Encodings.Web.dll` & `tableau_migration-2.1.0/src/tableau_migration/bin/runtimes/browser/lib/net6.0/System.Text.Encodings.Web.dll`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/.gitignore` & `tableau_migration-2.1.0/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -169,17 +169,19 @@
 #  and can be added to the global gitignore or merged into this file.  For a more nuclear
 #  option (not recommended) you can uncomment the following to ignore the entire idea folder.
 #.idea/
 
 # Other stuff
 UpgradeLog.htm
 appsettings.Development.json
+clean-server-settings.dev.json
 launchSettings.json
 UpgradeLog.htm
 *.DEV.ini
 *.DEV.json
 /src/Python/Documentation/_build
 /src/Python/Documentation/_static
 /src/Python/Python.pyproj.user
 /src/Documentation/_python
 /src/Python/Documentation/generated
 /tests/Python.TestApplication/manifest.json
+
```

### Comparing `tableau_migration-2.0.0/pyproject.toml` & `tableau_migration-2.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tableau_migration-2.0.0/PKG-INFO` & `tableau_migration-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: tableau_migration
-Version: 2.0.0
+Version: 2.1.0
 Summary: Tableau Migration SDK
 Project-URL: Homepage, http://www.tableau.com
 Project-URL: Bug Tracker, http://www.tableau.com
 Project-URL: Repository, https://github.com/tableau/tableau-migration-sdk
 Author: Tableau a Salesforce Product
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
```

