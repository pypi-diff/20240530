# Comparing `tmp/precli-0.5.5.tar.gz` & `tmp/precli-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "precli-0.5.5.tar", last modified: Tue May 28 20:46:17 2024, max compression
+gzip compressed data, was "precli-0.5.6.tar", last modified: Thu May 30 16:26:51 2024, max compression
```

## Comparing `precli-0.5.5.tar` & `precli-0.5.6.tar`

### file list

```diff
@@ -1,740 +1,741 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.779386 precli-0.5.5/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.667387 precli-0.5.5/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-28 20:46:14.000000 precli-0.5.5/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-28 20:46:14.000000 precli-0.5.5/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.667387 precli-0.5.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-28 20:46:14.000000 precli-0.5.5/.github/workflows/dependency-review.yml
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-28 20:46:14.000000 precli-0.5.5/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-28 20:46:14.000000 precli-0.5.5/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-28 20:46:14.000000 precli-0.5.5/.github/workflows/unit-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-28 20:46:14.000000 precli-0.5.5/.github/workflows/upload-asset.yml
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-28 20:46:14.000000 precli-0.5.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-28 20:46:14.000000 precli-0.5.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-28 20:46:17.000000 precli-0.5.5/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-28 20:46:14.000000 precli-0.5.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)    19910 2024-05-28 20:46:17.000000 precli-0.5.5/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-05-28 20:46:14.000000 precli-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-28 20:46:17.779386 precli-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-28 20:46:14.000000 precli-0.5.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-28 20:46:14.000000 precli-0.5.5/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.667387 precli-0.5.5/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-28 20:46:14.000000 precli-0.5.5/docs/getting-started.md
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-28 20:46:14.000000 precli-0.5.5/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.667387 precli-0.5.5/docs/man/
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-28 20:46:14.000000 precli-0.5.5/docs/man/precli.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-28 20:46:14.000000 precli-0.5.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.655387 precli-0.5.5/docs/rules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.651387 precli-0.5.5/docs/rules/go/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.667387 precli-0.5.5/docs/rules/go/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/go/stdlib/crypto-weak-cipher.md
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/go/stdlib/crypto-weak-hash.md
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/go/stdlib/crypto-weak-key.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.655387 precli-0.5.5/docs/rules/java/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.671387 precli-0.5.5/docs/rules/java/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/java/stdlib/java-net-insecure-cookie.md
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/java/stdlib/java-security-weak-hash.md
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/java/stdlib/java-security-weak-key.md
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/java/stdlib/java-security-weak-random.md
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/java/stdlib/javax-crypto-weak-cipher.md
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/java/stdlib/javax-servlet-http-insecure-cookie.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.655387 precli-0.5.5/docs/rules/python/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.675387 precli-0.5.5/docs/rules/python/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/argparse-sensitive-info.md
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/assert.md
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/crypt-weak-hash.md
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/ftplib-cleartext.md
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/ftplib-unverified-context.md
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/hashlib-improper-prng.md
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/hashlib-weak-hash.md
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/hmac-timing-attack.md
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/hmac-weak-hash.md
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/hmac-weak-key.md
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/http-server-unrestricted-bind.md
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/http-url-secret.md
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/imaplib-cleartext.md
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/imaplib-unverified-context.md
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/json-load.md
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/logging-insecure-listen-config.md
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/marshal-load.md
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/nntplib-cleartext.md
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/nntplib-unverified-context.md
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/pickle-load.md
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/poplib-cleartext.md
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/poplib-unverified-context.md
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/re-denial-of-service.md
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/secrets-weak-token.md
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/shelve-open.md
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/smtplib-cleartext.md
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/smtplib-unverified-context.md
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/socket-unrestricted-bind.md
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/socketserver-unrestricted-bind.md
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/ssl-context-weak-key.md
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/ssl-create-unverified-context.md
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/ssl-insecure-tls-version.md
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/telnetlib-cleartext.md
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/tempfile-mktemp-race-condition.md
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules/python/stdlib/xmlrpc-server-unrestricted-bind.md
--rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-28 20:46:14.000000 precli-0.5.5/docs/rules.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.675387 precli-0.5.5/logo/
--rw-r--r--   0 runner    (1001) docker     (127)   179541 2024-05-28 20:46:14.000000 precli-0.5.5/logo/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-28 20:46:14.000000 precli-0.5.5/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.675387 precli-0.5.5/precli/
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-28 20:46:14.000000 precli-0.5.5/precli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-28 20:46:14.000000 precli-0.5.5/precli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.679386 precli-0.5.5/precli/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/precli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11643 2024-05-28 20:46:14.000000 precli-0.5.5/precli/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.683386 precli-0.5.5/precli/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/argument.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/artifact.py
--rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/call.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/comparison.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/fix.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/kind.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/level.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/linecache.py
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/loader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/location.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/redos.py
--rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     6475 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/suppression.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/symtab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/tool.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-28 20:46:14.000000 precli-0.5.5/precli/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.683386 precli-0.5.5/precli/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)     7123 2024-05-28 20:46:14.000000 precli-0.5.5/precli/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7637 2024-05-28 20:46:14.000000 precli-0.5.5/precli/parsers/go.py
--rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-05-28 20:46:14.000000 precli-0.5.5/precli/parsers/java.py
--rw-r--r--   0 runner    (1001) docker     (127)    19412 2024-05-28 20:46:14.000000 precli-0.5.5/precli/parsers/python.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-28 20:46:14.000000 precli-0.5.5/precli/parsers/tokens.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.683386 precli-0.5.5/precli/renderers/
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-28 20:46:14.000000 precli-0.5.5/precli/renderers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-05-28 20:46:14.000000 precli-0.5.5/precli/renderers/detailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-05-28 20:46:14.000000 precli-0.5.5/precli/renderers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-28 20:46:14.000000 precli-0.5.5/precli/renderers/markdown.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-28 20:46:14.000000 precli-0.5.5/precli/renderers/plain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.683386 precli-0.5.5/precli/rules/
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.683386 precli-0.5.5/precli/rules/go/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/go/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.683386 precli-0.5.5/precli/rules/go/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/go/stdlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/go/stdlib/crypto_weak_cipher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/go/stdlib/crypto_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/go/stdlib/crypto_weak_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.683386 precli-0.5.5/precli/rules/java/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.687387 precli-0.5.5/precli/rules/java/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/java/stdlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/java/stdlib/java_net_insecure_cookie.py
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/java/stdlib/java_security_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/java/stdlib/java_security_weak_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/java/stdlib/java_security_weak_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/java/stdlib/javax_crypto_weak_cipher.py
--rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/java/stdlib/javax_servlet_http_insecure_cookie.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.687387 precli-0.5.5/precli/rules/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.691387 precli-0.5.5/precli/rules/python/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/argparse_sensitive_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/assert.py
--rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/crypt_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/ftplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/ftplib_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/hashlib_improper_prng.py
--rw-r--r--   0 runner    (1001) docker     (127)     6955 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/hashlib_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/hmac_timing_attack.py
--rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/hmac_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/hmac_weak_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/http_server_unrestricted_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/http_url_secret.py
--rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/imaplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/imaplib_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/json_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/logging_insecure_listen_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/marshal_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/nntplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/nntplib_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/pickle_load.py
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/poplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/poplib_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/re_denial_of_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/secrets_weak_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/shelve_open.py
--rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/smtplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/smtplib_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/socket_unrestricted_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/socketserver_unrestricted_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/ssl_context_weak_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/ssl_create_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/ssl_insecure_tls_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/telnetlib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/tempfile_mktemp_race_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-28 20:46:14.000000 precli-0.5.5/precli/rules/python/stdlib/xmlrpc_server_unrestricted_bind.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.779386 precli-0.5.5/precli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-05-28 20:46:17.000000 precli-0.5.5/precli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    39522 2024-05-28 20:46:17.000000 precli-0.5.5/precli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 20:46:17.000000 precli-0.5.5/precli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-28 20:46:17.000000 precli-0.5.5/precli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 20:46:17.000000 precli-0.5.5/precli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-28 20:46:17.000000 precli-0.5.5/precli.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-28 20:46:17.000000 precli-0.5.5/precli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-28 20:46:17.000000 precli-0.5.5/precli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-28 20:46:14.000000 precli-0.5.5/pylintrc
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-28 20:46:14.000000 precli-0.5.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-05-28 20:46:17.779386 precli-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-28 20:46:14.000000 precli-0.5.5/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 20:46:14.000000 precli-0.5.5/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.691387 precli-0.5.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.691387 precli-0.5.5/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.691387 precli-0.5.5/tests/unit/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.695387 precli-0.5.5/tests/unit/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/core/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.695387 precli-0.5.5/tests/unit/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.699386 precli-0.5.5/tests/unit/parsers/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/bad_coding.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/expression_list_assignment.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/expression_list_assignment_uneven.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/importlib_import_module.py
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/pep3120.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress.go
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_lowercase_rule.go
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_lowercase_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_multiline.go
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_multiline.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_multiple_comments.go
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_multiple_comments.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_multiple_rules.go
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_multiple_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_preceding.go
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_preceding.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_spaced_rules.go
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_spaced_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_wrong_rule.go
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/examples/suppress_wrong_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/test_go.py
--rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/parsers/test_python.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.699386 precli-0.5.5/tests/unit/rules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.699386 precli-0.5.5/tests/unit/rules/go/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.699386 precli-0.5.5/tests/unit/rules/go/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.699386 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.703386 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_aes.go
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_des.go
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_rc4.go
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_md5_new.go
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_md5_sum.go
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha1_new.go
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha1_sum.go
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha256_new.go
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha256_sum.go
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_1024.go
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_2048.go
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_3072.go
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_1024.go
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_2048.go
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_4096.go
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_bits_as_var.go
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_cipher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.703386 precli-0.5.5/tests/unit/rules/java/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.703386 precli-0.5.5/tests/unit/rules/java/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.703386 precli-0.5.5/tests/unit/rules/java/stdlib/java_net/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.703386 precli-0.5.5/tests/unit/rules/java/stdlib/java_net/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_net/examples/HttpCookieSecureFalse.java
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_net/examples/HttpCookieSecureTrue.java
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_net/test_insecure_cookie.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.703386 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.707387 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/JavaSecuritySecureRandomSHA1PRNG.java
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/KeyPairGeneratorDSA.java
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/KeyPairGeneratorRSA.java
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestMD2.java
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestMD5.java
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestMD5Property.java
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestSHA1.java
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestSHA256.java
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/SecureRandomDefault.java
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/SecureRandomSHA1PRNG.java
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/test_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/test_weak_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/java_security/test_weak_random.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.707387 precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.707387 precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/Cipher3DESCBC.java
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherAESCBC.java
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherArcfour.java
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherBlowfishCBC.java
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherDESCBC.java
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC2.java
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC4.java
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC5.java
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/test_weak_cipher.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.707387 precli-0.5.5/tests/unit/rules/java/stdlib/javax_servlet_http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_servlet_http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.707387 precli-0.5.5/tests/unit/rules/java/stdlib/javax_servlet_http/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_servlet_http/examples/CookieSecureFalse.java
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_servlet_http/examples/CookieSecureTrue.java
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/java/stdlib/javax_servlet_http/test_insecure_cookie.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.707387 precli-0.5.5/tests/unit/rules/python/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.707387 precli-0.5.5/tests/unit/rules/python/stdlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.707387 precli-0.5.5/tests/unit/rules/python/stdlib/argparse/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/argparse/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.711387 precli-0.5.5/tests/unit/rules/python/stdlib/argparse/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_api_key.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_default_action.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_password.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_password_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_password_store_true.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/argparse/test_argparse_sensitive_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.711387 precli-0.5.5/tests/unit/rules/python/stdlib/assert/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/assert/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.711387 precli-0.5.5/tests/unit/rules/python/stdlib/assert/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/assert/examples/assert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/assert/test_assert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.711387 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.711387 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_blowfish.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_blowfish.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_crypt.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/crypt/test_crypt_weak_hash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.715386 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.715386 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftp_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftp_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftp_tls.py
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_login.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_login_single_statement.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls.py
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_user_password.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_user_password.py
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/test_ftplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/test_ftplib_unverified_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.715386 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.727387 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_pbkdf2_hmac.py
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_scrypt.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5_as_identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5_importlib.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5_usedforsecurity_true.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md5_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md5_usedforsecurity_true.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_name_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha_usedforsecurity_false.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha_usedforsecurity_false.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/test_hashlib_improper_prng.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/test_hashlib_weak_hash.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.727387 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.743386 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_md5_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_hashlib_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_hashlib_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_hashlib_sm3.py
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_blake2b.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_md4.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_md5_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_ripemd160.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha1.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha224.py
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha512.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_shake_128.py
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_shake_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_blake2s.py
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_hashlib_sha3_224.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_hashlib_sha3_384.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_hashlib_sha3_512.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_sha384.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_sha512_256.py
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack_class.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack_class_hexdigest.py
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack_compare_digest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/test_hmac_timing_attack.py
--rw-r--r--   0 runner    (1001) docker     (127)     4317 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_hash.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_key.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.747386 precli-0.5.5/tests/unit/rules/python/stdlib/http/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/http/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.747386 precli-0.5.5/tests/unit/rules/python/stdlib/http/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/http/examples/http_server_http_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/http/examples/http_server_threading_http_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/http/examples/http_url_secret_apikey.py
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/http/examples/http_url_secret_apikey_in_header.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/http/examples/http_url_secret_basic_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/http/examples/http_url_secret_basic_auth_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/http/examples/http_url_secret_password.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/http/examples/http_url_secret_username.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/http/test_http_server_unrestricted_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/http/test_http_url_secret.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.747386 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.751387 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_authenticate.py
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_login_cram_md5.py
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_stream.py
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/test_imaplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/test_imaplib_unverified_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.751387 precli-0.5.5/tests/unit/rules/python/stdlib/json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/json/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.751387 precli-0.5.5/tests/unit/rules/python/stdlib/json/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/json/examples/json_jsondecoder_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/json/examples/json_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/json/examples/json_loads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/json/test_json_load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.751387 precli-0.5.5/tests/unit/rules/python/stdlib/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.751387 precli-0.5.5/tests/unit/rules/python/stdlib/logging/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_empty_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_port.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_port_verify_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_port_verify_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_verify_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_verify_none_port.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_verify_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/logging/test_logging_insecure_listen_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.751387 precli-0.5.5/tests/unit/rules/python/stdlib/marshal/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/marshal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.751387 precli-0.5.5/tests/unit/rules/python/stdlib/marshal/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/marshal/examples/marshal_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/marshal/examples/marshal_loads.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/marshal/test_marshal_load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.755386 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.755386 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls.py
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/test_nntplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/test_nntplib_unverified_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.755386 precli-0.5.5/tests/unit/rules/python/stdlib/pickle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/pickle/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.755386 precli-0.5.5/tests/unit/rules/python/stdlib/pickle/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/pickle/examples/pickle_load.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/pickle/examples/pickle_loads.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/pickle/examples/pickle_unpickler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/pickle/test_pickle_load.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.755386 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.759386 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_apop.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_pass_.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_rpop.py
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/test_poplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/poplib/test_poplib_unverified_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.759386 precli-0.5.5/tests/unit/rules/python/stdlib/re/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/re/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.763386 precli-0.5.5/tests/unit/rules/python/stdlib/re/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/re/examples/re_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/re/examples/re_compile_good.py
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/re/examples/re_findall.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/re/examples/re_finditer.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/re/examples/re_fullmatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/re/examples/re_match.py
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/re/examples/re_search.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/re/examples/re_search_good.py
--rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/re/examples/re_split.py
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/re/examples/re_sub.py
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/re/examples/re_subn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/re/test_re_denial_of_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.763386 precli-0.5.5/tests/unit/rules/python/stdlib/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/secrets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.763386 precli-0.5.5/tests/unit/rules/python/stdlib/secrets/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_bytes_default.py
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_bytes_size_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_hex.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_hex_nbytes_unknown.py
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_urlsafe.py
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/secrets/test_secrets_weak_token.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.763386 precli-0.5.5/tests/unit/rules/python/stdlib/shelve/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/shelve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.763386 precli-0.5.5/tests/unit/rules/python/stdlib/shelve/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/shelve/examples/shelve_dbfilenameshelf.py
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/shelve/examples/shelve_open.py
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/shelve/examples/shelve_open_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/shelve/test_shelve_open.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.763386 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.767386 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_login.py
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_none.py
--rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_unset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/test_smtplib_cleartext.py
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/test_smtplib_unverified_context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.767386 precli-0.5.5/tests/unit/rules/python/stdlib/socket/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.767386 precli-0.5.5/tests/unit/rules/python/stdlib/socket/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socket/examples/socket_create_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socket/examples/socket_socket_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socket/examples/socket_socket_bind_as_var.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socket/examples/socket_socket_bind_as_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socket/test_socket_unrestricted_bind.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.767386 precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.767386 precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_tcp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_udp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_tcp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_tcp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_udp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_udp_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/test_socketserver_unrestricted_bind.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.771386 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.775386 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/create_default_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/create_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_sslv2.py
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_sslv23.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_sslv3.py
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_tlsv1.py
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_tlsv11.py
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_tlsv12.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP256r1.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP384r1.py
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP384r1tls13.py
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP512r1.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_default_context.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_ffdhe2048.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_prime192v1.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_prime256v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_secp160r2.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_secp256r1.py
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_sect163k1.py
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_sect571k1.py
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_typed_default_param.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_typed_param.py
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_unverified_context.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_sslv2.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_sslv23.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_sslv3.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_tlsv1.py
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_tlsv11.py
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_tlsv12.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv2.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv23.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv2_server_side_true.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv3.py
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_tlsv1.py
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_tlsv11.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_tlsv12.py
--rw-r--r--   0 runner    (1001) docker     (127)     1406 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/test_ssl_context_tls_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/test_ssl_context_weak_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/test_ssl_create_context.py
--rw-r--r--   0 runner    (1001) docker     (127)     1473 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/test_ssl_get_server_certificate_tls_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/ssl/test_ssl_wrap_socket_tls_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.775386 precli-0.5.5/tests/unit/rules/python/stdlib/telnetlib/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/telnetlib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.779386 precli-0.5.5/tests/unit/rules/python/stdlib/telnetlib/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/telnetlib/examples/telnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/telnetlib/examples/telnetlib_telnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/telnetlib/examples/telnetlib_telnet_context_mgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/telnetlib/test_telnetlib_cleartext.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.779386 precli-0.5.5/tests/unit/rules/python/stdlib/tempfile/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/tempfile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.779386 precli-0.5.5/tests/unit/rules/python/stdlib/tempfile/examples/
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp.py
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_args_open.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_args_with_open_args.py
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_open.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_walrus_open.py
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_with_open.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_with_open_multiline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/tempfile/test_tempfile_mktemp_race_condition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.779386 precli-0.5.5/tests/unit/rules/python/stdlib/xmlrpc/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/xmlrpc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 20:46:17.779386 precli-0.5.5/tests/unit/rules/python/stdlib/xmlrpc/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/xmlrpc/examples/xmlrpc_server_doc_xml_rpc_server.py
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/xmlrpc/examples/xmlrpc_server_simple_xml_rpc_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/python/stdlib/xmlrpc/test_xmlrpc_server_unrestricted_bind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-28 20:46:14.000000 precli-0.5.5/tests/unit/rules/test_case.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-28 20:46:14.000000 precli-0.5.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.132983 precli-0.5.6/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.024983 precli-0.5.6/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 16:26:47.000000 precli-0.5.6/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-30 16:26:47.000000 precli-0.5.6/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.024983 precli-0.5.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-30 16:26:47.000000 precli-0.5.6/.github/workflows/dependency-review.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-30 16:26:47.000000 precli-0.5.6/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-30 16:26:47.000000 precli-0.5.6/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2288 2024-05-30 16:26:47.000000 precli-0.5.6/.github/workflows/unit-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-30 16:26:47.000000 precli-0.5.6/.github/workflows/upload-asset.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-05-30 16:26:47.000000 precli-0.5.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-30 16:26:47.000000 precli-0.5.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-30 16:26:50.000000 precli-0.5.6/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)     5224 2024-05-30 16:26:47.000000 precli-0.5.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)    20116 2024-05-30 16:26:50.000000 precli-0.5.6/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)     4673 2024-05-30 16:26:47.000000 precli-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-30 16:26:51.132983 precli-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-30 16:26:47.000000 precli-0.5.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-30 16:26:47.000000 precli-0.5.6/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.028983 precli-0.5.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-30 16:26:47.000000 precli-0.5.6/docs/getting-started.md
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-05-30 16:26:47.000000 precli-0.5.6/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.028983 precli-0.5.6/docs/man/
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-30 16:26:47.000000 precli-0.5.6/docs/man/precli.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-30 16:26:47.000000 precli-0.5.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.012983 precli-0.5.6/docs/rules/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.012983 precli-0.5.6/docs/rules/go/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.028983 precli-0.5.6/docs/rules/go/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/go/stdlib/crypto-weak-cipher.md
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/go/stdlib/crypto-weak-hash.md
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/go/stdlib/crypto-weak-key.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.012983 precli-0.5.6/docs/rules/java/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.028983 precli-0.5.6/docs/rules/java/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/java/stdlib/java-net-insecure-cookie.md
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/java/stdlib/java-security-weak-hash.md
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/java/stdlib/java-security-weak-key.md
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/java/stdlib/java-security-weak-random.md
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/java/stdlib/javax-crypto-weak-cipher.md
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/java/stdlib/javax-servlet-http-insecure-cookie.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.012983 precli-0.5.6/docs/rules/python/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.036983 precli-0.5.6/docs/rules/python/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/argparse-sensitive-info.md
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/assert.md
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/crypt-weak-hash.md
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/ftplib-cleartext.md
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/ftplib-unverified-context.md
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/hashlib-improper-prng.md
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/hashlib-weak-hash.md
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/hmac-timing-attack.md
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/hmac-weak-hash.md
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/hmac-weak-key.md
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/http-server-unrestricted-bind.md
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/http-url-secret.md
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/imaplib-cleartext.md
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/imaplib-unverified-context.md
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/json-load.md
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/logging-insecure-listen-config.md
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/marshal-load.md
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/nntplib-cleartext.md
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/nntplib-unverified-context.md
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/pickle-load.md
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/poplib-cleartext.md
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/poplib-unverified-context.md
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/re-denial-of-service.md
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/secrets-weak-token.md
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/shelve-open.md
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/smtplib-cleartext.md
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/smtplib-unverified-context.md
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/socket-unrestricted-bind.md
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/socketserver-unrestricted-bind.md
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/ssl-context-weak-key.md
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/ssl-create-unverified-context.md
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/ssl-insecure-tls-version.md
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/telnetlib-cleartext.md
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/tempfile-mktemp-race-condition.md
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules/python/stdlib/xmlrpc-server-unrestricted-bind.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6533 2024-05-30 16:26:47.000000 precli-0.5.6/docs/rules.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.036983 precli-0.5.6/logo/
+-rw-r--r--   0 runner    (1001) docker     (127)   179541 2024-05-30 16:26:47.000000 precli-0.5.6/logo/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-30 16:26:47.000000 precli-0.5.6/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.036983 precli-0.5.6/precli/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-30 16:26:47.000000 precli-0.5.6/precli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-30 16:26:47.000000 precli-0.5.6/precli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.036983 precli-0.5.6/precli/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/precli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11274 2024-05-30 16:26:47.000000 precli-0.5.6/precli/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.040983 precli-0.5.6/precli/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/precli/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-05-30 16:26:47.000000 precli-0.5.6/precli/core/argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-05-30 16:26:47.000000 precli-0.5.6/precli/core/artifact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3238 2024-05-30 16:26:47.000000 precli-0.5.6/precli/core/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-30 16:26:47.000000 precli-0.5.6/precli/core/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-30 16:26:47.000000 precli-0.5.6/precli/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-30 16:26:47.000000 precli-0.5.6/precli/core/cwe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-30 16:26:47.000000 precli-0.5.6/precli/core/fix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-30 16:26:47.000000 precli-0.5.6/precli/core/kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-30 16:26:47.000000 precli-0.5.6/precli/core/level.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-05-30 16:26:47.000000 precli-0.5.6/precli/core/linecache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-30 16:26:47.000000 precli-0.5.6/precli/core/loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-30 16:26:47.000000 precli-0.5.6/precli/core/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-30 16:26:47.000000 precli-0.5.6/precli/core/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9635 2024-05-30 16:26:47.000000 precli-0.5.6/precli/core/redos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4305 2024-05-30 16:26:47.000000 precli-0.5.6/precli/core/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6983 2024-05-30 16:26:47.000000 precli-0.5.6/precli/core/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-30 16:26:47.000000 precli-0.5.6/precli/core/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-30 16:26:47.000000 precli-0.5.6/precli/core/suppression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-30 16:26:47.000000 precli-0.5.6/precli/core/symtab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-05-30 16:26:47.000000 precli-0.5.6/precli/core/tool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-30 16:26:47.000000 precli-0.5.6/precli/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.040983 precli-0.5.6/precli/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)     7219 2024-05-30 16:26:47.000000 precli-0.5.6/precli/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7692 2024-05-30 16:26:47.000000 precli-0.5.6/precli/parsers/go.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13972 2024-05-30 16:26:47.000000 precli-0.5.6/precli/parsers/java.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19467 2024-05-30 16:26:47.000000 precli-0.5.6/precli/parsers/python.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-30 16:26:47.000000 precli-0.5.6/precli/parsers/tokens.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.044983 precli-0.5.6/precli/renderers/
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-30 16:26:47.000000 precli-0.5.6/precli/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5682 2024-05-30 16:26:47.000000 precli-0.5.6/precli/renderers/detailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7421 2024-05-30 16:26:47.000000 precli-0.5.6/precli/renderers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-05-30 16:26:47.000000 precli-0.5.6/precli/renderers/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-05-30 16:26:47.000000 precli-0.5.6/precli/renderers/plain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.044983 precli-0.5.6/precli/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.044983 precli-0.5.6/precli/rules/go/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/go/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.044983 precli-0.5.6/precli/rules/go/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/go/stdlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/go/stdlib/crypto_weak_cipher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/go/stdlib/crypto_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4578 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/go/stdlib/crypto_weak_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.044983 precli-0.5.6/precli/rules/java/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.044983 precli-0.5.6/precli/rules/java/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/java/stdlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/java/stdlib/java_net_insecure_cookie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/java/stdlib/java_security_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4763 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/java/stdlib/java_security_weak_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/java/stdlib/java_security_weak_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6537 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/java/stdlib/javax_crypto_weak_cipher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/java/stdlib/javax_servlet_http_insecure_cookie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.044983 precli-0.5.6/precli/rules/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.052983 precli-0.5.6/precli/rules/python/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3128 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/argparse_sensitive_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/assert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3895 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/crypt_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/ftplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3284 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/ftplib_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4833 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/hashlib_improper_prng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6955 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/hashlib_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/hmac_timing_attack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6579 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/hmac_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6812 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/hmac_weak_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3788 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/http_server_unrestricted_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3031 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/http_url_secret.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3472 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/imaplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/imaplib_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/json_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2228 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/logging_insecure_listen_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/marshal_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/nntplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/nntplib_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/pickle_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/poplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3583 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/poplib_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3176 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/re_denial_of_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/secrets_weak_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2084 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/shelve_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4035 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/smtplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/smtplib_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3358 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/socket_unrestricted_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4913 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/socketserver_unrestricted_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/ssl_context_weak_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/ssl_create_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/ssl_insecure_tls_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/telnetlib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6124 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/tempfile_mktemp_race_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-30 16:26:47.000000 precli-0.5.6/precli/rules/python/stdlib/xmlrpc_server_unrestricted_bind.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.132983 precli-0.5.6/precli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-05-30 16:26:50.000000 precli-0.5.6/precli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    39541 2024-05-30 16:26:51.000000 precli-0.5.6/precli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 16:26:50.000000 precli-0.5.6/precli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-05-30 16:26:50.000000 precli-0.5.6/precli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 16:26:50.000000 precli-0.5.6/precli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-30 16:26:50.000000 precli-0.5.6/precli.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-30 16:26:50.000000 precli-0.5.6/precli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-30 16:26:50.000000 precli-0.5.6/precli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-30 16:26:47.000000 precli-0.5.6/pylintrc
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-30 16:26:47.000000 precli-0.5.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4389 2024-05-30 16:26:51.132983 precli-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-30 16:26:47.000000 precli-0.5.6/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 16:26:47.000000 precli-0.5.6/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.052983 precli-0.5.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.052983 precli-0.5.6/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.052983 precli-0.5.6/tests/unit/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.052983 precli-0.5.6/tests/unit/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/core/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.052983 precli-0.5.6/tests/unit/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/parsers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.056983 precli-0.5.6/tests/unit/parsers/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/parsers/examples/bad_coding.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/parsers/examples/expression_list_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/parsers/examples/expression_list_assignment_uneven.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/parsers/examples/importlib_import_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/parsers/examples/pep3120.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/parsers/examples/suppress.go
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/parsers/examples/suppress.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/parsers/examples/suppress_lowercase_rule.go
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/parsers/examples/suppress_lowercase_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/parsers/examples/suppress_multiline.go
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/parsers/examples/suppress_multiline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/parsers/examples/suppress_multiple_comments.go
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/parsers/examples/suppress_multiple_comments.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/parsers/examples/suppress_multiple_rules.go
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/parsers/examples/suppress_multiple_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/parsers/examples/suppress_preceding.go
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/parsers/examples/suppress_preceding.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/parsers/examples/suppress_spaced_rules.go
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/parsers/examples/suppress_spaced_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/parsers/examples/suppress_wrong_rule.go
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/parsers/examples/suppress_wrong_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/parsers/test_go.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/parsers/test_python.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.056983 precli-0.5.6/tests/unit/rules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.056983 precli-0.5.6/tests/unit/rules/go/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/go/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.056983 precli-0.5.6/tests/unit/rules/go/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/go/stdlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.056983 precli-0.5.6/tests/unit/rules/go/stdlib/crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/go/stdlib/crypto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.060983 precli-0.5.6/tests/unit/rules/go/stdlib/crypto/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_aes.go
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_des.go
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_rc4.go
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_md5_new.go
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_md5_sum.go
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha1_new.go
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha1_sum.go
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha256_new.go
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_hash_sha256_sum.go
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_1024.go
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_2048.go
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_3072.go
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_1024.go
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_2048.go
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_4096.go
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_bits_as_var.go
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_cipher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.060983 precli-0.5.6/tests/unit/rules/java/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.060983 precli-0.5.6/tests/unit/rules/java/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.060983 precli-0.5.6/tests/unit/rules/java/stdlib/java_net/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/java_net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.060983 precli-0.5.6/tests/unit/rules/java/stdlib/java_net/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/java_net/examples/HttpCookieSecureFalse.java
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/java_net/examples/HttpCookieSecureTrue.java
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/java_net/test_insecure_cookie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.060983 precli-0.5.6/tests/unit/rules/java/stdlib/java_security/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/java_security/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.064983 precli-0.5.6/tests/unit/rules/java/stdlib/java_security/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/java_security/examples/JavaSecuritySecureRandomSHA1PRNG.java
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/java_security/examples/KeyPairGeneratorDSA.java
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/java_security/examples/KeyPairGeneratorRSA.java
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestMD2.java
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestMD5.java
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestMD5Property.java
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestSHA1.java
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestSHA256.java
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/java_security/examples/SecureRandomDefault.java
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/java_security/examples/SecureRandomSHA1PRNG.java
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/java_security/test_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/java_security/test_weak_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/java_security/test_weak_random.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.064983 precli-0.5.6/tests/unit/rules/java/stdlib/javax_crypto/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/javax_crypto/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.064983 precli-0.5.6/tests/unit/rules/java/stdlib/javax_crypto/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/javax_crypto/examples/Cipher3DESCBC.java
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherAESCBC.java
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherArcfour.java
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherBlowfishCBC.java
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherDESCBC.java
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC2.java
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC4.java
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC5.java
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/javax_crypto/test_weak_cipher.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.064983 precli-0.5.6/tests/unit/rules/java/stdlib/javax_servlet_http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/javax_servlet_http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.064983 precli-0.5.6/tests/unit/rules/java/stdlib/javax_servlet_http/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/javax_servlet_http/examples/CookieSecureFalse.java
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/javax_servlet_http/examples/CookieSecureTrue.java
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/java/stdlib/javax_servlet_http/test_insecure_cookie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.064983 precli-0.5.6/tests/unit/rules/python/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.064983 precli-0.5.6/tests/unit/rules/python/stdlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.064983 precli-0.5.6/tests/unit/rules/python/stdlib/argparse/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/argparse/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.068983 precli-0.5.6/tests/unit/rules/python/stdlib/argparse/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_default_action.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_password_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/argparse/examples/argparse_add_argument_password_store_true.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/argparse/test_argparse_sensitive_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.068983 precli-0.5.6/tests/unit/rules/python/stdlib/assert/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/assert/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.068983 precli-0.5.6/tests/unit/rules/python/stdlib/assert/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/assert/examples/assert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/assert/test_assert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.068983 precli-0.5.6/tests/unit/rules/python/stdlib/crypt/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/crypt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.068983 precli-0.5.6/tests/unit/rules/python/stdlib/crypt/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_blowfish.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/crypt/examples/crypt_crypt_method_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt.py
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_blowfish.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_crypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/crypt/examples/crypt_mksalt_method_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/crypt/test_crypt_weak_hash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.072983 precli-0.5.6/tests/unit/rules/python/stdlib/ftplib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ftplib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.072983 precli-0.5.6/tests/unit/rules/python/stdlib/ftplib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ftplib/examples/ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ftplib/examples/ftp_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ftplib/examples/ftp_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ftplib/examples/ftp_tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_login_single_statement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_tls_user_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ftplib/examples/ftplib_ftp_user_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ftplib/test_ftplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ftplib/test_ftplib_unverified_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.072983 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.084983 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_pbkdf2_hmac.py
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_improper_prng_scrypt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5_as_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5_importlib.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_md5_usedforsecurity_true.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md5_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_md5_usedforsecurity_true.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_name_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_sha_usedforsecurity_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_new_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_pbkdf2_hmac_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_sha_usedforsecurity_false.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/examples/hashlib_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/test_hashlib_improper_prng.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3392 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/test_hashlib_weak_hash.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.084983 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.100983 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_hashlib_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_md5_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_hashlib_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_hashlib_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_hashlib_sm3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_digest_weak_key_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_blake2b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_hashlib_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_md4.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_md5_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_ripemd160.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_sha512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_shake_128.py
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_digestmod_shake_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_blake2s.py
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_hashlib_sha3_224.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_hashlib_sha3_384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_hashlib_sha3_512.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_sha384.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_new_weak_key_sha512_256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack_class_hexdigest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/examples/hmac_timing_attack_compare_digest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/test_hmac_timing_attack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4311 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1760 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_key.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.100983 precli-0.5.6/tests/unit/rules/python/stdlib/http/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/http/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.100983 precli-0.5.6/tests/unit/rules/python/stdlib/http/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/http/examples/http_server_http_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/http/examples/http_server_threading_http_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/http/examples/http_url_secret_apikey.py
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/http/examples/http_url_secret_apikey_in_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/http/examples/http_url_secret_basic_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/http/examples/http_url_secret_basic_auth_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/http/examples/http_url_secret_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/http/examples/http_url_secret_username.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/http/test_http_server_unrestricted_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/http/test_http_url_secret.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.100983 precli-0.5.6/tests/unit/rules/python/stdlib/imaplib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/imaplib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.104983 precli-0.5.6/tests/unit/rules/python/stdlib/imaplib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_authenticate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_login_cram_md5.py
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_ssl_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      387 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_starttls_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/imaplib/examples/imaplib_imap4_stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/imaplib/test_imaplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/imaplib/test_imaplib_unverified_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.104983 precli-0.5.6/tests/unit/rules/python/stdlib/json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/json/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.104983 precli-0.5.6/tests/unit/rules/python/stdlib/json/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/json/examples/json_jsondecoder_decode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/json/examples/json_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/json/examples/json_loads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/json/test_json_load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.104983 precli-0.5.6/tests/unit/rules/python/stdlib/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.104983 precli-0.5.6/tests/unit/rules/python/stdlib/logging/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_empty_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_port_verify_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_port_verify_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_verify_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_verify_none_port.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/logging/examples/insecure_listen_config_verify_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/logging/test_logging_insecure_listen_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.104983 precli-0.5.6/tests/unit/rules/python/stdlib/marshal/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/marshal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.104983 precli-0.5.6/tests/unit/rules/python/stdlib/marshal/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      271 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/marshal/examples/marshal_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/marshal/examples/marshal_loads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/marshal/test_marshal_load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.108983 precli-0.5.6/tests/unit/rules/python/stdlib/nntplib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/nntplib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.108983 precli-0.5.6/tests/unit/rules/python/stdlib/nntplib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      209 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_ssl_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/nntplib/examples/nntplib_nntp_starttls_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/nntplib/test_nntplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/nntplib/test_nntplib_unverified_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.108983 precli-0.5.6/tests/unit/rules/python/stdlib/pickle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/pickle/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.108983 precli-0.5.6/tests/unit/rules/python/stdlib/pickle/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/pickle/examples/pickle_load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/pickle/examples/pickle_loads.py
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/pickle/examples/pickle_unpickler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/pickle/test_pickle_load.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.108983 precli-0.5.6/tests/unit/rules/python/stdlib/poplib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/poplib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.112983 precli-0.5.6/tests/unit/rules/python/stdlib/poplib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_apop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_pass_.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_rpop.py
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_ssl_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_stls_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/poplib/examples/poplib_pop3_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/poplib/test_poplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/poplib/test_poplib_unverified_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.112983 precli-0.5.6/tests/unit/rules/python/stdlib/re/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/re/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.112983 precli-0.5.6/tests/unit/rules/python/stdlib/re/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/re/examples/re_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/re/examples/re_compile_good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/re/examples/re_findall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/re/examples/re_finditer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/re/examples/re_fullmatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/re/examples/re_match.py
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/re/examples/re_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/re/examples/re_search_good.py
+-rw-r--r--   0 runner    (1001) docker     (127)      176 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/re/examples/re_split.py
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/re/examples/re_sub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/re/examples/re_subn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/re/test_re_denial_of_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.112983 precli-0.5.6/tests/unit/rules/python/stdlib/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/secrets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.116983 precli-0.5.6/tests/unit/rules/python/stdlib/secrets/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_bytes_default.py
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_bytes_size_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_hex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_hex_nbytes_unknown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/secrets/examples/secrets_token_urlsafe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/secrets/test_secrets_weak_token.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.116983 precli-0.5.6/tests/unit/rules/python/stdlib/shelve/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/shelve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.116983 precli-0.5.6/tests/unit/rules/python/stdlib/shelve/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/shelve/examples/shelve_dbfilenameshelf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/shelve/examples/shelve_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/shelve/examples/shelve_open_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/shelve/test_shelve_open.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.116983 precli-0.5.6/tests/unit/rules/python/stdlib/smtplib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/smtplib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.116983 precli-0.5.6/tests/unit/rules/python/stdlib/smtplib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_none.py
+-rw-r--r--   0 runner    (1001) docker     (127)      731 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_unset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/smtplib/test_smtplib_cleartext.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/smtplib/test_smtplib_unverified_context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.120983 precli-0.5.6/tests/unit/rules/python/stdlib/socket/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/socket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.120983 precli-0.5.6/tests/unit/rules/python/stdlib/socket/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/socket/examples/socket_create_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/socket/examples/socket_socket_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/socket/examples/socket_socket_bind_as_var.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/socket/examples/socket_socket_bind_as_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/socket/test_socket_unrestricted_bind.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.120983 precli-0.5.6/tests/unit/rules/python/stdlib/socketserver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/socketserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.120983 precli-0.5.6/tests/unit/rules/python/stdlib/socketserver/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_tcp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_udp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_tcp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_tcp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_udp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_udp_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/socketserver/test_socketserver_unrestricted_bind.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.120983 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.128983 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/create_default_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/create_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_sslv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_sslv23.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_sslv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_tlsv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_tlsv11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/get_server_certificate_tlsv12.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP256r1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP384r1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP384r1tls13.py
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_brainpoolP512r1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_default_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_ffdhe2048.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_prime192v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_prime256v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_secp160r2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_secp256r1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_sect163k1.py
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_sect571k1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_typed_default_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_typed_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_set_ecdh_curve_unverified_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_sslv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_sslv23.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_sslv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_tlsv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_tlsv11.py
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/ssl_context_tlsv12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv23.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv2_server_side_true.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_sslv3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_tlsv1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_tlsv11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/examples/wrap_socket_tlsv12.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/test_ssl_context_tls_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2063 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/test_ssl_context_weak_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/test_ssl_create_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/test_ssl_get_server_certificate_tls_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/ssl/test_ssl_wrap_socket_tls_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.128983 precli-0.5.6/tests/unit/rules/python/stdlib/telnetlib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/telnetlib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.128983 precli-0.5.6/tests/unit/rules/python/stdlib/telnetlib/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/telnetlib/examples/telnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/telnetlib/examples/telnetlib_telnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/telnetlib/examples/telnetlib_telnet_context_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/telnetlib/test_telnetlib_cleartext.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.128983 precli-0.5.6/tests/unit/rules/python/stdlib/tempfile/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/tempfile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.132983 precli-0.5.6/tests/unit/rules/python/stdlib/tempfile/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_args_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_args_with_open_args.py
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_walrus_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_with_open.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/tempfile/examples/tempfile_mktemp_with_open_multiline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/tempfile/test_tempfile_mktemp_race_condition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.132983 precli-0.5.6/tests/unit/rules/python/stdlib/xmlrpc/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/xmlrpc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 16:26:51.132983 precli-0.5.6/tests/unit/rules/python/stdlib/xmlrpc/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/xmlrpc/examples/xmlrpc_server_doc_xml_rpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/xmlrpc/examples/xmlrpc_server_simple_xml_rpc_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/python/stdlib/xmlrpc/test_xmlrpc_server_unrestricted_bind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2211 2024-05-30 16:26:47.000000 precli-0.5.6/tests/unit/rules/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-30 16:26:47.000000 precli-0.5.6/tox.ini
```

### Comparing `precli-0.5.5/.github/workflows/dependency-review.yml` & `precli-0.5.6/.github/workflows/dependency-review.yml`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/.github/workflows/publish-to-pypi.yml` & `precli-0.5.6/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/.github/workflows/publish-to-test-pypi.yml` & `precli-0.5.6/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/.github/workflows/unit-test.yml` & `precli-0.5.6/.github/workflows/unit-test.yml`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/.github/workflows/upload-asset.yml` & `precli-0.5.6/.github/workflows/upload-asset.yml`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/.pre-commit-config.yaml` & `precli-0.5.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/CODE_OF_CONDUCT.md` & `precli-0.5.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/ChangeLog` & `precli-0.5.6/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 CHANGES
 =======
 
+0.5.6
+-----
+
+* Removal of the Cwe2 dependency (#499)
+* Bump requests from 2.32.2 to 2.32.3 (#498)
+* Return a rule ID for syntax and other errors (#496)
+* Small refactor on where Tool is initialized (#495)
+
 0.5.5
 -----
 
 * Fix for traceback in plain renderer (#494)
 * Filter the list of artifacts during discovery (#491)
 * Nit: Rearrange args to partial (#490)
 * Delay reading of file contents until parser decided (#489)
```

### Comparing `precli-0.5.5/LICENSE` & `precli-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/PKG-INFO` & `precli-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: precli
-Version: 0.5.5
+Version: 0.5.6
 Summary: Static analysis security tool command line
 Home-page: https://github.com/securesauce/precli
 Download-URL: https://pypi.org/project/precli/#files
 Author: Secure Sauce
 Project-URL: Release notes, https://github.com/securesauce/precli/releases
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -15,21 +15,20 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
 Requires-Python: >=3.12
 License-File: LICENSE
-Requires-Dist: cwe2==2.0.0
 Requires-Dist: Pygments==2.18.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: tree-sitter==0.21.3
 Requires-Dist: tree-sitter-languages==1.10.2
 Requires-Dist: ignorelib==0.3.0
-Requires-Dist: requests==2.32.2
+Requires-Dist: requests==2.32.3
 Requires-Dist: sarif-om==1.0.4
 Requires-Dist: jschema-to-python==1.2.3
 Requires-Dist: outdated==0.2.2
 
 .. image:: https://raw.githubusercontent.com/securesauce/precli/main/logo/logo.png
     :alt: Precaution CLI
```

### Comparing `precli-0.5.5/README.rst` & `precli-0.5.6/README.rst`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/SECURITY.md` & `precli-0.5.6/SECURITY.md`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/docs/getting-started.md` & `precli-0.5.6/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/docs/man/precli.rst` & `precli-0.5.6/docs/man/precli.rst`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/docs/rules.md` & `precli-0.5.6/docs/rules.md`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/logo/logo.png` & `precli-0.5.6/logo/logo.png`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/cli/main.py` & `precli-0.5.6/precli/cli/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from outdated import check_outdated
 from rich import progress
 from rich.console import Console
 
 import precli
 from precli.core.artifact import Artifact
 from precli.core.run import Run
-from precli.core.tool import Tool
 from precli.renderers.detailed import Detailed
 from precli.renderers.json import Json
 from precli.renderers.markdown import Markdown
 from precli.renderers.plain import Plain
 
 
 BUSL_URL = "https://spdx.org/licenses/BUSL-1.1.html"
@@ -343,27 +342,16 @@
 
     console = Console(
         file=file,
         no_color=True if file.name != sys.stdout.name else False,
         highlight=False,
     )
 
-    # Initialize the run
-    tool = Tool(
-        name="Precaution",
-        download_uri=precli.__download_url__,
-        full_description=precli.__summary__,
-        information_uri=precli.__url__,
-        organization=precli.__author__,
-        short_description=precli.__summary__,
-        version=precli.__version__,
-    )
-    run = Run(tool, enabled, disabled, artifacts, console, debug)
-
     # Invoke the run
+    run = Run(enabled, disabled, artifacts, console, debug)
     run.invoke()
 
     if args.json is True:
         renderer = "json"
         json = Json(console)
         json.render(run)
     elif args.plain is True:
```

### Comparing `precli-0.5.5/precli/core/argument.py` & `precli-0.5.6/precli/core/argument.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/core/artifact.py` & `precli-0.5.6/precli/core/artifact.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/core/call.py` & `precli-0.5.6/precli/core/call.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/core/comparison.py` & `precli-0.5.6/precli/core/comparison.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/core/config.py` & `precli-0.5.6/precli/core/config.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/core/fix.py` & `precli-0.5.6/precli/core/fix.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/core/kind.py` & `precli-0.5.6/precli/core/kind.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/core/level.py` & `precli-0.5.6/precli/core/level.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/core/linecache.py` & `precli-0.5.6/precli/core/linecache.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/core/location.py` & `precli-0.5.6/precli/core/location.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/core/metrics.py` & `precli-0.5.6/precli/core/metrics.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/core/redos.py` & `precli-0.5.6/precli/core/redos.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/core/result.py` & `precli-0.5.6/precli/core/result.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/core/run.py` & `precli-0.5.6/precli/core/run.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from functools import partial
 from multiprocessing import Pool
 
 from pygments import lexers
 from rich.console import Console
 from rich.progress import Progress
 
+import precli
 from precli.core import loader
 from precli.core.artifact import Artifact
 from precli.core.level import Level
 from precli.core.location import Location
 from precli.core.metrics import Metrics
 from precli.core.result import Result
 from precli.core.tool import Tool
@@ -26,14 +27,15 @@
 PROGRESS_THRESHOLD = 50
 parsers = loader.load_parsers()
 
 
 def parse_file(
     artifact: Artifact, enabled: list[str], disabled: list[str]
 ) -> list[Result]:
+    parser = None
     results = []
     try:
         if artifact.file_name == "-":
             open_fd = os.fdopen(sys.stdin.fileno(), "rb", 0)
             fdata = io.BytesIO(open_fd.read())
             artifact.file_name = "<stdin>"
             artifact.contents = fdata.read()
@@ -56,68 +58,66 @@
             artifact.language = parser.lexer
             with open(artifact.file_name, "rb") as f:
                 artifact.contents = f.read()
             return parser.parse(artifact, enabled, disabled)
     except OSError as e:
         results.append(
             Result(
-                "NO_RULE",
+                f"{parser.rule_prefix()}000" if parser else "NO_RULE",
                 location=Location(parser.context["node"]),
                 artifact=artifact,
                 level=Level.ERROR,
                 message=e.strerror,
             )
         )
     except SyntaxError as e:
         results.append(
             Result(
-                "NO_RULE",
+                f"{parser.rule_prefix()}000" if parser else "NO_RULE",
                 location=Location(
                     start_line=e.lineno,
                     end_line=e.lineno,
                 ),
                 artifact=artifact,
                 level=Level.ERROR,
                 message="Syntax error while parsing file.",
             )
         )
     except UnicodeDecodeError:
         results.append(
             Result(
-                "NO_RULE",
+                f"{parser.rule_prefix()}000" if parser else "NO_RULE",
                 location=Location(parser.context["node"]),
                 artifact=artifact,
                 level=Level.ERROR,
                 message="Invalid unicode character while parsing file.",
             )
         )
     except Exception as e:
         results.append(
             Result(
-                "NO_RULE",
+                f"{parser.rule_prefix()}000" if parser else "NO_RULE",
                 location=Location(parser.context["node"]),
                 artifact=artifact,
                 level=Level.ERROR,
                 message=": ".join([type(e).__name__, str(e)]),
             )
         )
     return results
 
 
 class Run:
     def __init__(
         self,
-        tool: Tool,
         enabled: list[str],
         disabled: list[str],
         artifacts: list[Artifact],
         console: Console,
         debug,
     ):
-        self._tool = tool
         self._enabled = enabled
         self._disabled = disabled
         self._artifacts = artifacts
         self._console = console
         self._init_logger(debug)
         self._start_time = None
         self._end_time = None
@@ -131,14 +131,24 @@
         LOG.handlers = []
         logging.captureWarnings(True)
         LOG.setLevel(log_level)
         handler = logging.StreamHandler(sys.stderr)
         LOG.addHandler(handler)
         LOG.debug("logging initialized")
 
+        self._tool = Tool(
+            name="Precaution",
+            download_uri=precli.__download_url__,
+            full_description=precli.__summary__,
+            information_uri=precli.__url__,
+            organization=precli.__author__,
+            short_description=precli.__summary__,
+            version=precli.__version__,
+        )
+
     @property
     def tool(self) -> Tool:
         """Get the tool associated with this run."""
         return self._tool
 
     @property
     def rules(self) -> list[Rule]:
```

### Comparing `precli-0.5.5/precli/core/suppression.py` & `precli-0.5.6/precli/core/suppression.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/core/symtab.py` & `precli-0.5.6/precli/core/symtab.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/core/tool.py` & `precli-0.5.6/precli/core/tool.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/core/utils.py` & `precli-0.5.6/precli/core/utils.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/parsers/__init__.py` & `precli-0.5.6/precli/parsers/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,18 @@
         """The name of the lexer"""
         return self._lexer
 
     @abstractmethod
     def file_extensions(self) -> list[str]:
         """File extension of files this parser can handle."""
 
+    @abstractmethod
+    def rule_prefix(self) -> str:
+        """The prefix for the rule ID"""
+
     def parse(
         self, artifact: Artifact, enabled: list = None, disabled: list = None
     ) -> list[Result]:
         """File extension of files this parser can handle."""
         for rule in self.rules.values():
             if enabled is not None and (
                 enabled == ["all"]
```

### Comparing `precli-0.5.5/precli/parsers/go.py` & `precli-0.5.6/precli/parsers/go.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,17 @@
             r"// suppress:? (?P<rules>[^#]+)?#?"
         )
         self.SUPPRESSED_RULES = re.compile(r"(?:(GO\d\d\d|[a-z_]+),?)+")
 
     def file_extensions(self) -> list[str]:
         return [".go"]
 
+    def rule_prefix(self) -> str:
+        return "GO"
+
     def get_file_encoding(self, file_path):
         return "utf-8"
 
     def visit_source_file(self, nodes: list[Node]):
         self.suppressions = {}
         self.current_symtab = SymbolTable("<source_file>")
         self.visit(nodes)
```

### Comparing `precli-0.5.5/precli/parsers/java.py` & `precli-0.5.6/precli/parsers/java.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,17 @@
             r"// suppress:? (?P<rules>[^#]+)?#?"
         )
         self.SUPPRESSED_RULES = re.compile(r"(?:(JAV\d\d\d|[a-z_]+),?)+")
 
     def file_extensions(self) -> list[str]:
         return [".java"]
 
+    def rule_prefix(self) -> str:
+        return "JAV"
+
     def get_file_encoding(self, file_path):
         return "utf-8"
 
     def visit_program(self, nodes: list[Node]):
         self.suppressions = {}
         self.current_symtab = SymbolTable("<program>")
         self.visit(nodes)
```

### Comparing `precli-0.5.5/precli/parsers/python.py` & `precli-0.5.6/precli/parsers/python.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,17 @@
         super().__init__("python")
         self.SUPPRESS_COMMENT = re.compile(r"# suppress:? (?P<rules>[^#]+)?#?")
         self.SUPPRESSED_RULES = re.compile(r"(?:(PY\d\d\d|[a-z_]+),?)+")
 
     def file_extensions(self) -> list[str]:
         return [".py", ".pyw"]
 
+    def rule_prefix(self) -> str:
+        return "PY"
+
     def get_file_encoding(self, file_path):
         with open(file_path, "rb") as f:
             first_two_lines = f.readline() + f.readline()
 
         encoding_match = re.search(rb"coding[:=]\s*([-\w.]+)", first_two_lines)
         if encoding_match:
             encoding = encoding_match.group(1).decode("ascii")
```

### Comparing `precli-0.5.5/precli/parsers/tokens.py` & `precli-0.5.6/precli/parsers/tokens.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/renderers/detailed.py` & `precli-0.5.6/precli/renderers/detailed.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/renderers/json.py` & `precli-0.5.6/precli/renderers/json.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
             ),
             message_strings={
                 "default": sarif_om.MultiformatMessageString(text=rule.message)
             },
             properties={
                 "tags": [
                     "security",
-                    f"external/cwe/cwe-{rule.cwe.cwe_id}",
+                    f"external/cwe/cwe-{rule.cwe.id}",
                 ],
                 "security-severity": (rule.default_config.level.to_severity()),
             },
         )
 
         index = len(rules)
         rules[rule.id] = reporting_descriptor
```

### Comparing `precli-0.5.5/precli/renderers/markdown.py` & `precli-0.5.6/precli/renderers/markdown.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/renderers/plain.py` & `precli-0.5.6/precli/renderers/plain.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/__init__.py` & `precli-0.5.6/precli/rules/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 # Copyright 2024 Secure Sauce LLC
 from abc import ABC
 from typing import Self
 
-from cwe2.database import Database
-from cwe2.weakness import Weakness
-
 from precli.core.config import Config
+from precli.core.cwe import Cwe
 from precli.core.fix import Fix
 from precli.core.location import Location
 
 
 class Rule(ABC):
     _rules = {}
-    _cwedb = Database()
 
     def __init__(
         self,
         id: str,
         name: str,
         description: str,
         cwe_id: int,
@@ -37,15 +34,15 @@
             end = len(description)
         self._short_descr = description[start:end].replace("`", "")
         try:
             start = description.index("\n\n") + 2
         except ValueError:
             start = 0
         self._full_descr = description[start:]
-        self._cwe = Rule._cwedb.get(cwe_id)
+        self._cwe = Cwe(cwe_id)
         self._message = message
         self._wildcards = wildcards
         self._config = Config() if not config else config
         self._enabled = self._config.enabled
         self._help_url = f"https://docs.securesauce.dev/rules/{id}"
         Rule._rules[id] = self
 
@@ -103,15 +100,15 @@
 
     @enabled.setter
     def enabled(self, enabled):
         """Set whether the rule is enabled"""
         self._enabled = enabled
 
     @property
-    def cwe(self) -> Weakness:
+    def cwe(self) -> Cwe:
         """CWE weakness object for this rule."""
         return self._cwe
 
     @property
     def message(self) -> str:
         """Concise description message of the found issue."""
         return self._message
```

### Comparing `precli-0.5.5/precli/rules/go/stdlib/crypto_weak_cipher.py` & `precli-0.5.6/precli/rules/go/stdlib/crypto_weak_cipher.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/go/stdlib/crypto_weak_hash.py` & `precli-0.5.6/precli/rules/go/stdlib/crypto_weak_hash.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/go/stdlib/crypto_weak_key.py` & `precli-0.5.6/precli/rules/go/stdlib/crypto_weak_key.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/java/stdlib/java_net_insecure_cookie.py` & `precli-0.5.6/precli/rules/java/stdlib/java_net_insecure_cookie.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/java/stdlib/java_security_weak_hash.py` & `precli-0.5.6/precli/rules/java/stdlib/java_security_weak_hash.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/java/stdlib/java_security_weak_key.py` & `precli-0.5.6/precli/rules/java/stdlib/java_security_weak_key.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/java/stdlib/java_security_weak_random.py` & `precli-0.5.6/precli/rules/java/stdlib/java_security_weak_random.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/java/stdlib/javax_crypto_weak_cipher.py` & `precli-0.5.6/precli/rules/java/stdlib/javax_crypto_weak_cipher.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/java/stdlib/javax_servlet_http_insecure_cookie.py` & `precli-0.5.6/precli/rules/java/stdlib/javax_servlet_http_insecure_cookie.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/argparse_sensitive_info.py` & `precli-0.5.6/precli/rules/python/stdlib/argparse_sensitive_info.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/assert.py` & `precli-0.5.6/precli/rules/python/stdlib/assert.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/crypt_weak_hash.py` & `precli-0.5.6/precli/rules/python/stdlib/crypt_weak_hash.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/ftplib_cleartext.py` & `precli-0.5.6/precli/rules/python/stdlib/ftplib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/ftplib_unverified_context.py` & `precli-0.5.6/precli/rules/python/stdlib/ftplib_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/hashlib_improper_prng.py` & `precli-0.5.6/precli/rules/python/stdlib/hashlib_improper_prng.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/hashlib_weak_hash.py` & `precli-0.5.6/precli/rules/python/stdlib/hashlib_weak_hash.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/hmac_timing_attack.py` & `precli-0.5.6/precli/rules/python/stdlib/hmac_timing_attack.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/hmac_weak_hash.py` & `precli-0.5.6/precli/rules/python/stdlib/hmac_weak_hash.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/hmac_weak_key.py` & `precli-0.5.6/precli/rules/python/stdlib/hmac_weak_key.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/http_server_unrestricted_bind.py` & `precli-0.5.6/precli/rules/python/stdlib/http_server_unrestricted_bind.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/http_url_secret.py` & `precli-0.5.6/precli/rules/python/stdlib/http_url_secret.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/imaplib_cleartext.py` & `precli-0.5.6/precli/rules/python/stdlib/imaplib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/imaplib_unverified_context.py` & `precli-0.5.6/precli/rules/python/stdlib/imaplib_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/json_load.py` & `precli-0.5.6/precli/rules/python/stdlib/json_load.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/logging_insecure_listen_config.py` & `precli-0.5.6/precli/rules/python/stdlib/logging_insecure_listen_config.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/marshal_load.py` & `precli-0.5.6/precli/rules/python/stdlib/marshal_load.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/nntplib_cleartext.py` & `precli-0.5.6/precli/rules/python/stdlib/nntplib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/nntplib_unverified_context.py` & `precli-0.5.6/precli/rules/python/stdlib/nntplib_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/pickle_load.py` & `precli-0.5.6/precli/rules/python/stdlib/pickle_load.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/poplib_cleartext.py` & `precli-0.5.6/precli/rules/python/stdlib/poplib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/poplib_unverified_context.py` & `precli-0.5.6/precli/rules/python/stdlib/poplib_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/re_denial_of_service.py` & `precli-0.5.6/precli/rules/python/stdlib/re_denial_of_service.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/secrets_weak_token.py` & `precli-0.5.6/precli/rules/python/stdlib/secrets_weak_token.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/shelve_open.py` & `precli-0.5.6/precli/rules/python/stdlib/shelve_open.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/smtplib_cleartext.py` & `precli-0.5.6/precli/rules/python/stdlib/smtplib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/smtplib_unverified_context.py` & `precli-0.5.6/precli/rules/python/stdlib/smtplib_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/socket_unrestricted_bind.py` & `precli-0.5.6/precli/rules/python/stdlib/socket_unrestricted_bind.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/socketserver_unrestricted_bind.py` & `precli-0.5.6/precli/rules/python/stdlib/socketserver_unrestricted_bind.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/ssl_context_weak_key.py` & `precli-0.5.6/precli/rules/python/stdlib/ssl_context_weak_key.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/ssl_create_unverified_context.py` & `precli-0.5.6/precli/rules/python/stdlib/ssl_create_unverified_context.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/ssl_insecure_tls_version.py` & `precli-0.5.6/precli/rules/python/stdlib/ssl_insecure_tls_version.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/telnetlib_cleartext.py` & `precli-0.5.6/precli/rules/python/stdlib/telnetlib_cleartext.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/tempfile_mktemp_race_condition.py` & `precli-0.5.6/precli/rules/python/stdlib/tempfile_mktemp_race_condition.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli/rules/python/stdlib/xmlrpc_server_unrestricted_bind.py` & `precli-0.5.6/precli/rules/python/stdlib/xmlrpc_server_unrestricted_bind.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/precli.egg-info/PKG-INFO` & `precli-0.5.6/precli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: precli
-Version: 0.5.5
+Version: 0.5.6
 Summary: Static analysis security tool command line
 Home-page: https://github.com/securesauce/precli
 Download-URL: https://pypi.org/project/precli/#files
 Author: Secure Sauce
 Project-URL: Release notes, https://github.com/securesauce/precli/releases
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -15,21 +15,20 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
 Requires-Python: >=3.12
 License-File: LICENSE
-Requires-Dist: cwe2==2.0.0
 Requires-Dist: Pygments==2.18.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: tree-sitter==0.21.3
 Requires-Dist: tree-sitter-languages==1.10.2
 Requires-Dist: ignorelib==0.3.0
-Requires-Dist: requests==2.32.2
+Requires-Dist: requests==2.32.3
 Requires-Dist: sarif-om==1.0.4
 Requires-Dist: jschema-to-python==1.2.3
 Requires-Dist: outdated==0.2.2
 
 .. image:: https://raw.githubusercontent.com/securesauce/precli/main/logo/logo.png
     :alt: Precaution CLI
```

### Comparing `precli-0.5.5/precli.egg-info/SOURCES.txt` & `precli-0.5.6/precli.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 precli/cli/main.py
 precli/core/__init__.py
 precli/core/argument.py
 precli/core/artifact.py
 precli/core/call.py
 precli/core/comparison.py
 precli/core/config.py
+precli/core/cwe.py
 precli/core/fix.py
 precli/core/kind.py
 precli/core/level.py
 precli/core/linecache.py
 precli/core/loader.py
 precli/core/location.py
 precli/core/metrics.py
```

### Comparing `precli-0.5.5/precli.egg-info/entry_points.txt` & `precli-0.5.6/precli.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/pylintrc` & `precli-0.5.6/pylintrc`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/setup.cfg` & `precli-0.5.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/parsers/test_go.py` & `precli-0.5.6/tests/unit/parsers/test_go.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/parsers/test_python.py` & `precli-0.5.6/tests/unit/parsers/test_python.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_rc4.go` & `precli-0.5.6/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_cipher_rc4.go`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_1024.go` & `precli-0.5.6/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_1024.go`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_2048.go` & `precli-0.5.6/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_2048.go`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_3072.go` & `precli-0.5.6/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_dsa_3072.go`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_1024.go` & `precli-0.5.6/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_1024.go`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_2048.go` & `precli-0.5.6/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_2048.go`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_4096.go` & `precli-0.5.6/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_4096.go`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_bits_as_var.go` & `precli-0.5.6/tests/unit/rules/go/stdlib/crypto/examples/crypto_weak_key_rsa_bits_as_var.go`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_cipher.py` & `precli-0.5.6/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_cipher.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.ERROR
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "327"
+        assert rule.cwe.id == 327
 
     @pytest.mark.parametrize(
         "filename",
         [
             "crypto_weak_cipher_aes.go",
             "crypto_weak_cipher_des.go",
             "crypto_weak_cipher_rc4.go",
```

### Comparing `precli-0.5.5/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_hash.py` & `precli-0.5.6/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_hash.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.ERROR
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "328"
+        assert rule.cwe.id == 328
 
     @pytest.mark.parametrize(
         "filename",
         [
             "crypto_weak_hash_md5_new.go",
             "crypto_weak_hash_md5_sum.go",
             "crypto_weak_hash_sha1_new.go",
```

### Comparing `precli-0.5.5/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_key.py` & `precli-0.5.6/tests/unit/rules/go/stdlib/crypto/test_crypto_weak_key.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "326"
+        assert rule.cwe.id == 326
 
     @pytest.mark.parametrize(
         "filename",
         [
             "crypto_weak_key_dsa_1024.go",
             "crypto_weak_key_dsa_2048.go",
             "crypto_weak_key_dsa_3072.go",
```

### Comparing `precli-0.5.5/tests/unit/rules/java/stdlib/java_net/test_insecure_cookie.py` & `precli-0.5.6/tests/unit/rules/java/stdlib/javax_servlet_http/test_insecure_cookie.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,41 +8,41 @@
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
 class TestInsecureCookie(test_case.TestCase):
     @classmethod
     def setup_class(cls):
-        cls.rule_id = "JAV006"
+        cls.rule_id = "JAV005"
         cls.parser = java.Java()
         cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "java",
             "stdlib",
-            "java_net",
+            "javax_servlet_http",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
         assert rule.id == self.rule_id
         assert rule.name == "insecure_cookie"
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "614"
+        assert rule.cwe.id == 614
 
     @pytest.mark.parametrize(
         "filename",
         [
-            "HttpCookieSecureFalse.java",
-            "HttpCookieSecureTrue.java",
+            "CookieSecureFalse.java",
+            "CookieSecureTrue.java",
         ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/KeyPairGeneratorDSA.java` & `precli-0.5.6/tests/unit/rules/java/stdlib/java_security/examples/KeyPairGeneratorDSA.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/KeyPairGeneratorRSA.java` & `precli-0.5.6/tests/unit/rules/java/stdlib/java_security/examples/KeyPairGeneratorRSA.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestMD5Property.java` & `precli-0.5.6/tests/unit/rules/java/stdlib/java_security/examples/MessageDigestMD5Property.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/java/stdlib/java_security/test_weak_hash.py` & `precli-0.5.6/tests/unit/rules/java/stdlib/java_security/test_weak_hash.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.ERROR
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "328"
+        assert rule.cwe.id == 328
 
     @pytest.mark.parametrize(
         "filename",
         [
             "MessageDigestMD2.java",
             "MessageDigestMD5.java",
             "MessageDigestMD5Property.java",
```

### Comparing `precli-0.5.5/tests/unit/rules/java/stdlib/java_security/test_weak_key.py` & `precli-0.5.6/tests/unit/rules/java/stdlib/java_security/test_weak_key.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "326"
+        assert rule.cwe.id == 326
 
     @pytest.mark.parametrize(
         "filename",
         [
             "KeyPairGeneratorDSA.java",
             "KeyPairGeneratorRSA.java",
         ],
```

### Comparing `precli-0.5.5/tests/unit/rules/java/stdlib/java_security/test_weak_random.py` & `precli-0.5.6/tests/unit/rules/java/stdlib/java_security/test_weak_random.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "338"
+        assert rule.cwe.id == 338
 
     @pytest.mark.parametrize(
         "filename",
         [
             "JavaSecuritySecureRandomSHA1PRNG.java",
             "SecureRandomDefault.java",
             "SecureRandomSHA1PRNG.java",
```

### Comparing `precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/Cipher3DESCBC.java` & `precli-0.5.6/tests/unit/rules/java/stdlib/javax_crypto/examples/Cipher3DESCBC.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherAESCBC.java` & `precli-0.5.6/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherAESCBC.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherArcfour.java` & `precli-0.5.6/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherArcfour.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherBlowfishCBC.java` & `precli-0.5.6/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherBlowfishCBC.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherDESCBC.java` & `precli-0.5.6/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherDESCBC.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC2.java` & `precli-0.5.6/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC2.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC5.java` & `precli-0.5.6/tests/unit/rules/java/stdlib/javax_crypto/examples/CipherRC5.java`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/java/stdlib/javax_crypto/test_weak_cipher.py` & `precli-0.5.6/tests/unit/rules/java/stdlib/javax_crypto/test_weak_cipher.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.ERROR
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "327"
+        assert rule.cwe.id == 327
 
     @pytest.mark.parametrize(
         "filename",
         [
             "Cipher3DESCBC.java",
             "CipherAESCBC.java",
             "CipherArcfour.java",
```

### Comparing `precli-0.5.5/tests/unit/rules/java/stdlib/javax_servlet_http/test_insecure_cookie.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/test_hashlib_improper_prng.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,50 @@
 # Copyright 2024 Secure Sauce LLC
 import os
 
 import pytest
 
 from precli.core.level import Level
-from precli.parsers import java
+from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class TestInsecureCookie(test_case.TestCase):
+class TestHashlibImproperPrng(test_case.TestCase):
     @classmethod
     def setup_class(cls):
-        cls.rule_id = "JAV005"
-        cls.parser = java.Java()
+        cls.rule_id = "PY035"
+        cls.parser = python.Python()
         cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
-            "java",
+            "python",
             "stdlib",
-            "javax_servlet_http",
+            "hashlib",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
         assert rule.id == self.rule_id
-        assert rule.name == "insecure_cookie"
+        assert rule.name == "improper_random"
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "614"
+        assert rule.cwe.id == 330
 
     @pytest.mark.parametrize(
         "filename",
         [
-            "CookieSecureFalse.java",
-            "CookieSecureTrue.java",
+            "hashlib_improper_prng_blake2b.py",
+            "hashlib_improper_prng_blake2s.py",
+            "hashlib_improper_prng_pbkdf2_hmac.py",
+            "hashlib_improper_prng_scrypt.py",
         ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/argparse/test_argparse_sensitive_info.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/argparse/test_argparse_sensitive_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.ERROR
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "214"
+        assert rule.cwe.id == 214
 
     @pytest.mark.parametrize(
         "filename",
         [
             "argparse_add_argument_api_key.py",
             "argparse_add_argument_default_action.py",
             "argparse_add_argument_password.py",
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/assert/test_assert.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/assert/test_assert.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "703"
+        assert rule.cwe.id == 703
 
     @pytest.mark.parametrize(
         "filename",
         [
             "assert.py",
         ],
     )
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/crypt/test_crypt_weak_hash.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/crypt/test_crypt_weak_hash.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "328"
+        assert rule.cwe.id == 328
 
     @pytest.mark.parametrize(
         "filename",
         [
             "crypt_crypt.py",
             "crypt_crypt_method_blowfish.py",
             "crypt_crypt_method_crypt.py",
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/test_ftplib_cleartext.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/ftplib/test_ftplib_cleartext.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "319"
+        assert rule.cwe.id == 319
 
     @pytest.mark.parametrize(
         "filename",
         [
             "ftp.py",
             "ftp_context_mgr.py",
             "ftp_tls.py",
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/ftplib/test_ftplib_unverified_context.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/ftplib/test_ftplib_unverified_context.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "295"
+        assert rule.cwe.id == 295
 
     @pytest.mark.parametrize(
         "filename",
         [
             "ftplib_ftp_tls_context_as_var.py",
             "ftplib_ftp_tls_context_none.py",
             "ftplib_ftp_tls_context_unset.py",
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/test_hashlib_improper_prng.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/http/test_http_server_unrestricted_bind.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,46 +5,44 @@
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class TestHashlibImproperPrng(test_case.TestCase):
+class TestHttpServerUnrestrictedBind(test_case.TestCase):
     @classmethod
     def setup_class(cls):
-        cls.rule_id = "PY035"
+        cls.rule_id = "PY031"
         cls.parser = python.Python()
         cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
-            "hashlib",
+            "http",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
         assert rule.id == self.rule_id
-        assert rule.name == "improper_random"
+        assert rule.name == "unrestricted_bind"
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "330"
+        assert rule.cwe.id == 1327
 
     @pytest.mark.parametrize(
         "filename",
         [
-            "hashlib_improper_prng_blake2b.py",
-            "hashlib_improper_prng_blake2s.py",
-            "hashlib_improper_prng_pbkdf2_hmac.py",
-            "hashlib_improper_prng_scrypt.py",
+            "http_server_http_server.py",
+            "http_server_threading_http_server.py",
         ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/hashlib/test_hashlib_weak_hash.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/hashlib/test_hashlib_weak_hash.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.ERROR
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "328"
+        assert rule.cwe.id == 328
 
     @pytest.mark.parametrize(
         "filename",
         [
             "hashlib_blake2b.py",
             "hashlib_blake2s.py",
             "hashlib_md4.py",
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/hmac/test_hmac_timing_attack.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/hmac/test_hmac_timing_attack.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.ERROR
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "208"
+        assert rule.cwe.id == 208
 
     @pytest.mark.parametrize(
         "filename",
         [
             "hmac_timing_attack.py",
             "hmac_timing_attack_class.py",
             "hmac_timing_attack_class_hexdigest.py",
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_hash.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_hash.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.ERROR
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "328"
+        assert rule.cwe.id == 328
 
     @pytest.mark.parametrize(
         "filename",
         [
             "hmac_digest_blake2b.py",
             "hmac_digest_blake2s.py",
             "hmac_digest_hashlib_blake2b.py",
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_key.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/hmac/test_hmac_weak_key.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "326"
+        assert rule.cwe.id == 326
 
     @pytest.mark.parametrize(
         "filename",
         [
             "hmac_digest_weak_key_hashlib_blake2b.py",
             "hmac_digest_weak_key_hashlib_sha3_256.py",
             "hmac_digest_weak_key_hashlib_sm3.py",
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/http/test_http_server_unrestricted_bind.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/xmlrpc/test_xmlrpc_server_unrestricted_bind.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,44 +5,44 @@
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class TestHttpServerUnrestrictedBind(test_case.TestCase):
+class TestXmlrpcServerUnrestrictedBind(test_case.TestCase):
     @classmethod
     def setup_class(cls):
-        cls.rule_id = "PY031"
+        cls.rule_id = "PY032"
         cls.parser = python.Python()
         cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
-            "http",
+            "xmlrpc",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
         assert rule.id == self.rule_id
         assert rule.name == "unrestricted_bind"
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "1327"
+        assert rule.cwe.id == 1327
 
     @pytest.mark.parametrize(
         "filename",
         [
-            "http_server_http_server.py",
-            "http_server_threading_http_server.py",
+            "xmlrpc_server_doc_xml_rpc_server.py",
+            "xmlrpc_server_simple_xml_rpc_server.py",
         ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/http/test_http_url_secret.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/http/test_http_url_secret.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.ERROR
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "598"
+        assert rule.cwe.id == 598
 
     @pytest.mark.parametrize(
         "filename",
         [
             "http_url_secret_apikey.py",
             "http_url_secret_apikey_in_header.py",
             "http_url_secret_basic_auth.py",
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/test_imaplib_cleartext.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/imaplib/test_imaplib_cleartext.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.ERROR
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "319"
+        assert rule.cwe.id == 319
 
     @pytest.mark.parametrize(
         "filename",
         [
             "imaplib_imap4_authenticate.py",
             "imaplib_imap4_context_mgr.py",
             "imaplib_imap4_login.py",
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/imaplib/test_imaplib_unverified_context.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/imaplib/test_imaplib_unverified_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "295"
+        assert rule.cwe.id == 295
 
     @pytest.mark.parametrize(
         "filename",
         [
             "imaplib_imap4_ssl_context_as_var.py",
             "imaplib_imap4_ssl_context_none.py",
             "imaplib_imap4_ssl_context_unset.py",
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/json/test_json_load.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/json/test_json_load.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is False
         assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "502"
+        assert rule.cwe.id == 502
 
     @pytest.mark.parametrize(
         "filename",
         [
             "json_jsondecoder_decode.py",
             "json_load.py",
             "json_loads.py",
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/logging/test_logging_insecure_listen_config.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/logging/test_logging_insecure_listen_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "94"
+        assert rule.cwe.id == 94
 
     @pytest.mark.parametrize(
         "filename",
         [
             "insecure_listen_config_empty_args.py",
             "insecure_listen_config_port.py",
             "insecure_listen_config_port_verify_as_var.py",
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/marshal/test_marshal_load.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/marshal/test_marshal_load.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "502"
+        assert rule.cwe.id == 502
 
     @pytest.mark.parametrize(
         "filename",
         [
             "marshal_load.py",
             "marshal_loads.py",
         ],
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/test_nntplib_cleartext.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/nntplib/test_nntplib_cleartext.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.ERROR
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "319"
+        assert rule.cwe.id == 319
 
     @pytest.mark.parametrize(
         "filename",
         [
             "nntplib_nntp_context_mgr.py",
             "nntplib_nntp_login.py",
             "nntplib_nntp_ssl.py",
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/nntplib/test_nntplib_unverified_context.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/nntplib/test_nntplib_unverified_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "295"
+        assert rule.cwe.id == 295
 
     @pytest.mark.parametrize(
         "filename",
         [
             "nntplib_nntp_ssl_context_as_var.py",
             "nntplib_nntp_ssl_context_none.py",
             "nntplib_nntp_ssl_context_unset.py",
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/pickle/test_pickle_load.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/pickle/test_pickle_load.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "502"
+        assert rule.cwe.id == 502
 
     @pytest.mark.parametrize(
         "filename",
         [
             "pickle_load.py",
             "pickle_loads.py",
             "pickle_unpickler.py",
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/poplib/test_poplib_cleartext.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/poplib/test_poplib_cleartext.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.ERROR
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "319"
+        assert rule.cwe.id == 319
 
     @pytest.mark.parametrize(
         "filename",
         [
             "poplib_pop3_apop.py",
             "poplib_pop3_context_mgr.py",
             "poplib_pop3_pass_.py",
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/poplib/test_poplib_unverified_context.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/poplib/test_poplib_unverified_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "295"
+        assert rule.cwe.id == 295
 
     @pytest.mark.parametrize(
         "filename",
         [
             "poplib_pop3_ssl_context_as_var.py",
             "poplib_pop3_ssl_context_none.py",
             "poplib_pop3_ssl_context_unset.py",
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/re/test_re_denial_of_service.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/ssl/test_ssl_wrap_socket_tls_version.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,57 +1,53 @@
-# Copyright 2024 Secure Sauce LLC
+# Copyright 2023 Secure Sauce LLC
 import os
 
 import pytest
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class TestReDenialOfService(test_case.TestCase):
+class TestWrapSocket(test_case.TestCase):
     @classmethod
     def setup_class(cls):
-        cls.rule_id = "PY033"
+        cls.rule_id = "PY018"
         cls.parser = python.Python()
         cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
-            "re",
+            "ssl",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
         assert rule.id == self.rule_id
-        assert rule.name == "regex_denial_of_service"
+        assert rule.name == "inadequate_encryption_strength"
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.ERROR
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "1333"
+        assert rule.cwe.id == 326
 
     @pytest.mark.parametrize(
         "filename",
         [
-            "re_compile.py",
-            "re_compile_good.py",
-            "re_search.py",
-            "re_search_good.py",
-            "re_match.py",
-            "re_fullmatch.py",
-            "re_split.py",
-            "re_findall.py",
-            "re_finditer.py",
-            "re_sub.py",
-            "re_subn.py",
+            "wrap_socket_sslv2.py",
+            "wrap_socket_sslv23.py",
+            "wrap_socket_sslv2_server_side_true.py",
+            "wrap_socket_sslv3.py",
+            "wrap_socket_tlsv1.py",
+            "wrap_socket_tlsv11.py",
+            "wrap_socket_tlsv12.py",
         ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/secrets/test_secrets_weak_token.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/secrets/test_secrets_weak_token.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "326"
+        assert rule.cwe.id == 326
 
     @pytest.mark.parametrize(
         "filename",
         [
             "secrets_token_bytes.py",
             "secrets_token_bytes_default.py",
             "secrets_token_bytes_size_var.py",
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/shelve/test_shelve_open.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/shelve/test_shelve_open.py`

 * *Files 9% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "502"
+        assert rule.cwe.id == 502
 
     @pytest.mark.parametrize(
         "filename",
         [
             "shelve_dbfilenameshelf.py",
             "shelve_open.py",
             "shelve_open_context_mgr.py",
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_auth.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_auth.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_login.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_login.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_as_var.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_as_var.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_none.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_none.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_unset.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_ssl_context_unset.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_as_var.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_as_var.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_none.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_none.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_unset.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/smtplib/examples/smtplib_smtp_starttls_context_unset.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/test_smtplib_cleartext.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/smtplib/test_smtplib_unverified_context.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,47 +5,48 @@
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class TestSmtpCleartext(test_case.TestCase):
+class TestSmtplibUnverifiedContext(test_case.TestCase):
     @classmethod
     def setup_class(cls):
-        cls.rule_id = "PY016"
+        cls.rule_id = "PY026"
         cls.parser = python.Python()
         cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
             "smtplib",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
         assert rule.id == self.rule_id
-        assert rule.name == "cleartext_transmission"
+        assert rule.name == "improper_certificate_validation"
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
-        assert rule.default_config.level == Level.ERROR
+        assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "319"
+        assert rule.cwe.id == 295
 
     @pytest.mark.parametrize(
         "filename",
         [
-            "smtplib_smtp_auth.py",
-            "smtplib_smtp_context_mgr.py",
-            "smtplib_smtp_login.py",
-            "smtplib_smtp_ssl.py",
-            "smtplib_smtp_starttls.py",
+            "smtplib_smtp_ssl_context_as_var.py",
+            "smtplib_smtp_ssl_context_none.py",
+            "smtplib_smtp_ssl_context_unset.py",
+            "smtplib_smtp_starttls_context_as_var.py",
+            "smtplib_smtp_starttls_context_none.py",
+            "smtplib_smtp_starttls_context_unset.py",
         ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/smtplib/test_smtplib_unverified_context.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/ssl/test_ssl_create_context.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,48 +5,44 @@
 
 from precli.core.level import Level
 from precli.parsers import python
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class TestSmtplibUnverifiedContext(test_case.TestCase):
+class TestSslCreateContext(test_case.TestCase):
     @classmethod
     def setup_class(cls):
-        cls.rule_id = "PY026"
+        cls.rule_id = "PY017"
         cls.parser = python.Python()
         cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
             "python",
             "stdlib",
-            "smtplib",
+            "ssl",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
         assert rule.id == self.rule_id
         assert rule.name == "improper_certificate_validation"
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "295"
+        assert rule.cwe.id == 295
 
     @pytest.mark.parametrize(
         "filename",
         [
-            "smtplib_smtp_ssl_context_as_var.py",
-            "smtplib_smtp_ssl_context_none.py",
-            "smtplib_smtp_ssl_context_unset.py",
-            "smtplib_smtp_starttls_context_as_var.py",
-            "smtplib_smtp_starttls_context_none.py",
-            "smtplib_smtp_starttls_context_unset.py",
+            "create_default_context.py",
+            "create_unverified_context.py",
         ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/socket/test_socket_unrestricted_bind.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/socket/test_socket_unrestricted_bind.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "1327"
+        assert rule.cwe.id == 1327
 
     @pytest.mark.parametrize(
         "filename",
         [
             "socket_create_server.py",
             "socket_socket_bind.py",
             "socket_socket_bind_as_var.py",
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_tcp_server.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_tcp_server.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_udp_server.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_forking_udp_server.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_tcp_server.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_tcp_server.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_tcp_server.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_tcp_server.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_udp_server.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_threading_udp_server.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_udp_server.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/socketserver/examples/socketserver_udp_server.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/socketserver/test_socketserver_unrestricted_bind.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/socketserver/test_socketserver_unrestricted_bind.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "1327"
+        assert rule.cwe.id == 1327
 
     @pytest.mark.parametrize(
         "filename",
         [
             "socketserver_tcp_server.py",
             "socketserver_udp_server.py",
             "socketserver_forking_tcp_server.py",
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/ssl/test_ssl_context_tls_version.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/ssl/test_ssl_context_tls_version.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.ERROR
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "326"
+        assert rule.cwe.id == 326
 
     @pytest.mark.parametrize(
         "filename",
         [
             "ssl_context_sslv2.py",
             "ssl_context_sslv23.py",
             "ssl_context_sslv3.py",
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/ssl/test_ssl_context_weak_key.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/ssl/test_ssl_context_weak_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "326"
+        assert rule.cwe.id == 326
 
     @pytest.mark.parametrize(
         "filename",
         [
             "ssl_context_set_ecdh_curve_brainpoolP256r1.py",
             "ssl_context_set_ecdh_curve_brainpoolP384r1.py",
             "ssl_context_set_ecdh_curve_brainpoolP384r1tls13.py",
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/ssl/test_ssl_get_server_certificate_tls_version.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/ssl/test_ssl_get_server_certificate_tls_version.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.ERROR
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "326"
+        assert rule.cwe.id == 326
 
     @pytest.mark.parametrize(
         "filename",
         [
             "get_server_certificate_sslv2.py",
             "get_server_certificate_sslv23.py",
             "get_server_certificate_sslv3.py",
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/ssl/test_ssl_wrap_socket_tls_version.py` & `precli-0.5.6/tests/unit/rules/java/stdlib/java_net/test_insecure_cookie.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,53 +1,48 @@
-# Copyright 2023 Secure Sauce LLC
+# Copyright 2024 Secure Sauce LLC
 import os
 
 import pytest
 
 from precli.core.level import Level
-from precli.parsers import python
+from precli.parsers import java
 from precli.rules import Rule
 from tests.unit.rules import test_case
 
 
-class TestWrapSocket(test_case.TestCase):
+class TestInsecureCookie(test_case.TestCase):
     @classmethod
     def setup_class(cls):
-        cls.rule_id = "PY018"
-        cls.parser = python.Python()
+        cls.rule_id = "JAV006"
+        cls.parser = java.Java()
         cls.base_path = os.path.join(
             "tests",
             "unit",
             "rules",
-            "python",
+            "java",
             "stdlib",
-            "ssl",
+            "java_net",
             "examples",
         )
 
     def test_rule_meta(self):
         rule = Rule.get_by_id(self.rule_id)
         assert rule.id == self.rule_id
-        assert rule.name == "inadequate_encryption_strength"
+        assert rule.name == "insecure_cookie"
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
-        assert rule.default_config.level == Level.ERROR
+        assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "326"
+        assert rule.cwe.id == 614
 
     @pytest.mark.parametrize(
         "filename",
         [
-            "wrap_socket_sslv2.py",
-            "wrap_socket_sslv23.py",
-            "wrap_socket_sslv2_server_side_true.py",
-            "wrap_socket_sslv3.py",
-            "wrap_socket_tlsv1.py",
-            "wrap_socket_tlsv11.py",
-            "wrap_socket_tlsv12.py",
+            "HttpCookieSecureFalse.java",
+            "HttpCookieSecureTrue.java",
         ],
     )
     def test(self, filename):
         self.check(filename)
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/telnetlib/test_telnetlib_cleartext.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/telnetlib/test_telnetlib_cleartext.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.ERROR
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "319"
+        assert rule.cwe.id == 319
 
     @pytest.mark.parametrize(
         "filename",
         [
             "telnet.py",
             "telnetlib_telnet.py",
             "telnetlib_telnet_context_mgr.py",
```

### Comparing `precli-0.5.5/tests/unit/rules/python/stdlib/tempfile/test_tempfile_mktemp_race_condition.py` & `precli-0.5.6/tests/unit/rules/python/stdlib/tempfile/test_tempfile_mktemp_race_condition.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         assert (
             rule.help_url
             == f"https://docs.securesauce.dev/rules/{self.rule_id}"
         )
         assert rule.default_config.enabled is True
         assert rule.default_config.level == Level.WARNING
         assert rule.default_config.rank == -1.0
-        assert rule.cwe.cwe_id == "377"
+        assert rule.cwe.id == 377
 
     @pytest.mark.parametrize(
         "filename",
         [
             "tempfile_mktemp.py",
             "tempfile_mktemp_args_open.py",
             "tempfile_mktemp_args_with_open_args.py",
```

### Comparing `precli-0.5.5/tests/unit/rules/test_case.py` & `precli-0.5.6/tests/unit/rules/test_case.py`

 * *Files identical despite different names*

### Comparing `precli-0.5.5/tox.ini` & `precli-0.5.6/tox.ini`

 * *Files identical despite different names*

