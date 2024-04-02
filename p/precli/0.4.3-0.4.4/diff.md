# Comparing `tmp/precli-0.4.3.tar.gz` & `tmp/precli-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "precli-0.4.3.tar", last modified: Thu Mar 28 17:29:38 2024, max compression
+gzip compressed data, was "precli-0.4.4.tar", last modified: Tue Apr  2 19:20:18 2024, max compression
```

## Comparing `precli-0.4.3.tar` & `precli-0.4.4.tar`

### file list

```diff
@@ -1,681 +1,683 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.940044 precli-0.4.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.832043 precli-0.4.3/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-28 17:29:31.000000 precli-0.4.3/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-03-28 17:29:31.000000 precli-0.4.3/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.832043 precli-0.4.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-03-28 17:29:31.000000 precli-0.4.3/.github/workflows/dependency-review.yml
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-03-28 17:29:31.000000 precli-0.4.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-03-28 17:29:31.000000 precli-0.4.3/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-03-28 17:29:31.000000 precli-0.4.3/.github/workflows/unit-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-03-28 17:29:31.000000 precli-0.4.3/.github/workflows/upload-asset.yml
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-28 17:29:31.000000 precli-0.4.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-28 17:29:31.000000 precli-0.4.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-03-28 17:29:31.000000 precli-0.4.3/.stestr.conf
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-03-28 17:29:38.000000 precli-0.4.3/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-03-28 17:29:31.000000 precli-0.4.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    16129 2024-03-28 17:29:38.000000 precli-0.4.3/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-03-28 17:29:31.000000 precli-0.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-03-28 17:29:38.940044 precli-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-03-28 17:29:31.000000 precli-0.4.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-03-28 17:29:31.000000 precli-0.4.3/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.836043 precli-0.4.3/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-03-28 17:29:31.000000 precli-0.4.3/docs/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-03-28 17:29:31.000000 precli-0.4.3/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.836043 precli-0.4.3/docs/man/
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-03-28 17:29:31.000000 precli-0.4.3/docs/man/precli.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-28 17:29:31.000000 precli-0.4.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.820043 precli-0.4.3/docs/rules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.820043 precli-0.4.3/docs/rules/go/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.836043 precli-0.4.3/docs/rules/go/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/go/stdlib/crypto-weak-cipher.md
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/go/stdlib/crypto-weak-hash.md
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/go/stdlib/crypto-weak-key.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.820043 precli-0.4.3/docs/rules/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.840043 precli-0.4.3/docs/rules/python/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/argparse-sensitive-info.md
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/assert.md
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/crypt-weak-hash.md
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/ftplib-cleartext.md
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/ftplib-unverified-context.md
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/hashlib-improper-prng.md
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/hashlib-weak-hash.md
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/hmac-timing-attack.md
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/hmac-weak-hash.md
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/hmac-weak-key.md
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/http-server-unrestricted-bind.md
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/http-url-secret.md
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/imaplib-cleartext.md
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/imaplib-unverified-context.md
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/json-load.md
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/logging-insecure-listen-config.md
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/marshal-load.md
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/nntplib-cleartext.md
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/nntplib-unverified-context.md
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/pickle-load.md
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/poplib-cleartext.md
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/poplib-unverified-context.md
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/re-denial-of-service.md
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/secrets-weak-token.md
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/shelve-open.md
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/smtplib-cleartext.md
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/smtplib-unverified-context.md
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/socket-unrestricted-bind.md
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/socketserver-unrestricted-bind.md
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/ssl-context-weak-key.md
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/ssl-create-unverified-context.md
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/ssl-insecure-tls-version.md
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/telnetlib-cleartext.md
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/tempfile-mktemp-race-condition.md
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules/python/stdlib/xmlrpc-server-unrestricted-bind.md
--rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-03-28 17:29:31.000000 precli-0.4.3/docs/rules.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.840043 precli-0.4.3/logo/
--rw-r--r--   0 runner    (1001) docker     (127)    47438 2024-03-28 17:29:31.000000 precli-0.4.3/logo/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-28 17:29:31.000000 precli-0.4.3/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.840043 precli-0.4.3/precli/
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-28 17:29:31.000000 precli-0.4.3/precli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-28 17:29:31.000000 precli-0.4.3/precli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.844043 precli-0.4.3/precli/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/precli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10857 2024-03-28 17:29:31.000000 precli-0.4.3/precli/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.848043 precli-0.4.3/precli/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/precli/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-03-28 17:29:31.000000 precli-0.4.3/precli/core/argument.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-03-28 17:29:31.000000 precli-0.4.3/precli/core/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-03-28 17:29:31.000000 precli-0.4.3/precli/core/call.py
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-03-28 17:29:31.000000 precli-0.4.3/precli/core/comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-03-28 17:29:31.000000 precli-0.4.3/precli/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-03-28 17:29:31.000000 precli-0.4.3/precli/core/fix.py
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-03-28 17:29:31.000000 precli-0.4.3/precli/core/kind.py
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-03-28 17:29:31.000000 precli-0.4.3/precli/core/level.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-03-28 17:29:31.000000 precli-0.4.3/precli/core/linecache.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-28 17:29:31.000000 precli-0.4.3/precli/core/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-03-28 17:29:31.000000 precli-0.4.3/precli/core/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-03-28 17:29:31.000000 precli-0.4.3/precli/core/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9636 2024-03-28 17:29:31.000000 precli-0.4.3/precli/core/redos.py
--rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-03-28 17:29:31.000000 precli-0.4.3/precli/core/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-03-28 17:29:31.000000 precli-0.4.3/precli/core/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-03-28 17:29:31.000000 precli-0.4.3/precli/core/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-03-28 17:29:31.000000 precli-0.4.3/precli/core/suppression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-03-28 17:29:31.000000 precli-0.4.3/precli/core/symtab.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-03-28 17:29:31.000000 precli-0.4.3/precli/core/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-03-28 17:29:31.000000 precli-0.4.3/precli/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.848043 precli-0.4.3/precli/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-03-28 17:29:31.000000 precli-0.4.3/precli/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6909 2024-03-28 17:29:31.000000 precli-0.4.3/precli/parsers/go.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-28 17:29:31.000000 precli-0.4.3/precli/parsers/java.py
--rw-r--r--   0 runner    (1001) docker     (127)    16686 2024-03-28 17:29:31.000000 precli-0.4.3/precli/parsers/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-03-28 17:29:31.000000 precli-0.4.3/precli/parsers/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.848043 precli-0.4.3/precli/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-28 17:29:31.000000 precli-0.4.3/precli/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-03-28 17:29:31.000000 precli-0.4.3/precli/renderers/detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-03-28 17:29:31.000000 precli-0.4.3/precli/renderers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-03-28 17:29:31.000000 precli-0.4.3/precli/renderers/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-03-28 17:29:31.000000 precli-0.4.3/precli/renderers/plain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.852043 precli-0.4.3/precli/rules/
--rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.852043 precli-0.4.3/precli/rules/go/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/go/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.852043 precli-0.4.3/precli/rules/go/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/go/stdlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/go/stdlib/crypto_weak_cipher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/go/stdlib/crypto_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/go/stdlib/crypto_weak_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.852043 precli-0.4.3/precli/rules/java/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.852043 precli-0.4.3/precli/rules/java/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/java/stdlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.852043 precli-0.4.3/precli/rules/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.860043 precli-0.4.3/precli/rules/python/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/argparse_sensitive_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/assert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/crypt_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/ftplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/ftplib_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/hashlib_improper_prng.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/hashlib_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/hmac_timing_attack.py
--rw-r--r--   0 runner    (1001) docker     (127)     4971 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/hmac_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/hmac_weak_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/http_server_unrestricted_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/http_url_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/imaplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/imaplib_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/json_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/logging_insecure_listen_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/marshal_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/nntplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/nntplib_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/pickle_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/poplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/poplib_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/re_denial_of_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/secrets_weak_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/shelve_open.py
--rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/smtplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/smtplib_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/socket_unrestricted_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/socketserver_unrestricted_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/ssl_context_weak_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/ssl_create_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/ssl_insecure_tls_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/telnetlib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/tempfile_mktemp_race_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-03-28 17:29:31.000000 precli-0.4.3/precli/rules/python/stdlib/xmlrpc_server_unrestricted_bind.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.940044 precli-0.4.3/precli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-03-28 17:29:38.000000 precli-0.4.3/precli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    36291 2024-03-28 17:29:38.000000 precli-0.4.3/precli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:29:38.000000 precli-0.4.3/precli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-03-28 17:29:38.000000 precli-0.4.3/precli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 17:29:38.000000 precli-0.4.3/precli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-28 17:29:38.000000 precli-0.4.3/precli.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-28 17:29:38.000000 precli-0.4.3/precli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-28 17:29:38.000000 precli-0.4.3/precli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-03-28 17:29:31.000000 precli-0.4.3/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-28 17:29:31.000000 precli-0.4.3/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.860043 precli-0.4.3/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)       94 2024-03-28 17:29:31.000000 precli-0.4.3/scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-03-28 17:29:38.940044 precli-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-03-28 17:29:31.000000 precli-0.4.3/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-28 17:29:31.000000 precli-0.4.3/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.860043 precli-0.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.860043 precli-0.4.3/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.860043 precli-0.4.3/tests/unit/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.860043 precli-0.4.3/tests/unit/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/core/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.860043 precli-0.4.3/tests/unit/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.864043 precli-0.4.3/tests/unit/parsers/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/parsers/examples/suppress.go
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/parsers/examples/suppress.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/parsers/examples/suppress_lowercase_rule.go
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/parsers/examples/suppress_lowercase_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/parsers/examples/suppress_multiline.go
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/parsers/examples/suppress_multiline.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/parsers/examples/suppress_multiple_comments.go
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/parsers/examples/suppress_multiple_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/parsers/examples/suppress_multiple_rules.go
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/parsers/examples/suppress_multiple_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/parsers/examples/suppress_preceding.go
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/parsers/examples/suppress_preceding.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/parsers/examples/suppress_spaced_rules.go
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/parsers/examples/suppress_spaced_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/parsers/examples/suppress_wrong_rule.go
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/parsers/examples/suppress_wrong_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     5512 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/parsers/test_go.py
--rw-r--r--   0 runner    (1001) docker     (127)     5524 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/parsers/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.864043 precli-0.4.3/tests/unit/rules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.864043 precli-0.4.3/tests/unit/rules/go/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/go/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.864043 precli-0.4.3/tests/unit/rules/go/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/go/stdlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.864043 precli-0.4.3/tests/unit/rules/go/stdlib/crypto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/go/stdlib/crypto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.868043 precli-0.4.3/tests/unit/rules/go/stdlib/crypto/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_aes.go
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_des.go
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_rc4.go
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_md5_new.go
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_md5_sum.go
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha1_new.go
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha1_sum.go
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha256_new.go
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha256_sum.go
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_1024.go
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_2048.go
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_3072.go
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_1024.go
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_2048.go
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_4096.go
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_bits_as_var.go
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_cipher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.868043 precli-0.4.3/tests/unit/rules/java/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.868043 precli-0.4.3/tests/unit/rules/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.868043 precli-0.4.3/tests/unit/rules/python/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.868043 precli-0.4.3/tests/unit/rules/python/stdlib/argparse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/argparse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.868043 precli-0.4.3/tests/unit/rules/python/stdlib/argparse/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_default_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_password.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_password_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_password_store_true.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/argparse/test_argparse_sensitive_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.868043 precli-0.4.3/tests/unit/rules/python/stdlib/assert/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/assert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.868043 precli-0.4.3/tests/unit/rules/python/stdlib/assert/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/assert/examples/assert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/assert/test_assert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.868043 precli-0.4.3/tests/unit/rules/python/stdlib/crypt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/crypt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.872043 precli-0.4.3/tests/unit/rules/python/stdlib/crypt/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_blowfish.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_blowfish.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/crypt/test_crypt_weak_hash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.872043 precli-0.4.3/tests/unit/rules/python/stdlib/ftplib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ftplib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.876043 precli-0.4.3/tests/unit/rules/python/stdlib/ftplib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ftplib/examples/ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ftplib/examples/ftp_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ftplib/examples/ftp_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ftplib/examples/ftp_tls.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_login.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_login_single_statement.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_user_password.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_user_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ftplib/test_ftplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ftplib/test_ftplib_unverified_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.876043 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.888043 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_pbkdf2_hmac.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_scrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5_as_identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5_importlib.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5_usedforsecurity_true.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md5_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md5_usedforsecurity_true.py
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_name_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha_usedforsecurity_false.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha_usedforsecurity_false.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/test_hashlib_improper_prng.py
--rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/test_hashlib_weak_hash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.888043 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.904044 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_md5_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_hashlib_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_hashlib_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_hashlib_sm3.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_md5_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_hashlib_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_hashlib_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_hashlib_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_sha512_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack_class_hexdigest.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack_compare_digest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/test_hmac_timing_attack.py
--rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.904044 precli-0.4.3/tests/unit/rules/python/stdlib/http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.904044 precli-0.4.3/tests/unit/rules/python/stdlib/http/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/http/examples/http_server_http_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/http/examples/http_server_threading_http_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/http/examples/http_url_secret_apikey.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/http/examples/http_url_secret_apikey_in_header.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/http/examples/http_url_secret_basic_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/http/examples/http_url_secret_basic_auth_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/http/examples/http_url_secret_password.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/http/examples/http_url_secret_username.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/http/test_http_server_unrestricted_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/http/test_http_url_secret.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.908044 precli-0.4.3/tests/unit/rules/python/stdlib/imaplib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/imaplib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.908044 precli-0.4.3/tests/unit/rules/python/stdlib/imaplib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_authenticate.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_login_cram_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/imaplib/test_imaplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/imaplib/test_imaplib_unverified_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.908044 precli-0.4.3/tests/unit/rules/python/stdlib/json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/json/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.908044 precli-0.4.3/tests/unit/rules/python/stdlib/json/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/json/examples/json_jsondecoder_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/json/examples/json_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/json/examples/json_loads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/json/test_json_load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.908044 precli-0.4.3/tests/unit/rules/python/stdlib/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.912044 precli-0.4.3/tests/unit/rules/python/stdlib/logging/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_empty_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_port.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_port_verify_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_port_verify_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_verify_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_verify_none_port.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_verify_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/logging/test_logging_insecure_listen_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.912044 precli-0.4.3/tests/unit/rules/python/stdlib/marshal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/marshal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.912044 precli-0.4.3/tests/unit/rules/python/stdlib/marshal/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/marshal/examples/marshal_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/marshal/examples/marshal_loads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/marshal/test_marshal_load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.912044 precli-0.4.3/tests/unit/rules/python/stdlib/nntplib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/nntplib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.916044 precli-0.4.3/tests/unit/rules/python/stdlib/nntplib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/nntplib/test_nntplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/nntplib/test_nntplib_unverified_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.916044 precli-0.4.3/tests/unit/rules/python/stdlib/pickle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/pickle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.916044 precli-0.4.3/tests/unit/rules/python/stdlib/pickle/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/pickle/examples/pickle_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/pickle/examples/pickle_loads.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/pickle/examples/pickle_unpickler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/pickle/test_pickle_load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.916044 precli-0.4.3/tests/unit/rules/python/stdlib/poplib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/poplib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.920044 precli-0.4.3/tests/unit/rules/python/stdlib/poplib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_apop.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_pass_.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_rpop.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/poplib/test_poplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/poplib/test_poplib_unverified_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.920044 precli-0.4.3/tests/unit/rules/python/stdlib/re/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/re/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.920044 precli-0.4.3/tests/unit/rules/python/stdlib/re/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/re/examples/re_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/re/examples/re_compile_good.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/re/examples/re_findall.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/re/examples/re_finditer.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/re/examples/re_fullmatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/re/examples/re_match.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/re/examples/re_search.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/re/examples/re_search_good.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/re/examples/re_split.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/re/examples/re_sub.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/re/examples/re_subn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/re/test_re_denial_of_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.920044 precli-0.4.3/tests/unit/rules/python/stdlib/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.920044 precli-0.4.3/tests/unit/rules/python/stdlib/secrets/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_bytes_default.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_bytes_size_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_hex.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_urlsafe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/secrets/test_secrets_weak_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.920044 precli-0.4.3/tests/unit/rules/python/stdlib/shelve/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/shelve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.924044 precli-0.4.3/tests/unit/rules/python/stdlib/shelve/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/shelve/examples/shelve_dbfilenameshelf.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/shelve/examples/shelve_open.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/shelve/examples/shelve_open_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/shelve/test_shelve_open.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.924044 precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.924044 precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/test_smtplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/test_smtplib_unverified_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.924044 precli-0.4.3/tests/unit/rules/python/stdlib/socket/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/socket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.928044 precli-0.4.3/tests/unit/rules/python/stdlib/socket/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/socket/examples/socket_create_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/socket/examples/socket_socket_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/socket/examples/socket_socket_bind_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/socket/examples/socket_socket_bind_as_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/socket/test_socket_unrestricted_bind.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.928044 precli-0.4.3/tests/unit/rules/python/stdlib/socketserver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/socketserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.928044 precli-0.4.3/tests/unit/rules/python/stdlib/socketserver/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_tcp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_udp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_tcp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_tcp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_udp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_udp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/socketserver/test_socketserver_unrestricted_bind.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.928044 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.936044 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/create_default_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/create_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_sslv2.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_sslv23.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_sslv3.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_tlsv1.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_tlsv11.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_tlsv12.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP256r1.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP384r1.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP384r1tls13.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP512r1.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_default_context.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_ffdhe2048.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_prime192v1.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_prime256v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_secp160r2.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_secp256r1.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_sect163k1.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_sect571k1.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_typed_default_param.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_typed_param.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_sslv2.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_sslv23.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_sslv3.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_tlsv1.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_tlsv11.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_tlsv12.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv2.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv23.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv2_server_side_true.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv3.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_tlsv1.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_tlsv11.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_tlsv12.py
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/test_ssl_context_tls_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/test_ssl_context_weak_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/test_ssl_create_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/test_ssl_get_server_certificate_tls_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/ssl/test_ssl_wrap_socket_tls_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.936044 precli-0.4.3/tests/unit/rules/python/stdlib/telnetlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/telnetlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.936044 precli-0.4.3/tests/unit/rules/python/stdlib/telnetlib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/telnetlib/examples/telnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/telnetlib/examples/telnetlib_telnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/telnetlib/examples/telnetlib_telnet_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/telnetlib/test_telnetlib_cleartext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.936044 precli-0.4.3/tests/unit/rules/python/stdlib/tempfile/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/tempfile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.936044 precli-0.4.3/tests/unit/rules/python/stdlib/tempfile/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_args_open.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_args_with_open_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_open.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_walrus_open.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_with_open.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_with_open_multiline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/tempfile/test_tempfile_mktemp_race_condition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.940044 precli-0.4.3/tests/unit/rules/python/stdlib/xmlrpc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/xmlrpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 17:29:38.940044 precli-0.4.3/tests/unit/rules/python/stdlib/xmlrpc/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/xmlrpc/examples/xmlrpc_server_doc_xml_rpc_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/xmlrpc/examples/xmlrpc_server_simple_xml_rpc_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/python/stdlib/xmlrpc/test_xmlrpc_server_unrestricted_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-03-28 17:29:31.000000 precli-0.4.3/tests/unit/rules/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-03-28 17:29:31.000000 precli-0.4.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.754189 precli-0.4.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.658188 precli-0.4.4/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-02 19:20:15.000000 precli-0.4.4/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-02 19:20:15.000000 precli-0.4.4/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.658188 precli-0.4.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-02 19:20:15.000000 precli-0.4.4/.github/workflows/dependency-review.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-02 19:20:15.000000 precli-0.4.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-02 19:20:15.000000 precli-0.4.4/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-04-02 19:20:15.000000 precli-0.4.4/.github/workflows/unit-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-02 19:20:15.000000 precli-0.4.4/.github/workflows/upload-asset.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-04-02 19:20:15.000000 precli-0.4.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-02 19:20:15.000000 precli-0.4.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-04-02 19:20:15.000000 precli-0.4.4/.stestr.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-02 19:20:18.000000 precli-0.4.4/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-04-02 19:20:15.000000 precli-0.4.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-02 19:20:18.000000 precli-0.4.4/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-04-02 19:20:15.000000 precli-0.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-02 19:20:18.754189 precli-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-02 19:20:15.000000 precli-0.4.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-04-02 19:20:15.000000 precli-0.4.4/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.658188 precli-0.4.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-02 19:20:15.000000 precli-0.4.4/docs/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-02 19:20:15.000000 precli-0.4.4/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.658188 precli-0.4.4/docs/man/
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-02 19:20:15.000000 precli-0.4.4/docs/man/precli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 19:20:15.000000 precli-0.4.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.646188 precli-0.4.4/docs/rules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.646188 precli-0.4.4/docs/rules/go/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.658188 precli-0.4.4/docs/rules/go/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/go/stdlib/crypto-weak-cipher.md
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/go/stdlib/crypto-weak-hash.md
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/go/stdlib/crypto-weak-key.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.646188 precli-0.4.4/docs/rules/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.666189 precli-0.4.4/docs/rules/python/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/argparse-sensitive-info.md
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/assert.md
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/crypt-weak-hash.md
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/ftplib-cleartext.md
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/ftplib-unverified-context.md
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/hashlib-improper-prng.md
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/hashlib-weak-hash.md
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/hmac-timing-attack.md
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/hmac-weak-hash.md
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/hmac-weak-key.md
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/http-server-unrestricted-bind.md
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/http-url-secret.md
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/imaplib-cleartext.md
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/imaplib-unverified-context.md
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/json-load.md
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/logging-insecure-listen-config.md
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/marshal-load.md
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/nntplib-cleartext.md
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/nntplib-unverified-context.md
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/pickle-load.md
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/poplib-cleartext.md
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/poplib-unverified-context.md
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/re-denial-of-service.md
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/secrets-weak-token.md
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/shelve-open.md
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/smtplib-cleartext.md
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/smtplib-unverified-context.md
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/socket-unrestricted-bind.md
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/socketserver-unrestricted-bind.md
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/ssl-context-weak-key.md
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/ssl-create-unverified-context.md
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/ssl-insecure-tls-version.md
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/telnetlib-cleartext.md
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/tempfile-mktemp-race-condition.md
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules/python/stdlib/xmlrpc-server-unrestricted-bind.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5482 2024-04-02 19:20:15.000000 precli-0.4.4/docs/rules.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.666189 precli-0.4.4/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)    47438 2024-04-02 19:20:15.000000 precli-0.4.4/logo/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-02 19:20:15.000000 precli-0.4.4/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.666189 precli-0.4.4/precli/
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-02 19:20:15.000000 precli-0.4.4/precli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-02 19:20:15.000000 precli-0.4.4/precli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.666189 precli-0.4.4/precli/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/precli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10978 2024-04-02 19:20:15.000000 precli-0.4.4/precli/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.670189 precli-0.4.4/precli/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/precli/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-04-02 19:20:15.000000 precli-0.4.4/precli/core/argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-02 19:20:15.000000 precli-0.4.4/precli/core/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4479 2024-04-02 19:20:15.000000 precli-0.4.4/precli/core/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-04-02 19:20:15.000000 precli-0.4.4/precli/core/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-02 19:20:15.000000 precli-0.4.4/precli/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-02 19:20:15.000000 precli-0.4.4/precli/core/fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-04-02 19:20:15.000000 precli-0.4.4/precli/core/kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-02 19:20:15.000000 precli-0.4.4/precli/core/level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-02 19:20:15.000000 precli-0.4.4/precli/core/linecache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-02 19:20:15.000000 precli-0.4.4/precli/core/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-02 19:20:15.000000 precli-0.4.4/precli/core/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-02 19:20:15.000000 precli-0.4.4/precli/core/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9636 2024-04-02 19:20:15.000000 precli-0.4.4/precli/core/redos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-02 19:20:15.000000 precli-0.4.4/precli/core/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5426 2024-04-02 19:20:15.000000 precli-0.4.4/precli/core/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-02 19:20:15.000000 precli-0.4.4/precli/core/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-02 19:20:15.000000 precli-0.4.4/precli/core/suppression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-02 19:20:15.000000 precli-0.4.4/precli/core/symtab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-04-02 19:20:15.000000 precli-0.4.4/precli/core/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-02 19:20:15.000000 precli-0.4.4/precli/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.670189 precli-0.4.4/precli/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-04-02 19:20:15.000000 precli-0.4.4/precli/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6909 2024-04-02 19:20:15.000000 precli-0.4.4/precli/parsers/go.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-02 19:20:15.000000 precli-0.4.4/precli/parsers/java.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16850 2024-04-02 19:20:15.000000 precli-0.4.4/precli/parsers/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-04-02 19:20:15.000000 precli-0.4.4/precli/parsers/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.674188 precli-0.4.4/precli/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-02 19:20:15.000000 precli-0.4.4/precli/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5744 2024-04-02 19:20:15.000000 precli-0.4.4/precli/renderers/detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6287 2024-04-02 19:20:15.000000 precli-0.4.4/precli/renderers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-04-02 19:20:15.000000 precli-0.4.4/precli/renderers/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-02 19:20:15.000000 precli-0.4.4/precli/renderers/plain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.674188 precli-0.4.4/precli/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)     4314 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.674188 precli-0.4.4/precli/rules/go/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/go/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.674188 precli-0.4.4/precli/rules/go/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/go/stdlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5476 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/go/stdlib/crypto_weak_cipher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/go/stdlib/crypto_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/go/stdlib/crypto_weak_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.674188 precli-0.4.4/precli/rules/java/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.674188 precli-0.4.4/precli/rules/java/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/java/stdlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.674188 precli-0.4.4/precli/rules/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.678188 precli-0.4.4/precli/rules/python/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/argparse_sensitive_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/assert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/crypt_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/ftplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3285 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/ftplib_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4834 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/hashlib_improper_prng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/hashlib_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/hmac_timing_attack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6580 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/hmac_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6813 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/hmac_weak_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/http_server_unrestricted_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/http_url_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3473 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/imaplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3717 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/imaplib_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/json_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2229 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/logging_insecure_listen_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/marshal_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/nntplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/nntplib_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2696 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/pickle_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3329 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/poplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/poplib_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/re_denial_of_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/secrets_weak_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2085 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/shelve_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4036 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/smtplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3676 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/smtplib_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3359 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/socket_unrestricted_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/socketserver_unrestricted_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3541 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/ssl_context_weak_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/ssl_create_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6515 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/ssl_insecure_tls_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4246 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/telnetlib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6125 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/tempfile_mktemp_race_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-04-02 19:20:15.000000 precli-0.4.4/precli/rules/python/stdlib/xmlrpc_server_unrestricted_bind.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.754189 precli-0.4.4/precli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-04-02 19:20:18.000000 precli-0.4.4/precli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    36404 2024-04-02 19:20:18.000000 precli-0.4.4/precli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:20:18.000000 precli-0.4.4/precli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2024-04-02 19:20:18.000000 precli-0.4.4/precli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 19:20:18.000000 precli-0.4.4/precli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-02 19:20:18.000000 precli-0.4.4/precli.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-02 19:20:18.000000 precli-0.4.4/precli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-02 19:20:18.000000 precli-0.4.4/precli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-02 19:20:15.000000 precli-0.4.4/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-02 19:20:15.000000 precli-0.4.4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.678188 precli-0.4.4/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)       94 2024-04-02 19:20:15.000000 precli-0.4.4/scripts/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-04-02 19:20:18.754189 precli-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-02 19:20:15.000000 precli-0.4.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-02 19:20:15.000000 precli-0.4.4/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.678188 precli-0.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.682189 precli-0.4.4/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.682189 precli-0.4.4/tests/unit/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.682189 precli-0.4.4/tests/unit/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/core/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.682189 precli-0.4.4/tests/unit/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.682189 precli-0.4.4/tests/unit/parsers/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/parsers/examples/expression_list_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/parsers/examples/importlib_import_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/parsers/examples/suppress.go
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/parsers/examples/suppress.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/parsers/examples/suppress_lowercase_rule.go
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/parsers/examples/suppress_lowercase_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/parsers/examples/suppress_multiline.go
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/parsers/examples/suppress_multiline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/parsers/examples/suppress_multiple_comments.go
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/parsers/examples/suppress_multiple_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/parsers/examples/suppress_multiple_rules.go
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/parsers/examples/suppress_multiple_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/parsers/examples/suppress_preceding.go
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/parsers/examples/suppress_preceding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/parsers/examples/suppress_spaced_rules.go
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/parsers/examples/suppress_spaced_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/parsers/examples/suppress_wrong_rule.go
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/parsers/examples/suppress_wrong_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5514 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/parsers/test_go.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6022 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/parsers/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.686189 precli-0.4.4/tests/unit/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.686189 precli-0.4.4/tests/unit/rules/go/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/go/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.686189 precli-0.4.4/tests/unit/rules/go/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/go/stdlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.686189 precli-0.4.4/tests/unit/rules/go/stdlib/crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/go/stdlib/crypto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.686189 precli-0.4.4/tests/unit/rules/go/stdlib/crypto/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_aes.go
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_des.go
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_rc4.go
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_md5_new.go
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_md5_sum.go
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha1_new.go
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha1_sum.go
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha256_new.go
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha256_sum.go
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_1024.go
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_2048.go
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_3072.go
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_1024.go
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_2048.go
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_4096.go
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_bits_as_var.go
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_cipher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1536 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.690189 precli-0.4.4/tests/unit/rules/java/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.690189 precli-0.4.4/tests/unit/rules/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.690189 precli-0.4.4/tests/unit/rules/python/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.690189 precli-0.4.4/tests/unit/rules/python/stdlib/argparse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/argparse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.690189 precli-0.4.4/tests/unit/rules/python/stdlib/argparse/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_default_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_password_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_password_store_true.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/argparse/test_argparse_sensitive_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.690189 precli-0.4.4/tests/unit/rules/python/stdlib/assert/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/assert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.690189 precli-0.4.4/tests/unit/rules/python/stdlib/assert/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/assert/examples/assert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/assert/test_assert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.690189 precli-0.4.4/tests/unit/rules/python/stdlib/crypt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/crypt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.694189 precli-0.4.4/tests/unit/rules/python/stdlib/crypt/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_blowfish.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_blowfish.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/crypt/test_crypt_weak_hash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.694189 precli-0.4.4/tests/unit/rules/python/stdlib/ftplib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ftplib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.694189 precli-0.4.4/tests/unit/rules/python/stdlib/ftplib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ftplib/examples/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ftplib/examples/ftp_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ftplib/examples/ftp_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ftplib/examples/ftp_tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_login_single_statement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_user_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_user_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ftplib/test_ftplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ftplib/test_ftplib_unverified_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.698189 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.706189 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_pbkdf2_hmac.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_scrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5_as_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5_importlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5_usedforsecurity_true.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md5_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md5_usedforsecurity_true.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_name_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha_usedforsecurity_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha_usedforsecurity_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/test_hashlib_improper_prng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3456 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/test_hashlib_weak_hash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.706189 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.722189 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_md5_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_hashlib_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_hashlib_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_hashlib_sm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_md5_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_hashlib_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_hashlib_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_hashlib_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_sha512_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack_class_hexdigest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack_compare_digest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/test_hmac_timing_attack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4375 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.722189 precli-0.4.4/tests/unit/rules/python/stdlib/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.722189 precli-0.4.4/tests/unit/rules/python/stdlib/http/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/http/examples/http_server_http_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/http/examples/http_server_threading_http_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/http/examples/http_url_secret_apikey.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/http/examples/http_url_secret_apikey_in_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/http/examples/http_url_secret_basic_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/http/examples/http_url_secret_basic_auth_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/http/examples/http_url_secret_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/http/examples/http_url_secret_username.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/http/test_http_server_unrestricted_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/http/test_http_url_secret.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.722189 precli-0.4.4/tests/unit/rules/python/stdlib/imaplib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/imaplib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.726189 precli-0.4.4/tests/unit/rules/python/stdlib/imaplib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_login_cram_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/imaplib/test_imaplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/imaplib/test_imaplib_unverified_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.726189 precli-0.4.4/tests/unit/rules/python/stdlib/json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/json/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.726189 precli-0.4.4/tests/unit/rules/python/stdlib/json/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/json/examples/json_jsondecoder_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/json/examples/json_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/json/examples/json_loads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/json/test_json_load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.726189 precli-0.4.4/tests/unit/rules/python/stdlib/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.726189 precli-0.4.4/tests/unit/rules/python/stdlib/logging/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_empty_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_port_verify_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_port_verify_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_verify_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_verify_none_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_verify_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/logging/test_logging_insecure_listen_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.730189 precli-0.4.4/tests/unit/rules/python/stdlib/marshal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/marshal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.730189 precli-0.4.4/tests/unit/rules/python/stdlib/marshal/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/marshal/examples/marshal_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/marshal/examples/marshal_loads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/marshal/test_marshal_load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.730189 precli-0.4.4/tests/unit/rules/python/stdlib/nntplib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/nntplib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.730189 precli-0.4.4/tests/unit/rules/python/stdlib/nntplib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/nntplib/test_nntplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/nntplib/test_nntplib_unverified_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.730189 precli-0.4.4/tests/unit/rules/python/stdlib/pickle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/pickle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.730189 precli-0.4.4/tests/unit/rules/python/stdlib/pickle/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/pickle/examples/pickle_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/pickle/examples/pickle_loads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/pickle/examples/pickle_unpickler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/pickle/test_pickle_load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.730189 precli-0.4.4/tests/unit/rules/python/stdlib/poplib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/poplib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.734189 precli-0.4.4/tests/unit/rules/python/stdlib/poplib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_apop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_pass_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_rpop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/poplib/test_poplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/poplib/test_poplib_unverified_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.734189 precli-0.4.4/tests/unit/rules/python/stdlib/re/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/re/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.738189 precli-0.4.4/tests/unit/rules/python/stdlib/re/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/re/examples/re_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/re/examples/re_compile_good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/re/examples/re_findall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/re/examples/re_finditer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/re/examples/re_fullmatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/re/examples/re_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/re/examples/re_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/re/examples/re_search_good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/re/examples/re_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/re/examples/re_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/re/examples/re_subn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/re/test_re_denial_of_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.738189 precli-0.4.4/tests/unit/rules/python/stdlib/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.738189 precli-0.4.4/tests/unit/rules/python/stdlib/secrets/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_bytes_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_bytes_size_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_hex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_urlsafe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/secrets/test_secrets_weak_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.738189 precli-0.4.4/tests/unit/rules/python/stdlib/shelve/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/shelve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.738189 precli-0.4.4/tests/unit/rules/python/stdlib/shelve/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/shelve/examples/shelve_dbfilenameshelf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/shelve/examples/shelve_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/shelve/examples/shelve_open_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/shelve/test_shelve_open.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.738189 precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.742189 precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/test_smtplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/test_smtplib_unverified_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.742189 precli-0.4.4/tests/unit/rules/python/stdlib/socket/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/socket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.742189 precli-0.4.4/tests/unit/rules/python/stdlib/socket/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/socket/examples/socket_create_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/socket/examples/socket_socket_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/socket/examples/socket_socket_bind_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/socket/examples/socket_socket_bind_as_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/socket/test_socket_unrestricted_bind.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.742189 precli-0.4.4/tests/unit/rules/python/stdlib/socketserver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/socketserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.742189 precli-0.4.4/tests/unit/rules/python/stdlib/socketserver/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_tcp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_udp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_tcp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_tcp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_udp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_udp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1541 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/socketserver/test_socketserver_unrestricted_bind.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.742189 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.750189 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/create_default_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/create_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_sslv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_sslv23.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_sslv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_tlsv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_tlsv11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_tlsv12.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP256r1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP384r1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP384r1tls13.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP512r1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_default_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_ffdhe2048.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_prime192v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_prime256v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_secp160r2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_secp256r1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_sect163k1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_sect571k1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_typed_default_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_typed_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_sslv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_sslv23.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_sslv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_tlsv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_tlsv11.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_tlsv12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv23.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv2_server_side_true.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_tlsv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_tlsv11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_tlsv12.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/test_ssl_context_tls_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2127 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/test_ssl_context_weak_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/test_ssl_create_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/test_ssl_get_server_certificate_tls_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/ssl/test_ssl_wrap_socket_tls_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.750189 precli-0.4.4/tests/unit/rules/python/stdlib/telnetlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/telnetlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.750189 precli-0.4.4/tests/unit/rules/python/stdlib/telnetlib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/telnetlib/examples/telnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/telnetlib/examples/telnetlib_telnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/telnetlib/examples/telnetlib_telnet_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/telnetlib/test_telnetlib_cleartext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.750189 precli-0.4.4/tests/unit/rules/python/stdlib/tempfile/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/tempfile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.750189 precli-0.4.4/tests/unit/rules/python/stdlib/tempfile/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_args_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_args_with_open_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_walrus_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_with_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_with_open_multiline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/tempfile/test_tempfile_mktemp_race_condition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.750189 precli-0.4.4/tests/unit/rules/python/stdlib/xmlrpc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/xmlrpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 19:20:18.754189 precli-0.4.4/tests/unit/rules/python/stdlib/xmlrpc/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/xmlrpc/examples/xmlrpc_server_doc_xml_rpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/xmlrpc/examples/xmlrpc_server_simple_xml_rpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/python/stdlib/xmlrpc/test_xmlrpc_server_unrestricted_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-02 19:20:15.000000 precli-0.4.4/tests/unit/rules/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-02 19:20:15.000000 precli-0.4.4/tox.ini
```

### Comparing `precli-0.4.3/.github/workflows/dependency-review.yml` & `precli-0.4.4/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/.github/workflows/publish-to-pypi.yml` & `precli-0.4.4/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/.github/workflows/publish-to-test-pypi.yml` & `precli-0.4.4/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/.github/workflows/unit-test.yml` & `precli-0.4.4/.github/workflows/unit-test.yml`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/.github/workflows/upload-asset.yml` & `precli-0.4.4/.github/workflows/upload-asset.yml`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/.pre-commit-config.yaml` & `precli-0.4.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/CODE_OF_CONDUCT.md` & `precli-0.4.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/ChangeLog` & `precli-0.4.4/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 CHANGES
 =======
 
+0.4.4
+-----
+
+* Fix for IndexError in an expression list assignment (#408)
+* Fix traceback from usage of importlib.import\_module (#406)
+* Add suggested fixes for weak hashes in hmac function (#404)
+* Add suggested fixes for the hashlib weak hash rule (#403)
+* Add dependabot checks for PyPI packages (#402)
+* Do update check only if git target or gist output (#401)
+
 0.4.3
 -----
 
 * Check for no action passed in argparse rule (#396)
 * Bump tree-sitter to version 0.21.3 (#395)
 * Add rule to check for improper random generator usage (#394)
 * Correct invalid examples for hmac timing attack (#393)
```

### Comparing `precli-0.4.3/LICENSE` & `precli-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/PKG-INFO` & `precli-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: precli
-Version: 0.4.3
+Version: 0.4.4
 Summary: Static analysis security tool command line
 Home-page: https://github.com/securesauce/precli
 Download-URL: https://pypi.org/project/precli/#files
 Author: Secure Sauce
 Project-URL: Release notes, https://github.com/securesauce/precli/releases
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `precli-0.4.3/README.rst` & `precli-0.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/SECURITY.md` & `precli-0.4.4/SECURITY.md`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/docs/getting-started.md` & `precli-0.4.4/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/docs/man/precli.rst` & `precli-0.4.4/docs/man/precli.rst`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/docs/rules.md` & `precli-0.4.4/docs/rules.md`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/logo/logo.png` & `precli-0.4.4/logo/logo.png`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/cli/main.py` & `precli-0.4.4/precli/cli/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 from precli.core.tool import Tool
 from precli.renderers.detailed import Detailed
 from precli.renderers.json import Json
 from precli.renderers.markdown import Markdown
 from precli.renderers.plain import Plain
 
 
+GITHUB_URL = "https://github.com"
+
+
 def setup_arg_parser():
     parser = argparse.ArgumentParser(
         description="precli - a static analysis security tool",
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
 
     parser.add_argument(
@@ -184,22 +187,22 @@
 
 
 def file_to_url(owner, repo, branch, target, root, file):
     target_len = len(target)
     prefix = root[target_len:].lstrip("/")
     urlpath = f"{owner}/{repo}/blob/{branch}"
     rel_path = "/".join([urlpath, prefix, file])
-    return urljoin("https://github.com", rel_path)
+    return urljoin(GITHUB_URL, rel_path)
 
 
 def discover_files(targets: list[str], recursive: bool):
     artifacts = []
 
     for target in targets:
-        if target.startswith("https://github.com"):
+        if target.startswith(GITHUB_URL):
             owner, repo = get_owner_repo(target)
             if repo:
                 try:
                     branch = get_default_branch(owner, repo)
                     target = extract_github_repo(owner, repo, branch)
                 except requests.exceptions.ConnectionError:
                     owner = None
@@ -300,15 +303,17 @@
     )
     logging.getLogger("urllib3").setLevel(debug)
 
     # Setup the command line arguments
     args = setup_arg_parser()
 
     # Check if a newer version is available
-    if args.quiet is False:
+    git_target = any(filter(lambda x: x.startswith(GITHUB_URL), args.targets))
+
+    if (git_target or args.gist) and not args.quiet:
         check_for_update()
 
     enabled = args.enable.split(",") if args.enable else []
     disabled = args.disable.split(",") if args.disable else []
     parsers = loader.load_parsers(enabled, disabled)
 
     # Compile a list of the targets
```

### Comparing `precli-0.4.3/precli/core/argument.py` & `precli-0.4.4/precli/core/argument.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/core/artifact.py` & `precli-0.4.4/precli/core/artifact.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/core/call.py` & `precli-0.4.4/precli/core/call.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/core/comparison.py` & `precli-0.4.4/precli/core/comparison.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/core/config.py` & `precli-0.4.4/precli/core/config.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/core/fix.py` & `precli-0.4.4/precli/core/fix.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/core/kind.py` & `precli-0.4.4/precli/core/kind.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/core/level.py` & `precli-0.4.4/precli/core/level.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/core/linecache.py` & `precli-0.4.4/precli/core/linecache.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/core/location.py` & `precli-0.4.4/precli/core/location.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/core/metrics.py` & `precli-0.4.4/precli/core/metrics.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/core/redos.py` & `precli-0.4.4/precli/core/redos.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/core/result.py` & `precli-0.4.4/precli/core/result.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/core/run.py` & `precli-0.4.4/precli/core/run.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/core/suppression.py` & `precli-0.4.4/precli/core/suppression.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/core/symtab.py` & `precli-0.4.4/precli/core/symtab.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/core/tool.py` & `precli-0.4.4/precli/core/tool.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/core/utils.py` & `precli-0.4.4/precli/core/utils.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/parsers/__init__.py` & `precli-0.4.4/precli/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/parsers/go.py` & `precli-0.4.4/precli/parsers/go.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/parsers/python.py` & `precli-0.4.4/precli/parsers/python.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,14 +88,15 @@
             self.visit(nodes)
 
     def visit_assignment(self, nodes: list[Node]):
         # pattern_list = expression_list (i.e. HOST, PORT = "", 9999)
         if (
             nodes[0].type == tokens.PATTERN_LIST
             and nodes[2].type == tokens.EXPRESSION_LIST
+            and len(nodes[0].named_children) == len(nodes[2].named_children)
         ):
             for i in range(len(nodes[0].named_children)):
                 self.visit_assignment(
                     [
                         nodes[0].named_children[i],
                         nodes[1],
                         nodes[2].named_children[i],
@@ -154,18 +155,19 @@
         )
 
         if (
             call.name_qualified == "importlib.import_module"
             and self.context["node"].parent.type == tokens.ASSIGNMENT
         ):
             module = self.importlib_import_module(call)
-            left_hand = self.context["node"].parent.children[0]
-            identifier = left_hand.text.decode()
-            self.current_symtab.remove(identifier)
-            self.current_symtab.put(identifier, tokens.IMPORT, module)
+            if module:
+                left_hand = self.context["node"].parent.children[0]
+                identifier = left_hand.text.decode()
+                self.current_symtab.remove(identifier)
+                self.current_symtab.put(identifier, tokens.IMPORT, module)
 
         self.analyze_node(self.context["node"].type, call=call)
 
         if call.var_node is not None:
             symbol = self.current_symtab.get(call.var_node.text.decode())
             if symbol is not None and symbol.type == tokens.IDENTIFIER:
                 symbol.push_call(call)
@@ -310,16 +312,18 @@
         for imp in imports[1]:
             if imp.alias is not None:
                 modules.append(imp.module + " as " + imp.alias)
             else:
                 modules.append(imp.module)
         return f"from {package} import {', '.join(modules)}"
 
-    def importlib_import_module(self, call: Call) -> dict:
+    def importlib_import_module(self, call: Call) -> str:
         name = call.get_argument(position=0, name="name").value_str
+        if name is None:
+            return None
         package = call.get_argument(position=1, name="package").value_str
         if package is None:
             return name
         subpkg = len(name) - len(name.lstrip(".")) - 1
         package = package.rsplit(".", subpkg)
         return ".".join((package[0], name.lstrip(".")))
```

### Comparing `precli-0.4.3/precli/parsers/tokens.py` & `precli-0.4.4/precli/parsers/tokens.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/renderers/__init__.py` & `precli-0.4.4/precli/renderers/__init__.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/renderers/detailed.py` & `precli-0.4.4/precli/renderers/detailed.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/renderers/json.py` & `precli-0.4.4/precli/renderers/json.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/renderers/markdown.py` & `precli-0.4.4/precli/renderers/markdown.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/renderers/plain.py` & `precli-0.4.4/precli/renderers/plain.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/__init__.py` & `precli-0.4.4/precli/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/go/stdlib/crypto_weak_cipher.py` & `precli-0.4.4/precli/rules/go/stdlib/crypto_weak_cipher.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/go/stdlib/crypto_weak_hash.py` & `precli-0.4.4/precli/rules/go/stdlib/crypto_weak_hash.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/go/stdlib/crypto_weak_key.py` & `precli-0.4.4/precli/rules/go/stdlib/crypto_weak_key.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/argparse_sensitive_info.py` & `precli-0.4.4/precli/rules/python/stdlib/argparse_sensitive_info.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/assert.py` & `precli-0.4.4/precli/rules/python/stdlib/assert.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/crypt_weak_hash.py` & `precli-0.4.4/precli/rules/python/stdlib/crypt_weak_hash.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/ftplib_cleartext.py` & `precli-0.4.4/precli/rules/python/stdlib/ftplib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/ftplib_unverified_context.py` & `precli-0.4.4/precli/rules/python/stdlib/ftplib_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/hashlib_improper_prng.py` & `precli-0.4.4/precli/rules/python/stdlib/hashlib_improper_prng.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/hashlib_weak_hash.py` & `precli-0.4.4/precli/rules/python/stdlib/hashlib_weak_hash.py`

 * *Files 15% similar despite different names*

```diff
@@ -94,16 +94,16 @@
 class HashlibWeakHash(Rule):
     def __init__(self, id: str):
         super().__init__(
             id=id,
             name="reversible_one_way_hash",
             description=__doc__,
             cwe_id=328,
-            message="Use of weak hash function '{0}' does not meet security "
-            "expectations.",
+            message="The hash function '{0}' is vulnerable to collision and "
+            "pre-image attacks.",
             wildcards={
                 "hashlib.*": [
                     "md4",
                     "md5",
                     "ripemd160",
                     "sha",
                     "sha1",
@@ -123,45 +123,73 @@
             hashlib.sha1(string=b'', *, usedforsecurity=True)
             """
             used_for_security = call.get_argument(
                 name="usedforsecurity", default=Argument(None, True)
             ).value
 
             if used_for_security is True:
+                fixes = Rule.get_fixes(
+                    context=context,
+                    deleted_location=Location(node=call.identifier_node),
+                    description="For cryptographic purposes, use a hash length"
+                    " of at least 256-bits with hashes such as SHA-256.",
+                    inserted_content="sha256",
+                )
+
                 return Result(
                     rule_id=self.id,
-                    location=Location(node=call.function_node),
+                    location=Location(node=call.identifier_node),
                     message=self.message.format(call.name_qualified),
+                    fixes=fixes,
                 )
         elif call.name_qualified in ["hashlib.pbkdf2_hmac"]:
             """
             hashlib.pbkdf2_hmac(
                 hash_name,
                 password,
                 salt,
                 iterations,
                 dklen=None
             )
             """
             argument = call.get_argument(position=0, name="hash_name")
 
             if argument.is_str and argument.value_str.lower() in WEAK_HASHES:
+                fixes = Rule.get_fixes(
+                    context=context,
+                    deleted_location=Location(node=argument.node),
+                    description="For cryptographic purposes, use a hash length"
+                    " of at least 256-bits with hashes such as SHA-256.",
+                    inserted_content='"sha256"',
+                )
+
                 return Result(
                     rule_id=self.id,
-                    location=Location(node=call.function_node),
+                    location=Location(node=argument.node),
                     message=self.message.format(argument.value_str),
+                    fixes=fixes,
                 )
         elif call.name_qualified in ["hashlib.new"]:
             # hashlib.new(name, data=b'', **kwargs)
             argument = call.get_argument(position=0, name="name")
 
             if argument.is_str and argument.value_str.lower() in WEAK_HASHES:
                 used_for_security = call.get_argument(
                     name="usedforsecurity", default=Argument(None, True)
                 ).value
 
                 if used_for_security is True:
+                    fixes = Rule.get_fixes(
+                        context=context,
+                        deleted_location=Location(node=argument.node),
+                        description="For cryptographic purposes, use a hash "
+                        "length of at least 256-bits with hashes such as "
+                        "SHA-256.",
+                        inserted_content='"sha256"',
+                    )
+
                     return Result(
                         rule_id=self.id,
-                        location=Location(node=call.function_node),
+                        location=Location(node=argument.node),
                         message=self.message.format(argument.value_str),
+                        fixes=fixes,
                     )
```

### Comparing `precli-0.4.3/precli/rules/python/stdlib/hmac_timing_attack.py` & `precli-0.4.4/precli/rules/python/stdlib/hmac_timing_attack.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/hmac_weak_hash.py` & `precli-0.4.4/precli/rules/python/stdlib/hmac_weak_hash.py`

 * *Files 20% similar despite different names*

```diff
@@ -87,16 +87,16 @@
 class HmacWeakHash(Rule):
     def __init__(self, id: str):
         super().__init__(
             id=id,
             name="reversible_one_way_hash",
             description=__doc__,
             cwe_id=328,
-            message="Use of weak hash function '{0}' does not meet security "
-            "expectations.",
+            message="The hash function '{0}' is vulnerable to collision and "
+            "pre-image attacks.",
             wildcards={
                 "hashlib.*": [
                     "md4",
                     "md5",
                     "ripemd160",
                     "sha",
                     "sha1",
@@ -111,34 +111,66 @@
 
     def analyze_call(self, context: dict, call: Call) -> Result:
         if call.name_qualified in ["hmac.new"]:
             # hmac.new(key, msg=None, digestmod='')
             argument = call.get_argument(position=2, name="digestmod")
 
             if argument.is_str and argument.value_str.lower() in WEAK_HASHES:
+                fixes = Rule.get_fixes(
+                    context=context,
+                    deleted_location=Location(node=argument.node),
+                    description="For cryptographic purposes, use a hash length"
+                    " of at least 256-bits with hashes such as SHA-256.",
+                    inserted_content='"sha256"',
+                )
                 return Result(
                     rule_id=self.id,
                     location=Location(node=argument.node),
                     message=self.message.format(argument.value_str),
+                    fixes=fixes,
                 )
             if argument.value in HASHLIB_WEAK_HASHES:
+                fixes = Rule.get_fixes(
+                    context=context,
+                    deleted_location=Location(node=argument.node),
+                    description="For cryptographic purposes, use a hash length"
+                    " of at least 256-bits with hashes such as SHA-256.",
+                    inserted_content="hashlib.sha256",
+                )
                 return Result(
                     rule_id=self.id,
                     location=Location(node=argument.node),
                     message=self.message.format(argument.value),
+                    fixes=fixes,
                 )
         elif call.name_qualified in ["hmac.digest"]:
             # hmac.digest(key, msg, digest)
             argument = call.get_argument(position=2, name="digest")
 
             if argument.is_str and argument.value_str.lower() in WEAK_HASHES:
+                fixes = Rule.get_fixes(
+                    context=context,
+                    deleted_location=Location(node=argument.node),
+                    description="For cryptographic purposes, use a hash length"
+                    " of at least 256-bits with hashes such as SHA-256.",
+                    inserted_content='"sha256"',
+                )
                 return Result(
                     rule_id=self.id,
                     location=Location(node=argument.node),
                     message=self.message.format(argument.value_str),
+                    fixes=fixes,
                 )
             if argument.value in HASHLIB_WEAK_HASHES:
+                fixes = Rule.get_fixes(
+                    context=context,
+                    deleted_location=Location(node=argument.node),
+                    description="For cryptographic purposes, use a hash length"
+                    " of at least 256-bits with hashes such as SHA-256.",
+                    inserted_content="hashlib.sha256",
+                )
                 return Result(
                     rule_id=self.id,
                     location=Location(node=argument.node),
                     message=self.message.format(argument.value),
+                    fixes=fixes,
                 )
```

### Comparing `precli-0.4.3/precli/rules/python/stdlib/hmac_weak_key.py` & `precli-0.4.4/precli/rules/python/stdlib/hmac_weak_key.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/http_server_unrestricted_bind.py` & `precli-0.4.4/precli/rules/python/stdlib/http_server_unrestricted_bind.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/http_url_secret.py` & `precli-0.4.4/precli/rules/python/stdlib/http_url_secret.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/imaplib_cleartext.py` & `precli-0.4.4/precli/rules/python/stdlib/imaplib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/imaplib_unverified_context.py` & `precli-0.4.4/precli/rules/python/stdlib/imaplib_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/json_load.py` & `precli-0.4.4/precli/rules/python/stdlib/json_load.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/logging_insecure_listen_config.py` & `precli-0.4.4/precli/rules/python/stdlib/logging_insecure_listen_config.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/marshal_load.py` & `precli-0.4.4/precli/rules/python/stdlib/marshal_load.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/nntplib_cleartext.py` & `precli-0.4.4/precli/rules/python/stdlib/nntplib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/nntplib_unverified_context.py` & `precli-0.4.4/precli/rules/python/stdlib/nntplib_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/pickle_load.py` & `precli-0.4.4/precli/rules/python/stdlib/pickle_load.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/poplib_cleartext.py` & `precli-0.4.4/precli/rules/python/stdlib/poplib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/poplib_unverified_context.py` & `precli-0.4.4/precli/rules/python/stdlib/poplib_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/re_denial_of_service.py` & `precli-0.4.4/precli/rules/python/stdlib/re_denial_of_service.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/secrets_weak_token.py` & `precli-0.4.4/precli/rules/python/stdlib/secrets_weak_token.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/shelve_open.py` & `precli-0.4.4/precli/rules/python/stdlib/shelve_open.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/smtplib_cleartext.py` & `precli-0.4.4/precli/rules/python/stdlib/smtplib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/smtplib_unverified_context.py` & `precli-0.4.4/precli/rules/python/stdlib/smtplib_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/socket_unrestricted_bind.py` & `precli-0.4.4/precli/rules/python/stdlib/socket_unrestricted_bind.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/socketserver_unrestricted_bind.py` & `precli-0.4.4/precli/rules/python/stdlib/socketserver_unrestricted_bind.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/ssl_context_weak_key.py` & `precli-0.4.4/precli/rules/python/stdlib/ssl_context_weak_key.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/ssl_create_unverified_context.py` & `precli-0.4.4/precli/rules/python/stdlib/ssl_create_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/ssl_insecure_tls_version.py` & `precli-0.4.4/precli/rules/python/stdlib/ssl_insecure_tls_version.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/telnetlib_cleartext.py` & `precli-0.4.4/precli/rules/python/stdlib/telnetlib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/tempfile_mktemp_race_condition.py` & `precli-0.4.4/precli/rules/python/stdlib/tempfile_mktemp_race_condition.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli/rules/python/stdlib/xmlrpc_server_unrestricted_bind.py` & `precli-0.4.4/precli/rules/python/stdlib/xmlrpc_server_unrestricted_bind.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/precli.egg-info/PKG-INFO` & `precli-0.4.4/precli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: precli
-Version: 0.4.3
+Version: 0.4.4
 Summary: Static analysis security tool command line
 Home-page: https://github.com/securesauce/precli
 Download-URL: https://pypi.org/project/precli/#files
 Author: Secure Sauce
 Project-URL: Release notes, https://github.com/securesauce/precli/releases
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `precli-0.4.3/precli.egg-info/SOURCES.txt` & `precli-0.4.4/precli.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -158,14 +158,16 @@
 tests/unit/__init__.py
 tests/unit/cli/__init__.py
 tests/unit/core/__init__.py
 tests/unit/core/test_python.py
 tests/unit/parsers/__init__.py
 tests/unit/parsers/test_go.py
 tests/unit/parsers/test_python.py
+tests/unit/parsers/examples/expression_list_assignment.py
+tests/unit/parsers/examples/importlib_import_module.py
 tests/unit/parsers/examples/suppress.go
 tests/unit/parsers/examples/suppress.py
 tests/unit/parsers/examples/suppress_lowercase_rule.go
 tests/unit/parsers/examples/suppress_lowercase_rule.py
 tests/unit/parsers/examples/suppress_multiline.go
 tests/unit/parsers/examples/suppress_multiline.py
 tests/unit/parsers/examples/suppress_multiple_comments.go
```

### Comparing `precli-0.4.3/precli.egg-info/entry_points.txt` & `precli-0.4.4/precli.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/pylintrc` & `precli-0.4.4/pylintrc`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/setup.cfg` & `precli-0.4.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/parsers/test_go.py` & `precli-0.4.4/tests/unit/parsers/test_go.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import testtools
 
 from precli.core.artifact import Artifact
 from precli.core.level import Level
 from precli.parsers import go
 
 
-class TestCase(testtools.TestCase):
+class GoTestCase(testtools.TestCase):
     def setUp(self):
         super().setUp()
         self.parser = go.Go()
         self.base_path = os.path.join(
             "tests",
             "unit",
             "parsers",
```

### Comparing `precli-0.4.3/tests/unit/parsers/test_python.py` & `precli-0.4.4/tests/unit/parsers/test_python.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,49 +4,63 @@
 import testtools
 
 from precli.core.artifact import Artifact
 from precli.core.level import Level
 from precli.parsers import python
 
 
-class TestCase(testtools.TestCase):
+class PythonTestCase(testtools.TestCase):
     def setUp(self):
         super().setUp()
         self.parser = python.Python()
         self.base_path = os.path.join(
             "tests",
             "unit",
             "parsers",
             "examples",
         )
 
+    def test_expression_list_assignment(self):
+        artifact = Artifact(
+            os.path.join(self.base_path, "expression_list_assignment.py")
+        )
+        results = self.parser.parse(artifact)
+        self.assertEqual(0, len(results))
+
+    def test_importlib_import_module(self):
+        artifact = Artifact(
+            os.path.join(self.base_path, "importlib_import_module.py")
+        )
+        results = self.parser.parse(artifact)
+        self.assertEqual(0, len(results))
+
     def test_suppress(self):
         artifact = Artifact(os.path.join(self.base_path, "suppress.py"))
         results = self.parser.parse(artifact)
         self.assertEqual(1, len(results))
         result = results[0]
         self.assertEqual("PY004", result.rule_id)
         self.assertEqual(4, result.location.start_line)
         self.assertEqual(4, result.location.end_line)
-        self.assertEqual(0, result.location.start_column)
+        self.assertEqual(8, result.location.start_column)
         self.assertEqual(11, result.location.end_column)
         self.assertEqual(Level.NOTE, result.level)
         self.assertEqual(-1.0, result.rank)
 
     def test_suppress_lowercase_rule(self):
         artifact = Artifact(
             os.path.join(self.base_path, "suppress_lowercase_rule.py")
         )
         results = self.parser.parse(artifact)
         self.assertEqual(1, len(results))
         result = results[0]
         self.assertEqual("PY004", result.rule_id)
         self.assertEqual(4, result.location.start_line)
         self.assertEqual(4, result.location.end_line)
-        self.assertEqual(0, result.location.start_column)
+        self.assertEqual(8, result.location.start_column)
         self.assertEqual(11, result.location.end_column)
         self.assertEqual(Level.ERROR, result.level)
         self.assertEqual(-1.0, result.rank)
 
     def test_suppress_multiline(self):
         # TODO: not testing multiline
         artifact = Artifact(
@@ -54,86 +68,86 @@
         )
         results = self.parser.parse(artifact)
         self.assertEqual(1, len(results))
         result = results[0]
         self.assertEqual("PY004", result.rule_id)
         self.assertEqual(4, result.location.start_line)
         self.assertEqual(4, result.location.end_line)
-        self.assertEqual(0, result.location.start_column)
+        self.assertEqual(8, result.location.start_column)
         self.assertEqual(11, result.location.end_column)
         self.assertEqual(Level.NOTE, result.level)
         self.assertEqual(-1.0, result.rank)
 
     def test_suppress_multiple_comments(self):
         artifact = Artifact(
             os.path.join(self.base_path, "suppress_multiple_comments.py")
         )
         results = self.parser.parse(artifact)
         self.assertEqual(1, len(results))
         result = results[0]
         self.assertEqual("PY004", result.rule_id)
         self.assertEqual(4, result.location.start_line)
         self.assertEqual(4, result.location.end_line)
-        self.assertEqual(0, result.location.start_column)
+        self.assertEqual(8, result.location.start_column)
         self.assertEqual(11, result.location.end_column)
         self.assertEqual(Level.NOTE, result.level)
         self.assertEqual(-1.0, result.rank)
 
     def test_suppress_multiple_rules(self):
         artifact = Artifact(
             os.path.join(self.base_path, "suppress_multiple_rules.py")
         )
         results = self.parser.parse(artifact)
         self.assertEqual(1, len(results))
         result = results[0]
         self.assertEqual("PY004", result.rule_id)
         self.assertEqual(4, result.location.start_line)
         self.assertEqual(4, result.location.end_line)
-        self.assertEqual(0, result.location.start_column)
+        self.assertEqual(8, result.location.start_column)
         self.assertEqual(11, result.location.end_column)
         self.assertEqual(Level.NOTE, result.level)
         self.assertEqual(-1.0, result.rank)
 
     def test_suppress_preceding(self):
         artifact = Artifact(
             os.path.join(self.base_path, "suppress_preceding.py")
         )
         results = self.parser.parse(artifact)
         self.assertEqual(1, len(results))
         result = results[0]
         self.assertEqual("PY004", result.rule_id)
         self.assertEqual(5, result.location.start_line)
         self.assertEqual(5, result.location.end_line)
-        self.assertEqual(0, result.location.start_column)
+        self.assertEqual(8, result.location.start_column)
         self.assertEqual(11, result.location.end_column)
         self.assertEqual(Level.NOTE, result.level)
         self.assertEqual(-1.0, result.rank)
 
     def test_suppress_spaced_rules(self):
         artifact = Artifact(
             os.path.join(self.base_path, "suppress_spaced_rules.py")
         )
         results = self.parser.parse(artifact)
         self.assertEqual(1, len(results))
         result = results[0]
         self.assertEqual("PY004", result.rule_id)
         self.assertEqual(4, result.location.start_line)
         self.assertEqual(4, result.location.end_line)
-        self.assertEqual(0, result.location.start_column)
+        self.assertEqual(8, result.location.start_column)
         self.assertEqual(11, result.location.end_column)
         self.assertEqual(Level.NOTE, result.level)
         self.assertEqual(-1.0, result.rank)
 
     def test_suppress_wrong_rule(self):
         artifact = Artifact(
             os.path.join(self.base_path, "suppress_wrong_rule.py")
         )
         results = self.parser.parse(artifact)
         self.assertEqual(1, len(results))
         result = results[0]
         self.assertEqual("PY004", result.rule_id)
         self.assertEqual(4, result.location.start_line)
         self.assertEqual(4, result.location.end_line)
-        self.assertEqual(0, result.location.start_column)
+        self.assertEqual(8, result.location.start_column)
         self.assertEqual(11, result.location.end_column)
         self.assertEqual(Level.ERROR, result.level)
         self.assertEqual(-1.0, result.rank)
```

### Comparing `precli-0.4.3/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_rc4.go` & `precli-0.4.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_rc4.go`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_1024.go` & `precli-0.4.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_1024.go`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_2048.go` & `precli-0.4.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_2048.go`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_3072.go` & `precli-0.4.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_3072.go`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_1024.go` & `precli-0.4.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_1024.go`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_2048.go` & `precli-0.4.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_2048.go`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_4096.go` & `precli-0.4.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_4096.go`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_bits_as_var.go` & `precli-0.4.4/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_bits_as_var.go`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_cipher.py` & `precli-0.4.4/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_cipher.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_hash.py` & `precli-0.4.4/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_hash.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_key.py` & `precli-0.4.4/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_key.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/argparse/test_argparse_sensitive_info.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/argparse/test_argparse_sensitive_info.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/assert/test_assert.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/assert/test_assert.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/crypt/test_crypt_weak_hash.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/crypt/test_crypt_weak_hash.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/ftplib/test_ftplib_cleartext.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/ftplib/test_ftplib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/ftplib/test_ftplib_unverified_context.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/ftplib/test_ftplib_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/test_hashlib_improper_prng.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/test_hashlib_improper_prng.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/hashlib/test_hashlib_weak_hash.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/hashlib/test_hashlib_weak_hash.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/hmac/test_hmac_timing_attack.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/hmac/test_hmac_timing_attack.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_hash.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_hash.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_key.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_key.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/http/test_http_server_unrestricted_bind.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/http/test_http_server_unrestricted_bind.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/http/test_http_url_secret.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/http/test_http_url_secret.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/imaplib/test_imaplib_cleartext.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/imaplib/test_imaplib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/imaplib/test_imaplib_unverified_context.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/imaplib/test_imaplib_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/json/test_json_load.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/json/test_json_load.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/logging/test_logging_insecure_listen_config.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/logging/test_logging_insecure_listen_config.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/marshal/test_marshal_load.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/marshal/test_marshal_load.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/nntplib/test_nntplib_cleartext.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/nntplib/test_nntplib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/nntplib/test_nntplib_unverified_context.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/nntplib/test_nntplib_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/pickle/test_pickle_load.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/pickle/test_pickle_load.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/poplib/test_poplib_cleartext.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/poplib/test_poplib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/poplib/test_poplib_unverified_context.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/poplib/test_poplib_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/re/test_re_denial_of_service.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/re/test_re_denial_of_service.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/secrets/test_secrets_weak_token.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/secrets/test_secrets_weak_token.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/shelve/test_shelve_open.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/shelve/test_shelve_open.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_auth.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_auth.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_login.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_login.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_as_var.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_as_var.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_none.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_none.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_unset.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_unset.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_as_var.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_as_var.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_none.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_none.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_unset.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_unset.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/test_smtplib_cleartext.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/test_smtplib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/smtplib/test_smtplib_unverified_context.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/smtplib/test_smtplib_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/socket/test_socket_unrestricted_bind.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/socket/test_socket_unrestricted_bind.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_tcp_server.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_tcp_server.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_udp_server.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_udp_server.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_tcp_server.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_tcp_server.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_tcp_server.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_tcp_server.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_udp_server.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_udp_server.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_udp_server.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_udp_server.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/socketserver/test_socketserver_unrestricted_bind.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/socketserver/test_socketserver_unrestricted_bind.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/ssl/test_ssl_context_tls_version.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/ssl/test_ssl_context_tls_version.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/ssl/test_ssl_context_weak_key.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/ssl/test_ssl_context_weak_key.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/ssl/test_ssl_create_context.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/ssl/test_ssl_create_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/ssl/test_ssl_get_server_certificate_tls_version.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/ssl/test_ssl_get_server_certificate_tls_version.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/ssl/test_ssl_wrap_socket_tls_version.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/ssl/test_ssl_wrap_socket_tls_version.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/telnetlib/test_telnetlib_cleartext.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/telnetlib/test_telnetlib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/tempfile/test_tempfile_mktemp_race_condition.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/tempfile/test_tempfile_mktemp_race_condition.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/python/stdlib/xmlrpc/test_xmlrpc_server_unrestricted_bind.py` & `precli-0.4.4/tests/unit/rules/python/stdlib/xmlrpc/test_xmlrpc_server_unrestricted_bind.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tests/unit/rules/test_case.py` & `precli-0.4.4/tests/unit/rules/test_case.py`

 * *Files identical despite different names*

### Comparing `precli-0.4.3/tox.ini` & `precli-0.4.4/tox.ini`

 * *Files identical despite different names*

