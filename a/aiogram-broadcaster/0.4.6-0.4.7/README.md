# Comparing `tmp/aiogram_broadcaster-0.4.6.tar.gz` & `tmp/aiogram_broadcaster-0.4.7.tar.gz`

## Comparing `aiogram_broadcaster-0.4.6.tar` & `aiogram_broadcaster-0.4.7.tar`

### file list

```diff
@@ -1,66 +1,91 @@
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/.editorconfig
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/Makefile
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/mypy.ini
--rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/ruff.toml
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0      744 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/.github/workflows/tests.yml
--rw-r--r--   0        0        0      282 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/__meta__.py
--rw-r--r--   0        0        0     9111 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/broadcaster.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/event.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/loggers.py
--rw-r--r--   0        0        0     6112 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/placeholder.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/py.typed
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/__init__.py
--rw-r--r--   0        0        0     2781 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/animation.py
--rw-r--r--   0        0        0     2633 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/audio.py
--rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/base.py
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/chat_action.py
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/contact.py
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/dice.py
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/document.py
--rw-r--r--   0        0        0     2938 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/from_chat.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/game.py
--rw-r--r--   0        0        0     3717 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/invoice.py
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/key_based.py
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/lazy.py
--rw-r--r--   0        0        0     2319 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/location.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/media_group.py
--rw-r--r--   0        0        0     4259 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/message.py
--rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/photo.py
--rw-r--r--   0        0        0     3788 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/poll.py
--rw-r--r--   0        0        0     1803 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/sticker.py
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/text.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/venue.py
--rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/video.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/video_note.py
--rw-r--r--   0        0        0     2283 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/voice.py
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/mailer/__init__.py
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/mailer/chat_engine.py
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/mailer/container.py
--rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/mailer/group.py
--rw-r--r--   0        0        0    10395 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/mailer/mailer.py
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/mailer/settings.py
--rw-r--r--   0        0        0     4014 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/mailer/statistic.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/mailer/status.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/mailer/task_manager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/storage/__init__.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/storage/base.py
--rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/storage/file.py
--rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/storage/mongodb.py
--rw-r--r--   0        0        0     2722 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/storage/redis.py
--rw-r--r--   0        0        0     3767 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/storage/sqlalchemy.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/utils/__init__.py
--rw-r--r--   0        0        0     3623 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/utils/chain.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/aiogram_broadcaster/utils/interrupt.py
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/examples/events.py
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/examples/key_based_content.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/examples/lazy_content.py
--rw-r--r--   0        0        0     1444 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/examples/mre.py
--rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/examples/multibot.py
--rw-r--r--   0        0        0     2132 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/examples/placeholders.py
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/LICENSE
--rw-r--r--   0        0        0    15147 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/README.md
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/pyproject.toml
--rw-r--r--   0        0        0    16593 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/.editorconfig
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/Makefile
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/__meta__.py
+-rw-r--r--   0        0        0     9159 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/broadcaster.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/py.typed
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/__init__.py
+-rw-r--r--   0        0        0     2853 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/animation.py
+-rw-r--r--   0        0        0     2705 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/audio.py
+-rw-r--r--   0        0        0     3069 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/base.py
+-rw-r--r--   0        0        0      708 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/chat_action.py
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/contact.py
+-rw-r--r--   0        0        0     1735 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/dice.py
+-rw-r--r--   0        0        0     2599 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/document.py
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/from_chat.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/game.py
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/invoice.py
+-rw-r--r--   0        0        0     1279 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/key_based.py
+-rw-r--r--   0        0        0      566 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/lazy.py
+-rw-r--r--   0        0        0     2391 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/location.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/media_group.py
+-rw-r--r--   0        0        0     4425 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/message.py
+-rw-r--r--   0        0        0     2369 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/photo.py
+-rw-r--r--   0        0        0     3860 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/poll.py
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/sticker.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/text.py
+-rw-r--r--   0        0        0     2525 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/venue.py
+-rw-r--r--   0        0        0     2977 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/video.py
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/video_note.py
+-rw-r--r--   0        0        0     2355 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/voice.py
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/event/__init__.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/event/manager.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/event/observer.py
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/event/registry.py
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/__init__.py
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/chat_engine.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/container.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/group.py
+-rw-r--r--   0        0        0    10530 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/mailer.py
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/settings.py
+-rw-r--r--   0        0        0     4073 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/statistic.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/status.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/task_manager.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/placeholder/__init__.py
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/placeholder/item.py
+-rw-r--r--   0        0        0     2620 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/placeholder/manager.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/placeholder/placeholder.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/placeholder/registry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/storages/__init__.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/storages/base.py
+-rw-r--r--   0        0        0     2579 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/storages/file.py
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/storages/mongodb.py
+-rw-r--r--   0        0        0     2725 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/storages/redis.py
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/storages/sqlalchemy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/utils/__init__.py
+-rw-r--r--   0        0        0     3290 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/utils/chain.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/utils/interrupt.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/aiogram_broadcaster/utils/loggers.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/examples/events.py
+-rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/examples/key_based_content.py
+-rw-r--r--   0        0        0     1476 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/examples/lazy_content.py
+-rw-r--r--   0        0        0     1393 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/examples/mre.py
+-rw-r--r--   0        0        0     1139 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/examples/multibot.py
+-rw-r--r--   0        0        0     2119 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/examples/placeholders.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_contents/__init__.py
+-rw-r--r--   0        0        0     2608 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_contents/test_base.py
+-rw-r--r--   0        0        0     6332 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_contents/test_contents.py
+-rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_contents/test_key_based.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_contents/test_lazy.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_event/__init__.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_event/test_manager.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_event/test_observer.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_event/test_registry.py
+-rw-r--r--   0        0        0     2697 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_mailer/test_settings.py
+-rw-r--r--   0        0        0     1942 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_mailer/test_task_manager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_placeholder/__init__.py
+-rw-r--r--   0        0        0      779 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_placeholder/test_item.py
+-rw-r--r--   0        0        0     4899 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_placeholder/test_manager.py
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_placeholder/test_placeholder.py
+-rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_placeholder/test_registry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_utils/__init__.py
+-rw-r--r--   0        0        0     4720 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_utils/test_chain.py
+-rw-r--r--   0        0        0      540 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/tests/test_utils/test_interrupt.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/LICENSE
+-rw-r--r--   0        0        0    15641 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/README.md
+-rw-r--r--   0        0        0     3734 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0    18852 2020-02-02 00:00:00.000000 aiogram_broadcaster-0.4.7/PKG-INFO
```

### Comparing `aiogram_broadcaster-0.4.6/.github/workflows/pypi-publish.yml` & `aiogram_broadcaster-0.4.7/.github/workflows/tests.yml`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,60 @@
-name: PYPI-Publish
+name: Tests
 
 on:
   push:
     branches:
       - main
-  workflow_dispatch:
+      - dev
+  pull_request:
+    branches:
+      - main
+      - dev
+  workflow_dispatch: null
 
 jobs:
-  build:
-    name: Build
-    runs-on: ubuntu-latest
+  tests:
+    name: Tests
+    runs-on: "${{ matrix.os }}"
+    strategy:
+      matrix:
+        os:
+          - ubuntu-latest
+          - macos-latest
+          - windows-latest
+        python-version:
+          - "3.8"
+          - "3.9"
+          - "3.10"
+          - "3.11"
+          - "3.12"
+    defaults:
+      run:
+        shell: bash
+    env:
+      VENV_BIN: "${{ startsWith(matrix.os, 'windows') && 'Scripts' || 'bin' }}"
     steps:
-      - uses: actions/checkout@v4
+      - name: Checkout repository
+        uses: actions/checkout@v4
 
-      - name: Setup python
+      - name: Setup Python
         uses: actions/setup-python@v5
         with:
-          python-version: "3.10"
-
-      - name: Install build dependencies
-        run: python -m pip install --upgrade build
-
-      - name: Build source distribution
-        run: python -m build .
-
-      - name: Publish artifacts
-        uses: actions/upload-artifact@v4
-        with:
-          name: dist
-          path: dist/*
-
-  publish:
-    name: Publish
-    needs: build
-    if: "success()"
-    runs-on: ubuntu-latest
-    permissions:
-      id-token: write
-    steps:
-      - name: Download artifacts
-        uses: actions/download-artifact@v4
-        with:
-          name: dist
-          path: dist
-
-      - name: Publish a Python distribution to PyPI
-        uses: pypa/gh-action-pypi-publish@release/v1
-        with:
-          user: __token__
-          password: ${{ secrets.PYPI_TOKEN }}
-          skip-existing: true
+          python-version: "${{ matrix.python-version }}"
+          cache: pip
+          cache-dependency-path: pyproject.toml
+
+      - name: Install dependencies
+        run: python -m pip install --upgrade .[dev,test,redis,mongo,sqlalchemy] build pip
+
+      - name: Lint code
+        run: make lint
+
+      - name: Run tests
+        run: make test
+
+      - name: Check installable
+        run: |
+          python -m build --wheel .
+          python -m venv ./venv
+          ./venv/${{ env.VENV_BIN }}/pip install ./dist/*.whl
+          ./venv/${{ env.VENV_BIN }}/python -c 'import aiogram_broadcaster;print(aiogram_broadcaster.__version__)'
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/broadcaster.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/broadcaster.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 from typing import Any, Dict, Iterable, Literal, Optional, Set, Tuple, Union, cast
 from uuid import uuid4
 
 from aiogram import Bot, Dispatcher
 from pydantic import JsonValue
 from pydantic_core import PydanticSerializationError, ValidationError
+from typing_extensions import Self
 
-from . import loggers
 from .contents.base import BaseContent, ContentType
-from .event import EventManager
+from .event.manager import EventManager
 from .mailer.chat_engine import ChatsRegistry
 from .mailer.container import MailerContainer
 from .mailer.group import MailerGroup
 from .mailer.mailer import Mailer
 from .mailer.settings import DefaultMailerSettings, MailerSettings
 from .mailer.status import MailerStatus
-from .placeholder import PlaceholderManager
-from .storage.base import BaseMailerStorage, StorageRecord
+from .placeholder.manager import PlaceholderManager
+from .storages.base import BaseMailerStorage, StorageRecord
+from .utils import loggers
 
 
 class Broadcaster(MailerContainer):
     bots: Tuple[Bot, ...]
     storage: Optional[BaseMailerStorage]
     default: DefaultMailerSettings
     context_key: str
@@ -225,15 +226,15 @@
     def setup(
         self,
         dispatcher: Dispatcher,
         *,
         fetch_dispatcher_context: bool = True,
         restore_mailers: bool = True,
         run_mailers: bool = True,
-    ) -> "Broadcaster":
+    ) -> Self:
         dispatcher[self.context_key] = self
         self.context["dispatcher"] = dispatcher
         if fetch_dispatcher_context:
             self.context.update(dispatcher.workflow_data)
         if self.storage:
             dispatcher.startup.register(self.storage.startup)
             dispatcher.shutdown.register(self.storage.shutdown)
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/__init__.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/animation.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/animation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, List, Optional, Union
+from typing import TYPE_CHECKING, Any, List, Optional, Union
 
 from aiogram.client.default import Default
 from aiogram.methods import SendAnimation
 from aiogram.types import (
     ForceReply,
     InlineKeyboardMarkup,
     InputFile,
@@ -48,14 +48,15 @@
             caption=self.caption,
             parse_mode=self.parse_mode,
             caption_entities=self.caption_entities,
             has_spoiler=self.has_spoiler,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
             reply_markup=self.reply_markup,
+            **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
@@ -75,8 +76,9 @@
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
             ] = ...,
+            **kwargs: Any,
         ) -> None: ...
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/audio.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/audio.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, List, Optional, Union
+from typing import TYPE_CHECKING, Any, List, Optional, Union
 
 from aiogram.client.default import Default
 from aiogram.methods import SendAudio
 from aiogram.types import (
     ForceReply,
     InlineKeyboardMarkup,
     InputFile,
@@ -46,14 +46,15 @@
             duration=self.duration,
             performer=self.performer,
             title=self.title,
             thumbnail=self.thumbnail,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
             reply_markup=self.reply_markup,
+            **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
@@ -72,8 +73,9 @@
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
             ] = ...,
+            **kwargs: Any,
         ) -> None: ...
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/base.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,51 +19,65 @@
     ContentType = TypeVar("ContentType", bound="BaseContent")
 
 VALIDATOR_KEY = "__V"
 
 
 class BaseContent(BaseModel, ABC):
     model_config = ConfigDict(
-        extra="forbid",
+        extra="allow",
         frozen=True,
         validate_assignment=True,
         arbitrary_types_allowed=True,
     )
 
     _validators: ClassVar[Dict[str, Type["BaseContent"]]] = {}
-    _callback: ClassVar[CallableObject]
+    _callback: CallableObject
 
-    def __init_subclass__(cls, **kwargs: Any) -> None:
-        cls._callback = CallableObject(callback=cls.__call__)
-        if kwargs.pop("register", True):
+    def __init_subclass__(
+        cls,
+        register: bool = True,  # noqa: FBT001, FBT002
+        **kwargs: Any,
+    ) -> None:
+        if register:
             cls.register()
         super().__init_subclass__(**kwargs)
 
     if TYPE_CHECKING:
         __call__: Callable[..., Any]
     else:
 
         @abstractmethod
         async def __call__(self, **kwargs: Any) -> Any:
             pass
 
     async def as_method(self, **context: Any) -> TelegramMethod[Any]:
-        method = await self._callback.call(self, **context)
+        method = await self._callback.call(**context)
         return cast(TelegramMethod[Any], method)
 
     @classmethod
     def is_registered(cls) -> bool:
         return cls.__name__ in cls._validators
 
     @classmethod
     def register(cls) -> None:
+        if cls is BaseContent:
+            raise TypeError("BaseContent cannot be registered.")
         if cls.is_registered():
             raise RuntimeError(f"The content {cls.__name__!r} is already registered.")
         cls._validators[cls.__name__] = cls
 
+    @classmethod
+    def unregister(cls) -> None:
+        if not cls.is_registered():
+            raise RuntimeError(f"The content {cls.__name__!r} is not registered.")
+        del cls._validators[cls.__name__]
+
+    def model_post_init(self, __context: Any) -> None:
+        self._callback = CallableObject(callback=self.__call__)
+
     @model_validator(mode="wrap")
     @classmethod
     def _validate(cls, value: Any, handler: ValidatorFunctionWrapHandler) -> Any:
         if not isinstance(value, dict):
             return handler(value)
         if VALIDATOR_KEY not in value:
             return handler(value)
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/chat_action.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/chat_action.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Optional
+from typing import TYPE_CHECKING, Any, Optional
 
 from aiogram.methods import SendChatAction
 
 from .base import BaseContent
 
 
 class ChatActionContent(BaseContent):
@@ -10,17 +10,19 @@
     business_connection_id: Optional[str] = None
 
     async def __call__(self, chat_id: int) -> SendChatAction:
         return SendChatAction(
             chat_id=chat_id,
             action=self.action,
             business_connection_id=self.business_connection_id,
+            **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
             action: str,
             business_connection_id: Optional[str] = ...,
+            **kwargs: Any,
         ) -> None: ...
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/contact.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/contact.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Optional, Union
+from typing import TYPE_CHECKING, Any, Optional, Union
 
 from aiogram.client.default import Default
 from aiogram.methods import SendContact
 from aiogram.types import (
     ForceReply,
     InlineKeyboardMarkup,
     ReplyKeyboardMarkup,
@@ -36,14 +36,15 @@
             first_name=self.first_name,
             business_connection_id=self.business_connection_id,
             last_name=self.last_name,
             vcard=self.vcard,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
             reply_markup=self.reply_markup,
+            **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
@@ -58,8 +59,9 @@
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
             ] = ...,
+            **kwargs: Any,
         ) -> None: ...
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/dice.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/dice.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Optional, Union
+from typing import TYPE_CHECKING, Any, Optional, Union
 
 from aiogram.client.default import Default
 from aiogram.methods import SendDice
 from aiogram.types import (
     ForceReply,
     InlineKeyboardMarkup,
     ReplyKeyboardMarkup,
@@ -30,14 +30,15 @@
         return SendDice(
             chat_id=chat_id,
             business_connection_id=self.business_connection_id,
             emoji=self.emoji,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
             reply_markup=self.reply_markup,
+            **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
@@ -49,8 +50,9 @@
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
             ] = ...,
+            **kwargs: Any,
         ) -> None: ...
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/document.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/document.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, List, Optional, Union
+from typing import TYPE_CHECKING, Any, List, Optional, Union
 
 from aiogram.client.default import Default
 from aiogram.methods import SendDocument
 from aiogram.types import (
     ForceReply,
     InlineKeyboardMarkup,
     InputFile,
@@ -42,14 +42,15 @@
             caption=self.caption,
             parse_mode=self.parse_mode,
             caption_entities=self.caption_entities,
             disable_content_type_detection=self.disable_content_type_detection,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
             reply_markup=self.reply_markup,
+            **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
@@ -66,8 +67,9 @@
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
             ] = ...,
+            **kwargs: Any,
         ) -> None: ...
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/from_chat.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/photo.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,93 +1,72 @@
-from typing import TYPE_CHECKING, List, Optional, Union
+from typing import TYPE_CHECKING, Any, List, Optional, Union
 
 from aiogram.client.default import Default
-from aiogram.methods import CopyMessage, ForwardMessage
+from aiogram.methods import SendPhoto
 from aiogram.types import (
     ForceReply,
     InlineKeyboardMarkup,
+    InputFile,
     MessageEntity,
     ReplyKeyboardMarkup,
     ReplyKeyboardRemove,
 )
 
 from .base import BaseContent
 
 
-class FromChatCopyContent(BaseContent):
-    from_chat_id: Union[int, str]
-    message_id: int
+class PhotoContent(BaseContent):
+    photo: Union[InputFile, str]
+    business_connection_id: Optional[str] = None
     caption: Optional[str] = None
     parse_mode: Optional[Union[str, Default]] = Default("parse_mode")
     caption_entities: Optional[List[MessageEntity]] = None
+    has_spoiler: Optional[bool] = None
     disable_notification: Optional[bool] = None
     protect_content: Optional[Union[bool, Default]] = Default("protect_content")
     reply_markup: Optional[
         Union[
             InlineKeyboardMarkup,
             ReplyKeyboardMarkup,
             ReplyKeyboardRemove,
             ForceReply,
         ]
     ] = None
 
-    async def __call__(self, chat_id: int) -> CopyMessage:
-        return CopyMessage(
+    async def __call__(self, chat_id: int) -> SendPhoto:
+        return SendPhoto(
             chat_id=chat_id,
-            from_chat_id=self.from_chat_id,
-            message_id=self.message_id,
+            photo=self.photo,
+            business_connection_id=self.business_connection_id,
             caption=self.caption,
             parse_mode=self.parse_mode,
             caption_entities=self.caption_entities,
+            has_spoiler=self.has_spoiler,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
             reply_markup=self.reply_markup,
+            **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
-            from_chat_id: Union[int, str],
-            message_id: int,
+            photo: Union[InputFile, str],
+            business_connection_id: Optional[str] = ...,
             caption: Optional[str] = ...,
-            parse_mode: Optional[str] = ...,
+            parse_mode: Optional[Union[str, Default]] = ...,
             caption_entities: Optional[List[MessageEntity]] = ...,
+            has_spoiler: Optional[bool] = ...,
             disable_notification: Optional[bool] = ...,
-            protect_content: Optional[bool] = ...,
+            protect_content: Optional[Union[bool, Default]] = ...,
             reply_markup: Optional[
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
             ] = ...,
-        ) -> None: ...
-
-
-class FromChatForwardContent(BaseContent):
-    from_chat_id: Union[int, str]
-    message_id: int
-    disable_notification: Optional[bool] = None
-    protect_content: Optional[Union[bool, Default]] = Default("protect_content")
-
-    async def __call__(self, chat_id: int) -> ForwardMessage:
-        return ForwardMessage(
-            chat_id=chat_id,
-            from_chat_id=self.from_chat_id,
-            message_id=self.message_id,
-            disable_notification=self.disable_notification,
-            protect_content=self.protect_content,
-        )
-
-    if TYPE_CHECKING:
-
-        def __init__(
-            self,
-            *,
-            from_chat_id: Union[int, str],
-            message_id: int,
-            disable_notification: Optional[bool] = ...,
-            protect_content: Optional[Union[bool, Default]] = ...,
+            **kwargs: Any,
         ) -> None: ...
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/game.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/game.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,12 @@
-from typing import TYPE_CHECKING, Optional, Union
+from typing import TYPE_CHECKING, Any, Optional, Union
 
 from aiogram.client.default import Default
 from aiogram.methods import SendGame
-from aiogram.types import (
-    InlineKeyboardMarkup,
-)
+from aiogram.types import InlineKeyboardMarkup
 
 from .base import BaseContent
 
 
 class GameContent(BaseContent):
     game_short_name: str
     business_connection_id: Optional[str] = None
@@ -20,20 +18,22 @@
         return SendGame(
             chat_id=chat_id,
             game_short_name=self.game_short_name,
             business_connection_id=self.business_connection_id,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
             reply_markup=self.reply_markup,
+            **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
             game_short_name: str,
             business_connection_id: Optional[str] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
             reply_markup: Optional[InlineKeyboardMarkup] = ...,
+            **kwargs: Any,
         ) -> None: ...
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/invoice.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/invoice.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-from typing import TYPE_CHECKING, List, Optional, Union
+from typing import TYPE_CHECKING, Any, List, Optional, Union
 
 from aiogram.client.default import Default
 from aiogram.methods import SendInvoice
-from aiogram.types import (
-    InlineKeyboardMarkup,
-    LabeledPrice,
-)
+from aiogram.types import InlineKeyboardMarkup, LabeledPrice
 
 from .base import BaseContent
 
 
 class InvoiceContent(BaseContent):
     title: str
     description: str
@@ -59,14 +56,15 @@
             need_shipping_address=self.need_shipping_address,
             send_phone_number_to_provider=self.send_phone_number_to_provider,
             send_email_to_provider=self.send_email_to_provider,
             is_flexible=self.is_flexible,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
             reply_markup=self.reply_markup,
+            **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
@@ -90,8 +88,9 @@
             need_shipping_address: Optional[bool] = ...,
             send_phone_number_to_provider: Optional[bool] = ...,
             send_email_to_provider: Optional[bool] = ...,
             is_flexible: Optional[bool] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
             reply_markup: Optional[InlineKeyboardMarkup] = ...,
+            **kwargs: Any,
         ) -> None: ...
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/key_based.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/key_based.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,32 +9,29 @@
 class KeyBasedContent(BaseContent, register=False):
     model_config = ConfigDict(extra="allow")
 
     default: Optional[SerializeAsAny[BaseContent]] = None
     __pydantic_extra__: Dict[str, SerializeAsAny[BaseContent]]
 
     def __getitem__(self, item: str) -> BaseContent:
+        if self.default:
+            return self.__pydantic_extra__.get(item, self.default)
         return self.__pydantic_extra__[item]
 
     def __contains__(self, item: str) -> bool:
         return item in self.__pydantic_extra__
 
+    async def as_method(self, **context: Any) -> TelegramMethod[Any]:
+        key = await self._callback.call(**context)
+        return await self[key].as_method(**context)
+
     def model_post_init(self, __context: Any) -> None:
         if not self.default and not self.__pydantic_extra__:
             raise ValueError("At least one content must be specified.")
-
-    async def as_method(self, **context: Any) -> TelegramMethod[Any]:
-        key = await self._callback.call(self, **context)
-        content = self.resolve_content(key=key)
-        return await content.as_method(**context)
-
-    def resolve_content(self, key: Any) -> BaseContent:
-        if self.default:
-            return self.__pydantic_extra__.get(key, self.default)
-        return self.__pydantic_extra__[key]
+        super().model_post_init(__context)
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
             default: Optional[BaseContent] = ...,
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/lazy.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/lazy.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,14 +3,14 @@
 from aiogram.methods import TelegramMethod
 
 from .base import BaseContent
 
 
 class LazyContent(BaseContent, register=False):
     async def as_method(self, **context: Any) -> TelegramMethod[Any]:
-        content = await self._callback.call(self, **context)
+        content = await self._callback.call(**context)
         if not isinstance(content, BaseContent):
             raise TypeError(
-                f"The {type(self).__name__} expected to return an content of "
+                f"The {type(self).__name__!r} expected to return an content of "
                 f"type BaseContent, not a {type(content).__name__}.",
             )
         return await content.as_method(**context)
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/location.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/location.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, Optional, Union
+from typing import TYPE_CHECKING, Any, Optional, Union
 
 from aiogram.client.default import Default
 from aiogram.methods import SendLocation
 from aiogram.types import (
     ForceReply,
     InlineKeyboardMarkup,
     ReplyKeyboardMarkup,
@@ -40,14 +40,15 @@
             horizontal_accuracy=self.horizontal_accuracy,
             live_period=self.live_period,
             heading=self.heading,
             proximity_alert_radius=self.proximity_alert_radius,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
             reply_markup=self.reply_markup,
+            **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
@@ -64,8 +65,9 @@
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
             ] = ...,
+            **kwargs: Any,
         ) -> None: ...
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/media_group.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/media_group.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, List, Optional, Union
+from typing import TYPE_CHECKING, Any, List, Optional, Union
 
 from aiogram.client.default import Default
 from aiogram.methods import SendMediaGroup
 from aiogram.types import InputMediaAudio, InputMediaDocument, InputMediaPhoto, InputMediaVideo
 
 from .base import BaseContent
 
@@ -23,14 +23,15 @@
     async def __call__(self, chat_id: int) -> SendMediaGroup:
         return SendMediaGroup(
             chat_id=chat_id,
             media=self.media,
             business_connection_id=self.business_connection_id,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
+            **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
@@ -41,8 +42,9 @@
                     InputMediaPhoto,
                     InputMediaVideo,
                 ]
             ],
             business_connection_id: Optional[str] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
+            **kwargs: Any,
         ) -> None: ...
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/message.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/message.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import TYPE_CHECKING, List, Optional, Union
+from typing import TYPE_CHECKING, Any, List, Optional, Union
 
 from aiogram.client.default import Default
 from aiogram.methods import (
     CopyMessage,
     ForwardMessage,
     SendAnimation,
     SendAudio,
@@ -52,14 +52,15 @@
             chat_id=chat_id,
             caption=self.caption,
             parse_mode=self.parse_mode,
             caption_entities=self.caption_entities,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
             reply_markup=self.reply_markup,
+            **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
@@ -73,37 +74,40 @@
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
             ] = ...,
+            **kwargs: Any,
         ) -> None: ...
 
 
 class MessageForwardContent(BaseContent):
     message: Message
     disable_notification: Optional[bool] = None
     protect_content: Optional[Union[bool, Default]] = Default("protect_content")
 
     async def __call__(self, chat_id: int) -> ForwardMessage:
         return self.message.forward(
             chat_id=chat_id,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
+            **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
             message: Message,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
+            **kwargs: Any,
         ) -> None: ...
 
 
 class MessageSendContent(BaseContent):
     message: Message
     disable_notification: Optional[bool] = None
     reply_markup: Optional[Union[InlineKeyboardMarkup, ReplyKeyboardMarkup]] = None
@@ -144,8 +148,9 @@
             self,
             *,
             message: Message,
             disable_notification: Optional[bool] = ...,
             reply_markup: Optional[Union[InlineKeyboardMarkup, ReplyKeyboardMarkup]] = ...,
             business_connection_id: Optional[str] = ...,
             parse_mode: Optional[str] = ...,
+            **kwargs: Any,
         ) -> None: ...
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/photo.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/video.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,70 +1,87 @@
-from typing import TYPE_CHECKING, List, Optional, Union
+from typing import TYPE_CHECKING, Any, List, Optional, Union
 
 from aiogram.client.default import Default
-from aiogram.methods import SendPhoto
+from aiogram.methods import SendVideo
 from aiogram.types import (
     ForceReply,
     InlineKeyboardMarkup,
     InputFile,
     MessageEntity,
     ReplyKeyboardMarkup,
     ReplyKeyboardRemove,
 )
 
 from .base import BaseContent
 
 
-class PhotoContent(BaseContent):
-    photo: Union[InputFile, str]
+class VideoContent(BaseContent):
+    video: Union[InputFile, str]
     business_connection_id: Optional[str] = None
+    duration: Optional[int] = None
+    width: Optional[int] = None
+    height: Optional[int] = None
+    thumbnail: Optional[InputFile] = None
     caption: Optional[str] = None
     parse_mode: Optional[Union[str, Default]] = Default("parse_mode")
     caption_entities: Optional[List[MessageEntity]] = None
     has_spoiler: Optional[bool] = None
+    supports_streaming: Optional[bool] = None
     disable_notification: Optional[bool] = None
     protect_content: Optional[Union[bool, Default]] = Default("protect_content")
     reply_markup: Optional[
         Union[
             InlineKeyboardMarkup,
             ReplyKeyboardMarkup,
             ReplyKeyboardRemove,
             ForceReply,
         ]
     ] = None
 
-    async def __call__(self, chat_id: int) -> SendPhoto:
-        return SendPhoto(
+    async def __call__(self, chat_id: int) -> SendVideo:
+        return SendVideo(
             chat_id=chat_id,
-            photo=self.photo,
+            video=self.video,
             business_connection_id=self.business_connection_id,
+            duration=self.duration,
+            width=self.width,
+            height=self.height,
+            thumbnail=self.thumbnail,
             caption=self.caption,
             parse_mode=self.parse_mode,
             caption_entities=self.caption_entities,
             has_spoiler=self.has_spoiler,
+            supports_streaming=self.supports_streaming,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
             reply_markup=self.reply_markup,
+            **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
-            photo: Union[InputFile, str],
+            video: Union[InputFile, str],
             business_connection_id: Optional[str] = ...,
+            duration: Optional[int] = ...,
+            width: Optional[int] = ...,
+            height: Optional[int] = ...,
+            thumbnail: Optional[InputFile] = ...,
             caption: Optional[str] = ...,
             parse_mode: Optional[Union[str, Default]] = ...,
             caption_entities: Optional[List[MessageEntity]] = ...,
             has_spoiler: Optional[bool] = ...,
+            supports_streaming: Optional[bool] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
             reply_markup: Optional[
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
             ] = ...,
+            **kwargs: Any,
         ) -> None: ...
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/poll.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/poll.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime, timedelta
-from typing import TYPE_CHECKING, List, Optional, Union
+from typing import TYPE_CHECKING, Any, List, Optional, Union
 
 from aiogram.client.default import Default
 from aiogram.methods import SendPoll
 from aiogram.types import (
     ForceReply,
     InlineKeyboardMarkup,
     InputPollOption,
@@ -59,14 +59,15 @@
             explanation_entities=self.explanation_entities,
             open_period=self.open_period,
             close_date=self.close_date,
             is_closed=self.is_closed,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
             reply_markup=self.reply_markup,
+            **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
@@ -91,8 +92,9 @@
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
             ] = ...,
+            **kwargs: Any,
         ) -> None: ...
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/sticker.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/text.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,60 +1,69 @@
-from typing import TYPE_CHECKING, Optional, Union
+from typing import TYPE_CHECKING, Any, List, Optional, Union
 
 from aiogram.client.default import Default
-from aiogram.methods import SendSticker
+from aiogram.methods import SendMessage
 from aiogram.types import (
     ForceReply,
     InlineKeyboardMarkup,
-    InputFile,
+    LinkPreviewOptions,
+    MessageEntity,
     ReplyKeyboardMarkup,
     ReplyKeyboardRemove,
 )
 
 from .base import BaseContent
 
 
-class StickerContent(BaseContent):
-    sticker: Union[InputFile, str]
+class TextContent(BaseContent):
+    text: str
     business_connection_id: Optional[str] = None
-    emoji: Optional[str] = None
+    parse_mode: Optional[Union[str, Default]] = Default("parse_mode")
+    entities: Optional[List[MessageEntity]] = None
+    link_preview_options: Optional[Union[LinkPreviewOptions, Default]] = Default("link_preview")
     disable_notification: Optional[bool] = None
     protect_content: Optional[Union[bool, Default]] = Default("protect_content")
     reply_markup: Optional[
         Union[
             InlineKeyboardMarkup,
             ReplyKeyboardMarkup,
             ReplyKeyboardRemove,
             ForceReply,
         ]
     ] = None
 
-    async def __call__(self, chat_id: int) -> SendSticker:
-        return SendSticker(
+    async def __call__(self, chat_id: int) -> SendMessage:
+        return SendMessage(
             chat_id=chat_id,
-            sticker=self.sticker,
+            text=self.text,
             business_connection_id=self.business_connection_id,
-            emoji=self.emoji,
+            parse_mode=self.parse_mode,
+            entities=self.entities,
+            link_preview_options=self.link_preview_options,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
             reply_markup=self.reply_markup,
+            **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
-            sticker: Union[InputFile, str],
+            text: str,
             business_connection_id: Optional[str] = ...,
-            emoji: Optional[str] = ...,
+            parse_mode: Optional[Union[str, Default]] = ...,
+            entities: Optional[List[MessageEntity]] = ...,
+            link_preview_options: Optional[Union[LinkPreviewOptions, Default]] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
             reply_markup: Optional[
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
             ] = ...,
+            **kwargs: Any,
         ) -> None: ...
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/text.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/venue.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,67 +1,79 @@
-from typing import TYPE_CHECKING, List, Optional, Union
+from typing import TYPE_CHECKING, Any, Optional, Union
 
 from aiogram.client.default import Default
-from aiogram.methods import SendMessage
+from aiogram.methods import SendVenue
 from aiogram.types import (
     ForceReply,
     InlineKeyboardMarkup,
-    LinkPreviewOptions,
-    MessageEntity,
     ReplyKeyboardMarkup,
     ReplyKeyboardRemove,
 )
 
 from .base import BaseContent
 
 
-class TextContent(BaseContent):
-    text: str
+class VenueContent(BaseContent):
+    latitude: float
+    longitude: float
+    title: str
+    address: str
     business_connection_id: Optional[str] = None
-    parse_mode: Optional[Union[str, Default]] = Default("parse_mode")
-    entities: Optional[List[MessageEntity]] = None
-    link_preview_options: Optional[Union[LinkPreviewOptions, Default]] = Default("link_preview")
+    foursquare_id: Optional[str] = None
+    foursquare_type: Optional[str] = None
+    google_place_id: Optional[str] = None
+    google_place_type: Optional[str] = None
     disable_notification: Optional[bool] = None
     protect_content: Optional[Union[bool, Default]] = Default("protect_content")
     reply_markup: Optional[
         Union[
             InlineKeyboardMarkup,
             ReplyKeyboardMarkup,
             ReplyKeyboardRemove,
             ForceReply,
         ]
     ] = None
 
-    async def __call__(self, chat_id: int) -> SendMessage:
-        return SendMessage(
+    async def __call__(self, chat_id: int) -> SendVenue:
+        return SendVenue(
             chat_id=chat_id,
-            text=self.text,
+            latitude=self.latitude,
+            longitude=self.longitude,
+            title=self.title,
+            address=self.address,
             business_connection_id=self.business_connection_id,
-            parse_mode=self.parse_mode,
-            entities=self.entities,
-            link_preview_options=self.link_preview_options,
+            foursquare_id=self.foursquare_id,
+            foursquare_type=self.foursquare_type,
+            google_place_id=self.google_place_id,
+            google_place_type=self.google_place_type,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
             reply_markup=self.reply_markup,
+            **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
-            text: str,
+            latitude: float,
+            longitude: float,
+            title: str,
+            address: str,
             business_connection_id: Optional[str] = ...,
-            parse_mode: Optional[Union[str, Default]] = ...,
-            entities: Optional[List[MessageEntity]] = ...,
-            link_preview_options: Optional[Union[LinkPreviewOptions, Default]] = ...,
+            foursquare_id: Optional[str] = ...,
+            foursquare_type: Optional[str] = ...,
+            google_place_id: Optional[str] = ...,
+            google_place_type: Optional[str] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
             reply_markup: Optional[
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
             ] = ...,
+            **kwargs: Any,
         ) -> None: ...
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/venue.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/video_note.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,77 +1,68 @@
-from typing import TYPE_CHECKING, Optional, Union
+from typing import TYPE_CHECKING, Any, Optional, Union
 
 from aiogram.client.default import Default
-from aiogram.methods import SendVenue
+from aiogram.methods import SendVideoNote
 from aiogram.types import (
     ForceReply,
     InlineKeyboardMarkup,
+    InputFile,
     ReplyKeyboardMarkup,
     ReplyKeyboardRemove,
 )
 
 from .base import BaseContent
 
 
-class VenueContent(BaseContent):
-    latitude: float
-    longitude: float
-    title: str
-    address: str
+class VideoNoteContent(BaseContent):
+    video_note: Union[InputFile, str]
     business_connection_id: Optional[str] = None
-    foursquare_id: Optional[str] = None
-    foursquare_type: Optional[str] = None
-    google_place_id: Optional[str] = None
-    google_place_type: Optional[str] = None
+    duration: Optional[int] = None
+    length: Optional[int] = None
+    thumbnail: Optional[InputFile] = None
     disable_notification: Optional[bool] = None
     protect_content: Optional[Union[bool, Default]] = Default("protect_content")
     reply_markup: Optional[
         Union[
             InlineKeyboardMarkup,
             ReplyKeyboardMarkup,
             ReplyKeyboardRemove,
             ForceReply,
         ]
     ] = None
 
-    async def __call__(self, chat_id: int) -> SendVenue:
-        return SendVenue(
+    async def __call__(self, chat_id: int) -> SendVideoNote:
+        return SendVideoNote(
             chat_id=chat_id,
-            latitude=self.latitude,
-            longitude=self.longitude,
-            title=self.title,
-            address=self.address,
+            video_note=self.video_note,
             business_connection_id=self.business_connection_id,
-            foursquare_id=self.foursquare_id,
-            foursquare_type=self.foursquare_type,
-            google_place_id=self.google_place_id,
-            google_place_type=self.google_place_type,
+            duration=self.duration,
+            length=self.length,
+            thumbnail=self.thumbnail,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
             reply_markup=self.reply_markup,
+            **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
-            latitude: float,
-            longitude: float,
-            title: str,
-            address: str,
+            video_note: Union[InputFile, str],
             business_connection_id: Optional[str] = ...,
-            foursquare_id: Optional[str] = ...,
-            foursquare_type: Optional[str] = ...,
-            google_place_id: Optional[str] = ...,
-            google_place_type: Optional[str] = ...,
+            duration: Optional[int] = ...,
+            length: Optional[int] = ...,
+            thumbnail: Optional[InputFile] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
             reply_markup: Optional[
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
             ] = ...,
+            **kwargs: Any,
         ) -> None: ...
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/video.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/voice.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,85 +1,72 @@
-from typing import TYPE_CHECKING, List, Optional, Union
+from typing import TYPE_CHECKING, Any, List, Optional, Union
 
 from aiogram.client.default import Default
-from aiogram.methods import SendVideo
+from aiogram.methods import SendVoice
 from aiogram.types import (
     ForceReply,
     InlineKeyboardMarkup,
     InputFile,
     MessageEntity,
     ReplyKeyboardMarkup,
     ReplyKeyboardRemove,
 )
 
 from .base import BaseContent
 
 
-class VideoContent(BaseContent):
-    video: Union[InputFile, str]
+class VoiceContent(BaseContent):
+    voice: Union[InputFile, str]
     business_connection_id: Optional[str] = None
-    duration: Optional[int] = None
-    width: Optional[int] = None
-    height: Optional[int] = None
-    thumbnail: Optional[InputFile] = None
     caption: Optional[str] = None
     parse_mode: Optional[Union[str, Default]] = Default("parse_mode")
     caption_entities: Optional[List[MessageEntity]] = None
-    has_spoiler: Optional[bool] = None
-    supports_streaming: Optional[bool] = None
+    duration: Optional[int] = None
     disable_notification: Optional[bool] = None
     protect_content: Optional[Union[bool, Default]] = Default("protect_content")
     reply_markup: Optional[
         Union[
             InlineKeyboardMarkup,
             ReplyKeyboardMarkup,
             ReplyKeyboardRemove,
             ForceReply,
         ]
     ] = None
 
-    async def __call__(self, chat_id: int) -> SendVideo:
-        return SendVideo(
+    async def __call__(self, chat_id: int) -> SendVoice:
+        return SendVoice(
             chat_id=chat_id,
-            video=self.video,
+            voice=self.voice,
             business_connection_id=self.business_connection_id,
-            duration=self.duration,
-            width=self.width,
-            height=self.height,
-            thumbnail=self.thumbnail,
             caption=self.caption,
             parse_mode=self.parse_mode,
             caption_entities=self.caption_entities,
-            has_spoiler=self.has_spoiler,
-            supports_streaming=self.supports_streaming,
+            duration=self.duration,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
             reply_markup=self.reply_markup,
+            **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
-            video: Union[InputFile, str],
+            voice: Union[InputFile, str],
             business_connection_id: Optional[str] = ...,
-            duration: Optional[int] = ...,
-            width: Optional[int] = ...,
-            height: Optional[int] = ...,
-            thumbnail: Optional[InputFile] = ...,
             caption: Optional[str] = ...,
             parse_mode: Optional[Union[str, Default]] = ...,
             caption_entities: Optional[List[MessageEntity]] = ...,
-            has_spoiler: Optional[bool] = ...,
-            supports_streaming: Optional[bool] = ...,
+            duration: Optional[int] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
             reply_markup: Optional[
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
             ] = ...,
+            **kwargs: Any,
         ) -> None: ...
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/contents/video_note.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/contents/sticker.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,62 @@
-from typing import TYPE_CHECKING, Optional, Union
+from typing import TYPE_CHECKING, Any, Optional, Union
 
 from aiogram.client.default import Default
-from aiogram.methods import SendVideoNote
+from aiogram.methods import SendSticker
 from aiogram.types import (
     ForceReply,
     InlineKeyboardMarkup,
     InputFile,
     ReplyKeyboardMarkup,
     ReplyKeyboardRemove,
 )
 
 from .base import BaseContent
 
 
-class VideoNoteContent(BaseContent):
-    video_note: Union[InputFile, str]
+class StickerContent(BaseContent):
+    sticker: Union[InputFile, str]
     business_connection_id: Optional[str] = None
-    duration: Optional[int] = None
-    length: Optional[int] = None
-    thumbnail: Optional[InputFile] = None
+    emoji: Optional[str] = None
     disable_notification: Optional[bool] = None
     protect_content: Optional[Union[bool, Default]] = Default("protect_content")
     reply_markup: Optional[
         Union[
             InlineKeyboardMarkup,
             ReplyKeyboardMarkup,
             ReplyKeyboardRemove,
             ForceReply,
         ]
     ] = None
 
-    async def __call__(self, chat_id: int) -> SendVideoNote:
-        return SendVideoNote(
+    async def __call__(self, chat_id: int) -> SendSticker:
+        return SendSticker(
             chat_id=chat_id,
-            video_note=self.video_note,
+            sticker=self.sticker,
             business_connection_id=self.business_connection_id,
-            duration=self.duration,
-            length=self.length,
-            thumbnail=self.thumbnail,
+            emoji=self.emoji,
             disable_notification=self.disable_notification,
             protect_content=self.protect_content,
             reply_markup=self.reply_markup,
+            **(self.model_extra or {}),
         )
 
     if TYPE_CHECKING:
 
         def __init__(
             self,
             *,
-            video_note: Union[InputFile, str],
+            sticker: Union[InputFile, str],
             business_connection_id: Optional[str] = ...,
-            duration: Optional[int] = ...,
-            length: Optional[int] = ...,
-            thumbnail: Optional[InputFile] = ...,
+            emoji: Optional[str] = ...,
             disable_notification: Optional[bool] = ...,
             protect_content: Optional[Union[bool, Default]] = ...,
             reply_markup: Optional[
                 Union[
                     InlineKeyboardMarkup,
                     ReplyKeyboardMarkup,
                     ReplyKeyboardRemove,
                     ForceReply,
                 ]
             ] = ...,
+            **kwargs: Any,
         ) -> None: ...
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/mailer/chat_engine.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/chat_engine.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from enum import Enum, auto
 from typing import TYPE_CHECKING, AsyncGenerator, DefaultDict, Iterable, Optional, Set
 
 from pydantic import BaseModel, ConfigDict
+from typing_extensions import Self
 
 
 if TYPE_CHECKING:
-    from aiogram_broadcaster.storage.base import BaseMailerStorage
+    from aiogram_broadcaster.storages.base import BaseMailerStorage
 
 
 class ChatState(str, Enum):
     PENDING = auto()
     SUCCESS = auto()
     FAILED = auto()
 
@@ -20,16 +21,16 @@
     chats: DefaultDict[ChatState, Set[int]]
 
     @classmethod
     def from_iterable(
         cls,
         chats: Iterable[int],
         state: ChatState = ChatState.PENDING,
-    ) -> "ChatsRegistry":
-        return ChatsRegistry(chats={state: chats})
+    ) -> Self:
+        return cls(chats={state: chats})
 
 
 class ChatEngine:
     registry: ChatsRegistry
     mailer_id: Optional[int]
     storage: Optional["BaseMailerStorage"]
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/mailer/container.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/container.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/mailer/group.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/group.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/mailer/mailer.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/mailer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from asyncio import Event, TimeoutError, wait_for
 from typing import Any, Dict, Generic, Iterable, Optional, Set
 
 from aiogram import Bot
 from aiogram.exceptions import TelegramAPIError, TelegramRetryAfter
 
-from aiogram_broadcaster import loggers
 from aiogram_broadcaster.contents.base import ContentType
-from aiogram_broadcaster.event import EventManager
-from aiogram_broadcaster.placeholder import PlaceholderManager
-from aiogram_broadcaster.storage.base import BaseMailerStorage
+from aiogram_broadcaster.event.manager import EventManager
+from aiogram_broadcaster.placeholder.manager import PlaceholderManager
+from aiogram_broadcaster.storages.base import BaseMailerStorage
+from aiogram_broadcaster.utils import loggers
 
 from .chat_engine import ChatEngine, ChatsRegistry, ChatState
 from .settings import MailerSettings
 from .statistic import MailerStatistic
 from .status import MailerStatus
 from .task_manager import TaskManager
 
@@ -77,14 +77,20 @@
 
     def __str__(self) -> str:
         return str(self._statistic)
 
     def __bool__(self) -> bool:
         return self._status is MailerStatus.COMPLETED
 
+    def __int__(self) -> int:
+        return self._id
+
+    def __index__(self) -> int:
+        return self._id
+
     def __hash__(self) -> int:
         return hash(self._id)
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, Mailer):
             return False
         return hash(self) == hash(other)
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/mailer/settings.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     disable_events: bool = False
     exclude_placeholders: Optional[Union[Literal[True], Set[str]]] = None
     preserved: bool = Field(default=True, exclude=True)
 
 
 _dataclass_properties: Dict[str, Any] = {}
 if version_info >= (3, 10):
-    _dataclass_properties.update(slots=True, kw_only=True)
+    _dataclass_properties.update(slots=True, kw_only=True)  # pragma: no cover
 
 
 @dataclass(**_dataclass_properties)
 class DefaultMailerSettings:
     interval: float = 0
     dynamic_interval: bool = False
     run_on_startup: bool = False
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/mailer/statistic.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/statistic.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,14 +55,17 @@
 
     def __len__(self) -> int:
         return self.total
 
     def __int__(self) -> int:
         return self.total
 
+    def __index__(self) -> int:
+        return self.total
+
     def __bool__(self) -> bool:
         return self.range == 0
 
     def __lt__(self, other: SupportsInt) -> bool:
         return self.total < int(other)
 
     def __gt__(self, other: SupportsInt) -> bool:
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/mailer/task_manager.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/mailer/task_manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,20 +20,22 @@
 
     @property
     def waited(self) -> bool:
         return self._waited
 
     def start(self, target: Coroutine[Any, Any, Any]) -> None:
         if self._task:
-            return
+            raise RuntimeError("Task is already started.")
         self._task = create_task(target)
         self._task.add_done_callback(self._on_task_done)
 
     async def wait(self) -> None:
-        if not self._task or self._waited:
-            return
+        if not self._task:
+            raise RuntimeError("No task for wait.")
+        if self._waited:
+            raise RuntimeError("Task is already waited.")
         self._waited = True
         await self._task
 
     def _on_task_done(self, _: "Task[Any]") -> None:
         self._task = None
         self._waited = False
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/storage/base.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/storages/base.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/storage/file.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/storages/file.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/storage/mongodb.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/storages/mongodb.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, Set
 
 from motor.motor_asyncio import AsyncIOMotorClient, AsyncIOMotorCollection
+from typing_extensions import Self
 
 from .base import BaseMailerStorage, StorageRecord
 
 
 DEFAULT_DATABASE_NAME = "broadcaster"
 DEFAULT_COLLECTION_NAME = "mailers"
 
@@ -29,15 +30,15 @@
     @classmethod
     def from_url(
         cls,
         url: str,
         database_name: str = DEFAULT_DATABASE_NAME,
         collection_name: str = DEFAULT_COLLECTION_NAME,
         **client_options: Any,
-    ) -> "MongoDBMailerStorage":
+    ) -> Self:
         client = AsyncIOMotorClient(url, **client_options)
         return cls(client=client, database_name=database_name, collection_name=collection_name)
 
     async def get_mailer_ids(self) -> Set[int]:
         result = await self.collection.distinct(key="_id")
         return set(result)
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/storage/redis.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/storages/redis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import Any, Optional, Set, Union
 
 from redis.asyncio import ConnectionPool, Redis
+from typing_extensions import Self
 
 from .base import BaseMailerStorage, StorageRecord
 
 
 DEFAULT_KEY_PREFIX = "mailer"
 DEFAULT_KEY_SEPERATOR = ":"
 
@@ -26,26 +27,26 @@
 
     @classmethod
     def from_pool(
         cls,
         pool: ConnectionPool,
         key_prefix: str = DEFAULT_KEY_PREFIX,
         key_seperator: str = DEFAULT_KEY_SEPERATOR,
-    ) -> "RedisMailerStorage":
+    ) -> Self:
         redis = Redis.from_pool(connection_pool=pool)
         return cls(redis=redis, key_prefix=key_prefix, key_seperator=key_seperator)
 
     @classmethod
     def from_url(
         cls,
         url: str,
         key_prefix: str = DEFAULT_KEY_PREFIX,
         key_seperator: str = DEFAULT_KEY_SEPERATOR,
         **connection_options: Any,
-    ) -> "RedisMailerStorage":
+    ) -> Self:
         connection_pool = ConnectionPool.from_url(url=url, **connection_options)
         redis = Redis.from_pool(connection_pool=connection_pool)
         return cls(redis=redis, key_prefix=key_prefix, key_seperator=key_seperator)
 
     async def get_mailer_ids(self) -> Set[int]:
         pattern = self.build_key()
         result = await self.redis.keys(pattern=pattern)
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/storage/sqlalchemy.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/storages/sqlalchemy.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from sqlalchemy.exc import IntegrityError
 from sqlalchemy.ext.asyncio import (
     AsyncEngine,
     AsyncSession,
     async_sessionmaker,
     create_async_engine,
 )
+from typing_extensions import Self
 
 from .base import BaseMailerStorage, StorageRecord
 
 
 DEFAULT_TABLE_NAME = "mailers"
 
 
@@ -48,26 +49,26 @@
 
     @classmethod
     def from_engine(
         cls,
         engine: AsyncEngine,
         table_name: str = DEFAULT_TABLE_NAME,
         **session_options: Any,
-    ) -> "SQLAlchemyMailerStorage":
+    ) -> Self:
         session_maker = async_sessionmaker(bind=engine, **session_options)
         return cls(session_maker=session_maker, table_name=table_name)
 
     @classmethod
     def from_url(
         cls,
         url: Union[str, URL],
         table_name: str = DEFAULT_TABLE_NAME,
         engine_options: Optional[Dict[str, Any]] = None,
         session_options: Optional[Dict[str, Any]] = None,
-    ) -> "SQLAlchemyMailerStorage":
+    ) -> Self:
         engine = create_async_engine(url=url, **(engine_options or {}))
         session_maker = async_sessionmaker(bind=engine, **(session_options or {}))
         return cls(session_maker=session_maker, table_name=table_name)
 
     @property
     def engine(self) -> AsyncEngine:
         return cast(AsyncEngine, self.session_maker.kw["bind"])
```

### Comparing `aiogram_broadcaster-0.4.6/aiogram_broadcaster/utils/chain.py` & `aiogram_broadcaster-0.4.7/aiogram_broadcaster/utils/chain.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-from typing import Any, ClassVar, Generator, Generic, List, Optional, TypeVar, overload
-from unittest.mock import sentinel
+from typing import Any, ClassVar, Generator, Generic, List, Optional, TypeVar
 
 
-EntityType = TypeVar("EntityType", bound="ChainObject[Any]")
+EntityType = TypeVar("EntityType", bound="Chain[Any]")
 
-UNSET_ENTITY = sentinel.UNSET_ENTITY
 
-
-class ChainObject(Generic[EntityType]):
-    __chain_root__: ClassVar[bool] = False
-    __entity: EntityType = UNSET_ENTITY
-    __sub_name: ClassVar[str]
+class Chain(Generic[EntityType]):
+    __chain_entity__: EntityType
+    __chain_sub_name__: ClassVar[str]
+    __chain_root__: ClassVar[bool]
     name: str
     head: Optional[EntityType]
     tail: List[EntityType]
 
-    def __init_subclass__(cls, **kwargs: Any) -> None:
-        if cls.__entity is UNSET_ENTITY:
-            cls.__entity = cls
-            cls.__sub_name = kwargs.pop("sub_name", cls.__name__.lower())
+    def __init_subclass__(cls, sub_name: Optional[str] = None, **kwargs: Any) -> None:
+        if not hasattr(cls, "__chain_entity__"):
+            cls.__chain_root__ = False
+            cls.__chain_entity__ = cls
+            cls.__chain_sub_name__ = sub_name or cls.__name__.lower()
         super().__init_subclass__(**kwargs)
 
     def __init__(self, name: Optional[str] = None) -> None:
-        self.name = hex(id(self)) if name is None else name
+        self.name = name or hex(id(self))
         self.head = None
         self.tail = []
 
     def __repr__(self) -> str:
-        fields = [f"name={self.name!r}"]
+        fields = []
+        fields.append(f"name={self.name!r}")
         if self.tail:
             fields.append(f"nested={list(self.tail)!r}")
         fields_sting = ", ".join(fields)
         return f"{type(self).__name__}({fields_sting})"
 
     def __str__(self) -> str:
-        fields = [f"name={self.name!r}"]
+        fields = []
+        fields.append(f"name={self.name!r}")
         if self.head:
             fields.append(f"parent={self.head!s}")
         fields_sting = ", ".join(fields)
         return f"{type(self).__name__}({fields_sting})"
 
     @property
     def chain_head(self: EntityType) -> Generator[EntityType, None, None]:
@@ -49,52 +49,42 @@
 
     @property
     def chain_tail(self: EntityType) -> Generator[EntityType, None, None]:
         yield self
         for entity in self.tail:
             yield from entity.chain_tail
 
-    @overload
-    def include(self: EntityType, entity: EntityType, /) -> EntityType: ...  # type: ignore[overload-overlap]
-
-    @overload
-    def include(self: EntityType, *entities: EntityType) -> None: ...
-
-    def include(self: EntityType, *entities: EntityType) -> Optional[EntityType]:
+    def bind(self: EntityType, *entities: EntityType) -> EntityType:
         if not entities:
             raise ValueError(
-                f"At least one {self.__sub_name} must be provided to include.",
+                f"At least one {self.__chain_sub_name__} must be provided to bind.",
             )
         for entity in entities:
-            if not isinstance(entity, self.__entity):
+            if not isinstance(entity, self.__chain_entity__):
                 raise TypeError(
-                    f"The {self.__sub_name} must be an instance of "
-                    f"{self.__entity.__name__}, not a {type(entity).__name__}.",
+                    f"The {self.__chain_sub_name__} must be an instance of "
+                    f"{self.__chain_entity__.__name__}, not a {type(entity).__name__}.",
                 )
             entity._chain_bind(entity=self)  # noqa: SLF001
-        return entities[-1] if len(entities) == 1 else None
+        return entities[-1] if len(entities) == 1 else self
 
     def _chain_bind(self: EntityType, entity: EntityType) -> None:
-        if self.__chain_root__:
-            raise RuntimeError(
-                f"{type(self).__name__} cannot be attached to another {self.__sub_name}.",
-            )
-        if not isinstance(entity, self.__entity):
-            raise TypeError(
-                f"The {self.__sub_name} must be an instance of "
-                f"{self.__entity.__name__}, not a {type(entity).__name__}.",
+        if self == entity:
+            raise ValueError(
+                f"Cannot bind the {self.__chain_sub_name__} on itself.",
             )
         if self.head:
             raise RuntimeError(
-                f"The {self.__sub_name} name={self.name!r} is already attached to "
-                f"{self.__sub_name} name={self.head.name!r}.",
-            )
-        if self == entity:
-            raise ValueError(
-                f"Cannot include the {self.__sub_name} on itself.",
+                f"The {self.__chain_entity__.__name__}(name={self.name!r}) is already attached to "
+                f"{self.__chain_entity__.__name__}(name={self.head.name!r}).",
             )
         if self in entity.chain_head:
             raise RuntimeError(
                 "Circular referencing detected.",
             )
+        if self.__chain_root__:
+            raise RuntimeError(
+                f"{type(self).__name__}(name={self.name!r}) cannot be attached to "
+                f"another {self.__chain_sub_name__}.",
+            )
         self.head = entity
         entity.tail.append(self)
```

### Comparing `aiogram_broadcaster-0.4.6/examples/events.py` & `aiogram_broadcaster-0.4.7/examples/events.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,24 +4,23 @@
 
 from aiogram import Bot, Dispatcher, Router, html
 from aiogram.client.default import DefaultBotProperties
 from aiogram.enums import ParseMode
 from aiogram.exceptions import TelegramForbiddenError
 from aiogram.types import Message
 
-from aiogram_broadcaster import Broadcaster, EventRouter
+from aiogram_broadcaster import Broadcaster, EventRegistry, Mailer
 from aiogram_broadcaster.contents import MessageSendContent
-from aiogram_broadcaster.mailer import Mailer
 
 
-TOKEN = "1234:Abc"  # noqa: S105
+TOKEN = "1234:Abc"
 USER_IDS = {78238238, 78378343, 98765431, 12345678}  # Your user IDs list
 
 router = Router(name=__name__)
-event = EventRouter(name=__name__)
+event = EventRegistry(name=__name__)
 
 
 @router.message()
 async def process_any_message(message: Message, broadcaster: Broadcaster, bot: Bot) -> Any:
     content = MessageSendContent(message=message)
     mailer = await broadcaster.create_mailer(
         content=content,
@@ -50,30 +49,30 @@
             f"Mailer ID: {mailer.id}\n"
             f"{html.blockquote(str(mailer.statistic))}"
         ),
     )
 
 
 @event.failed_sent()
-async def mailer_failed_sent(chat_id: int, error: Exception) -> None:  # noqa: ARG001, RUF029
+async def mailer_failed_sent(chat_id: int, error: Exception) -> None:
     if not isinstance(error, TelegramForbiddenError):
         return
     # Do something...
 
 
 def main() -> None:
     logging.basicConfig(level=logging.INFO, stream=sys.stdout)
 
     default = DefaultBotProperties(parse_mode=ParseMode.HTML)
     bot = Bot(token=TOKEN, default=default)
     dispatcher = Dispatcher()
     dispatcher.include_router(router)
 
     broadcaster = Broadcaster()
-    broadcaster.event.include(event)
+    broadcaster.event.bind(event)
     broadcaster.setup(dispatcher=dispatcher)
 
     dispatcher.run_polling(bot)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `aiogram_broadcaster-0.4.6/examples/key_based_content.py` & `aiogram_broadcaster-0.4.7/examples/key_based_content.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from aiogram.filters import CommandStart
 from aiogram.types import Message
 
 from aiogram_broadcaster import Broadcaster
 from aiogram_broadcaster.contents import KeyBasedContent, TextContent
 
 
-TOKEN = "1234:Abc"  # noqa: S105
+TOKEN = "1234:Abc"
 USER_IDS = {78238238, 78378343, 98765431, 12345678}  # Your user IDs list
 
 router = Router(name=__name__)
 
 
 class LanguageBasedContent(KeyBasedContent):
     """Content based on the user's language."""
```

### Comparing `aiogram_broadcaster-0.4.6/examples/lazy_content.py` & `aiogram_broadcaster-0.4.7/examples/lazy_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from aiogram.types import Message
 from pydantic import SerializeAsAny
 
 from aiogram_broadcaster import Broadcaster
 from aiogram_broadcaster.contents import BaseContent, LazyContent, TextContent
 
 
-TOKEN = "1234:Abc"  # noqa: S105
+TOKEN = "1234:Abc"
 USER_IDS = {78238238, 78378343, 98765431, 12345678}  # Your user IDs list
 
 router = Router(name=__name__)
 
 
 class RandomizedContent(LazyContent):
     contents: List[SerializeAsAny[BaseContent]]
```

### Comparing `aiogram_broadcaster-0.4.6/examples/mre.py` & `aiogram_broadcaster-0.4.7/examples/mre.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import logging
 import sys
 from typing import Any
 
 from aiogram import Bot, Dispatcher, Router
 from aiogram.types import Message
 
-from aiogram_broadcaster import Broadcaster
+from aiogram_broadcaster import Broadcaster, DefaultMailerSettings
 from aiogram_broadcaster.contents import MessageSendContent
-from aiogram_broadcaster.mailer import DefaultMailerSettings
-from aiogram_broadcaster.storage.file import FileMailerStorage
+from aiogram_broadcaster.storages.file import FileMailerStorage
 
 
-TOKEN = "1234:Abc"  # noqa: S105
+TOKEN = "1234:Abc"
 USER_IDS = {78238238, 78378343, 98765431, 12345678}  # Your user IDs list
 
 router = Router(name=__name__)
 
 
 @router.message()
 async def process_any_message(message: Message, broadcaster: Broadcaster) -> Any:
```

### Comparing `aiogram_broadcaster-0.4.6/examples/multibot.py` & `aiogram_broadcaster-0.4.7/examples/multibot.py`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.6/examples/placeholders.py` & `aiogram_broadcaster-0.4.7/examples/placeholders.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 from aiogram import Bot, Dispatcher, Router
 from aiogram.client.default import DefaultBotProperties
 from aiogram.enums import ParseMode
 from aiogram.filters import CommandStart
 from aiogram.types import Message
 
-from aiogram_broadcaster import Broadcaster, PlaceholderItem, PlaceholderRouter
+from aiogram_broadcaster import Broadcaster, PlaceholderItem, PlaceholderRegistry
 from aiogram_broadcaster.contents import TextContent
 
 
-TOKEN = "1234:Abc"  # noqa: S105
+TOKEN = "1234:Abc"
 USER_IDS = {78238238, 78378343, 98765431, 12345678}  # Your user IDs list
 
 router = Router(name=__name__)
-placeholder = PlaceholderRouter(name=__name__)
+placeholder = PlaceholderRegistry(name=__name__)
 
 
 @placeholder(key="mention")
 async def mention_placeholder(chat_id: int, bot: Bot) -> str:
     member = await bot.get_chat_member(chat_id=chat_id, user_id=chat_id)
     return member.user.mention_html(name=member.user.first_name)
 
@@ -60,15 +60,15 @@
 
     default = DefaultBotProperties(parse_mode=ParseMode.HTML)
     bot = Bot(token=TOKEN, default=default)
     dispatcher = Dispatcher()
     dispatcher.include_router(router)
 
     broadcaster = Broadcaster()
-    broadcaster.placeholder.include(placeholder)
+    broadcaster.placeholder.bind(placeholder)
     broadcaster.placeholder.register(TimePlaceholder())
     broadcaster.setup(dispatcher=dispatcher)
 
     dispatcher.run_polling(bot)
 
 
 if __name__ == "__main__":
```

### Comparing `aiogram_broadcaster-0.4.6/LICENSE` & `aiogram_broadcaster-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aiogram_broadcaster-0.4.6/README.md` & `aiogram_broadcaster-0.4.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # aiogram_broadcaster
 
-![GitHub License](https://img.shields.io/github/license/loRes228/aiogram_broadcaster?style=plastic&logo=github&link=https%3A%2F%2Fgithub.com%2FloRes228%2Faiogram_broadcaster%3Ftab%3DMIT-1-ov-file)
-![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/loRes228/aiogram_broadcaster/tests.yml?style=plastic&logo=github&link=https%3A%2F%2Fgithub.com%2FloRes228%2Faiogram_broadcaster%2Factions%2Fworkflows%2Ftests.yml)
-![GitHub last commit](https://img.shields.io/github/last-commit/loRes228/aiogram_broadcaster?style=plastic&logo=github)
-![Static Badge](https://img.shields.io/badge/python-3.8%2B-blue?style=plastic&logo=python&logoColor=blue&link=https%3A%2F%2Fwww.python.org%2Fdownloads%2F)
-![Static Badge](https://img.shields.io/badge/aiogram-3.4%2B-blue?style=plastic&logoColor=blue&link=https%3A%2F%2Fwww.python.org%2Fdownloads%2F)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/aiogram-broadcaster)
-![PyPI - Version](https://img.shields.io/pypi/v/aiogram-broadcaster)
+[![GitHub License](https://img.shields.io/github/license/loRes228/aiogram_broadcaster?style=plastic&logo=github&link=https%3A%2F%2Fgithub.com%2FloRes228%2Faiogram_broadcaster%3Ftab%3DMIT-1-ov-file)](https://github.com/loRes228/aiogram_broadcaster?tab=MIT-1-ov-file#MIT-1-ov-file)
+[![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/loRes228/aiogram_broadcaster/tests.yml?branch=main&style=plastic&logo=github)](https://github.com/loRes228/aiogram_broadcaster/actions)
+[![PyPI - Status](https://img.shields.io/pypi/status/aiogram-broadcaster?style=plastic&logo=pypi)](https://pypi.org/project/aiogram-broadcaster/)
+[![PyPI - Version](https://img.shields.io/pypi/v/aiogram-broadcaster?style=plastic&color=blue&logo=pypi)](https://pypi.org/project/aiogram-broadcaster/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/aiogram-broadcaster?style=plastic&color=green&logo=pypi)](https://pypi.org/project/aiogram-broadcaster/)
+[![PyPI - Python Version](https://img.shields.io/badge/python-3.8%2B-blue?style=plastic&logo=python)](https://www.python.org/downloads/)
+[![Static Badge](https://img.shields.io/badge/aiogram-3.6%2B-blue?style=plastic&logoColor=blue&link=https%3A%2F%2Fwww.python.org%2Fdownloads%2F&logo=pypi)](https://aiogram.dev)
 
 ### **aiogram_broadcaster** is lightweight aiogram-based library for broadcasting Telegram messages.
 
 ## Features
 
 * #### [Event system](https://github.com/loRes228/aiogram_broadcaster?tab=readme-ov-file#event-system-1)
 * #### [Placeholders](https://github.com/loRes228/aiogram_broadcaster?tab=readme-ov-file#placeholders) (variables in texts)
@@ -19,16 +19,24 @@
 * #### [Statistics](https://github.com/loRes228/aiogram_broadcaster?tab=readme-ov-file#statistic-mailerstatistic-instance-containing-statistics-about-the-mailers-performance)
 * #### [Statuses](https://github.com/loRes228/aiogram_broadcaster?tab=readme-ov-file#status-current-status-of-the-mailer-eg-started-stopped-completed)
 * #### Supports [multiple mailings](https://github.com/loRes228/aiogram_broadcaster?tab=readme-ov-file#mailer)
 * #### Supports [multibot](https://github.com/loRes228/aiogram_broadcaster?tab=readme-ov-file#multibot)
 
 ## Installation
 
+* #### From PyPI
+
+```commandline
+pip install -U aiogram-broadcaster
+```
+
+* #### From GitHub (_Development build_)
+
 ```commandline
-$ pip install aiogram-broadcaster
+pip install https://github.com/loRes228/aiogram_broadcaster/archive/refs/heads/dev.zip
 ```
 
 ## Creating a mailer and running broadcasting
 
 #### How to create a mailer and initiate broadcasting.
 
 #### Usage:
@@ -39,15 +47,15 @@
 from typing import Any
 
 from aiogram import Bot, Dispatcher, Router
 from aiogram.types import Message
 
 from aiogram_broadcaster import Broadcaster
 from aiogram_broadcaster.contents import MessageSendContent
-from aiogram_broadcaster.storage.file import FileMailerStorage
+from aiogram_broadcaster.storages.file import FileMailerStorage
 
 TOKEN = "1234:Abc"
 USER_IDS = {78238238, 78378343, 98765431, 12345678}
 
 router = Router(name=__name__)
 
 
@@ -152,23 +160,23 @@
 await mailer_group.run()
 ```
 
 ## Event system
 
 #### The event system empowers you to effectively manage events throughout the broadcast process.
 
-> **_NOTE:_** `EventRouter` supports chained nesting, similar to
-> aiogram [Router](https://docs.aiogram.dev/en/latest/dispatcher/router.html#nested-routers).
+> [!NOTE]
+> `EventRegistry` supports chained nesting, similar to aiogram [Router](https://docs.aiogram.dev/en/latest/dispatcher/router.html#nested-routers).
 
 #### Usage:
 
 ```python
-from aigoram_broadcaster import EventRouter
+from aigoram_broadcaster import EventRegistry
 
-event = EventRouter(name=__name__)
+event = EventRegistry(name=__name__)
 
 
 # Define event handlers
 
 
 @event.started()
 async def mailer_started() -> None:
@@ -214,42 +222,43 @@
     Exclusive parameters for this type of event:
         chat_id (int): ID of the chat.
         response (Any): Response from the sent mail.
     """
 
 
 # Include the event instance in the broadcaster
-broadcaster.event.include(event)
+broadcaster.event.bind(event)
 ```
 
 ## Placeholders
 
 #### Placeholders facilitate the insertion of dynamic content within texts, this feature allows for personalized messaging.
 
-> **_NOTE:_** `PlaceholderRouter` supports chained nesting, similar to
+> [!NOTE]
+> `PlaceholderRegistry` supports chained nesting, similar to
 > aiogram [Router](https://docs.aiogram.dev/en/latest/dispatcher/router.html#nested-routers).
 
 #### Usage:
 
 * #### Function-based
 
 ```python
-from aiogram_broadcaster import PlaceholderRouter
+from aiogram_broadcaster import PlaceholderRegistry
 
-placeholder = PlaceholderRouter(name=__name__)
+placeholder = PlaceholderRegistry(name=__name__)
 
 
 @placeholder(key="name")
 async def get_username(chat_id: int, bot: Bot) -> str:
     """Retrieves the username using the Telegram Bot API."""
     member = await bot.get_chat_member(chat_id=chat_id, user_id=chat_id)
     return member.user.first_name
 
 
-broadcaster.placeholder.include(placeholder)
+broadcaster.placeholder.bind(placeholder)
 ```
 
 * #### Class-based
 
 ```python
 from aiogram_broadcaster import PlaceholderItem
 
@@ -263,30 +272,30 @@
 broadcaster.placeholder.register(NamePlaceholder())
 ```
 
 * #### Other registration methods
 
 ```python
 placeholder["name"] = function
-placeholder.add(key="key", value="value")
-placeholder.attach({"key": "value"}, key="value")
+placeholder.add({"key": "value"}, name=function)
 ```
 
 ### And then
 
 ```python
 text_content = TextContent(text="Hello, $name!")
 photo_content = PhotoContent(photo=..., caption="Photo especially for $name!")
 ```
 
 ## Key-based content
 
 #### This module provides utilities to create personalized content targeted to specific users or groups based on their language preferences or geographical location, etc.
 
-> **_NOTE:_** If the default key is not specified, an error will be given if the key is not found.
+> [!NOTE]
+> If the default key is not specified, an error will be given if the key is not found.
 
 #### Usage:
 
 ```python
 from aiogram.exceptions import TelegramBadRequest
 
 from aiogram_broadcaster.contents import KeyBasedContent, TextContent
@@ -382,45 +391,46 @@
 await broadcaster.create_mailer(content=..., chats=..., stored_context={"key": "value"})
 ```
 
 * #### Event-to-event
 
 ```python
 @event.completed()
-async def transfer_content(mailer: Mailer) -> Dict[str, Any]:
-    return {"mailer_content": mailer.content}
+async def transfer_content() -> Dict[str, Any]:
+    return {"my_data": 1}
 
 
 @event.completed()
-async def mailer_completed(mailer_content: BaseContent) -> None:
-    print(mailer_content)
+async def mailer_completed(my_data: 1) -> None:
+    print(my_data)
 ```
 
 ## Storages
 
 #### Storage allow you to save mailer states to external storage.
 
-* #### [FileMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storage/file.py) Saves the mailers to a file.
-* #### [MongoDBMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storage/mongodb.py) Saves the mailers to a MongoDB.
-* #### [RedisMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storage/redis.py) Saves the mailers to a Redis.
-* #### [SQLAlchemyMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storage/sqlalchemy.py) Saves the mailers using SQLAlchemy.
+* #### [BaseMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storages/base.py) Abstract class of storage.
+* #### [FileMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storages/file.py) Saves the mailers to a file.
+* #### [MongoDBMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storages/mongodb.py) Saves the mailers to a MongoDB.
+* #### [RedisMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storages/redis.py) Saves the mailers to a Redis.
+* #### [SQLAlchemyMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storages/sqlalchemy.py) Saves the mailers using SQLAlchemy.
 
 #### Usage:
 
 ```python
 from aiogram_broadcaster import Broadcaster
-from aiogram_broadcaster.storage.redis import RedisMailerStorage
+from aiogram_broadcaster.storages.redis import RedisMailerStorage
 
-# from aiogram_broadcaster.storage.file import FileMailerStorage
-# from aiogram_broadcaster.storage.mongodb import MongoDBMailerStorage
-# from aiogram_broadcaster.storage.sqlalchemy import SQLAlchemyMailerStorage
-
-# storage = FileMailerStorage()
-# storage = MongoDBMailerStorage.from_url(url="mongodb://localhost:27017")
-# storage = SQLAlchemyMailerStorage.from_url(url="sqlite+aiosqlite:///database.db")
+# from aiogram_broadcaster.storages.file import FileMailerStorage
+# from aiogram_broadcaster.storages.mongodb import MongoDBMailerStorage
+# from aiogram_broadcaster.storages.sqlalchemy import SQLAlchemyMailerStorage
+
+# storages = FileMailerStorage()
+# storages = MongoDBMailerStorage.from_url(url="mongodb://localhost:27017")
+# storages = SQLAlchemyMailerStorage.from_url(url="sqlite+aiosqlite:///database.db")
 
 storage = RedisMailerStorage.from_url(url="redis://localhost:6379")
 broadcaster = Broadcaster(storage=storage)
 ```
 
 ## Default mailer settings
```

### Comparing `aiogram_broadcaster-0.4.6/PKG-INFO` & `aiogram_broadcaster-0.4.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,82 @@
 Metadata-Version: 2.3
 Name: aiogram_broadcaster
-Version: 0.4.6
+Version: 0.4.7
 Summary: A lightweight aiogram-based library for broadcasting Telegram messages.
-Project-URL: Source, https://github.com/loRes228/aiogram_broadcaster
+Project-URL: Repository, https://github.com/loRes228/aiogram_broadcaster.git
+Project-URL: Issues, https://github.com/loRes228/aiogram_broadcaster/issues
 Author: LORES
-License-Expression: MIT
+Maintainer: LORES
+License: MIT License
+        
+        Copyright (c) 2024 LORES
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
 License-File: LICENSE
 Keywords: api,asyncio,boadcasting,bot,broadcast,broadcaster,framework,mailing,mailing-system,telegram,wrapper
+Classifier: Development Status :: 3 - Alpha
+Classifier: Framework :: AsyncIO
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
 Requires-Dist: aiogram>=3.6.0
 Provides-Extra: dev
-Requires-Dist: mypy>=1.9.0; extra == 'dev'
-Requires-Dist: ruff>=0.3.2; extra == 'dev'
+Requires-Dist: mypy>=1.10.0; extra == 'dev'
+Requires-Dist: ruff>=0.4.0; extra == 'dev'
 Requires-Dist: types-aiofiles>=23.2.0; extra == 'dev'
 Provides-Extra: mongo
 Requires-Dist: motor>=3.0.0; extra == 'mongo'
 Provides-Extra: redis
 Requires-Dist: redis[hiredis]>=5.0.0; extra == 'redis'
 Provides-Extra: sqlalchemy
 Requires-Dist: sqlalchemy>=2.0.0; extra == 'sqlalchemy'
+Provides-Extra: test
+Requires-Dist: pytest-asyncio>=0.23.0; extra == 'test'
+Requires-Dist: pytest-cov>=5.0.0; extra == 'test'
+Requires-Dist: pytest-html>=4.1.0; extra == 'test'
+Requires-Dist: pytest-lazy-fixtures>=1.0.0; extra == 'test'
+Requires-Dist: pytest>=8.2.0; extra == 'test'
 Description-Content-Type: text/markdown
 
 # aiogram_broadcaster
 
-![GitHub License](https://img.shields.io/github/license/loRes228/aiogram_broadcaster?style=plastic&logo=github&link=https%3A%2F%2Fgithub.com%2FloRes228%2Faiogram_broadcaster%3Ftab%3DMIT-1-ov-file)
-![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/loRes228/aiogram_broadcaster/tests.yml?style=plastic&logo=github&link=https%3A%2F%2Fgithub.com%2FloRes228%2Faiogram_broadcaster%2Factions%2Fworkflows%2Ftests.yml)
-![GitHub last commit](https://img.shields.io/github/last-commit/loRes228/aiogram_broadcaster?style=plastic&logo=github)
-![Static Badge](https://img.shields.io/badge/python-3.8%2B-blue?style=plastic&logo=python&logoColor=blue&link=https%3A%2F%2Fwww.python.org%2Fdownloads%2F)
-![Static Badge](https://img.shields.io/badge/aiogram-3.4%2B-blue?style=plastic&logoColor=blue&link=https%3A%2F%2Fwww.python.org%2Fdownloads%2F)
-![PyPI - Downloads](https://img.shields.io/pypi/dm/aiogram-broadcaster)
-![PyPI - Version](https://img.shields.io/pypi/v/aiogram-broadcaster)
+[![GitHub License](https://img.shields.io/github/license/loRes228/aiogram_broadcaster?style=plastic&logo=github&link=https%3A%2F%2Fgithub.com%2FloRes228%2Faiogram_broadcaster%3Ftab%3DMIT-1-ov-file)](https://github.com/loRes228/aiogram_broadcaster?tab=MIT-1-ov-file#MIT-1-ov-file)
+[![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/loRes228/aiogram_broadcaster/tests.yml?branch=main&style=plastic&logo=github)](https://github.com/loRes228/aiogram_broadcaster/actions)
+[![PyPI - Status](https://img.shields.io/pypi/status/aiogram-broadcaster?style=plastic&logo=pypi)](https://pypi.org/project/aiogram-broadcaster/)
+[![PyPI - Version](https://img.shields.io/pypi/v/aiogram-broadcaster?style=plastic&color=blue&logo=pypi)](https://pypi.org/project/aiogram-broadcaster/)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/aiogram-broadcaster?style=plastic&color=green&logo=pypi)](https://pypi.org/project/aiogram-broadcaster/)
+[![PyPI - Python Version](https://img.shields.io/badge/python-3.8%2B-blue?style=plastic&logo=python)](https://www.python.org/downloads/)
+[![Static Badge](https://img.shields.io/badge/aiogram-3.6%2B-blue?style=plastic&logoColor=blue&link=https%3A%2F%2Fwww.python.org%2Fdownloads%2F&logo=pypi)](https://aiogram.dev)
 
 ### **aiogram_broadcaster** is lightweight aiogram-based library for broadcasting Telegram messages.
 
 ## Features
 
 * #### [Event system](https://github.com/loRes228/aiogram_broadcaster?tab=readme-ov-file#event-system-1)
 * #### [Placeholders](https://github.com/loRes228/aiogram_broadcaster?tab=readme-ov-file#placeholders) (variables in texts)
@@ -53,16 +85,24 @@
 * #### [Statistics](https://github.com/loRes228/aiogram_broadcaster?tab=readme-ov-file#statistic-mailerstatistic-instance-containing-statistics-about-the-mailers-performance)
 * #### [Statuses](https://github.com/loRes228/aiogram_broadcaster?tab=readme-ov-file#status-current-status-of-the-mailer-eg-started-stopped-completed)
 * #### Supports [multiple mailings](https://github.com/loRes228/aiogram_broadcaster?tab=readme-ov-file#mailer)
 * #### Supports [multibot](https://github.com/loRes228/aiogram_broadcaster?tab=readme-ov-file#multibot)
 
 ## Installation
 
+* #### From PyPI
+
+```commandline
+pip install -U aiogram-broadcaster
+```
+
+* #### From GitHub (_Development build_)
+
 ```commandline
-$ pip install aiogram-broadcaster
+pip install https://github.com/loRes228/aiogram_broadcaster/archive/refs/heads/dev.zip
 ```
 
 ## Creating a mailer and running broadcasting
 
 #### How to create a mailer and initiate broadcasting.
 
 #### Usage:
@@ -73,15 +113,15 @@
 from typing import Any
 
 from aiogram import Bot, Dispatcher, Router
 from aiogram.types import Message
 
 from aiogram_broadcaster import Broadcaster
 from aiogram_broadcaster.contents import MessageSendContent
-from aiogram_broadcaster.storage.file import FileMailerStorage
+from aiogram_broadcaster.storages.file import FileMailerStorage
 
 TOKEN = "1234:Abc"
 USER_IDS = {78238238, 78378343, 98765431, 12345678}
 
 router = Router(name=__name__)
 
 
@@ -186,23 +226,23 @@
 await mailer_group.run()
 ```
 
 ## Event system
 
 #### The event system empowers you to effectively manage events throughout the broadcast process.
 
-> **_NOTE:_** `EventRouter` supports chained nesting, similar to
-> aiogram [Router](https://docs.aiogram.dev/en/latest/dispatcher/router.html#nested-routers).
+> [!NOTE]
+> `EventRegistry` supports chained nesting, similar to aiogram [Router](https://docs.aiogram.dev/en/latest/dispatcher/router.html#nested-routers).
 
 #### Usage:
 
 ```python
-from aigoram_broadcaster import EventRouter
+from aigoram_broadcaster import EventRegistry
 
-event = EventRouter(name=__name__)
+event = EventRegistry(name=__name__)
 
 
 # Define event handlers
 
 
 @event.started()
 async def mailer_started() -> None:
@@ -248,42 +288,43 @@
     Exclusive parameters for this type of event:
         chat_id (int): ID of the chat.
         response (Any): Response from the sent mail.
     """
 
 
 # Include the event instance in the broadcaster
-broadcaster.event.include(event)
+broadcaster.event.bind(event)
 ```
 
 ## Placeholders
 
 #### Placeholders facilitate the insertion of dynamic content within texts, this feature allows for personalized messaging.
 
-> **_NOTE:_** `PlaceholderRouter` supports chained nesting, similar to
+> [!NOTE]
+> `PlaceholderRegistry` supports chained nesting, similar to
 > aiogram [Router](https://docs.aiogram.dev/en/latest/dispatcher/router.html#nested-routers).
 
 #### Usage:
 
 * #### Function-based
 
 ```python
-from aiogram_broadcaster import PlaceholderRouter
+from aiogram_broadcaster import PlaceholderRegistry
 
-placeholder = PlaceholderRouter(name=__name__)
+placeholder = PlaceholderRegistry(name=__name__)
 
 
 @placeholder(key="name")
 async def get_username(chat_id: int, bot: Bot) -> str:
     """Retrieves the username using the Telegram Bot API."""
     member = await bot.get_chat_member(chat_id=chat_id, user_id=chat_id)
     return member.user.first_name
 
 
-broadcaster.placeholder.include(placeholder)
+broadcaster.placeholder.bind(placeholder)
 ```
 
 * #### Class-based
 
 ```python
 from aiogram_broadcaster import PlaceholderItem
 
@@ -297,30 +338,30 @@
 broadcaster.placeholder.register(NamePlaceholder())
 ```
 
 * #### Other registration methods
 
 ```python
 placeholder["name"] = function
-placeholder.add(key="key", value="value")
-placeholder.attach({"key": "value"}, key="value")
+placeholder.add({"key": "value"}, name=function)
 ```
 
 ### And then
 
 ```python
 text_content = TextContent(text="Hello, $name!")
 photo_content = PhotoContent(photo=..., caption="Photo especially for $name!")
 ```
 
 ## Key-based content
 
 #### This module provides utilities to create personalized content targeted to specific users or groups based on their language preferences or geographical location, etc.
 
-> **_NOTE:_** If the default key is not specified, an error will be given if the key is not found.
+> [!NOTE]
+> If the default key is not specified, an error will be given if the key is not found.
 
 #### Usage:
 
 ```python
 from aiogram.exceptions import TelegramBadRequest
 
 from aiogram_broadcaster.contents import KeyBasedContent, TextContent
@@ -416,45 +457,46 @@
 await broadcaster.create_mailer(content=..., chats=..., stored_context={"key": "value"})
 ```
 
 * #### Event-to-event
 
 ```python
 @event.completed()
-async def transfer_content(mailer: Mailer) -> Dict[str, Any]:
-    return {"mailer_content": mailer.content}
+async def transfer_content() -> Dict[str, Any]:
+    return {"my_data": 1}
 
 
 @event.completed()
-async def mailer_completed(mailer_content: BaseContent) -> None:
-    print(mailer_content)
+async def mailer_completed(my_data: 1) -> None:
+    print(my_data)
 ```
 
 ## Storages
 
 #### Storage allow you to save mailer states to external storage.
 
-* #### [FileMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storage/file.py) Saves the mailers to a file.
-* #### [MongoDBMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storage/mongodb.py) Saves the mailers to a MongoDB.
-* #### [RedisMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storage/redis.py) Saves the mailers to a Redis.
-* #### [SQLAlchemyMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storage/sqlalchemy.py) Saves the mailers using SQLAlchemy.
+* #### [BaseMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storages/base.py) Abstract class of storage.
+* #### [FileMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storages/file.py) Saves the mailers to a file.
+* #### [MongoDBMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storages/mongodb.py) Saves the mailers to a MongoDB.
+* #### [RedisMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storages/redis.py) Saves the mailers to a Redis.
+* #### [SQLAlchemyMailerStorage](https://github.com/loRes228/aiogram_broadcaster/blob/main/aiogram_broadcaster/storages/sqlalchemy.py) Saves the mailers using SQLAlchemy.
 
 #### Usage:
 
 ```python
 from aiogram_broadcaster import Broadcaster
-from aiogram_broadcaster.storage.redis import RedisMailerStorage
+from aiogram_broadcaster.storages.redis import RedisMailerStorage
 
-# from aiogram_broadcaster.storage.file import FileMailerStorage
-# from aiogram_broadcaster.storage.mongodb import MongoDBMailerStorage
-# from aiogram_broadcaster.storage.sqlalchemy import SQLAlchemyMailerStorage
-
-# storage = FileMailerStorage()
-# storage = MongoDBMailerStorage.from_url(url="mongodb://localhost:27017")
-# storage = SQLAlchemyMailerStorage.from_url(url="sqlite+aiosqlite:///database.db")
+# from aiogram_broadcaster.storages.file import FileMailerStorage
+# from aiogram_broadcaster.storages.mongodb import MongoDBMailerStorage
+# from aiogram_broadcaster.storages.sqlalchemy import SQLAlchemyMailerStorage
+
+# storages = FileMailerStorage()
+# storages = MongoDBMailerStorage.from_url(url="mongodb://localhost:27017")
+# storages = SQLAlchemyMailerStorage.from_url(url="sqlite+aiosqlite:///database.db")
 
 storage = RedisMailerStorage.from_url(url="redis://localhost:6379")
 broadcaster = Broadcaster(storage=storage)
 ```
 
 ## Default mailer settings
```

