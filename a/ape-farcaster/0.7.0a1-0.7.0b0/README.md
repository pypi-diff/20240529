# Comparing `tmp/ape-farcaster-0.7.0a1.tar.gz` & `tmp/ape-farcaster-0.7.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-farcaster-0.7.0a1.tar", last modified: Mon May 13 21:25:06 2024, max compression
+gzip compressed data, was "ape-farcaster-0.7.0b0.tar", last modified: Tue May 28 23:21:20 2024, max compression
```

## Comparing `ape-farcaster-0.7.0a1.tar` & `ape-farcaster-0.7.0b0.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:25:06.482769 ape-farcaster-0.7.0a1/
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:25:06.470769 ape-farcaster-0.7.0a1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/.github/.stale.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:25:06.474768 ape-farcaster-0.7.0a1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:25:06.474768 ape-farcaster-0.7.0a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-05-13 21:25:06.482769 ape-farcaster-0.7.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/SECURITY.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:25:06.474768 ape-farcaster-0.7.0a1/ape_farcaster/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/ape_farcaster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    36719 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/ape_farcaster/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/ape_farcaster/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    15463 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/ape_farcaster/models.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/ape_farcaster/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:25:06.474768 ape-farcaster-0.7.0a1/ape_farcaster/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/ape_farcaster/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4801 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/ape_farcaster/utils/stream_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:25:06.474768 ape-farcaster-0.7.0a1/ape_farcaster.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-05-13 21:25:06.000000 ape-farcaster-0.7.0a1/ape_farcaster.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-05-13 21:25:06.000000 ape-farcaster-0.7.0a1/ape_farcaster.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 21:25:06.000000 ape-farcaster-0.7.0a1/ape_farcaster.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-13 21:25:06.000000 ape-farcaster-0.7.0a1/ape_farcaster.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-13 21:25:06.000000 ape-farcaster-0.7.0a1/ape_farcaster.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:25:06.470769 ape-farcaster-0.7.0a1/assets/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:25:06.474768 ape-farcaster-0.7.0a1/assets/images/
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/assets/images/coverage.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:25:06.474768 ape-farcaster-0.7.0a1/docker/
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/docker/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:25:06.474768 ape-farcaster-0.7.0a1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:25:06.474768 ape-farcaster-0.7.0a1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/docs/images/favicon-16x16.webp
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/docs/images/favicon-32x32.webp
--rw-r--r--   0 runner    (1001) docker     (127)   189794 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/docs/images/logo.webp
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/docs/reference.md
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 21:25:06.482769 ape-farcaster-0.7.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:25:06.478769 ape-farcaster-0.7.0a1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:25:06.470769 ape-farcaster-0.7.0a1/tests/cassettes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:25:06.482769 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/TestRW.test_delete_cast.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/TestRW.test_delete_cast_likes.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/TestRW.test_delete_recast.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/TestRW.test_like_cast.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/TestRW.test_post_cast.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/TestRW.test_recast.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_follow_user.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_all_casts_in_thread.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   143181 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_all_followers.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    53083 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_all_following.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_cast.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    22393 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_cast_likes.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    12561 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_cast_recasters.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   113260 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_casts.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_custody_address.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    47853 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_followers.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   170816 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_following.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_me.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   141233 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_recent_casts.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    31003 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_recent_users.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_user.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_user_by_username.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_user_by_verification.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    30104 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_user_cast_likes.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_verifications.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_nonexistent_get_cast.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    25309 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_stream_casts.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    24898 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_stream_casts_skip_existing.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_stream_notifications.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_stream_notifications_skip_existing.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_stream_users.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_stream_users_skip_existing.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_unfollow_user.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:25:06.482769 ape-farcaster-0.7.0a1/tests/cassettes/test_merkle/
--rw-r--r--   0 runner    (1001) docker     (127)   131470 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_merkle/test_get_collection_owners.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_merkle/test_get_healthcheck.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    24843 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_merkle/test_get_user_collections.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/cassettes/test_merkle/test_mention_reply_notifications.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/integration_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/test_authentication.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    12465 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/test_farcaster.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/test_merkle.py
--rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-13 21:24:45.000000 ape-farcaster-0.7.0a1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:21:20.668974 ape-farcaster-0.7.0b0/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:21:20.656974 ape-farcaster-0.7.0b0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/.github/.stale.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:21:20.656974 ape-farcaster-0.7.0b0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:21:20.656974 ape-farcaster-0.7.0b0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    10549 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-05-28 23:21:20.668974 ape-farcaster-0.7.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/SECURITY.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:21:20.660974 ape-farcaster-0.7.0b0/ape_farcaster/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/ape_farcaster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36772 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/ape_farcaster/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/ape_farcaster/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15463 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/ape_farcaster/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/ape_farcaster/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:21:20.660974 ape-farcaster-0.7.0b0/ape_farcaster/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/ape_farcaster/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4805 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/ape_farcaster/utils/stream_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:21:20.660974 ape-farcaster-0.7.0b0/ape_farcaster.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-05-28 23:21:20.000000 ape-farcaster-0.7.0b0/ape_farcaster.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3434 2024-05-28 23:21:20.000000 ape-farcaster-0.7.0b0/ape_farcaster.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 23:21:20.000000 ape-farcaster-0.7.0b0/ape_farcaster.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-28 23:21:20.000000 ape-farcaster-0.7.0b0/ape_farcaster.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-28 23:21:20.000000 ape-farcaster-0.7.0b0/ape_farcaster.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:21:20.652974 ape-farcaster-0.7.0b0/assets/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:21:20.660974 ape-farcaster-0.7.0b0/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/assets/images/coverage.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:21:20.660974 ape-farcaster-0.7.0b0/docker/
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/docker/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:21:20.660974 ape-farcaster-0.7.0b0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:21:20.660974 ape-farcaster-0.7.0b0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/docs/images/favicon-16x16.webp
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/docs/images/favicon-32x32.webp
+-rw-r--r--   0 runner    (1001) docker     (127)   189794 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/docs/images/logo.webp
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/docs/reference.md
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4374 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 23:21:20.668974 ape-farcaster-0.7.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:21:20.660974 ape-farcaster-0.7.0b0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:21:20.652974 ape-farcaster-0.7.0b0/tests/cassettes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:21:20.668974 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/TestRW.test_delete_cast.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/TestRW.test_delete_cast_likes.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/TestRW.test_delete_recast.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/TestRW.test_like_cast.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/TestRW.test_post_cast.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2636 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/TestRW.test_recast.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_follow_user.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_all_casts_in_thread.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   143181 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_all_followers.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    53083 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_all_following.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3493 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_cast.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    22393 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_cast_likes.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    12561 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_cast_recasters.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   113260 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_casts.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5188 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_custody_address.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    47853 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_followers.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   170816 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_following.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2822 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_me.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   141233 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_recent_casts.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    31003 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_recent_users.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_user.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3163 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_user_by_username.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5833 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_user_by_verification.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    30104 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_user_cast_likes.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_verifications.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2709 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_nonexistent_get_cast.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    25309 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_stream_casts.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    24898 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_stream_casts_skip_existing.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3482 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_stream_notifications.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3484 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_stream_notifications_skip_existing.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5331 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_stream_users.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5322 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_stream_users_skip_existing.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_unfollow_user.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:21:20.668974 ape-farcaster-0.7.0b0/tests/cassettes/test_merkle/
+-rw-r--r--   0 runner    (1001) docker     (127)   131470 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_merkle/test_get_collection_owners.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_merkle/test_get_healthcheck.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    24843 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_merkle/test_get_user_collections.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3491 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/cassettes/test_merkle/test_mention_reply_notifications.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/integration_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2770 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/test_authentication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12465 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/test_farcaster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/test_merkle.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11587 2024-05-28 23:20:20.000000 ape-farcaster-0.7.0b0/tests/test_utils.py
```

### Comparing `ape-farcaster-0.7.0a1/.github/.stale.yml` & `ape-farcaster-0.7.0b0/.github/.stale.yml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/.github/ISSUE_TEMPLATE/bug_report.md` & `ape-farcaster-0.7.0b0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/.github/ISSUE_TEMPLATE/feature_request.md` & `ape-farcaster-0.7.0b0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/.github/PULL_REQUEST_TEMPLATE.md` & `ape-farcaster-0.7.0b0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/.github/dependabot.yml` & `ape-farcaster-0.7.0b0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/.github/release-drafter.yml` & `ape-farcaster-0.7.0b0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/.github/workflows/build.yml` & `ape-farcaster-0.7.0b0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/.github/workflows/publish.yaml` & `ape-farcaster-0.7.0b0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/.gitignore` & `ape-farcaster-0.7.0b0/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/.pre-commit-config.yaml` & `ape-farcaster-0.7.0b0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/CODE_OF_CONDUCT.md` & `ape-farcaster-0.7.0b0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/CONTRIBUTING.md` & `ape-farcaster-0.7.0b0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/LICENSE` & `ape-farcaster-0.7.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/Makefile` & `ape-farcaster-0.7.0b0/Makefile`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/PKG-INFO` & `ape-farcaster-0.7.0b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-farcaster
-Version: 0.7.0a1
+Version: 0.7.0b0
 Summary: ape-farcaster is a Python SDK for the Farcaster Protocol
 Author-email: Andreessen Horowitz <crypto-engineering@a16z.com>, "ApeWorX LTD." <admin@apeworx.io>
 Maintainer-email: "ApeWorX LTD." <admin@apeworx.io>
 Project-URL: Repository, https://github.com/ApeWorX/ape-farcaster
 Project-URL: Homepage, https://github.com/ApeWorX/ape-farcaster/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ape-farcaster-0.7.0a1/README.md` & `ape-farcaster-0.7.0b0/README.md`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/SECURITY.md` & `ape-farcaster-0.7.0b0/SECURITY.md`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/ape_farcaster/client.py` & `ape-farcaster-0.7.0b0/ape_farcaster/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,28 +2,27 @@
 
 import base64
 import logging
 import time
 
 import canonicaljson
 import requests
+from ape.api import AccountAPI
+from ape.types import MessageSignature
 from eth_account.account import Account
 from eth_account.datastructures import SignedMessage
 from eth_account.messages import encode_defunct
 from eth_account.signers.local import LocalAccount
 from pydantic import PositiveInt
 from requests.adapters import HTTPAdapter
 from urllib3.util import Retry
 
-from farcaster.config import *
-from farcaster.models import *
-from farcaster.utils.stream_generator import stream_generator
-
-from ape.api import AccountAPI
-from ape.types import MessageSignature
+from ape_farcaster.config import *
+from ape_farcaster.models import *
+from ape_farcaster.utils.stream_generator import stream_generator
 
 
 class Warpcast:
     """The Warpcast class is a wrapper around the Farcaster API.
     It also provides a number of helpful methods and utilities for interacting with the protocol.
     Pydantic models are used under the hood to validate the data returned from the API.
     """
@@ -52,15 +51,15 @@
             self.config.base_path,
             HTTPAdapter(
                 max_retries=Retry(
                     total=2, backoff_factor=1, status_forcelist=[520, 413, 429, 503]
                 )
             ),
         )
-        
+
         self.create_new_auth_token(expires_in=self.rotation_duration)
 
     def get_base_path(self):
         return self.config.base_path
 
     def get_base_options(self):
         return self.config.base_options
@@ -192,14 +191,16 @@
         header = self.generate_custody_auth_header(auth_params)
         body = AuthPutRequest(params=auth_params)
         response = requests.put(
             self.config.base_path + "auth",
             json=body.model_dump(by_alias=True, exclude_none=True),
             headers={"Authorization": header},
         ).json()
+        if "errors" in response:
+            raise Exception(response["errors"])  # pragma: no cover
         return AuthPutResponse(**response).result
 
     def delete_auth(self) -> StatusContent:
         """Delete an access token
 
         Returns:
             StatusContent: Status of the deletion
@@ -1064,22 +1065,21 @@
 
         Raises:
             Exception: account is required
 
         Returns:
             str: custody authorization header
         """
-       
+
         auth_put_request = AuthPutRequest(params=params)
         payload = auth_put_request.model_dump(by_alias=True, exclude_none=True)
         encoded_payload = canonicaljson.encode_canonical_json(payload)
         signable_message = encode_defunct(primitive=encoded_payload)
         signed_message: MessageSignature = self.account.sign_message(signable_message)
-        # TODO check if it is in vrs or rsv
-        data_hex_array = bytearray(signed_message.encode_vrs())
+        data_hex_array = bytearray(signed_message.encode_rsv())
         encoded = base64.b64encode(data_hex_array).decode()
         return f"Bearer eip191:{encoded}"
 
 
 def now_ms() -> int:
     """Get the current time in milliseconds
```

### Comparing `ape-farcaster-0.7.0a1/ape_farcaster/config.py` & `ape-farcaster-0.7.0b0/ape_farcaster/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Any, Dict, Optional
 
-from farcaster.models import *
+from ape_farcaster.models import *
 
 FARCASTER_API_BASE_URL = "https://api.warpcast.com/v2/"
 
 
 class ConfigurationParams(BaseModel):
     username: Optional[str] = None
     password: Optional[str] = None
```

### Comparing `ape-farcaster-0.7.0a1/ape_farcaster/models.py` & `ape-farcaster-0.7.0b0/ape_farcaster/models.py`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/ape_farcaster/utils/stream_generator.py` & `ape-farcaster-0.7.0b0/ape_farcaster/utils/stream_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import logging
 import random
 import time
 from collections import OrderedDict
 
 from pydantic import PositiveInt
 
-from farcaster.models import ApiCast, ApiUser, MentionNotification, ReplyNotification
+from ape_farcaster.models import ApiCast, ApiUser, MentionNotification, ReplyNotification
 
 Streamable = Union[
     List[Union[MentionNotification, ReplyNotification]],
     List[ApiUser],
     List[ApiCast],
 ]
```

### Comparing `ape-farcaster-0.7.0a1/ape_farcaster.egg-info/PKG-INFO` & `ape-farcaster-0.7.0b0/ape_farcaster.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-farcaster
-Version: 0.7.0a1
+Version: 0.7.0b0
 Summary: ape-farcaster is a Python SDK for the Farcaster Protocol
 Author-email: Andreessen Horowitz <crypto-engineering@a16z.com>, "ApeWorX LTD." <admin@apeworx.io>
 Maintainer-email: "ApeWorX LTD." <admin@apeworx.io>
 Project-URL: Repository, https://github.com/ApeWorX/ape-farcaster
 Project-URL: Homepage, https://github.com/ApeWorX/ape-farcaster/
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `ape-farcaster-0.7.0a1/ape_farcaster.egg-info/SOURCES.txt` & `ape-farcaster-0.7.0b0/ape_farcaster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/assets/images/coverage.svg` & `ape-farcaster-0.7.0b0/assets/images/coverage.svg`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/docker/Dockerfile` & `ape-farcaster-0.7.0b0/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/docker/README.md` & `ape-farcaster-0.7.0b0/docker/README.md`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/docs/images/favicon-32x32.webp` & `ape-farcaster-0.7.0b0/docs/images/favicon-32x32.webp`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/docs/images/logo.webp` & `ape-farcaster-0.7.0b0/docs/images/logo.webp`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/docs/index.md` & `ape-farcaster-0.7.0b0/docs/index.md`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/mkdocs.yml` & `ape-farcaster-0.7.0b0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/pyproject.toml` & `ape-farcaster-0.7.0b0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -30,20 +30,21 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
 ]
 
 dependencies = [
+  "eth-ape>=0.7",
   "python-dotenv >= 0.21,<1.1",
   "pydantic >= 1.9.2,<3.0.0",
   "pyhumps >= 3.7.2",
   "requests >= 2.28.1",
   "canonicaljson >= 1.6.4,<3.0.0",
-  "eth-account >= 0.8,<0.11",
+  "eth-account",  # Peer of eth-ape
   "parsimonious >= 0.8.1,<0.10.0",
 ]
 
 [project.urls]
 Repository = "https://github.com/ApeWorX/ape-farcaster"
 Homepage = "https://github.com/ApeWorX/ape-farcaster/"
```

### Comparing `ape-farcaster-0.7.0a1/requirements.txt` & `ape-farcaster-0.7.0b0/requirements.txt`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/TestRW.test_delete_cast.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/TestRW.test_delete_cast.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/TestRW.test_delete_cast_likes.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/TestRW.test_delete_cast_likes.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/TestRW.test_delete_recast.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/TestRW.test_delete_recast.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/TestRW.test_like_cast.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/TestRW.test_like_cast.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/TestRW.test_post_cast.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/TestRW.test_post_cast.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/TestRW.test_recast.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/TestRW.test_recast.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_follow_user.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_follow_user.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_all_casts_in_thread.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_all_casts_in_thread.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_all_followers.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_all_followers.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_all_following.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_all_following.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_cast.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_cast.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_cast_likes.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_cast_likes.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_cast_recasters.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_cast_recasters.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_casts.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_casts.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_custody_address.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_custody_address.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_followers.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_followers.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_following.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_following.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_me.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_me.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_recent_casts.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_recent_casts.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_recent_users.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_recent_users.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_user.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_user.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_user_by_username.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_user_by_username.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_user_by_verification.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_user_by_verification.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_user_cast_likes.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_user_cast_likes.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_get_verifications.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_get_verifications.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_nonexistent_get_cast.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_nonexistent_get_cast.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_stream_casts.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_stream_casts.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_stream_casts_skip_existing.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_stream_casts_skip_existing.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_stream_notifications.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_stream_notifications.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_stream_notifications_skip_existing.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_stream_notifications_skip_existing.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_stream_users.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_stream_users.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_stream_users_skip_existing.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_stream_users_skip_existing.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_farcaster/test_unfollow_user.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_farcaster/test_unfollow_user.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_merkle/test_get_collection_owners.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_merkle/test_get_collection_owners.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_merkle/test_get_healthcheck.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_merkle/test_get_healthcheck.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_merkle/test_get_user_collections.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_merkle/test_get_user_collections.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/cassettes/test_merkle/test_mention_reply_notifications.yaml` & `ape-farcaster-0.7.0b0/tests/cassettes/test_merkle/test_mention_reply_notifications.yaml`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/integration_tests.py` & `ape-farcaster-0.7.0b0/tests/integration_tests.py`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/test_authentication.py` & `ape-farcaster-0.7.0b0/tests/test_authentication.py`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/test_config.py` & `ape-farcaster-0.7.0b0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/test_farcaster.py` & `ape-farcaster-0.7.0b0/tests/test_farcaster.py`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/test_merkle.py` & `ape-farcaster-0.7.0b0/tests/test_merkle.py`

 * *Files identical despite different names*

### Comparing `ape-farcaster-0.7.0a1/tests/test_utils.py` & `ape-farcaster-0.7.0b0/tests/test_utils.py`

 * *Files identical despite different names*

