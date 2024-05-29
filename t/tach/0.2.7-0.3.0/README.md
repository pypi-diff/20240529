# Comparing `tmp/tach-0.2.7.tar.gz` & `tmp/tach-0.3.0.tar.gz`

## Comparing `tach-0.2.7.tar` & `tach-0.3.0.tar`

### file list

```diff
@@ -1,111 +1,184 @@
--rw-r--r--   0        0        0      233 1970-01-01 00:00:00.000000 tach-0.2.7/Cargo.toml
--rw-r--r--   0     1001      127     1641 2024-05-28 22:48:17.000000 tach-0.2.7/.github/workflows/ci.yml
--rw-r--r--   0     1001      127     3459 2024-05-28 22:48:17.000000 tach-0.2.7/.github/workflows/publish.yml
--rw-r--r--   0     1001      127      765 2024-05-28 22:48:17.000000 tach-0.2.7/.github/workflows/publish_docs.yml
--rw-r--r--   0     1001      127     3171 2024-05-28 22:48:17.000000 tach-0.2.7/.gitignore
--rw-r--r--   0     1001      127      132 2024-05-28 22:48:17.000000 tach-0.2.7/.pre-commit-hooks.yaml
--rw-r--r--   0     1001      127    35149 2024-05-28 22:48:17.000000 tach-0.2.7/LICENSE
--rw-r--r--   0     1001      127     4181 2024-05-28 22:48:17.000000 tach-0.2.7/README.md
--rw-r--r--   0     1001      127      162 2024-05-28 22:48:17.000000 tach-0.2.7/dev-requirements.txt
--rw-r--r--   0     1001      127     1294 2024-05-28 22:48:17.000000 tach-0.2.7/docs/configuration.md
--rw-r--r--   0     1001      127     1596 2024-05-28 22:48:17.000000 tach-0.2.7/docs/faq.md
--rw-r--r--   0     1001      127     4286 2024-05-28 22:48:17.000000 tach-0.2.7/docs/favicon.ico
--rw-r--r--   0     1001      127     2421 2024-05-28 22:48:17.000000 tach-0.2.7/docs/getting-started.md
--rw-r--r--   0     1001      127     1396 2024-05-28 22:48:17.000000 tach-0.2.7/docs/index.md
--rw-r--r--   0     1001      127     1562 2024-05-28 22:48:17.000000 tach-0.2.7/docs/strict-mode.md
--rw-r--r--   0     1001      127      573 2024-05-28 22:48:17.000000 tach-0.2.7/docs/tach-ignore.md
--rw-r--r--   0     1001      127     4925 2024-05-28 22:48:17.000000 tach-0.2.7/docs/usage.md
--rw-r--r--   0     1001      127     1677 2024-05-28 22:48:17.000000 tach-0.2.7/docs/why-tach.md
--rw-r--r--   0     1001      127     1477 2024-05-28 22:48:17.000000 tach-0.2.7/mkdocs.yml
--rw-r--r--   0     1001      127        0 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/__init__.py
--rw-r--r--   0     1001      127      101 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/__main__.py
--rw-r--r--   0     1001      127       97 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/cache/__init__.py
--rw-r--r--   0     1001      127      586 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/cache/access.py
--rw-r--r--   0     1001      127       35 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/cache/package.yml
--rw-r--r--   0     1001      127     1089 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/cache/setup.py
--rw-r--r--   0     1001      127     6461 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/check.py
--rw-r--r--   0     1001      127      438 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/clean.py
--rw-r--r--   0     1001      127    13450 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/cli.py
--rw-r--r--   0     1001      127      288 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/colors/__init__.py
--rw-r--r--   0     1001      127       34 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/colors/package.yml
--rw-r--r--   0     1001      127      218 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/constants/__init__.py
--rw-r--r--   0     1001      127       34 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/constants/package.yml
--rw-r--r--   0     1001      127      290 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/core/__init__.py
--rw-r--r--   0     1001      127     4321 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/core/config.py
--rw-r--r--   0     1001      127     3122 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/core/package.py
--rw-r--r--   0     1001      127       33 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/core/package.yml
--rw-r--r--   0     1001      127      209 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/errors/__init__.py
--rw-r--r--   0     1001      127       34 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/errors/package.yml
--rw-r--r--   0     1001      127      957 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/filesystem/__init__.py
--rw-r--r--   0     1001      127      791 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/filesystem/install.py
--rw-r--r--   0     1001      127      441 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/filesystem/package.py
--rw-r--r--   0     1001      127       39 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/filesystem/package.yml
--rw-r--r--   0     1001      127      880 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/filesystem/project.py
--rw-r--r--   0     1001      127     9989 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/filesystem/service.py
--rw-r--r--   0     1001      127      145 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/hooks/__init__.py
--rw-r--r--   0     1001      127       22 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/hooks/package.yml
--rwxr-xr-x   0     1001      127      380 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/hooks/pre_commit.py
--rw-r--r--   0     1001      127      193 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/interactive/__init__.py
--rw-r--r--   0     1001      127       40 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/interactive/package.yml
--rw-r--r--   0     1001      127    19399 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/interactive/packages.py
--rw-r--r--   0     1001      127     1490 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/loading.py
--rw-r--r--   0     1001      127      127 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/logging/__init__.py
--rw-r--r--   0     1001      127     1445 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/logging/api.py
--rw-r--r--   0     1001      127     2502 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/logging/logger.py
--rw-r--r--   0     1001      127       36 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/logging/package.yml
--rw-r--r--   0     1001      127       33 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/package.yml
--rw-r--r--   0     1001      127      512 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/parsing/__init__.py
--rw-r--r--   0     1001      127      461 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/parsing/ast_visitor.py
--rw-r--r--   0     1001      127     2060 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/parsing/config.py
--rw-r--r--   0     1001      127     5330 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/parsing/imports.py
--rw-r--r--   0     1001      127     1861 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/parsing/interface.py
--rw-r--r--   0     1001      127       36 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/parsing/package.yml
--rw-r--r--   0     1001      127      839 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/parsing/packages.py
--rw-r--r--   0     1001      127     4286 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/pkg.py
--rw-r--r--   0     1001      127     4200 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach/sync.py
--rw-r--r--   0     1001      127      708 2024-05-28 22:48:17.000000 tach-0.2.7/python/tach.yml
--rw-r--r--   0     1001      127        0 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/domain_one/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/domain_one/package.yml
--rw-r--r--   0     1001      127       91 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/domain_one/subdomain/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/domain_one/subdomain/package.yml
--rw-r--r--   0     1001      127        0 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/domain_three/__init__.py
--rw-r--r--   0     1001      127       59 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/domain_three/core.py
--rw-r--r--   0     1001      127        0 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/domain_three/package.yml
--rw-r--r--   0     1001      127        0 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/domain_two/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/domain_two/core.py
--rw-r--r--   0     1001      127        0 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/domain_two/package.yml
--rw-r--r--   0     1001      127        0 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/domain_two/subdomain/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/domain_two/subdomain/package.yml
--rw-r--r--   0     1001      127        0 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/invalid/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/invalid/empty/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/invalid/empty/package.yml
--rw-r--r--   0     1001      127        0 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/invalid/empty/tach.yml
--rw-r--r--   0     1001      127       91 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/invalid/hidden/.hidden/__init__.py
--rw-r--r--   0     1001      127       16 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/invalid/hidden/.hidden/package.yml
--rw-r--r--   0     1001      127        0 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/invalid/hidden/__init__.py
--rw-r--r--   0     1001      127      101 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/invalid/hidden/tach.yml
--rw-r--r--   0     1001      127        0 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/invalid/hidden/unhidden/__init__.py
--rw-r--r--   0     1001      127       31 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/invalid/hidden/unhidden/package.yml
--rw-r--r--   0     1001      127       51 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/invalid/hidden/unhidden/secret.py
--rw-r--r--   0     1001      127       26 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/invalid/package.yml
--rw-r--r--   0     1001      127      141 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/invalid/tach.yml
--rw-r--r--   0     1001      127        0 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/valid/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/valid/domain_one/__init__.py
--rw-r--r--   0     1001      127       27 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/valid/domain_one/package.yml
--rw-r--r--   0     1001      127       59 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/valid/domain_three/__init__.py
--rw-r--r--   0     1001      127       15 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/valid/domain_three/package.yml
--rw-r--r--   0     1001      127       80 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/valid/domain_two/__init__.py
--rw-r--r--   0     1001      127       23 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/valid/domain_two/package.yml
--rw-r--r--   0     1001      127      133 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/example/valid/tach.yml
--rw-r--r--   0     1001      127     3694 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/test_check.py
--rw-r--r--   0     1001      127     3340 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/test_cli.py
--rw-r--r--   0     1001      127      934 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/test_init.py
--rw-r--r--   0     1001      127     3513 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/test_package_trie.py
--rw-r--r--   0     1001      127     2404 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/test_parsing.py
--rw-r--r--   0     1001      127        1 2024-05-28 22:48:17.000000 tach-0.2.7/python/tests/test_show.py
--rw-r--r--   0     1001      127      355 2024-05-28 22:48:17.000000 tach-0.2.7/src/lib.rs
--rw-r--r--   0     1001      127     8086 2024-05-28 22:48:17.000000 tach-0.2.7/Cargo.lock
--rw-r--r--   0     1001      127     2270 2024-05-28 22:48:17.000000 tach-0.2.7/pyproject.toml
--rw-r--r--   0        0        0     5691 1970-01-01 00:00:00.000000 tach-0.2.7/PKG-INFO
+-rw-r--r--   0     1001      127      683 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_parser/Cargo.toml
+-rw-r--r--   0     1001      127    12381 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_parser/src/error.rs
+-rw-r--r--   0     1001      127     4363 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_parser/src/lexer/cursor.rs
+-rw-r--r--   0     1001      127     4309 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_parser/src/lexer/fstring.rs
+-rw-r--r--   0     1001      127     4545 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_parser/src/lexer/indentation.rs
+-rw-r--r--   0     1001      127    76323 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_parser/src/lexer.rs
+-rw-r--r--   0     1001      127    18342 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_parser/src/lib.rs
+-rw-r--r--   0     1001      127    91567 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_parser/src/parser/expression.rs
+-rw-r--r--   0     1001      127     1813 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_parser/src/parser/helpers.rs
+-rw-r--r--   0     1001      127    50720 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_parser/src/parser/mod.rs
+-rw-r--r--   0     1001      127    27319 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_parser/src/parser/pattern.rs
+-rw-r--r--   0     1001      127     1454 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_parser/src/parser/progress.rs
+-rw-r--r--   0     1001      127     6700 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_parser/src/parser/recovery.rs
+-rw-r--r--   0     1001      127   128210 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_parser/src/parser/statement.rs
+-rw-r--r--   0     1001      127     2760 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_parser/src/parser/tests.rs
+-rw-r--r--   0     1001      127     9691 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_parser/src/soft_keywords.rs
+-rw-r--r--   0     1001      127    30083 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_parser/src/string.rs
+-rw-r--r--   0     1001      127    35635 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_parser/src/token.rs
+-rw-r--r--   0     1001      127     1241 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_parser/src/token_set.rs
+-rw-r--r--   0     1001      127     2915 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_parser/src/token_source.rs
+-rw-r--r--   0     1001      127     1946 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_parser/src/typing.rs
+-rw-r--r--   0     1001      127      263 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_text_size/Cargo.toml
+-rw-r--r--   0     1001      127     1279 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_text_size/src/lib.rs
+-rw-r--r--   0     1001      127    15167 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_text_size/src/range.rs
+-rw-r--r--   0     1001      127     1193 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_text_size/src/schemars_impls.rs
+-rw-r--r--   0     1001      127     1188 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_text_size/src/serde_impls.rs
+-rw-r--r--   0     1001      127     5003 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_text_size/src/size.rs
+-rw-r--r--   0     1001      127     1421 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_text_size/src/traits.rs
+-rw-r--r--   0     1001      127      302 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_trivia/Cargo.toml
+-rw-r--r--   0     1001      127     7987 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_trivia/src/comment_ranges.rs
+-rw-r--r--   0     1001      127     4142 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_trivia/src/comments.rs
+-rw-r--r--   0     1001      127     3418 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_trivia/src/cursor.rs
+-rw-r--r--   0     1001      127      253 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_trivia/src/lib.rs
+-rw-r--r--   0     1001      127     1393 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_trivia/src/pragmas.rs
+-rw-r--r--   0     1001      127    10839 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_trivia/src/textwrap.rs
+-rw-r--r--   0     1001      127    29058 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_trivia/src/tokenizer.rs
+-rw-r--r--   0     1001      127     2872 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_trivia/src/whitespace.rs
+-rw-r--r--   0     1001      127      620 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_ast/Cargo.toml
+-rw-r--r--   0     1001      127    49228 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_ast/src/comparable.rs
+-rw-r--r--   0     1001      127      811 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_ast/src/docstrings.rs
+-rw-r--r--   0     1001      127    21272 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_ast/src/expression.rs
+-rw-r--r--   0     1001      127      896 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_ast/src/hashable.rs
+-rw-r--r--   0     1001      127    60068 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_ast/src/helpers.rs
+-rw-r--r--   0     1001      127     7552 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_ast/src/identifier.rs
+-rw-r--r--   0     1001      127     3084 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_ast/src/imports.rs
+-rw-r--r--   0     1001      127     6122 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_ast/src/int.rs
+-rw-r--r--   0     1001      127     2529 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_ast/src/lib.rs
+-rw-r--r--   0     1001      127    23813 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_ast/src/name.rs
+-rw-r--r--   0     1001      127   250987 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_ast/src/node.rs
+-rw-r--r--   0     1001      127   129226 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_ast/src/nodes.rs
+-rw-r--r--   0     1001      127     3168 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_ast/src/parenthesize.rs
+-rw-r--r--   0     1001      127     4416 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_ast/src/relocate.rs
+-rw-r--r--   0     1001      127     3219 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_ast/src/statement_visitor.rs
+-rw-r--r--   0     1001      127     1448 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_ast/src/stmt_if.rs
+-rw-r--r--   0     1001      127     6426 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_ast/src/str.rs
+-rw-r--r--   0     1001      127     6653 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_ast/src/str_prefix.rs
+-rw-r--r--   0     1001      127     3022 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_ast/src/traversal.rs
+-rw-r--r--   0     1001      127      105 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_ast/src/types.rs
+-rw-r--r--   0     1001      127    18387 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_ast/src/visitor/preorder.rs
+-rw-r--r--   0     1001      127    24758 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_ast/src/visitor/transformer.rs
+-rw-r--r--   0     1001      127    24667 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_ast/src/visitor.rs
+-rw-r--r--   0     1001      127     1392 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_python_ast/src/whitespace.rs
+-rw-r--r--   0     1001      127      377 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_source_file/Cargo.toml
+-rw-r--r--   0     1001      127     7165 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_source_file/src/lib.rs
+-rw-r--r--   0     1001      127    21158 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_source_file/src/line_index.rs
+-rw-r--r--   0     1001      127    16263 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_source_file/src/locator.rs
+-rw-r--r--   0     1001      127    13286 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/ruff_source_file/src/newlines.rs
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 tach-0.3.0/Cargo.toml
+-rw-r--r--   0     1001      127     1753 2024-05-29 18:25:42.000000 tach-0.3.0/.github/workflows/ci.yml
+-rw-r--r--   0     1001      127     3459 2024-05-29 18:25:42.000000 tach-0.3.0/.github/workflows/publish.yml
+-rw-r--r--   0     1001      127      765 2024-05-29 18:25:42.000000 tach-0.3.0/.github/workflows/publish_docs.yml
+-rw-r--r--   0     1001      127     3171 2024-05-29 18:25:42.000000 tach-0.3.0/.gitignore
+-rw-r--r--   0     1001      127      132 2024-05-29 18:25:42.000000 tach-0.3.0/.pre-commit-hooks.yaml
+-rw-r--r--   0     1001      127    35149 2024-05-29 18:25:42.000000 tach-0.3.0/LICENSE
+-rw-r--r--   0     1001      127     1667 2024-05-29 18:25:42.000000 tach-0.3.0/Makefile
+-rw-r--r--   0     1001      127     4181 2024-05-29 18:25:42.000000 tach-0.3.0/README.md
+-rw-r--r--   0     1001      127      529 2024-05-29 18:25:42.000000 tach-0.3.0/benches/get_project_imports.rs
+-rw-r--r--   0     1001      127    68613 2024-05-29 18:25:42.000000 tach-0.3.0/crates/vendored/LICENSE
+-rw-r--r--   0     1001      127      173 2024-05-29 18:25:42.000000 tach-0.3.0/dev-requirements.txt
+-rw-r--r--   0     1001      127     1294 2024-05-29 18:25:42.000000 tach-0.3.0/docs/configuration.md
+-rw-r--r--   0     1001      127     1596 2024-05-29 18:25:42.000000 tach-0.3.0/docs/faq.md
+-rw-r--r--   0     1001      127     4286 2024-05-29 18:25:42.000000 tach-0.3.0/docs/favicon.ico
+-rw-r--r--   0     1001      127     2421 2024-05-29 18:25:42.000000 tach-0.3.0/docs/getting-started.md
+-rw-r--r--   0     1001      127     1396 2024-05-29 18:25:42.000000 tach-0.3.0/docs/index.md
+-rw-r--r--   0     1001      127     1562 2024-05-29 18:25:42.000000 tach-0.3.0/docs/strict-mode.md
+-rw-r--r--   0     1001      127      573 2024-05-29 18:25:42.000000 tach-0.3.0/docs/tach-ignore.md
+-rw-r--r--   0     1001      127     4925 2024-05-29 18:25:42.000000 tach-0.3.0/docs/usage.md
+-rw-r--r--   0     1001      127     1677 2024-05-29 18:25:42.000000 tach-0.3.0/docs/why-tach.md
+-rw-r--r--   0     1001      127     1477 2024-05-29 18:25:42.000000 tach-0.3.0/mkdocs.yml
+-rw-r--r--   0     1001      127        0 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/__init__.py
+-rw-r--r--   0     1001      127      101 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/__main__.py
+-rw-r--r--   0     1001      127       97 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/cache/__init__.py
+-rw-r--r--   0     1001      127      555 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/cache/access.py
+-rw-r--r--   0     1001      127       35 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/cache/package.yml
+-rw-r--r--   0     1001      127     1058 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/cache/setup.py
+-rw-r--r--   0     1001      127     6447 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/check.py
+-rw-r--r--   0     1001      127      438 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/clean.py
+-rw-r--r--   0     1001      127    13423 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/cli.py
+-rw-r--r--   0     1001      127      288 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/colors/__init__.py
+-rw-r--r--   0     1001      127       34 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/colors/package.yml
+-rw-r--r--   0     1001      127      218 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/constants/__init__.py
+-rw-r--r--   0     1001      127       34 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/constants/package.yml
+-rw-r--r--   0     1001      127      290 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/core/__init__.py
+-rw-r--r--   0     1001      127     4298 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/core/config.py
+-rw-r--r--   0     1001      127     3099 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/core/package.py
+-rw-r--r--   0     1001      127       33 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/core/package.yml
+-rw-r--r--   0     1001      127      209 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/errors/__init__.py
+-rw-r--r--   0     1001      127       34 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/errors/package.yml
+-rw-r--r--   0     1001      127      131 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/extension.pyi
+-rw-r--r--   0     1001      127      957 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/filesystem/__init__.py
+-rw-r--r--   0     1001      127      791 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/filesystem/install.py
+-rw-r--r--   0     1001      127      410 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/filesystem/package.py
+-rw-r--r--   0     1001      127       39 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/filesystem/package.yml
+-rw-r--r--   0     1001      127      849 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/filesystem/project.py
+-rw-r--r--   0     1001      127     9931 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/filesystem/service.py
+-rw-r--r--   0     1001      127      145 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/hooks/__init__.py
+-rw-r--r--   0     1001      127       22 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/hooks/package.yml
+-rwxr-xr-x   0     1001      127      380 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/hooks/pre_commit.py
+-rw-r--r--   0     1001      127      193 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/interactive/__init__.py
+-rw-r--r--   0     1001      127       40 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/interactive/package.yml
+-rw-r--r--   0     1001      127    19313 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/interactive/packages.py
+-rw-r--r--   0     1001      127     1490 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/loading.py
+-rw-r--r--   0     1001      127      127 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/logging/__init__.py
+-rw-r--r--   0     1001      127     1445 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/logging/api.py
+-rw-r--r--   0     1001      127     2486 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/logging/logger.py
+-rw-r--r--   0     1001      127       36 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/logging/package.yml
+-rw-r--r--   0     1001      127       33 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/package.yml
+-rw-r--r--   0     1001      127      432 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/parsing/__init__.py
+-rw-r--r--   0     1001      127      461 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/parsing/ast_visitor.py
+-rw-r--r--   0     1001      127     2015 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/parsing/config.py
+-rw-r--r--   0     1001      127     1861 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/parsing/interface.py
+-rw-r--r--   0     1001      127       36 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/parsing/package.yml
+-rw-r--r--   0     1001      127      807 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/parsing/packages.py
+-rw-r--r--   0     1001      127     4249 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/pkg.py
+-rw-r--r--   0     1001      127     4151 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach/sync.py
+-rw-r--r--   0     1001      127      708 2024-05-29 18:25:42.000000 tach-0.3.0/python/tach.yml
+-rw-r--r--   0     1001      127        0 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/domain_one/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/domain_one/package.yml
+-rw-r--r--   0     1001      127       91 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/domain_one/subdomain/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/domain_one/subdomain/package.yml
+-rw-r--r--   0     1001      127        0 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/domain_three/__init__.py
+-rw-r--r--   0     1001      127       59 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/domain_three/core.py
+-rw-r--r--   0     1001      127        0 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/domain_three/package.yml
+-rw-r--r--   0     1001      127        0 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/domain_two/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/domain_two/core.py
+-rw-r--r--   0     1001      127        0 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/domain_two/package.yml
+-rw-r--r--   0     1001      127        0 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/domain_two/subdomain/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/domain_two/subdomain/package.yml
+-rw-r--r--   0     1001      127        0 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/invalid/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/invalid/empty/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/invalid/empty/package.yml
+-rw-r--r--   0     1001      127        0 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/invalid/empty/tach.yml
+-rw-r--r--   0     1001      127       91 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/invalid/hidden/.hidden/__init__.py
+-rw-r--r--   0     1001      127       16 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/invalid/hidden/.hidden/package.yml
+-rw-r--r--   0     1001      127        0 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/invalid/hidden/__init__.py
+-rw-r--r--   0     1001      127      101 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/invalid/hidden/tach.yml
+-rw-r--r--   0     1001      127        0 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/invalid/hidden/unhidden/__init__.py
+-rw-r--r--   0     1001      127       31 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/invalid/hidden/unhidden/package.yml
+-rw-r--r--   0     1001      127       51 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/invalid/hidden/unhidden/secret.py
+-rw-r--r--   0     1001      127       26 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/invalid/package.yml
+-rw-r--r--   0     1001      127      141 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/invalid/tach.yml
+-rw-r--r--   0     1001      127        0 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/valid/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/valid/domain_one/__init__.py
+-rw-r--r--   0     1001      127       27 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/valid/domain_one/package.yml
+-rw-r--r--   0     1001      127       59 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/valid/domain_three/__init__.py
+-rw-r--r--   0     1001      127       15 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/valid/domain_three/package.yml
+-rw-r--r--   0     1001      127       80 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/valid/domain_two/__init__.py
+-rw-r--r--   0     1001      127       23 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/valid/domain_two/package.yml
+-rw-r--r--   0     1001      127      133 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/example/valid/tach.yml
+-rw-r--r--   0     1001      127     3694 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/test_check.py
+-rw-r--r--   0     1001      127     3340 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/test_cli.py
+-rw-r--r--   0     1001      127     3961 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/test_imports.py
+-rw-r--r--   0     1001      127      934 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/test_init.py
+-rw-r--r--   0     1001      127     3505 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/test_package_trie.py
+-rw-r--r--   0     1001      127     2404 2024-05-29 18:25:42.000000 tach-0.3.0/python/tests/test_parsing.py
+-rw-r--r--   0     1001      127     2563 2024-05-29 18:25:42.000000 tach-0.3.0/src/filesystem.rs
+-rw-r--r--   0     1001      127    11025 2024-05-29 18:25:42.000000 tach-0.3.0/src/imports.rs
+-rw-r--r--   0     1001      127      833 2024-05-29 18:25:42.000000 tach-0.3.0/src/lib.rs
+-rw-r--r--   0     1001      127      196 2024-05-29 18:25:42.000000 tach-0.3.0/src/parsing.rs
+-rw-r--r--   0     1001      127    37722 2024-05-29 18:25:42.000000 tach-0.3.0/Cargo.lock
+-rw-r--r--   0     1001      127     2297 2024-05-29 18:25:42.000000 tach-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5691 1970-01-01 00:00:00.000000 tach-0.3.0/PKG-INFO
```

### Comparing `tach-0.2.7/.github/workflows/ci.yml` & `tach-0.3.0/.github/workflows/ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -26,16 +26,20 @@
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         python -m pip install uv
         uv venv
         source .venv/bin/activate
+        uv pip install pip
         uv pip install -r dev-requirements.txt
-        uv pip install -e .
+    - name: Build and install tach
+      uses: PyO3/maturin-action@v1
+      with:
+        command: develop
     - name: Check ruff
       run: |
         source .venv/bin/activate
         cd python
         ruff check
         ruff format --check
     - name: Test with pytest and report coverage
@@ -52,10 +56,10 @@
     - name: Check tach
       run: |
         source .venv/bin/activate
         tach check --root python
     - name: Check Rust linting
       run: cargo clippy
     - name: Check Rust formatting
-      run: cargo fmt --check
+      run: cargo fmt --all --check
     - name: Check Rust
       run: cargo check
```

### Comparing `tach-0.2.7/.github/workflows/publish.yml` & `tach-0.3.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `tach-0.2.7/.github/workflows/publish_docs.yml` & `tach-0.3.0/.github/workflows/publish_docs.yml`

 * *Files identical despite different names*

### Comparing `tach-0.2.7/.gitignore` & `tach-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `tach-0.2.7/LICENSE` & `tach-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tach-0.2.7/README.md` & `tach-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.7/docs/configuration.md` & `tach-0.3.0/docs/configuration.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.7/docs/faq.md` & `tach-0.3.0/docs/faq.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.7/docs/favicon.ico` & `tach-0.3.0/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `tach-0.2.7/docs/getting-started.md` & `tach-0.3.0/docs/getting-started.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.7/docs/index.md` & `tach-0.3.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.7/docs/strict-mode.md` & `tach-0.3.0/docs/strict-mode.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.7/docs/tach-ignore.md` & `tach-0.3.0/docs/tach-ignore.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.7/docs/usage.md` & `tach-0.3.0/docs/usage.md`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 
 ### With pre-commit framework
 If you use the [pre-commit framework](https://github.com/pre-commit/pre-commit), you can add the following to your `.pre-commit-hooks.yaml`:
 
 ```yaml
 repos:
 -   repo: https://github.com/gauge-sh/tach
-    rev: v0.2.4  # change this to the latest tag!
+    rev: v0.3.0  # change this to the latest tag!
     hooks:
     -   id: tach
         # args: ["--root=backend_root"]
 ```
 
 Note that you should specify the version you are using in the `rev` key.
```

### Comparing `tach-0.2.7/docs/why-tach.md` & `tach-0.3.0/docs/why-tach.md`

 * *Files identical despite different names*

### Comparing `tach-0.2.7/mkdocs.yml` & `tach-0.3.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `tach-0.2.7/python/tach/cache/access.py` & `tach-0.3.0/python/tach/cache/access.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from __future__ import annotations
 
 import uuid
 from pathlib import Path
-from typing import Optional
 
 from tach.cache.setup import resolve_dot_tach
 from tach.filesystem import find_project_config_root
 
 
-def get_uid() -> Optional[uuid.UUID]:
+def get_uid() -> uuid.UUID | None:
     project_root = find_project_config_root(str(Path.cwd()))
     if project_root is None:
         return
     project_path = Path(project_root)
     if not (project_path / ".tach" / "tach.info").exists():
         resolve_dot_tach()
     with open(project_path / ".tach" / "tach.info") as f:
```

### Comparing `tach-0.2.7/python/tach/cache/setup.py` & `tach-0.3.0/python/tach/cache/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import annotations
 
 import uuid
 from pathlib import Path
-from typing import Optional
 
 from tach.filesystem import find_project_config_root
 
 
-def resolve_dot_tach() -> Optional[Path]:
+def resolve_dot_tach() -> Path | None:
     project_dir = find_project_config_root(str(Path.cwd()))
     if project_dir is None:
         return
     project_path = Path(project_dir)
 
     def _create(path: Path, is_file: bool = False, file_content: str = "") -> None:
         if not path.exists():
```

### Comparing `tach-0.2.7/python/tach/check.py` & `tach-0.3.0/python/tach/check.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
 
 import os
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING
 
 from tach import errors
 from tach import filesystem as fs
-from tach.parsing import build_package_trie, get_project_imports
+from tach.extension import get_project_imports
+from tach.parsing import build_package_trie
 
 if TYPE_CHECKING:
     from tach.core import PackageNode, PackageTrie, ProjectConfig
 
 
 @dataclass
 class ErrorInfo:
@@ -41,16 +42,16 @@
 
 
 def check_import(
     project_config: ProjectConfig,
     package_trie: PackageTrie,
     import_mod_path: str,
     file_mod_path: str,
-    file_nearest_package: Optional[PackageNode] = None,
-) -> Optional[ErrorInfo]:
+    file_nearest_package: PackageNode | None = None,
+) -> ErrorInfo | None:
     import_nearest_package = package_trie.find_nearest(import_mod_path)
     if import_nearest_package is None:
         # This shouldn't happen since we intend to filter out any external imports,
         # but we should allow external imports if they have made it here.
         return None
 
     # Lookup file_mod_path if package not given
@@ -118,15 +119,15 @@
     import_mod_path: str
     error_info: ErrorInfo
 
 
 def check(
     root: str,
     project_config: ProjectConfig,
-    exclude_paths: Optional[list[str]] = None,
+    exclude_paths: list[str] | None = None,
 ) -> list[BoundaryError]:
     if not os.path.isdir(root):
         raise errors.TachSetupError(f"The path {root} is not a valid directory.")
 
     cwd = fs.get_cwd()
     try:
         fs.chdir(root)
@@ -158,26 +159,26 @@
                 file_path,
                 ignore_type_checking_imports=project_config.ignore_type_checking_imports,
             )
             for project_import in project_imports:
                 check_error = check_import(
                     project_config=project_config,
                     package_trie=package_trie,
-                    import_mod_path=project_import.mod_path,
+                    import_mod_path=project_import[0],
                     file_nearest_package=nearest_package,
                     file_mod_path=mod_path,
                 )
                 if check_error is None:
                     continue
 
                 boundary_errors.append(
                     BoundaryError(
                         file_path=file_path,
-                        import_mod_path=project_import.mod_path,
-                        line_number=project_import.line_number,
+                        import_mod_path=project_import[0],
+                        line_number=project_import[1],
                         error_info=check_error,
                     )
                 )
 
         return boundary_errors
     finally:
         fs.chdir(cwd)
```

### Comparing `tach-0.2.7/python/tach/cli.py` & `tach-0.3.0/python/tach/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import argparse
 import os
 import sys
 from enum import Enum
 from functools import lru_cache
 from pathlib import Path
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING
 
 from tach import filesystem as fs
 from tach.check import BoundaryError, check
 from tach.clean import clean_project
 from tach.colors import BCOLORS
 from tach.constants import CONFIG_FILE_NAME, TOOL_NAME
 from tach.filesystem import install_pre_commit
@@ -26,24 +26,24 @@
 
 class TerminalEnvironment(Enum):
     UNKNOWN = 1
     JETBRAINS = 2
     VSCODE = 3
 
 
-@lru_cache()
+@lru_cache
 def detect_environment() -> TerminalEnvironment:
     if "jetbrains" in os.environ.get("TERMINAL_EMULATOR", "").lower():
         return TerminalEnvironment.JETBRAINS
     elif "vscode" in os.environ.get("TERM_PROGRAM", "").lower():
         return TerminalEnvironment.VSCODE
     return TerminalEnvironment.UNKNOWN
 
 
-def create_clickable_link(file_path: str, line: Optional[int] = None) -> str:
+def create_clickable_link(file_path: str, line: int | None = None) -> str:
     terminal_env = detect_environment()
     abs_path = os.path.abspath(file_path)
 
     if terminal_env == TerminalEnvironment.JETBRAINS:
         link = f"file://{abs_path}:{line}" if line is not None else f"file://{abs_path}"
     elif terminal_env == TerminalEnvironment.VSCODE:
         link = (
@@ -219,15 +219,15 @@
     parsed_args = parser.parse_args(args)
     return parsed_args, parser
 
 
 def tach_check(
     root: str = ".",
     exact: bool = False,
-    exclude_paths: Optional[list[str]] = None,
+    exclude_paths: list[str] | None = None,
 ):
     logger.info(
         "tach check called",
         extra={
             "data": LogDataModel(
                 function="tach_check",
                 parameters={"exact": exact},
@@ -274,15 +274,15 @@
     if boundary_errors:
         print_errors(boundary_errors)
         sys.exit(1)
     print(f"✅ {BCOLORS.OKGREEN}All package dependencies validated!{BCOLORS.ENDC}")
     sys.exit(0)
 
 
-def tach_pkg(depth: Optional[int] = 1, exclude_paths: Optional[list[str]] = None):
+def tach_pkg(depth: int | None = 1, exclude_paths: list[str] | None = None):
     logger.info(
         "tach pkg called",
         extra={
             "data": LogDataModel(
                 function="tach_pkg",
                 parameters={"depth": depth},
             ),
@@ -302,15 +302,15 @@
         print(
             f"✅ {BCOLORS.OKGREEN}Set packages! You may want to run '{TOOL_NAME} sync' "
             f"to automatically set boundaries.{BCOLORS.ENDC}"
         )
     sys.exit(0)
 
 
-def tach_sync(prune: bool = False, exclude_paths: Optional[list[str]] = None):
+def tach_sync(prune: bool = False, exclude_paths: list[str] | None = None):
     logger.info(
         "tach sync called",
         extra={
             "data": LogDataModel(
                 function="tach_sync",
                 parameters={"prune": prune},
             ),
```

### Comparing `tach-0.2.7/python/tach/core/config.py` & `tach-0.3.0/python/tach/core/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 from __future__ import annotations
 
-from typing import Any, List, Optional
+from typing import Any
 
 from pydantic import BaseModel, Field
 
 
 class Config(BaseModel):
     model_config = {"extra": "forbid"}
 
 
 class PackageConfig(Config):
     """
     Configuration for a single package within a project.
     """
 
-    tags: List[str]
+    tags: list[str]
     strict: bool = False
 
 
 class TagDependencyRules(Config):
     """
     Dependency rules for a particular set of tags (typically one tag).
     """
 
     tag: str
-    depends_on: List[str]
+    depends_on: list[str]
 
 
 def is_deprecated_project_config(config: dict[str, Any]) -> bool:
     if not config:
         return False
     if "exclude_hidden_paths" in config:
         return True
@@ -52,16 +52,16 @@
 
 
 class ProjectConfig(Config):
     """
     Configuration applied globally to a project.
     """
 
-    constraints: List[TagDependencyRules] = Field(default_factory=list)
-    exclude: Optional[List[str]] = Field(default_factory=lambda: ["tests", "docs"])
+    constraints: list[TagDependencyRules] = Field(default_factory=list)
+    exclude: list[str] | None = Field(default_factory=lambda: ["tests", "docs"])
     exact: bool = False
     disable_logging: bool = False
     ignore_type_checking_imports: bool = False
 
     def dependencies_for_tag(self, tag: str) -> list[str]:
         return next(
             (
@@ -91,15 +91,15 @@
                 # Constraints already exist, set the union of existing and new as dependencies
                 new_dependencies = set(current_dependency_rules.depends_on) | set(
                     dependencies
                 )
                 current_dependency_rules.depends_on = list(new_dependencies)
 
     def find_extra_constraints(
-        self, other_config: "ProjectConfig"
+        self, other_config: ProjectConfig
     ) -> list[TagDependencyRules]:
         extra_constraints: list[TagDependencyRules] = []
         base_constraint_tags = set(constraint.tag for constraint in self.constraints)
         for constraint in other_config.constraints:
             if constraint.tag not in base_constraint_tags:
                 extra_constraints.append(constraint)
                 continue
@@ -117,15 +117,15 @@
                         depends_on=list(extra_dependencies),
                     )
                 )
 
         return extra_constraints
 
     @classmethod
-    def factory(cls, config: dict[str, Any]) -> tuple[bool, "ProjectConfig"]:
+    def factory(cls, config: dict[str, Any]) -> tuple[bool, ProjectConfig]:
         """
         Using this factory to catch deprecated config and flag it to the caller
         """
         if is_deprecated_project_config(config):
             fix_deprecated_config(config)
             return True, ProjectConfig(**config)
         return False, ProjectConfig(**config)  # type: ignore
```

### Comparing `tach-0.2.7/python/tach/core/package.py` & `tach-0.3.0/python/tach/core/package.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 from collections import deque
 from dataclasses import dataclass, field
-from typing import Generator, Optional
+from typing import Generator
 
 from tach.core.config import PackageConfig
 
 
 @dataclass
 class PackageNode:
     """
@@ -17,20 +17,20 @@
 
     If 'is_end_of_path' is False, this node does not represent a real package,
     and must have 'config' None and 'full_path' as the empty string.
     """
 
     is_end_of_path: bool
     full_path: str
-    config: Optional[PackageConfig]
+    config: PackageConfig | None
     interface_members: list[str] = field(default_factory=list)
-    children: dict[str, "PackageNode"] = field(default_factory=dict)
+    children: dict[str, PackageNode] = field(default_factory=dict)
 
     @classmethod
-    def empty(cls) -> "PackageNode":
+    def empty(cls) -> PackageNode:
         return PackageNode(is_end_of_path=False, full_path="", config=None)
 
     def fill(
         self, config: PackageConfig, full_path: str, interface_members: list[str]
     ) -> None:
         self.is_end_of_path = True
         self.config = config
@@ -52,15 +52,15 @@
 
     @staticmethod
     def _split_mod_path(path: str) -> list[str]:
         # By default "".split(".") -> ['']
         # so we want to remove any whitespace path components
         return [part for part in path.split(".") if part]
 
-    def get(self, path: str) -> Optional[PackageNode]:
+    def get(self, path: str) -> PackageNode | None:
         node = self.root
         parts = self._split_mod_path(path)
 
         for part in parts:
             if part not in node.children:
                 return None
             node = node.children[part]
@@ -74,15 +74,15 @@
         for part in parts:
             if part not in node.children:
                 node.children[part] = PackageNode.empty()
             node = node.children[part]
 
         node.fill(config, path, interface_members)
 
-    def find_nearest(self, path: str) -> Optional[PackageNode]:
+    def find_nearest(self, path: str) -> PackageNode | None:
         node = self.root
         parts = self._split_mod_path(path)
         nearest_parent = node
 
         for part in parts:
             if part in node.children:
                 node = node.children[part]
```

### Comparing `tach-0.2.7/python/tach/filesystem/__init__.py` & `tach-0.3.0/python/tach/filesystem/__init__.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.7/python/tach/filesystem/install.py` & `tach-0.3.0/python/tach/filesystem/install.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.7/python/tach/filesystem/project.py` & `tach-0.3.0/python/tach/filesystem/project.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import os
 from pathlib import Path
-from typing import Optional
 
 from tach.constants import CONFIG_FILE_NAME
 
 
 # TODO convert all str paths to pathlib.Path
 def get_project_config_path(root: str = ".") -> str:
     file_path = os.path.join(root, f"{CONFIG_FILE_NAME}.yml")
@@ -14,15 +13,15 @@
         return file_path
     file_path = os.path.join(root, f"{CONFIG_FILE_NAME}.yaml")
     if os.path.exists(file_path):
         return file_path
     return ""
 
 
-def find_project_config_root(path: str) -> Optional[str]:
+def find_project_config_root(path: str) -> str | None:
     path = os.path.abspath(path)
     if os.path.isdir(path):
         if get_project_config_path(path):
             return path
     path_obj = Path(path)
     # Iterate upwards, looking for project config
     for parent in path_obj.parents:
```

### Comparing `tach-0.2.7/python/tach/filesystem/service.py` & `tach-0.3.0/python/tach/filesystem/service.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 import stat
 import sys
 import threading
 from collections import defaultdict
 from dataclasses import dataclass
 from functools import lru_cache
 from pathlib import Path
-from typing import Generator, Optional
+from typing import Generator
 
 from tach import errors
 from tach.colors import BCOLORS
 
 
 @dataclass
 class FileInfo:
     path: str
-    content: Optional[str] = None
-    canonical_path: Optional[str] = None
-    ast: Optional["ast.AST"] = None
+    content: str | None = None
+    canonical_path: str | None = None
+    ast: ast.AST | None = None
 
 
 # Thread-local file cache to avoid going to disk as much as possible
 thread_local = threading.local()
 # Cannot type-hint non-self attributes (https://github.com/python/mypy/issues/2388)
 # cwd: str
 thread_local.cwd = os.getcwd()
@@ -55,15 +55,15 @@
     return file_caches_by_cwd[get_cwd()]
 
 
 def _file_cache_key(path: str) -> str:
     return f"{get_cwd()}:::{path}"
 
 
-def _cached_file(path: str) -> Optional[FileInfo]:
+def _cached_file(path: str) -> FileInfo | None:
     return _get_file_cache().get(_file_cache_key(path))
 
 
 def _set_cached_file(path: str, file_info: FileInfo):
     _get_file_cache()[_file_cache_key(path)] = file_info
 
 
@@ -87,15 +87,15 @@
 
 
 def read_file(path: str) -> str:
     cached_file = _cached_file(path)
     if cached_file and cached_file.content:
         return cached_file.content
 
-    with open(path, "r") as f:
+    with open(path) as f:
         content = f.read()
 
     if cached_file:
         cached_file.content = content
     else:
         _set_cached_file(path, FileInfo(path=path, content=content))
 
@@ -136,15 +136,15 @@
     if cached_file and cached_file.content:
         content = cached_file.content
         try:
             ast_result = ast.parse(cached_file.content)
         except SyntaxError as e:
             raise errors.TachParseError(f"Syntax error in {path}: {e}")
     else:
-        with open(path, "r") as f:
+        with open(path) as f:
             content = f.read()
         try:
             ast_result = ast.parse(content)
         except SyntaxError as e:
             raise errors.TachParseError(f"Syntax error in {path}: {e}")
 
     if cached_file:
@@ -154,17 +154,17 @@
         _set_cached_file(path, FileInfo(path=path, content=content, ast=ast_result))
 
     return ast_result
 
 
 def walk(
     root: str,
-    depth: Optional[int] = None,
+    depth: int | None = None,
     exclude_root: bool = True,
-    exclude_paths: Optional[list[str]] = None,
+    exclude_paths: list[str] | None = None,
 ) -> Generator[tuple[str, list[str]], None, None]:
     canonical_root = canonical(root)
     base_depth = 0 if canonical_root == "." else canonical_root.count(os.path.sep) + 1
     for dirpath, dirnames, filenames in os.walk(canonical_root):
         dirpath = canonical(dirpath)
         dirpath_for_matching = f"{dirpath}/"
 
@@ -200,46 +200,46 @@
             return True
 
         yield dirpath, list(filter(filter_filename, filenames))
 
 
 def walk_pyfiles(
     root: str,
-    depth: Optional[int] = None,
-    exclude_paths: Optional[list[str]] = None,
+    depth: int | None = None,
+    exclude_paths: list[str] | None = None,
 ) -> Generator[str, None, None]:
     for dirpath, filenames in walk(
         root,
         depth=depth,
         exclude_paths=exclude_paths,
     ):
         for filename in filenames:
             if filename.endswith(".py"):
                 yield os.path.join(dirpath, filename)
 
 
 def walk_pypackages(
     root: str,
-    depth: Optional[int] = None,
-    exclude_paths: Optional[list[str]] = None,
+    depth: int | None = None,
+    exclude_paths: list[str] | None = None,
 ) -> Generator[str, None, None]:
     for filepath in walk_pyfiles(
         root,
         depth=depth,
         exclude_paths=exclude_paths,
     ):
         init_file_ending = f"{os.path.sep}__init__.py"
         if filepath.endswith(init_file_ending):
             yield filepath[: -len(init_file_ending)]
 
 
 def walk_configured_packages(
     root: str,
-    depth: Optional[int] = None,
-    exclude_paths: Optional[list[str]] = None,
+    depth: int | None = None,
+    exclude_paths: list[str] | None = None,
 ) -> Generator[tuple[str, str], None, None]:
     for dirpath in walk_pypackages(
         root,
         depth=depth,
         exclude_paths=exclude_paths,
     ):
         package_yml_path = os.path.join(dirpath, "package.yml")
```

### Comparing `tach-0.2.7/python/tach/interactive/packages.py` & `tach-0.3.0/python/tach/interactive/packages.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import os
 import re
 from collections import deque
 from dataclasses import dataclass, field
 from enum import Enum
 from itertools import chain
-from typing import TYPE_CHECKING, Callable, Generator, Optional, Union
+from typing import TYPE_CHECKING, Callable, Generator
 
 from prompt_toolkit import ANSI
 from prompt_toolkit.application import Application
 from prompt_toolkit.data_structures import Point
 from prompt_toolkit.key_binding import KeyBindings, KeyPressEvent
 from prompt_toolkit.layout import (
     Container,
@@ -48,70 +48,70 @@
 
 @dataclass
 class FileNode:
     full_path: str
     is_dir: bool
     expanded: bool = False
     is_package: bool = False
-    parent: Optional["FileNode"] = None
-    children: list["FileNode"] = field(default_factory=list)
+    parent: FileNode | None = None
+    children: list[FileNode] = field(default_factory=list)
 
     @property
     def empty(self) -> bool:
         return len(self.children) == 0
 
     @property
-    def visible_children(self) -> list["FileNode"]:
+    def visible_children(self) -> list[FileNode]:
         if not self.expanded:
             return []
         return self.children
 
     @classmethod
-    def build_from_path(cls, path: str) -> "FileNode":
+    def build_from_path(cls, path: str) -> FileNode:
         is_dir = os.path.isdir(path)
         is_package = os.path.isfile(os.path.join(path, f"{PACKAGE_FILE_NAME}.yml"))
         return cls(full_path=path, is_dir=is_dir, is_package=is_package)
 
     @property
-    def parent_sorted_children(self) -> Optional[list["FileNode"]]:
+    def parent_sorted_children(self) -> list[FileNode] | None:
         if not self.parent:
             return None
         return sorted(self.parent.visible_children, key=lambda node: node.full_path)
 
     @property
-    def prev_sibling(self) -> Optional["FileNode"]:
+    def prev_sibling(self) -> FileNode | None:
         parent_sorted_children = self.parent_sorted_children
         if not parent_sorted_children:
             return None
 
         try:
             my_index = parent_sorted_children.index(self)
         except ValueError:
             raise errors.TachError("Error occurred in interactive file tree navigation")
 
         if my_index == 0:
             return None
         return parent_sorted_children[my_index - 1]
 
     @property
-    def next_sibling(self) -> Optional["FileNode"]:
+    def next_sibling(self) -> FileNode | None:
         parent_sorted_children = self.parent_sorted_children
         if not parent_sorted_children:
             return None
 
         try:
             my_index = parent_sorted_children.index(self)
         except ValueError:
             raise errors.TachError("Error occurred in interactive file tree navigation")
 
         if my_index == len(parent_sorted_children) - 1:
             return None
         return parent_sorted_children[my_index + 1]
 
-    def siblings(self, include_self: bool = True) -> list["FileNode"]:
+    def siblings(self, include_self: bool = True) -> list[FileNode]:
         if not self.parent:
             return [self] if include_self else []
 
         return (
             self.parent.children
             if include_self
             else [node for node in self.parent.children if node is not self]
@@ -123,18 +123,18 @@
     root: FileNode
     nodes: dict[str, FileNode] = field(default_factory=dict)
 
     @classmethod
     def build_from_path(
         cls,
         path: str,
-        depth: Optional[int] = 1,
-        exclude_paths: Optional[list[str]] = None,
+        depth: int | None = 1,
+        exclude_paths: list[str] | None = None,
         auto_select_initial_packages: bool = False,
-    ) -> "FileTree":
+    ) -> FileTree:
         root = FileNode.build_from_path(fs.canonical(path))
         root.expanded = True
         tree = cls(root)
         tree.nodes[fs.canonical(path)] = root
         tree._build_subtree(
             root, depth=depth if depth is not None else 1, exclude_paths=exclude_paths
         )
@@ -144,15 +144,15 @@
 
         return tree
 
     def _build_subtree(
         self,
         root: FileNode,
         depth: int = 1,
-        exclude_paths: Optional[list[str]] = None,
+        exclude_paths: list[str] | None = None,
     ):
         if root.is_dir:
             try:
                 for entry in os.listdir(root.full_path):
                     if entry.startswith("."):
                         # Ignore hidden files and directories
                         continue
@@ -183,15 +183,15 @@
                         )
             except PermissionError:
                 # This is expected to occur during listdir when the directory cannot be accessed
                 # We simply bail if that happens, meaning it won't show up in the interactive viewer
                 return
 
     def mark_pypackages_as_packages(
-        self, depth: Optional[int], exclude_paths: Optional[list[str]] = None
+        self, depth: int | None, exclude_paths: list[str] | None = None
     ):
         packages_found: list[str] = []
         for package_path in fs.walk_pypackages(
             self.root.full_path,
             depth=depth if depth is not None else 1,
             exclude_paths=exclude_paths,
         ):
@@ -247,16 +247,16 @@
 class InteractivePackageTree:
     TREE_LABEL = "Confirm Your Packages"
     AUTO_EXCLUDE_PATHS = [".*__pycache__"]
 
     def __init__(
         self,
         path: str,
-        depth: Optional[int] = 1,
-        exclude_paths: Optional[list[str]] = None,
+        depth: int | None = 1,
+        exclude_paths: list[str] | None = None,
         auto_select_initial_packages: bool = False,
     ):
         # By default, don't save if we exit for any reason
         self.exit_code: ExitCode = ExitCode.QUIT_NOSAVE
         if exclude_paths is None:
             exclude_paths = self.AUTO_EXCLUDE_PATHS
         else:
@@ -475,15 +475,15 @@
                 self.move_cursor_up()
                 self.selected_node = self.selected_node.prev_sibling
             self.move_cursor_up()
             self.selected_node = self.selected_node.parent
             self._update_display()
 
     def _render_node(self, node: FileNode) -> Text:
-        text_parts: list[Union[tuple[str, str], str]] = []
+        text_parts: list[tuple[str, str] | str] = []
         if node == self.selected_node:
             text_parts.append(("-> ", "bold cyan"))
 
         basename = os.path.basename(node.full_path)
         if node.is_package:
             text_parts.append((f"[Package] {basename}", "bold yellow"))
         elif node == self.selected_node:
@@ -522,30 +522,30 @@
         with self.console.capture() as capture:
             self.console.print(tree_root)
         return capture.get()
 
     def _update_display(self):
         self.tree_control.text = ANSI(self._render_tree())
 
-    def run(self) -> Optional[list[SelectedPackage]]:
+    def run(self) -> list[SelectedPackage] | None:
         self.app.run()
         if self.exit_code == ExitCode.QUIT_SAVE:
             return [
                 SelectedPackage(full_path=node.full_path)
                 for node in self.file_tree
                 if node.is_package
             ]
 
 
 def get_selected_packages_interactive(
     path: str,
-    depth: Optional[int] = 1,
-    exclude_paths: Optional[list[str]] = None,
+    depth: int | None = 1,
+    exclude_paths: list[str] | None = None,
     auto_select_initial_packages: bool = False,
-) -> Optional[list[SelectedPackage]]:
+) -> list[SelectedPackage] | None:
     ipt = InteractivePackageTree(
         path=path,
         depth=depth,
         exclude_paths=exclude_paths,
         auto_select_initial_packages=auto_select_initial_packages,
     )
     return ipt.run()
```

### Comparing `tach-0.2.7/python/tach/loading.py` & `tach-0.3.0/python/tach/loading.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.7/python/tach/logging/api.py` & `tach-0.3.0/python/tach/logging/api.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.7/python/tach/logging/logger.py` & `tach-0.3.0/python/tach/logging/logger.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 import logging
 import multiprocessing
 import os
 import signal
-from typing import TYPE_CHECKING, Any, Optional
+from typing import TYPE_CHECKING, Any
 
 from pydantic import BaseModel, Field
 
 from tach import cache
 from tach.logging.api import log_record, log_uid
 from tach.parsing import parse_project_config
 
@@ -20,15 +20,15 @@
     function: str
     parameters: dict[str, Any] = Field(default_factory=dict)
 
 
 def send_log_entry(record: logging.LogRecord, entry: str) -> None:
     is_ci = "CI" in os.environ
     is_gauge = "IS_GAUGE" in os.environ
-    data: Optional[LogDataModel] = getattr(record, "data", None)
+    data: LogDataModel | None = getattr(record, "data", None)
     uid = cache.get_uid()
     log_data: dict[str, Any] = {
         "user": str(uid) if uid else None,
         "message": entry,
         "level": record.levelname,
         "timestamp": record.created,
         "function": data.function if data else None,
@@ -49,15 +49,15 @@
 
     import sys
 
     devnull = open(os.devnull, "w")
     sys.stdout = devnull
     sys.stderr = devnull
 
-    def handler(signum: int, frame: Optional[FrameType]) -> None:
+    def handler(signum: int, frame: FrameType | None) -> None:
         raise TimeoutError()
 
     signal.signal(signal.SIGALRM, handler)  # ensure logging process always exits
     signal.alarm(3)  # 3 sec timeout
     try:
         send_log_entry(record=record, entry=entry)
     except Exception:  # noqa
```

### Comparing `tach-0.2.7/python/tach/parsing/config.py` & `tach-0.3.0/python/tach/parsing/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from __future__ import annotations
 
-from typing import Optional
-
 import yaml
 
 from tach import filesystem as fs
 from tach.colors import BCOLORS
 from tach.core import PackageConfig, ProjectConfig
 
 
@@ -17,35 +15,35 @@
     config.constraints.sort(key=lambda constr: constr.tag)
     for constr in config.constraints:
         constr.depends_on.sort()
     config.exclude = list(set(config.exclude)) if config.exclude else []
     return yaml.dump(config.model_dump(), sort_keys=False)
 
 
-def parse_project_config(root: str = ".") -> Optional[ProjectConfig]:
+def parse_project_config(root: str = ".") -> ProjectConfig | None:
     file_path = fs.get_project_config_path(root)
     if not file_path:
         return None
 
-    with open(file_path, "r") as f:
+    with open(file_path) as f:
         result = yaml.safe_load(f)
         if not result or not isinstance(result, dict):
             raise ValueError(f"Empty or invalid project config file: {file_path}")
     was_deprecated_config, config = ProjectConfig.factory(result)  # type: ignore
     # Automatically update the config if it used the deprecated format
     if was_deprecated_config:
         print(
             f"{BCOLORS.WARNING} Auto-updating project configuration format.{BCOLORS.ENDC}"
         )
         fs.write_file(file_path, dump_project_config_to_yaml(config))
     return config
 
 
-def parse_package_config(root: str = ".") -> Optional[PackageConfig]:
+def parse_package_config(root: str = ".") -> PackageConfig | None:
     file_path = fs.validate_package_config(root)
     if file_path:
-        with open(file_path, "r") as f:
+        with open(file_path) as f:
             result = yaml.safe_load(f)
             if not result or not isinstance(result, dict):
                 raise ValueError(f"Empty or invalid package config file: {file_path}")
         # We want to error on type issues here for now
         return PackageConfig(**result)  # type: ignore
```

### Comparing `tach-0.2.7/python/tach/parsing/interface.py` & `tach-0.3.0/python/tach/parsing/interface.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.7/python/tach/parsing/packages.py` & `tach-0.3.0/python/tach/parsing/packages.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from __future__ import annotations
 
-from typing import Optional
-
 from tach import filesystem as fs
 from tach.core import PackageTrie
 from tach.parsing import parse_interface_members, parse_package_config
 
 
 def build_package_trie(
     root: str,
-    exclude_paths: Optional[list[str]] = None,
+    exclude_paths: list[str] | None = None,
 ) -> PackageTrie:
     package_trie = PackageTrie()
 
     for dir_path, _ in fs.walk_configured_packages(
         root,
         exclude_paths=exclude_paths,
     ):
```

### Comparing `tach-0.2.7/python/tach/pkg.py` & `tach-0.3.0/python/tach/pkg.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import os
 from dataclasses import dataclass, field
-from typing import Optional
 
 from tach import errors
 from tach import filesystem as fs
 from tach.colors import BCOLORS
 from tach.constants import CONFIG_FILE_NAME, PACKAGE_FILE_NAME, TOOL_NAME
 from tach.core import ProjectConfig
 from tach.interactive import SelectedPackage, get_selected_packages_interactive
@@ -20,15 +19,15 @@
     package_paths: list[str] = field(default_factory=list)
     warnings: list[str] = field(default_factory=list)
 
 
 def set_packages(
     selected_packages: list[SelectedPackage],
     path: str,
-    exclude_paths: Optional[list[str]] = None,
+    exclude_paths: list[str] | None = None,
 ) -> SetPackagesResult:
     package_paths: list[str] = []
     warnings: list[str] = []
 
     for existing_package, package_yml_path in fs.walk_configured_packages(
         root=path, exclude_paths=exclude_paths
     ):
@@ -83,15 +82,15 @@
     config_yml_content = dump_project_config_to_yaml(project_config)
     fs.write_file(project_config_path, config_yml_content)
 
     return InitRootResult(warnings=[])
 
 
 def pkg_edit_interactive(
-    root: str, depth: Optional[int] = 1, exclude_paths: Optional[list[str]] = None
+    root: str, depth: int | None = 1, exclude_paths: list[str] | None = None
 ) -> tuple[bool, list[str]]:
     if not os.path.isdir(root):
         raise errors.TachSetupError(f"The path {root} is not a directory.")
 
     if exclude_paths is None:
         exclude_paths = ["tests/", "docs/"]
```

### Comparing `tach-0.2.7/python/tach/sync.py` & `tach-0.3.0/python/tach/sync.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 from __future__ import annotations
 
 import os
-from typing import Optional
 
 from tach import errors
 from tach import filesystem as fs
 from tach.check import check
 from tach.colors import BCOLORS
 from tach.constants import CONFIG_FILE_NAME
 from tach.core import ProjectConfig
 from tach.parsing import dump_project_config_to_yaml, parse_project_config
 
 
 def sync_dependency_constraints(
     root: str,
     project_config: ProjectConfig,
-    filter_tags: Optional[set[str]] = None,
-    exclude_paths: Optional[list[str]] = None,
+    filter_tags: set[str] | None = None,
+    exclude_paths: list[str] | None = None,
 ) -> ProjectConfig:
     """
     Update project configuration with auto-detected dependency constraints.
     This is additive, meaning it will create dependencies to resolve existing errors,
     but will not remove any constraints.
     Passing 'filter_tags' will limit updates to only those dependencies which include one of those tags.
     """
@@ -50,16 +49,16 @@
                     )
 
     return project_config
 
 
 def prune_dependency_constraints(
     root: str,
-    project_config: Optional[ProjectConfig] = None,
-    exclude_paths: Optional[list[str]] = None,
+    project_config: ProjectConfig | None = None,
+    exclude_paths: list[str] | None = None,
 ) -> ProjectConfig:
     """
     Build a minimal project configuration with auto-detected dependency constraints.
     """
     if project_config is not None:
         # Force constraints to be empty in case we received configuration with pre-existing constraints
         project_config = project_config.model_copy(update={"constraints": []})
@@ -69,17 +68,15 @@
     sync_dependency_constraints(
         root, project_config=project_config, exclude_paths=exclude_paths
     )
 
     return project_config
 
 
-def sync_project(
-    prune: bool = False, exclude_paths: Optional[list[str]] = None
-) -> None:
+def sync_project(prune: bool = False, exclude_paths: list[str] | None = None) -> None:
     original_cwd = fs.get_cwd()
     try:
         root = fs.find_project_config_root(original_cwd)
         if root is None:
             raise errors.TachSetupError(
                 f"{BCOLORS.WARNING}Could not find project configuration.{BCOLORS.ENDC}"
             )
```

### Comparing `tach-0.2.7/python/tach.yml` & `tach-0.3.0/python/tach.yml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -27,16 +27,16 @@
   - scope:core
   - scope:filesystem
   - scope:interactive
   - scope:logging
   - scope:parsing
   - scope:utils
 exclude:
-- docs/
+- dist/
+- tach.egg-info/
 - .*__pycache__/
 - tests/
 - build/
-- tach.egg-info/
-- dist/
+- docs/
 exact: true
 disable_logging: false
 ignore_type_checking_imports: false
```

### Comparing `tach-0.2.7/python/tests/test_check.py` & `tach-0.3.0/python/tests/test_check.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.7/python/tests/test_cli.py` & `tach-0.3.0/python/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.7/python/tests/test_init.py` & `tach-0.3.0/python/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.7/python/tests/test_package_trie.py` & `tach-0.3.0/python/tests/test_package_trie.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 
 def test_iterate_over_empty_trie():
     assert list(PackageTrie()) == []
 
 
 def test_iterate_over_populated_trie(package_trie):
-    assert set((node.full_path for node in package_trie)) == {
+    assert set(node.full_path for node in package_trie) == {
         "domain_one",
         "domain_one.subdomain",
         "domain_two",
         "domain_two.subdomain",
         "domain_three",
     }
 
@@ -81,27 +81,27 @@
 def test_get_actual_path(package_trie):
     assert package_trie.get("domain_one") is not None
 
 
 def test_insert_empty_path(test_config):
     trie = PackageTrie()
     trie.insert(test_config, "", [])
-    assert set((node.full_path for node in trie)) == {""}
+    assert set(node.full_path for node in trie) == {""}
 
 
 def test_insert_single_level_path(test_config):
     trie = PackageTrie()
     trie.insert(test_config, "domain", [])
-    assert set((node.full_path for node in trie)) == {"domain"}
+    assert set(node.full_path for node in trie) == {"domain"}
 
 
 def test_insert_multi_level_path(test_config):
     trie = PackageTrie()
     trie.insert(test_config, "domain.subdomain", [])
-    assert set((node.full_path for node in trie)) == {"domain.subdomain"}
+    assert set(node.full_path for node in trie) == {"domain.subdomain"}
 
 
 def test_find_nearest_at_root(package_trie):
     package = package_trie.find_nearest("other_domain")
     assert package is None
```

### Comparing `tach-0.2.7/python/tests/test_parsing.py` & `tach-0.3.0/python/tests/test_parsing.py`

 * *Files identical despite different names*

### Comparing `tach-0.2.7/pyproject.toml` & `tach-0.3.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "tach"
-version = "0.2.7"
+version = "0.3.0"
 authors = [
   { name="Caelean Barnes", email="caeleanb@gmail.com" },
   { name="Evan Doyle", email="evanmdoyle@gmail.com" },
 ]
 description = "A Python tool to maintain a modular package architecture."
 readme = "README.md"
 requires-python = ">=3.8"
@@ -38,16 +38,17 @@
 
 [project.urls]
 Homepage = "https://github.com/gauge-sh/tach"
 Issues = "https://github.com/gauge-sh/tach/issues"
 
 [tool.ruff]
 src = ["python"]
+exclude = ["crates"]
 target-version = "py38"
-lint.extend-select = ["I", "TCH"]
+lint.extend-select = ["I", "TCH", "UP"]
 
 [tool.ruff.lint.isort]
 required-imports = ["from __future__ import annotations"]
 
 [tool.ruff.lint.flake8-type-checking]
 runtime-evaluated-base-classes = [
     "pydantic.BaseModel",
```

### Comparing `tach-0.2.7/PKG-INFO` & `tach-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tach
-Version: 0.2.7
+Version: 0.3.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

