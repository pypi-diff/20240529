# Comparing `tmp/satsim-0.18.0.tar.gz` & `tmp/satsim-0.19.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "satsim-0.18.0.tar", last modified: Sat Mar 23 07:34:07 2024, max compression
+gzip compressed data, was "satsim-0.19.0.tar", last modified: Wed May 29 08:15:08 2024, max compression
```

## Comparing `satsim-0.18.0.tar` & `satsim-0.19.0.tar`

### file list

```diff
@@ -1,236 +1,239 @@
-drwxrwxrwx   0     1000     1000        0 2024-03-23 07:34:07.090011 satsim-0.18.0/
--rwxrwxrwx   0     1000     1000      170 2023-07-17 23:45:22.000000 satsim-0.18.0/AUTHORS.rst
--rwxrwxrwx   0     1000     1000     3255 2023-07-17 23:45:22.000000 satsim-0.18.0/CONTRIBUTING.rst
--rwxrwxrwx   0     1000     1000     8147 2024-03-21 00:37:03.000000 satsim-0.18.0/HISTORY.md
--rwxrwxrwx   0     1000     1000      291 2023-07-17 23:45:22.000000 satsim-0.18.0/MANIFEST.in
--rwxrwxrwx   0     1000     1000     9773 2024-03-23 07:34:07.091517 satsim-0.18.0/PKG-INFO
--rwxrwxrwx   0     1000     1000     1049 2023-07-17 23:45:22.000000 satsim-0.18.0/README.md
-drwxrwxrwx   0     1000     1000        0 2024-03-23 07:34:03.895568 satsim-0.18.0/docs/
--rwxrwxrwx   0     1000     1000      608 2023-07-17 23:45:22.000000 satsim-0.18.0/docs/Makefile
-drwxrwxrwx   0     1000     1000        0 2024-03-23 07:34:03.665871 satsim-0.18.0/docs/_build/
-drwxrwxrwx   0     1000     1000        0 2024-03-23 07:34:04.085369 satsim-0.18.0/docs/_build/html/
-drwxrwxrwx   0     1000     1000        0 2024-03-23 07:34:04.324259 satsim-0.18.0/docs/_build/html/_static/
--rwxrwxrwx   0     1000     1000    14813 2024-03-23 07:33:56.000000 satsim-0.18.0/docs/_build/html/_static/basic.css
-drwxrwxrwx   0     1000     1000        0 2024-03-23 07:34:04.370852 satsim-0.18.0/docs/_build/html/_static/css/
--rwxrwxrwx   0     1000     1000     3229 2024-03-23 07:30:24.000000 satsim-0.18.0/docs/_build/html/_static/css/badge_only.css
-drwxrwxrwx   0     1000     1000        0 2024-03-23 07:34:04.525009 satsim-0.18.0/docs/_build/html/_static/css/fonts/
--rwxrwxrwx   0     1000     1000   165742 2024-03-23 07:30:24.000000 satsim-0.18.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
--rwxrwxrwx   0     1000     1000   444379 2024-03-23 07:30:24.000000 satsim-0.18.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rwxrwxrwx   0     1000     1000   165548 2024-03-23 07:30:24.000000 satsim-0.18.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
--rwxrwxrwx   0     1000     1000    98024 2024-03-23 07:30:24.000000 satsim-0.18.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
--rwxrwxrwx   0     1000     1000    77160 2024-03-23 07:30:24.000000 satsim-0.18.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
--rwxrwxrwx   0     1000     1000   135235 2024-03-23 07:30:24.000000 satsim-0.18.0/docs/_build/html/_static/css/theme.css
--rwxrwxrwx   0     1000     1000     4472 2024-03-23 07:30:23.000000 satsim-0.18.0/docs/_build/html/_static/doctools.js
--rwxrwxrwx   0     1000     1000      421 2024-03-23 07:33:56.000000 satsim-0.18.0/docs/_build/html/_static/documentation_options.js
--rwxrwxrwx   0     1000     1000      286 2024-03-23 07:30:23.000000 satsim-0.18.0/docs/_build/html/_static/file.png
-drwxrwxrwx   0     1000     1000        0 2024-03-23 07:34:04.619439 satsim-0.18.0/docs/_build/html/_static/js/
--rwxrwxrwx   0     1000     1000      934 2024-03-23 07:30:24.000000 satsim-0.18.0/docs/_build/html/_static/js/badge_only.js
--rwxrwxrwx   0     1000     1000     4370 2024-03-23 07:30:24.000000 satsim-0.18.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js
--rwxrwxrwx   0     1000     1000     2734 2024-03-23 07:30:24.000000 satsim-0.18.0/docs/_build/html/_static/js/html5shiv.min.js
--rwxrwxrwx   0     1000     1000     5023 2024-03-23 07:30:24.000000 satsim-0.18.0/docs/_build/html/_static/js/theme.js
--rwxrwxrwx   0     1000     1000     4758 2024-03-23 07:33:56.000000 satsim-0.18.0/docs/_build/html/_static/language_data.js
--rwxrwxrwx   0     1000     1000       90 2024-03-23 07:30:23.000000 satsim-0.18.0/docs/_build/html/_static/minus.png
--rwxrwxrwx   0     1000     1000       90 2024-03-23 07:30:23.000000 satsim-0.18.0/docs/_build/html/_static/plus.png
--rwxrwxrwx   0     1000     1000     4929 2024-03-23 07:33:56.000000 satsim-0.18.0/docs/_build/html/_static/pygments.css
--rwxrwxrwx   0     1000     1000    18215 2024-03-23 07:30:23.000000 satsim-0.18.0/docs/_build/html/_static/searchtools.js
--rwxrwxrwx   0     1000     1000     4712 2024-03-23 07:30:23.000000 satsim-0.18.0/docs/_build/html/_static/sphinx_highlight.js
-drwxrwxrwx   0     1000     1000        0 2024-03-23 07:34:04.931497 satsim-0.18.0/docs/_build/html/api/
--rwxrwxrwx   0     1000     1000    10225 2024-03-23 07:33:53.000000 satsim-0.18.0/docs/_build/html/api/satsim.dataset.html
--rwxrwxrwx   0     1000     1000    10160 2024-03-23 07:33:53.000000 satsim-0.18.0/docs/_build/html/api/satsim.generator.html
--rwxrwxrwx   0     1000     1000    59266 2024-03-23 07:33:54.000000 satsim-0.18.0/docs/_build/html/api/satsim.generator.obs.html
--rwxrwxrwx   0     1000     1000   113765 2024-03-23 07:33:54.000000 satsim-0.18.0/docs/_build/html/api/satsim.geometry.html
--rwxrwxrwx   0     1000     1000   162448 2024-03-23 07:33:53.000000 satsim-0.18.0/docs/_build/html/api/satsim.html
--rwxrwxrwx   0     1000     1000    91803 2024-03-23 07:33:54.000000 satsim-0.18.0/docs/_build/html/api/satsim.image.html
--rwxrwxrwx   0     1000     1000    38820 2024-03-23 07:33:54.000000 satsim-0.18.0/docs/_build/html/api/satsim.io.html
--rwxrwxrwx   0     1000     1000    33975 2024-03-23 07:33:54.000000 satsim-0.18.0/docs/_build/html/api/satsim.math.html
--rwxrwxrwx   0     1000     1000    14651 2024-03-23 07:33:54.000000 satsim-0.18.0/docs/_build/html/api/satsim.pipeline.html
--rwxrwxrwx   0     1000     1000    12697 2024-03-23 07:33:54.000000 satsim-0.18.0/docs/_build/html/api/satsim.tfa.html
--rwxrwxrwx   0     1000     1000   156980 2024-03-23 07:33:55.000000 satsim-0.18.0/docs/_build/html/api/satsim.tfa.image.html
--rwxrwxrwx   0     1000     1000    11801 2024-03-23 07:33:55.000000 satsim-0.18.0/docs/_build/html/api/satsim.tfa.utils.html
--rwxrwxrwx   0     1000     1000    19461 2024-03-23 07:33:55.000000 satsim-0.18.0/docs/_build/html/api/satsim.time.html
--rwxrwxrwx   0     1000     1000    24971 2024-03-23 07:33:55.000000 satsim-0.18.0/docs/_build/html/api/satsim.util.html
--rwxrwxrwx   0     1000     1000   404550 2024-03-23 07:33:56.000000 satsim-0.18.0/docs/_build/html/api/satsim.vecmath.html
--rwxrwxrwx   0     1000     1000   129595 2024-03-23 07:33:53.000000 satsim-0.18.0/docs/_build/html/api.html
--rwxrwxrwx   0     1000     1000     5491 2024-03-23 07:33:56.000000 satsim-0.18.0/docs/_build/html/authors.html
--rwxrwxrwx   0     1000     1000    13939 2024-03-23 07:33:56.000000 satsim-0.18.0/docs/_build/html/contributing.html
--rwxrwxrwx   0     1000     1000   101500 2024-03-23 07:33:56.000000 satsim-0.18.0/docs/_build/html/genindex.html
--rwxrwxrwx   0     1000     1000    20568 2024-03-23 07:33:56.000000 satsim-0.18.0/docs/_build/html/history.html
--rwxrwxrwx   0     1000     1000    10004 2024-03-23 07:33:56.000000 satsim-0.18.0/docs/_build/html/index.html
--rwxrwxrwx   0     1000     1000     7949 2024-03-23 07:33:56.000000 satsim-0.18.0/docs/_build/html/installation.html
--rwxrwxrwx   0     1000     1000    19362 2024-03-23 07:33:56.000000 satsim-0.18.0/docs/_build/html/py-modindex.html
--rwxrwxrwx   0     1000     1000     4196 2024-03-23 07:33:56.000000 satsim-0.18.0/docs/_build/html/search.html
--rwxrwxrwx   0     1000     1000   132246 2024-03-23 07:33:56.000000 satsim-0.18.0/docs/_build/html/searchindex.js
--rwxrwxrwx   0     1000     1000    37538 2024-03-23 07:33:56.000000 satsim-0.18.0/docs/_build/html/usage.html
-drwxrwxrwx   0     1000     1000        0 2024-03-23 07:34:05.151644 satsim-0.18.0/docs/api/
--rwxrwxrwx   0     1000     1000      310 2024-03-23 07:33:40.000000 satsim-0.18.0/docs/api/satsim.dataset.rst
--rwxrwxrwx   0     1000     1000     1002 2024-03-23 07:33:40.000000 satsim-0.18.0/docs/api/satsim.generator.obs.rst
--rwxrwxrwx   0     1000     1000      218 2024-03-23 07:33:40.000000 satsim-0.18.0/docs/api/satsim.generator.rst
--rwxrwxrwx   0     1000     1000     2042 2024-03-23 07:33:40.000000 satsim-0.18.0/docs/api/satsim.geometry.rst
--rwxrwxrwx   0     1000     1000     1004 2024-03-23 07:33:40.000000 satsim-0.18.0/docs/api/satsim.image.rst
--rwxrwxrwx   0     1000     1000      673 2024-03-23 07:33:40.000000 satsim-0.18.0/docs/api/satsim.io.rst
--rwxrwxrwx   0     1000     1000     1138 2024-03-23 07:33:40.000000 satsim-0.18.0/docs/api/satsim.math.rst
--rwxrwxrwx   0     1000     1000      135 2024-03-23 07:33:40.000000 satsim-0.18.0/docs/api/satsim.pipeline.rst
--rwxrwxrwx   0     1000     1000      744 2024-03-23 07:33:40.000000 satsim-0.18.0/docs/api/satsim.rst
--rwxrwxrwx   0     1000     1000      678 2024-03-23 07:33:40.000000 satsim-0.18.0/docs/api/satsim.tfa.image.rst
--rwxrwxrwx   0     1000     1000      216 2024-03-23 07:33:40.000000 satsim-0.18.0/docs/api/satsim.tfa.rst
--rwxrwxrwx   0     1000     1000      488 2024-03-23 07:33:40.000000 satsim-0.18.0/docs/api/satsim.tfa.utils.rst
--rwxrwxrwx   0     1000     1000      123 2024-03-23 07:33:40.000000 satsim-0.18.0/docs/api/satsim.time.rst
--rwxrwxrwx   0     1000     1000      572 2024-03-23 07:33:40.000000 satsim-0.18.0/docs/api/satsim.util.rst
--rwxrwxrwx   0     1000     1000     1276 2024-03-23 07:33:40.000000 satsim-0.18.0/docs/api/satsim.vecmath.rst
--rwxrwxrwx   0     1000     1000      136 2023-07-17 23:45:22.000000 satsim-0.18.0/docs/api.rst
--rwxrwxrwx   0     1000     1000       28 2023-07-17 23:45:22.000000 satsim-0.18.0/docs/authors.rst
--rwxrwxrwx   0     1000     1000     4906 2024-03-21 01:07:55.000000 satsim-0.18.0/docs/conf.py
--rwxrwxrwx   0     1000     1000       33 2023-07-17 23:45:22.000000 satsim-0.18.0/docs/contributing.rst
--rwxrwxrwx   0     1000     1000       27 2023-07-17 23:45:22.000000 satsim-0.18.0/docs/history.rst
--rwxrwxrwx   0     1000     1000      265 2023-07-17 23:45:22.000000 satsim-0.18.0/docs/index.rst
--rwxrwxrwx   0     1000     1000     1523 2024-03-21 03:20:21.000000 satsim-0.18.0/docs/installation.rst
--rwxrwxrwx   0     1000     1000      768 2023-07-17 23:45:22.000000 satsim-0.18.0/docs/make.bat
--rwxrwxrwx   0     1000     1000    11419 2023-07-17 23:45:22.000000 satsim-0.18.0/docs/usage.rst
-drwxrwxrwx   0     1000     1000        0 2024-03-23 07:34:05.197919 satsim-0.18.0/satsim/
--rwxrwxrwx   0     1000     1000      264 2024-01-03 01:22:11.000000 satsim-0.18.0/satsim/__init__.py
--rwxrwxrwx   0     1000     1000     4131 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/cli.py
--rwxrwxrwx   0     1000     1000    20530 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/config.py
-drwxrwxrwx   0     1000     1000        0 2024-03-23 07:34:05.351546 satsim-0.18.0/satsim/dataset/
--rwxrwxrwx   0     1000     1000        0 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/dataset/__init__.py
--rwxrwxrwx   0     1000     1000     3507 2024-03-14 03:04:05.000000 satsim-0.18.0/satsim/dataset/augment.py
-drwxrwxrwx   0     1000     1000        0 2024-03-23 07:34:05.372126 satsim-0.18.0/satsim/generator/
--rwxrwxrwx   0     1000     1000        0 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/generator/__init__.py
-drwxrwxrwx   0     1000     1000        0 2024-03-23 07:34:05.542149 satsim-0.18.0/satsim/generator/obs/
--rwxrwxrwx   0     1000     1000        0 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/generator/obs/__init__.py
--rwxrwxrwx   0     1000     1000    12937 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/generator/obs/breakup.py
--rwxrwxrwx   0     1000     1000     2330 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/generator/obs/cso.py
--rwxrwxrwx   0     1000     1000     6239 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/generator/obs/geometry.py
--rwxrwxrwx   0     1000     1000     1248 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/generator/obs/io.py
--rwxrwxrwx   0     1000     1000     3703 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/generator/obs/rpo.py
-drwxrwxrwx   0     1000     1000        0 2024-03-23 07:34:05.830206 satsim-0.18.0/satsim/geometry/
--rwxrwxrwx   0     1000     1000       66 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/geometry/__init__.py
--rwxrwxrwx   0     1000     1000    22041 2024-03-20 18:13:52.000000 satsim-0.18.0/satsim/geometry/astrometric.py
--rwxrwxrwx   0     1000     1000     2386 2024-03-21 00:18:33.000000 satsim-0.18.0/satsim/geometry/csvsc.py
--rwxrwxrwx   0     1000     1000     5268 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/geometry/draw.py
--rwxrwxrwx   0     1000     1000     3404 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/geometry/ephemeris.py
--rwxrwxrwx   0     1000     1000     2966 2023-07-20 03:20:44.000000 satsim-0.18.0/satsim/geometry/observation.py
--rwxrwxrwx   0     1000     1000     1672 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/geometry/random.py
--rwxrwxrwx   0     1000     1000     1150 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/geometry/sgp4.py
--rwxrwxrwx   0     1000     1000      699 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/geometry/sprite.py
--rwxrwxrwx   0     1000     1000    11541 2024-03-21 00:18:00.000000 satsim-0.18.0/satsim/geometry/sstr7.py
--rwxrwxrwx   0     1000     1000     4340 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/geometry/transform.py
--rwxrwxrwx   0     1000     1000     4619 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/geometry/twobody.py
--rwxrwxrwx   0     1000     1000     3787 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/geometry/wcs.py
-drwxrwxrwx   0     1000     1000        0 2024-03-23 07:34:05.924254 satsim-0.18.0/satsim/image/
--rwxrwxrwx   0     1000     1000       58 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/image/__init__.py
--rwxrwxrwx   0     1000     1000     9786 2023-12-15 00:51:47.000000 satsim-0.18.0/satsim/image/augment.py
--rwxrwxrwx   0     1000     1000    16147 2024-03-20 23:10:59.000000 satsim-0.18.0/satsim/image/fpa.py
--rwxrwxrwx   0     1000     1000     5359 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/image/model.py
--rwxrwxrwx   0     1000     1000     2895 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/image/noise.py
--rwxrwxrwx   0     1000     1000     6836 2024-03-14 00:31:04.000000 satsim-0.18.0/satsim/image/psf.py
--rwxrwxrwx   0     1000     1000    10541 2024-03-23 05:16:18.000000 satsim-0.18.0/satsim/image/render.py
-drwxrwxrwx   0     1000     1000        0 2024-03-23 07:34:05.998300 satsim-0.18.0/satsim/io/
--rwxrwxrwx   0     1000     1000        0 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/io/__init__.py
--rwxrwxrwx   0     1000     1000    15817 2023-07-20 03:20:44.000000 satsim-0.18.0/satsim/io/czml.py
--rwxrwxrwx   0     1000     1000     4319 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/io/fits.py
--rwxrwxrwx   0     1000     1000     2632 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/io/image.py
--rwxrwxrwx   0     1000     1000    14273 2024-03-21 00:16:23.000000 satsim-0.18.0/satsim/io/satnet.py
-drwxrwxrwx   0     1000     1000        0 2024-03-23 07:34:06.110421 satsim-0.18.0/satsim/math/
--rwxrwxrwx   0     1000     1000       81 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/math/__init__.py
--rwxrwxrwx   0     1000     1000     2350 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/math/angle.py
--rwxrwxrwx   0     1000     1000      937 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/math/const.py
--rwxrwxrwx   0     1000     1000      951 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/math/conv.py
--rwxrwxrwx   0     1000     1000     5551 2024-03-14 00:29:14.000000 satsim-0.18.0/satsim/math/fft.py
--rwxrwxrwx   0     1000     1000     2726 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/math/interpolate.py
--rwxrwxrwx   0     1000     1000     3096 2023-07-20 03:20:44.000000 satsim-0.18.0/satsim/math/random.py
--rwxrwxrwx   0     1000     1000      590 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/math/stats.py
-drwxrwxrwx   0     1000     1000        0 2024-03-23 07:34:06.124110 satsim-0.18.0/satsim/pipeline/
--rwxrwxrwx   0     1000     1000     1087 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/pipeline/__init__.py
--rwxrwxrwx   0     1000     1000    54894 2024-03-23 07:27:57.000000 satsim-0.18.0/satsim/satsim.py
-drwxrwxrwx   0     1000     1000        0 2024-03-23 07:34:06.137432 satsim-0.18.0/satsim/tfa/
--rwxrwxrwx   0     1000     1000       63 2023-12-15 00:51:47.000000 satsim-0.18.0/satsim/tfa/__init__.py
-drwxrwxrwx   0     1000     1000        0 2024-03-23 07:34:06.201717 satsim-0.18.0/satsim/tfa/image/
--rwxrwxrwx   0     1000     1000      573 2023-12-15 00:51:47.000000 satsim-0.18.0/satsim/tfa/image/__init__.py
--rwxrwxrwx   0     1000     1000    14584 2023-12-15 00:51:47.000000 satsim-0.18.0/satsim/tfa/image/transform_ops.py
--rwxrwxrwx   0     1000     1000     5295 2023-12-15 00:51:47.000000 satsim-0.18.0/satsim/tfa/image/translate_ops.py
--rwxrwxrwx   0     1000     1000     4266 2024-03-20 22:49:03.000000 satsim-0.18.0/satsim/tfa/image/utils.py
-drwxrwxrwx   0     1000     1000        0 2024-03-23 07:34:06.248482 satsim-0.18.0/satsim/tfa/utils/
--rwxrwxrwx   0     1000     1000        0 2023-12-15 00:51:47.000000 satsim-0.18.0/satsim/tfa/utils/__init__.py
--rwxrwxrwx   0     1000     1000     1730 2024-03-20 22:51:54.000000 satsim-0.18.0/satsim/tfa/utils/test_utils.py
--rwxrwxrwx   0     1000     1000     1717 2023-12-15 00:51:47.000000 satsim-0.18.0/satsim/tfa/utils/types.py
-drwxrwxrwx   0     1000     1000        0 2024-03-23 07:34:06.263099 satsim-0.18.0/satsim/time/
--rwxrwxrwx   0     1000     1000     4259 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/time/__init__.py
-drwxrwxrwx   0     1000     1000        0 2024-03-23 07:34:06.318404 satsim-0.18.0/satsim/util/
--rwxrwxrwx   0     1000     1000      130 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/util/__init__.py
--rwxrwxrwx   0     1000     1000     2761 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/util/system.py
--rwxrwxrwx   0     1000     1000     3271 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/util/thread.py
--rwxrwxrwx   0     1000     1000     2044 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/util/timer.py
-drwxrwxrwx   0     1000     1000        0 2024-03-23 07:34:06.434872 satsim-0.18.0/satsim/vecmath/
--rwxrwxrwx   0     1000     1000    17668 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/vecmath/Cartesian2.py
--rwxrwxrwx   0     1000     1000    20896 2023-07-17 23:45:22.000000 satsim-0.18.0/satsim/vecmath/Cartesian3.py
--rwxrwxrwx   0     1000     1000    18429 2023-07-17 23:45:23.000000 satsim-0.18.0/satsim/vecmath/Cartesian4.py
--rwxrwxrwx   0     1000     1000    21727 2023-07-17 23:45:23.000000 satsim-0.18.0/satsim/vecmath/Matrix2.py
--rwxrwxrwx   0     1000     1000    42567 2023-07-17 23:45:23.000000 satsim-0.18.0/satsim/vecmath/Matrix3.py
--rwxrwxrwx   0     1000     1000    73877 2023-07-17 23:45:23.000000 satsim-0.18.0/satsim/vecmath/Matrix4.py
--rwxrwxrwx   0     1000     1000    25251 2023-07-17 23:45:23.000000 satsim-0.18.0/satsim/vecmath/Quaternion.py
--rwxrwxrwx   0     1000     1000      226 2023-07-17 23:45:23.000000 satsim-0.18.0/satsim/vecmath/__init__.py
-drwxrwxrwx   0     1000     1000        0 2024-03-23 07:34:05.315285 satsim-0.18.0/satsim.egg-info/
--rwxrwxrwx   0     1000     1000     9773 2024-03-23 07:33:58.000000 satsim-0.18.0/satsim.egg-info/PKG-INFO
--rwxrwxrwx   0     1000     1000     5696 2024-03-23 07:34:03.000000 satsim-0.18.0/satsim.egg-info/SOURCES.txt
--rwxrwxrwx   0     1000     1000        1 2024-03-23 07:33:58.000000 satsim-0.18.0/satsim.egg-info/dependency_links.txt
--rwxrwxrwx   0     1000     1000       44 2024-03-23 07:33:58.000000 satsim-0.18.0/satsim.egg-info/entry_points.txt
--rwxrwxrwx   0     1000     1000        1 2024-03-23 07:33:58.000000 satsim-0.18.0/satsim.egg-info/not-zip-safe
--rwxrwxrwx   0     1000     1000      367 2024-03-23 07:33:58.000000 satsim-0.18.0/satsim.egg-info/requires.txt
--rwxrwxrwx   0     1000     1000        7 2024-03-23 07:33:58.000000 satsim-0.18.0/satsim.egg-info/top_level.txt
--rwxrwxrwx   0     1000     1000      537 2024-03-23 07:34:07.094523 satsim-0.18.0/setup.cfg
--rwxrwxrwx   0     1000     1000     1851 2024-03-21 03:50:18.000000 satsim-0.18.0/setup.py
-drwxrwxrwx   0     1000     1000        0 2024-03-23 07:34:07.079890 satsim-0.18.0/tests/
--rwxrwxrwx   0     1000     1000        0 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/__init__.py
--rwxrwxrwx   0     1000     1000     1760 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/config.yml
--rwxrwxrwx   0     1000     1000     3412 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/config_dynamic.json
--rwxrwxrwx   0     1000     1000     3305 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/config_dynamic_legacy.json
--rwxrwxrwx   0     1000     1000     3255 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/config_dynamic_sstr7.json
--rwxrwxrwx   0     1000     1000     5481 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/config_function.json
--rwxrwxrwx   0     1000     1000    30489 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/config_generator.json
--rwxrwxrwx   0     1000     1000    30469 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/config_generator_legacy.json
--rwxrwxrwx   0     1000     1000     2376 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/config_import.json
--rwxrwxrwx   0     1000     1000    11039 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/config_none.json
--rwxrwxrwx   0     1000     1000      495 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/config_partial.json
--rwxrwxrwx   0     1000     1000     3016 2024-03-20 03:26:22.000000 satsim-0.18.0/tests/config_piecewise.json
--rwxrwxrwx   0     1000     1000     4690 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/config_pipeline.json
--rwxrwxrwx   0     1000     1000    11481 2024-03-20 03:54:42.000000 satsim-0.18.0/tests/config_poppy.json
--rwxrwxrwx   0     1000     1000     4577 2024-03-20 03:40:31.000000 satsim-0.18.0/tests/config_static.json
--rwxrwxrwx   0     1000     1000     4083 2024-03-20 03:46:30.000000 satsim-0.18.0/tests/config_static_sttr7_sgp4.json
--rwxrwxrwx   0     1000     1000    84644 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/geo.txt
--rwxrwxrwx   0     1000     1000      164 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/hip_main.txt
--rwxrwxrwx   0     1000     1000     5760 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/sprite.fits
--rwxrwxrwx   0     1000     1000      976 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/stray_light.asdf
--rwxrwxrwx   0     1000     1000     9310 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/test_astrometric.py
--rwxrwxrwx   0     1000     1000    76503 2024-03-19 21:48:07.000000 satsim-0.18.0/tests/test_cartesian.py
--rwxrwxrwx   0     1000     1000     2041 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/test_cli.py
--rwxrwxrwx   0     1000     1000      507 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/test_cli_graph.py
--rwxrwxrwx   0     1000     1000     6997 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/test_config.py
--rwxrwxrwx   0     1000     1000     1804 2024-03-21 00:01:03.000000 satsim-0.18.0/tests/test_csvsc.py
--rwxrwxrwx   0     1000     1000     1557 2024-03-14 03:03:55.000000 satsim-0.18.0/tests/test_czml.py
--rwxrwxrwx   0     1000     1000     3005 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/test_dataset.py
--rwxrwxrwx   0     1000     1000     5711 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/test_draw.py
--rwxrwxrwx   0     1000     1000     2019 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/test_ephemeris.py
--rwxrwxrwx   0     1000     1000     7308 2024-03-20 22:30:35.000000 satsim-0.18.0/tests/test_fpa.py
--rwxrwxrwx   0     1000     1000     4239 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/test_generator.py
--rwxrwxrwx   0     1000     1000    15965 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/test_image.py
--rwxrwxrwx   0     1000     1000     1952 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/test_io.py
--rwxrwxrwx   0     1000     1000     5013 2024-03-20 22:57:54.000000 satsim-0.18.0/tests/test_math.py
--rwxrwxrwx   0     1000     1000   146918 2024-03-20 04:16:00.000000 satsim-0.18.0/tests/test_matrix.py
--rwxrwxrwx   0     1000     1000     1559 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/test_noise.py
--rwxrwxrwx   0     1000     1000     1781 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/test_observation.py
--rwxrwxrwx   0     1000     1000     2023 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/test_pipeline.py
--rwxrwxrwx   0     1000     1000     3919 2024-03-14 00:22:48.000000 satsim-0.18.0/tests/test_psf.py
--rwxrwxrwx   0     1000     1000     1749 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/test_random.py
--rwxrwxrwx   0     1000     1000     6344 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/test_render.py
--rwxrwxrwx   0     1000     1000     6148 2024-03-20 23:09:42.000000 satsim-0.18.0/tests/test_satnet.py
--rwxrwxrwx   0     1000     1000    21367 2024-03-20 23:24:36.000000 satsim-0.18.0/tests/test_satsim.py
--rwxrwxrwx   0     1000     1000     1345 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/test_sgp4.py
--rwxrwxrwx   0     1000     1000      829 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/test_sprite.py
--rwxrwxrwx   0     1000     1000     3130 2024-03-21 01:03:10.000000 satsim-0.18.0/tests/test_sstr7.py
--rwxrwxrwx   0     1000     1000    16137 2024-03-14 00:29:23.000000 satsim-0.18.0/tests/test_tfa_transform_ops.py
--rwxrwxrwx   0     1000     1000     3096 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/test_tfa_translate_ops.py
--rwxrwxrwx   0     1000     1000     3474 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/test_tfa_utils_test.py
--rwxrwxrwx   0     1000     1000     1840 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/test_time.py
--rwxrwxrwx   0     1000     1000     2045 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/test_transform.py
--rwxrwxrwx   0     1000     1000     2497 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/test_twobody.py
--rwxrwxrwx   0     1000     1000     2360 2023-12-15 00:51:47.000000 satsim-0.18.0/tests/test_util.py
+drwxrwxrwx   0     1000     1000        0 2024-05-29 08:15:08.776284 satsim-0.19.0/
+-rwxrwxrwx   0     1000     1000      170 2023-07-17 23:45:22.000000 satsim-0.19.0/AUTHORS.rst
+-rwxrwxrwx   0     1000     1000     3255 2023-07-17 23:45:22.000000 satsim-0.19.0/CONTRIBUTING.rst
+-rwxrwxrwx   0     1000     1000     8434 2024-05-29 08:11:42.000000 satsim-0.19.0/HISTORY.md
+-rwxrwxrwx   0     1000     1000      291 2023-07-17 23:45:22.000000 satsim-0.19.0/MANIFEST.in
+-rwxrwxrwx   0     1000     1000    10750 2024-05-29 08:15:08.773638 satsim-0.19.0/PKG-INFO
+-rwxrwxrwx   0     1000     1000     1049 2023-07-17 23:45:22.000000 satsim-0.19.0/README.md
+drwxrwxrwx   0     1000     1000        0 2024-05-29 08:15:05.921665 satsim-0.19.0/docs/
+-rwxrwxrwx   0     1000     1000      608 2023-07-17 23:45:22.000000 satsim-0.19.0/docs/Makefile
+drwxrwxrwx   0     1000     1000        0 2024-05-29 08:15:05.699124 satsim-0.19.0/docs/_build/
+drwxrwxrwx   0     1000     1000        0 2024-05-29 08:15:06.108634 satsim-0.19.0/docs/_build/html/
+drwxrwxrwx   0     1000     1000        0 2024-05-29 08:15:06.312402 satsim-0.19.0/docs/_build/html/_static/
+-rwxrwxrwx   0     1000     1000    14813 2024-05-29 08:14:59.000000 satsim-0.19.0/docs/_build/html/_static/basic.css
+drwxrwxrwx   0     1000     1000        0 2024-05-29 08:15:06.355613 satsim-0.19.0/docs/_build/html/_static/css/
+-rwxrwxrwx   0     1000     1000     3229 2024-05-29 07:16:04.000000 satsim-0.19.0/docs/_build/html/_static/css/badge_only.css
+drwxrwxrwx   0     1000     1000        0 2024-05-29 08:15:06.495672 satsim-0.19.0/docs/_build/html/_static/css/fonts/
+-rwxrwxrwx   0     1000     1000   165742 2024-05-29 07:16:04.000000 satsim-0.19.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot
+-rwxrwxrwx   0     1000     1000   444379 2024-05-29 07:16:04.000000 satsim-0.19.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rwxrwxrwx   0     1000     1000   165548 2024-05-29 07:16:04.000000 satsim-0.19.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf
+-rwxrwxrwx   0     1000     1000    98024 2024-05-29 07:16:04.000000 satsim-0.19.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff
+-rwxrwxrwx   0     1000     1000    77160 2024-05-29 07:16:04.000000 satsim-0.19.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2
+-rwxrwxrwx   0     1000     1000   135235 2024-05-29 07:16:04.000000 satsim-0.19.0/docs/_build/html/_static/css/theme.css
+-rwxrwxrwx   0     1000     1000     4472 2024-05-29 07:16:03.000000 satsim-0.19.0/docs/_build/html/_static/doctools.js
+-rwxrwxrwx   0     1000     1000      421 2024-05-29 08:14:59.000000 satsim-0.19.0/docs/_build/html/_static/documentation_options.js
+-rwxrwxrwx   0     1000     1000      286 2024-05-29 07:16:03.000000 satsim-0.19.0/docs/_build/html/_static/file.png
+drwxrwxrwx   0     1000     1000        0 2024-05-29 08:15:06.586198 satsim-0.19.0/docs/_build/html/_static/js/
+-rwxrwxrwx   0     1000     1000      934 2024-05-29 07:16:04.000000 satsim-0.19.0/docs/_build/html/_static/js/badge_only.js
+-rwxrwxrwx   0     1000     1000     4370 2024-05-29 07:16:04.000000 satsim-0.19.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js
+-rwxrwxrwx   0     1000     1000     2734 2024-05-29 07:16:04.000000 satsim-0.19.0/docs/_build/html/_static/js/html5shiv.min.js
+-rwxrwxrwx   0     1000     1000     5023 2024-05-29 07:16:04.000000 satsim-0.19.0/docs/_build/html/_static/js/theme.js
+-rwxrwxrwx   0     1000     1000     4758 2024-05-29 08:14:59.000000 satsim-0.19.0/docs/_build/html/_static/language_data.js
+-rwxrwxrwx   0     1000     1000       90 2024-05-29 07:16:03.000000 satsim-0.19.0/docs/_build/html/_static/minus.png
+-rwxrwxrwx   0     1000     1000       90 2024-05-29 07:16:03.000000 satsim-0.19.0/docs/_build/html/_static/plus.png
+-rwxrwxrwx   0     1000     1000     4929 2024-05-29 08:14:59.000000 satsim-0.19.0/docs/_build/html/_static/pygments.css
+-rwxrwxrwx   0     1000     1000    18215 2024-05-29 07:16:03.000000 satsim-0.19.0/docs/_build/html/_static/searchtools.js
+-rwxrwxrwx   0     1000     1000     4712 2024-05-29 07:16:03.000000 satsim-0.19.0/docs/_build/html/_static/sphinx_highlight.js
+drwxrwxrwx   0     1000     1000        0 2024-05-29 08:15:06.887863 satsim-0.19.0/docs/_build/html/api/
+-rwxrwxrwx   0     1000     1000    10225 2024-05-29 08:14:57.000000 satsim-0.19.0/docs/_build/html/api/satsim.dataset.html
+-rwxrwxrwx   0     1000     1000    10160 2024-05-29 08:14:57.000000 satsim-0.19.0/docs/_build/html/api/satsim.generator.html
+-rwxrwxrwx   0     1000     1000    60070 2024-05-29 08:14:57.000000 satsim-0.19.0/docs/_build/html/api/satsim.generator.obs.html
+-rwxrwxrwx   0     1000     1000   118459 2024-05-29 08:14:57.000000 satsim-0.19.0/docs/_build/html/api/satsim.geometry.html
+-rwxrwxrwx   0     1000     1000   163677 2024-05-29 08:14:57.000000 satsim-0.19.0/docs/_build/html/api/satsim.html
+-rwxrwxrwx   0     1000     1000    91803 2024-05-29 08:14:57.000000 satsim-0.19.0/docs/_build/html/api/satsim.image.html
+-rwxrwxrwx   0     1000     1000    38820 2024-05-29 08:14:57.000000 satsim-0.19.0/docs/_build/html/api/satsim.io.html
+-rwxrwxrwx   0     1000     1000    33975 2024-05-29 08:14:57.000000 satsim-0.19.0/docs/_build/html/api/satsim.math.html
+-rwxrwxrwx   0     1000     1000    14651 2024-05-29 08:14:57.000000 satsim-0.19.0/docs/_build/html/api/satsim.pipeline.html
+-rwxrwxrwx   0     1000     1000    12697 2024-05-29 08:14:57.000000 satsim-0.19.0/docs/_build/html/api/satsim.tfa.html
+-rwxrwxrwx   0     1000     1000   156980 2024-05-29 08:14:58.000000 satsim-0.19.0/docs/_build/html/api/satsim.tfa.image.html
+-rwxrwxrwx   0     1000     1000    11801 2024-05-29 08:14:58.000000 satsim-0.19.0/docs/_build/html/api/satsim.tfa.utils.html
+-rwxrwxrwx   0     1000     1000    19461 2024-05-29 08:14:58.000000 satsim-0.19.0/docs/_build/html/api/satsim.time.html
+-rwxrwxrwx   0     1000     1000    26947 2024-05-29 08:14:58.000000 satsim-0.19.0/docs/_build/html/api/satsim.util.html
+-rwxrwxrwx   0     1000     1000   404550 2024-05-29 08:14:58.000000 satsim-0.19.0/docs/_build/html/api/satsim.vecmath.html
+-rwxrwxrwx   0     1000     1000   130848 2024-05-29 08:14:56.000000 satsim-0.19.0/docs/_build/html/api.html
+-rwxrwxrwx   0     1000     1000     5491 2024-05-29 08:14:58.000000 satsim-0.19.0/docs/_build/html/authors.html
+-rwxrwxrwx   0     1000     1000    13939 2024-05-29 08:14:58.000000 satsim-0.19.0/docs/_build/html/contributing.html
+-rwxrwxrwx   0     1000     1000   102658 2024-05-29 08:14:59.000000 satsim-0.19.0/docs/_build/html/genindex.html
+-rwxrwxrwx   0     1000     1000    21145 2024-05-29 08:14:58.000000 satsim-0.19.0/docs/_build/html/history.html
+-rwxrwxrwx   0     1000     1000    10098 2024-05-29 08:14:59.000000 satsim-0.19.0/docs/_build/html/index.html
+-rwxrwxrwx   0     1000     1000     7949 2024-05-29 08:14:59.000000 satsim-0.19.0/docs/_build/html/installation.html
+-rwxrwxrwx   0     1000     1000    19822 2024-05-29 08:14:59.000000 satsim-0.19.0/docs/_build/html/py-modindex.html
+-rwxrwxrwx   0     1000     1000     4196 2024-05-29 08:14:59.000000 satsim-0.19.0/docs/_build/html/search.html
+-rwxrwxrwx   0     1000     1000   133802 2024-05-29 08:14:59.000000 satsim-0.19.0/docs/_build/html/searchindex.js
+-rwxrwxrwx   0     1000     1000    37538 2024-05-29 08:14:59.000000 satsim-0.19.0/docs/_build/html/usage.html
+drwxrwxrwx   0     1000     1000        0 2024-05-29 08:15:07.097253 satsim-0.19.0/docs/api/
+-rwxrwxrwx   0     1000     1000      310 2024-05-29 08:14:45.000000 satsim-0.19.0/docs/api/satsim.dataset.rst
+-rwxrwxrwx   0     1000     1000     1002 2024-05-29 08:14:45.000000 satsim-0.19.0/docs/api/satsim.generator.obs.rst
+-rwxrwxrwx   0     1000     1000      218 2024-05-29 08:14:45.000000 satsim-0.19.0/docs/api/satsim.generator.rst
+-rwxrwxrwx   0     1000     1000     2212 2024-05-29 08:14:45.000000 satsim-0.19.0/docs/api/satsim.geometry.rst
+-rwxrwxrwx   0     1000     1000     1004 2024-05-29 08:14:45.000000 satsim-0.19.0/docs/api/satsim.image.rst
+-rwxrwxrwx   0     1000     1000      673 2024-05-29 08:14:45.000000 satsim-0.19.0/docs/api/satsim.io.rst
+-rwxrwxrwx   0     1000     1000     1138 2024-05-29 08:14:45.000000 satsim-0.19.0/docs/api/satsim.math.rst
+-rwxrwxrwx   0     1000     1000      135 2024-05-29 08:14:45.000000 satsim-0.19.0/docs/api/satsim.pipeline.rst
+-rwxrwxrwx   0     1000     1000      744 2024-05-29 08:14:45.000000 satsim-0.19.0/docs/api/satsim.rst
+-rwxrwxrwx   0     1000     1000      678 2024-05-29 08:14:45.000000 satsim-0.19.0/docs/api/satsim.tfa.image.rst
+-rwxrwxrwx   0     1000     1000      216 2024-05-29 08:14:45.000000 satsim-0.19.0/docs/api/satsim.tfa.rst
+-rwxrwxrwx   0     1000     1000      488 2024-05-29 08:14:45.000000 satsim-0.19.0/docs/api/satsim.tfa.utils.rst
+-rwxrwxrwx   0     1000     1000      123 2024-05-29 08:14:45.000000 satsim-0.19.0/docs/api/satsim.time.rst
+-rwxrwxrwx   0     1000     1000      715 2024-05-29 08:14:45.000000 satsim-0.19.0/docs/api/satsim.util.rst
+-rwxrwxrwx   0     1000     1000     1276 2024-05-29 08:14:45.000000 satsim-0.19.0/docs/api/satsim.vecmath.rst
+-rwxrwxrwx   0     1000     1000      136 2023-07-17 23:45:22.000000 satsim-0.19.0/docs/api.rst
+-rwxrwxrwx   0     1000     1000       28 2023-07-17 23:45:22.000000 satsim-0.19.0/docs/authors.rst
+-rwxrwxrwx   0     1000     1000     4908 2024-05-29 07:21:32.000000 satsim-0.19.0/docs/conf.py
+-rwxrwxrwx   0     1000     1000       33 2023-07-17 23:45:22.000000 satsim-0.19.0/docs/contributing.rst
+-rwxrwxrwx   0     1000     1000       27 2023-07-17 23:45:22.000000 satsim-0.19.0/docs/history.rst
+-rwxrwxrwx   0     1000     1000      265 2023-07-17 23:45:22.000000 satsim-0.19.0/docs/index.rst
+-rwxrwxrwx   0     1000     1000     1523 2024-03-23 07:59:56.000000 satsim-0.19.0/docs/installation.rst
+-rwxrwxrwx   0     1000     1000      768 2023-07-17 23:45:22.000000 satsim-0.19.0/docs/make.bat
+-rwxrwxrwx   0     1000     1000    11419 2023-07-17 23:45:22.000000 satsim-0.19.0/docs/usage.rst
+drwxrwxrwx   0     1000     1000        0 2024-05-29 08:15:07.140686 satsim-0.19.0/satsim/
+-rwxrwxrwx   0     1000     1000      264 2024-05-28 09:37:13.000000 satsim-0.19.0/satsim/__init__.py
+-rwxrwxrwx   0     1000     1000     4131 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/cli.py
+-rwxrwxrwx   0     1000     1000    20530 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/config.py
+drwxrwxrwx   0     1000     1000        0 2024-05-29 08:15:07.237537 satsim-0.19.0/satsim/dataset/
+-rwxrwxrwx   0     1000     1000        0 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/dataset/__init__.py
+-rwxrwxrwx   0     1000     1000     3507 2024-03-23 07:59:56.000000 satsim-0.19.0/satsim/dataset/augment.py
+drwxrwxrwx   0     1000     1000        0 2024-05-29 08:15:07.250907 satsim-0.19.0/satsim/generator/
+-rwxrwxrwx   0     1000     1000        0 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/generator/__init__.py
+drwxrwxrwx   0     1000     1000        0 2024-05-29 08:15:07.350290 satsim-0.19.0/satsim/generator/obs/
+-rwxrwxrwx   0     1000     1000        0 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/generator/obs/__init__.py
+-rwxrwxrwx   0     1000     1000    14912 2024-05-28 19:22:43.000000 satsim-0.19.0/satsim/generator/obs/breakup.py
+-rwxrwxrwx   0     1000     1000     2330 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/generator/obs/cso.py
+-rwxrwxrwx   0     1000     1000     6239 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/generator/obs/geometry.py
+-rwxrwxrwx   0     1000     1000     1248 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/generator/obs/io.py
+-rwxrwxrwx   0     1000     1000     3703 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/generator/obs/rpo.py
+drwxrwxrwx   0     1000     1000        0 2024-05-29 08:15:07.552641 satsim-0.19.0/satsim/geometry/
+-rwxrwxrwx   0     1000     1000       66 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/geometry/__init__.py
+-rwxrwxrwx   0     1000     1000    21442 2024-05-28 02:51:01.000000 satsim-0.19.0/satsim/geometry/astrometric.py
+-rwxrwxrwx   0     1000     1000     2386 2024-03-23 07:59:56.000000 satsim-0.19.0/satsim/geometry/csvsc.py
+-rwxrwxrwx   0     1000     1000     5268 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/geometry/draw.py
+-rwxrwxrwx   0     1000     1000     3404 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/geometry/ephemeris.py
+-rwxrwxrwx   0     1000     1000     2966 2023-07-20 03:20:44.000000 satsim-0.19.0/satsim/geometry/observation.py
+-rwxrwxrwx   0     1000     1000     2470 2024-05-28 00:33:08.000000 satsim-0.19.0/satsim/geometry/photometric.py
+-rwxrwxrwx   0     1000     1000     1672 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/geometry/random.py
+-rwxrwxrwx   0     1000     1000     1150 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/geometry/sgp4.py
+-rwxrwxrwx   0     1000     1000      699 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/geometry/sprite.py
+-rwxrwxrwx   0     1000     1000    11541 2024-03-23 07:59:56.000000 satsim-0.19.0/satsim/geometry/sstr7.py
+-rwxrwxrwx   0     1000     1000     4340 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/geometry/transform.py
+-rwxrwxrwx   0     1000     1000     4619 2024-05-28 10:04:45.000000 satsim-0.19.0/satsim/geometry/twobody.py
+-rwxrwxrwx   0     1000     1000     3787 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/geometry/wcs.py
+drwxrwxrwx   0     1000     1000        0 2024-05-29 08:15:07.654059 satsim-0.19.0/satsim/image/
+-rwxrwxrwx   0     1000     1000       58 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/image/__init__.py
+-rwxrwxrwx   0     1000     1000     9786 2023-12-15 00:51:47.000000 satsim-0.19.0/satsim/image/augment.py
+-rwxrwxrwx   0     1000     1000    16147 2024-03-23 07:59:56.000000 satsim-0.19.0/satsim/image/fpa.py
+-rwxrwxrwx   0     1000     1000     5359 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/image/model.py
+-rwxrwxrwx   0     1000     1000     2895 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/image/noise.py
+-rwxrwxrwx   0     1000     1000     6836 2024-03-14 00:31:04.000000 satsim-0.19.0/satsim/image/psf.py
+-rwxrwxrwx   0     1000     1000    10541 2024-03-23 07:59:56.000000 satsim-0.19.0/satsim/image/render.py
+drwxrwxrwx   0     1000     1000        0 2024-05-29 08:15:07.721252 satsim-0.19.0/satsim/io/
+-rwxrwxrwx   0     1000     1000        0 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/io/__init__.py
+-rwxrwxrwx   0     1000     1000    15817 2023-07-20 03:20:44.000000 satsim-0.19.0/satsim/io/czml.py
+-rwxrwxrwx   0     1000     1000     4319 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/io/fits.py
+-rwxrwxrwx   0     1000     1000     2632 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/io/image.py
+-rwxrwxrwx   0     1000     1000    14273 2024-03-23 07:59:56.000000 satsim-0.19.0/satsim/io/satnet.py
+drwxrwxrwx   0     1000     1000        0 2024-05-29 08:15:07.835189 satsim-0.19.0/satsim/math/
+-rwxrwxrwx   0     1000     1000       81 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/math/__init__.py
+-rwxrwxrwx   0     1000     1000     2350 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/math/angle.py
+-rwxrwxrwx   0     1000     1000      937 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/math/const.py
+-rwxrwxrwx   0     1000     1000      951 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/math/conv.py
+-rwxrwxrwx   0     1000     1000     5551 2024-03-14 00:29:14.000000 satsim-0.19.0/satsim/math/fft.py
+-rwxrwxrwx   0     1000     1000     2726 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/math/interpolate.py
+-rwxrwxrwx   0     1000     1000     3096 2023-07-20 03:20:44.000000 satsim-0.19.0/satsim/math/random.py
+-rwxrwxrwx   0     1000     1000      590 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/math/stats.py
+drwxrwxrwx   0     1000     1000        0 2024-05-29 08:15:07.849938 satsim-0.19.0/satsim/pipeline/
+-rwxrwxrwx   0     1000     1000     1087 2024-05-28 03:48:04.000000 satsim-0.19.0/satsim/pipeline/__init__.py
+-rwxrwxrwx   0     1000     1000    55573 2024-05-28 10:00:10.000000 satsim-0.19.0/satsim/satsim.py
+drwxrwxrwx   0     1000     1000        0 2024-05-29 08:15:07.864026 satsim-0.19.0/satsim/tfa/
+-rwxrwxrwx   0     1000     1000       63 2023-12-15 00:51:47.000000 satsim-0.19.0/satsim/tfa/__init__.py
+drwxrwxrwx   0     1000     1000        0 2024-05-29 08:15:07.928509 satsim-0.19.0/satsim/tfa/image/
+-rwxrwxrwx   0     1000     1000      573 2023-12-15 00:51:47.000000 satsim-0.19.0/satsim/tfa/image/__init__.py
+-rwxrwxrwx   0     1000     1000    14584 2023-12-15 00:51:47.000000 satsim-0.19.0/satsim/tfa/image/transform_ops.py
+-rwxrwxrwx   0     1000     1000     5295 2023-12-15 00:51:47.000000 satsim-0.19.0/satsim/tfa/image/translate_ops.py
+-rwxrwxrwx   0     1000     1000     4266 2024-03-23 07:59:56.000000 satsim-0.19.0/satsim/tfa/image/utils.py
+drwxrwxrwx   0     1000     1000        0 2024-05-29 08:15:07.976079 satsim-0.19.0/satsim/tfa/utils/
+-rwxrwxrwx   0     1000     1000        0 2023-12-15 00:51:47.000000 satsim-0.19.0/satsim/tfa/utils/__init__.py
+-rwxrwxrwx   0     1000     1000     1730 2024-03-23 07:59:56.000000 satsim-0.19.0/satsim/tfa/utils/test_utils.py
+-rwxrwxrwx   0     1000     1000     1717 2023-12-15 00:51:47.000000 satsim-0.19.0/satsim/tfa/utils/types.py
+drwxrwxrwx   0     1000     1000        0 2024-05-29 08:15:07.991598 satsim-0.19.0/satsim/time/
+-rwxrwxrwx   0     1000     1000     4259 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/time/__init__.py
+drwxrwxrwx   0     1000     1000        0 2024-05-29 08:15:08.062326 satsim-0.19.0/satsim/util/
+-rwxrwxrwx   0     1000     1000      152 2024-05-27 23:20:34.000000 satsim-0.19.0/satsim/util/__init__.py
+-rwxrwxrwx   0     1000     1000      927 2024-05-28 02:49:18.000000 satsim-0.19.0/satsim/util/python.py
+-rwxrwxrwx   0     1000     1000     2761 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/util/system.py
+-rwxrwxrwx   0     1000     1000     3271 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/util/thread.py
+-rwxrwxrwx   0     1000     1000     2044 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/util/timer.py
+drwxrwxrwx   0     1000     1000        0 2024-05-29 08:15:08.179462 satsim-0.19.0/satsim/vecmath/
+-rwxrwxrwx   0     1000     1000    17668 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/vecmath/Cartesian2.py
+-rwxrwxrwx   0     1000     1000    20896 2023-07-17 23:45:22.000000 satsim-0.19.0/satsim/vecmath/Cartesian3.py
+-rwxrwxrwx   0     1000     1000    18429 2023-07-17 23:45:23.000000 satsim-0.19.0/satsim/vecmath/Cartesian4.py
+-rwxrwxrwx   0     1000     1000    21727 2023-07-17 23:45:23.000000 satsim-0.19.0/satsim/vecmath/Matrix2.py
+-rwxrwxrwx   0     1000     1000    42567 2023-07-17 23:45:23.000000 satsim-0.19.0/satsim/vecmath/Matrix3.py
+-rwxrwxrwx   0     1000     1000    73877 2023-07-17 23:45:23.000000 satsim-0.19.0/satsim/vecmath/Matrix4.py
+-rwxrwxrwx   0     1000     1000    25251 2023-07-17 23:45:23.000000 satsim-0.19.0/satsim/vecmath/Quaternion.py
+-rwxrwxrwx   0     1000     1000      226 2023-07-17 23:45:23.000000 satsim-0.19.0/satsim/vecmath/__init__.py
+drwxrwxrwx   0     1000     1000        0 2024-05-29 08:15:07.212700 satsim-0.19.0/satsim.egg-info/
+-rwxrwxrwx   0     1000     1000    10750 2024-05-29 08:15:00.000000 satsim-0.19.0/satsim.egg-info/PKG-INFO
+-rwxrwxrwx   0     1000     1000     5775 2024-05-29 08:15:05.000000 satsim-0.19.0/satsim.egg-info/SOURCES.txt
+-rwxrwxrwx   0     1000     1000        1 2024-05-29 08:15:00.000000 satsim-0.19.0/satsim.egg-info/dependency_links.txt
+-rwxrwxrwx   0     1000     1000       43 2024-05-29 08:15:00.000000 satsim-0.19.0/satsim.egg-info/entry_points.txt
+-rwxrwxrwx   0     1000     1000        1 2024-05-29 08:15:00.000000 satsim-0.19.0/satsim.egg-info/not-zip-safe
+-rwxrwxrwx   0     1000     1000      367 2024-05-29 08:15:00.000000 satsim-0.19.0/satsim.egg-info/requires.txt
+-rwxrwxrwx   0     1000     1000        7 2024-05-29 08:15:00.000000 satsim-0.19.0/satsim.egg-info/top_level.txt
+-rwxrwxrwx   0     1000     1000      537 2024-05-29 08:15:08.779960 satsim-0.19.0/setup.cfg
+-rwxrwxrwx   0     1000     1000     1851 2024-05-28 09:37:12.000000 satsim-0.19.0/setup.py
+drwxrwxrwx   0     1000     1000        0 2024-05-29 08:15:08.761731 satsim-0.19.0/tests/
+-rwxrwxrwx   0     1000     1000        0 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/__init__.py
+-rwxrwxrwx   0     1000     1000     1760 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/config.yml
+-rwxrwxrwx   0     1000     1000     3412 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/config_dynamic.json
+-rwxrwxrwx   0     1000     1000     3305 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/config_dynamic_legacy.json
+-rwxrwxrwx   0     1000     1000     3255 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/config_dynamic_sstr7.json
+-rwxrwxrwx   0     1000     1000     5481 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/config_function.json
+-rwxrwxrwx   0     1000     1000    30489 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/config_generator.json
+-rwxrwxrwx   0     1000     1000    30469 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/config_generator_legacy.json
+-rwxrwxrwx   0     1000     1000     2376 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/config_import.json
+-rwxrwxrwx   0     1000     1000    11039 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/config_none.json
+-rwxrwxrwx   0     1000     1000      495 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/config_partial.json
+-rwxrwxrwx   0     1000     1000     3016 2024-03-23 07:59:56.000000 satsim-0.19.0/tests/config_piecewise.json
+-rwxrwxrwx   0     1000     1000     4690 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/config_pipeline.json
+-rwxrwxrwx   0     1000     1000    11481 2024-03-20 03:54:42.000000 satsim-0.19.0/tests/config_poppy.json
+-rwxrwxrwx   0     1000     1000     5061 2024-05-28 03:46:09.000000 satsim-0.19.0/tests/config_static.json
+-rwxrwxrwx   0     1000     1000     5007 2024-05-27 23:23:20.000000 satsim-0.19.0/tests/config_static_sttr7_sgp4.json
+-rwxrwxrwx   0     1000     1000    84644 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/geo.txt
+-rwxrwxrwx   0     1000     1000      164 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/hip_main.txt
+-rwxrwxrwx   0     1000     1000     5760 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/sprite.fits
+-rwxrwxrwx   0     1000     1000      976 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/stray_light.asdf
+-rwxrwxrwx   0     1000     1000     9349 2024-05-24 02:49:31.000000 satsim-0.19.0/tests/test_astrometric.py
+-rwxrwxrwx   0     1000     1000    76503 2024-03-23 07:59:56.000000 satsim-0.19.0/tests/test_cartesian.py
+-rwxrwxrwx   0     1000     1000     2041 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/test_cli.py
+-rwxrwxrwx   0     1000     1000      507 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/test_cli_graph.py
+-rwxrwxrwx   0     1000     1000     6997 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/test_config.py
+-rwxrwxrwx   0     1000     1000     1804 2024-03-23 07:59:56.000000 satsim-0.19.0/tests/test_csvsc.py
+-rwxrwxrwx   0     1000     1000     1557 2024-03-23 07:59:56.000000 satsim-0.19.0/tests/test_czml.py
+-rwxrwxrwx   0     1000     1000     3005 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/test_dataset.py
+-rwxrwxrwx   0     1000     1000     5711 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/test_draw.py
+-rwxrwxrwx   0     1000     1000     2019 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/test_ephemeris.py
+-rwxrwxrwx   0     1000     1000     7308 2024-03-23 07:59:56.000000 satsim-0.19.0/tests/test_fpa.py
+-rwxrwxrwx   0     1000     1000     6011 2024-05-29 07:07:07.000000 satsim-0.19.0/tests/test_generator.py
+-rwxrwxrwx   0     1000     1000    15965 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/test_image.py
+-rwxrwxrwx   0     1000     1000     1952 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/test_io.py
+-rwxrwxrwx   0     1000     1000     5013 2024-03-23 07:59:56.000000 satsim-0.19.0/tests/test_math.py
+-rwxrwxrwx   0     1000     1000   146918 2024-03-23 07:59:56.000000 satsim-0.19.0/tests/test_matrix.py
+-rwxrwxrwx   0     1000     1000     1559 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/test_noise.py
+-rwxrwxrwx   0     1000     1000     1781 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/test_observation.py
+-rwxrwxrwx   0     1000     1000     1903 2024-05-28 02:49:13.000000 satsim-0.19.0/tests/test_photometric.py
+-rwxrwxrwx   0     1000     1000     2023 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/test_pipeline.py
+-rwxrwxrwx   0     1000     1000     3919 2024-03-14 00:22:48.000000 satsim-0.19.0/tests/test_psf.py
+-rwxrwxrwx   0     1000     1000     1749 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/test_random.py
+-rwxrwxrwx   0     1000     1000     6344 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/test_render.py
+-rwxrwxrwx   0     1000     1000     6148 2024-03-23 07:59:56.000000 satsim-0.19.0/tests/test_satnet.py
+-rwxrwxrwx   0     1000     1000    21448 2024-05-28 03:47:23.000000 satsim-0.19.0/tests/test_satsim.py
+-rwxrwxrwx   0     1000     1000     1345 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/test_sgp4.py
+-rwxrwxrwx   0     1000     1000      829 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/test_sprite.py
+-rwxrwxrwx   0     1000     1000     3130 2024-03-23 07:59:56.000000 satsim-0.19.0/tests/test_sstr7.py
+-rwxrwxrwx   0     1000     1000    16137 2024-03-23 07:59:56.000000 satsim-0.19.0/tests/test_tfa_transform_ops.py
+-rwxrwxrwx   0     1000     1000     3096 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/test_tfa_translate_ops.py
+-rwxrwxrwx   0     1000     1000     3474 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/test_tfa_utils_test.py
+-rwxrwxrwx   0     1000     1000     1840 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/test_time.py
+-rwxrwxrwx   0     1000     1000     2045 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/test_transform.py
+-rwxrwxrwx   0     1000     1000     2497 2023-12-15 00:51:47.000000 satsim-0.19.0/tests/test_twobody.py
+-rwxrwxrwx   0     1000     1000     3587 2024-05-27 23:22:02.000000 satsim-0.19.0/tests/test_util.py
```

### Comparing `satsim-0.18.0/CONTRIBUTING.rst` & `satsim-0.19.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/HISTORY.md` & `satsim-0.19.0/HISTORY.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 History
 =======
 
+0.19.0
+---------------------
+
+* Add lambertian sphere brightness model for objects. Set object key `model` `mode` to `lambertian_sphere` and set `albedo` and `size` (meters) parameters. For 2D simulations, `distance` (km) and `phase_angle` (degrees) parameters must also be specified.
+
+
 0.18.0
 ---------------------
 
 * Add turbulent atmosphere to POPPY PSF generation. Set with psf option `turbulent_atmosphere` and sim option `psf_sample_frequency`.
 * Add star and object segmentation annotation. Set sim option `save_segmentation` to `true` and `star_annotation_threshold` to limit stars annotated.
```

### Comparing `satsim-0.18.0/PKG-INFO` & `satsim-0.19.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,46 @@
 Metadata-Version: 2.1
 Name: satsim
-Version: 0.18.0
+Version: 0.19.0
 Summary: Satellite observation and scene simulator.
 Home-page: https://github.com/ssc-ai/satsim
 Author: Alex Cabello
 Author-email: alexander.cabello@algoritics.com
-License: UNKNOWN
 Keywords: satsim
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta 
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: AUTHORS.rst
+Requires-Dist: Click>=8.1
+Requires-Dist: Cython>=0.29.0
+Requires-Dist: scikit-image>=0.19.3
+Requires-Dist: Pillow<10.0,>=9.0
+Requires-Dist: numpy>=1.21.0
+Requires-Dist: PyYAML>=6.0
+Requires-Dist: matplotlib>=3.7.0
+Requires-Dist: astropy<6,>=5.2.1
+Requires-Dist: apng>=0.3.4
+Requires-Dist: scipy>=1.10
+Requires-Dist: tensorflow>=2.4
+Requires-Dist: skyfield>=1.45
+Requires-Dist: sgp4>=2.21
+Requires-Dist: poliastro>=0.17.0
+Requires-Dist: poppy>=1.0.3
+Requires-Dist: diskcache>=5.0.3
+Requires-Dist: pydash>=4.9.0
+Requires-Dist: asdf<3,>=2.14.3
+Requires-Dist: pygc>=1.3.0
+Requires-Dist: numba>=0.56.0
+Requires-Dist: pooch>=1.6.0
+Requires-Dist: czmlpy>=0.9.0
+Requires-Dist: tifffile>=2023.4.12
+Requires-Dist: imagecodecs>=2023.3.16
 
 SatSim
 ======
 
 **SatSim source code was developed under contract with ARFL/RDSM, and is approved for public release under Public Affairs release approval
 #AFRL-2022-1116.**
 
@@ -37,14 +59,20 @@
 --------
 
 * [History](HISTORY.md)
 
 History
 =======
 
+0.19.0
+---------------------
+
+* Add lambertian sphere brightness model for objects. Set object key `model` `mode` to `lambertian_sphere` and set `albedo` and `size` (meters) parameters. For 2D simulations, `distance` (km) and `phase_angle` (degrees) parameters must also be specified.
+
+
 0.18.0
 ---------------------
 
 * Add turbulent atmosphere to POPPY PSF generation. Set with psf option `turbulent_atmosphere` and sim option `psf_sample_frequency`.
 * Add star and object segmentation annotation. Set sim option `save_segmentation` to `true` and `star_annotation_threshold` to limit stars annotated.
 
 
@@ -291,9 +319,7 @@
 * Updates to run GitLab CI.
 
 
 0.1.0
 ---------------------
 
 * First release.
-
-
```

### Comparing `satsim-0.18.0/README.md` & `satsim-0.19.0/README.md`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/Makefile` & `satsim-0.19.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/_build/html/_static/basic.css` & `satsim-0.19.0/docs/_build/html/_static/basic.css`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/_build/html/_static/css/badge_only.css` & `satsim-0.19.0/docs/_build/html/_static/css/badge_only.css`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot` & `satsim-0.19.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg` & `satsim-0.19.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf` & `satsim-0.19.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff` & `satsim-0.19.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2` & `satsim-0.19.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/_build/html/_static/css/theme.css` & `satsim-0.19.0/docs/_build/html/_static/css/theme.css`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/_build/html/_static/doctools.js` & `satsim-0.19.0/docs/_build/html/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/_build/html/_static/js/badge_only.js` & `satsim-0.19.0/docs/_build/html/_static/js/badge_only.js`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js` & `satsim-0.19.0/docs/_build/html/_static/js/html5shiv-printshiv.min.js`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/_build/html/_static/js/html5shiv.min.js` & `satsim-0.19.0/docs/_build/html/_static/js/html5shiv.min.js`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/_build/html/_static/js/theme.js` & `satsim-0.19.0/docs/_build/html/_static/js/theme.js`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/_build/html/_static/language_data.js` & `satsim-0.19.0/docs/_build/html/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/_build/html/_static/pygments.css` & `satsim-0.19.0/docs/_build/html/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/_build/html/_static/searchtools.js` & `satsim-0.19.0/docs/_build/html/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/_build/html/_static/sphinx_highlight.js` & `satsim-0.19.0/docs/_build/html/_static/sphinx_highlight.js`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/_build/html/api/satsim.dataset.html` & `satsim-0.19.0/docs/_build/html/api/satsim.dataset.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.dataset package &mdash; SatSim 0.18.0 documentation</title>
+  <title>satsim.dataset package &mdash; SatSim 0.19.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.18.0
+                0.19.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _S_a_t_S_i_m
-0.18.0
+0.19.0
 [q                   ]
 Contents:
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _U_s_a_g_e
     * _C_o_n_t_r_i_b_u_t_i_n_g
     * _A_P_I_ _D_o_c_u_m_e_n_t_a_t_i_o_n
           o _s_a_t_s_i_m_ _p_a_c_k_a_g_e
```

### Comparing `satsim-0.18.0/docs/_build/html/api/satsim.generator.html` & `satsim-0.19.0/docs/_build/html/api/satsim.generator.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.generator package &mdash; SatSim 0.18.0 documentation</title>
+  <title>satsim.generator package &mdash; SatSim 0.19.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.18.0
+                0.19.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _S_a_t_S_i_m
-0.18.0
+0.19.0
 [q                   ]
 Contents:
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _U_s_a_g_e
     * _C_o_n_t_r_i_b_u_t_i_n_g
     * _A_P_I_ _D_o_c_u_m_e_n_t_a_t_i_o_n
           o _s_a_t_s_i_m_ _p_a_c_k_a_g_e
```

### Comparing `satsim-0.18.0/docs/_build/html/api/satsim.generator.obs.html` & `satsim-0.19.0/docs/_build/html/api/satsim.generator.obs.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.generator.obs package &mdash; SatSim 0.18.0 documentation</title>
+  <title>satsim.generator.obs package &mdash; SatSim 0.19.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.18.0
+                0.19.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -108,28 +108,29 @@
 <section id="submodules">
 <h2>Submodules<a class="headerlink" href="#submodules" title="Permalink to this heading"></a></h2>
 </section>
 <section id="module-satsim.generator.obs.breakup">
 <span id="satsim-generator-obs-breakup-module"></span><h2>satsim.generator.obs.breakup module<a class="headerlink" href="#module-satsim.generator.obs.breakup" title="Permalink to this heading"></a></h2>
 <dl class="py function">
 <dt class="sig sig-object py" id="satsim.generator.obs.breakup.breakup_from_tle">
-<span class="sig-prename descclassname"><span class="pre">satsim.generator.obs.breakup.</span></span><span class="sig-name descname"><span class="pre">breakup_from_tle</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">tle</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">breakup_time</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">radius</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">37.5</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">breakup_velocity</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">108</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">n</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">100</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">target_mv_scale</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[0.5,</span> <span class="pre">2.0]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">target_mv</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">12.0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">offset</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[0.0,</span> <span class="pre">0.0]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">breakup_time_offset</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0.0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">variable_brightness</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">True</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.generator.obs.breakup.breakup_from_tle" title="Permalink to this definition"></a></dt>
+<span class="sig-prename descclassname"><span class="pre">satsim.generator.obs.breakup.</span></span><span class="sig-name descname"><span class="pre">breakup_from_tle</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">tle</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">breakup_time</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">radius</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">37.5</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">breakup_velocity</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">108</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">n</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">100</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">target_mv_scale</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[0.5,</span> <span class="pre">2.0]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">target_mv</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">12.0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">offset</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[0.0,</span> <span class="pre">0.0]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">breakup_time_offset</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0.0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">variable_brightness</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">brightness_model</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'mv'</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.generator.obs.breakup.breakup_from_tle" title="Permalink to this definition"></a></dt>
 <dd><p>Generates a breakup configuration from the input <cite>tle</cite>.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>tle</strong> – <cite>array</cite>, an array containing the SGP4 two line element set.</p></li>
 <li><p><strong>breakup_time</strong> – <cite>array</cite>, UCT time as year, month, day, hour, minute, seconds.</p></li>
 <li><p><strong>radius</strong> – <cite>float</cite>, one sigma breakup cone radius in degrees. default=37.5</p></li>
 <li><p><strong>breakup_velocity</strong> – <cite>float</cite>, the relative velocity of generated particles in km/s. default=108</p></li>
 <li><p><strong>n</strong> – <cite>array</cite>, number of particles to generate. default=100</p></li>
 <li><p><strong>target_mv_scale</strong> – <cite>array</cite>, brightness of target and total brightness of generated particles after breakup. scale based on original target brightness. default=[0.5,2.0]</p></li>
 <li><p><strong>offset</strong> – <cite>array</cite>, row column offset of target position on fpa in normalized coordinates. default=12</p></li>
 <li><p><strong>breakup_time_offset</strong> – <cite>float</cite>, number of seconds to offset breakup time from <cite>breakup</cite>. default=[0,0]</p></li>
 <li><p><strong>variable_brightness</strong> – <cite>boolean</cite>, if True randomly assign sine variable brightness between 0 to 1 hz. default=True</p></li>
+<li><p><strong>brightness_model</strong> – <cite>string</cite>, the model to use for brightness calculations. valid options <cite>mv</cite>, <cite>lambertian_sphere</cite> default=`mv`</p></li>
 </ul>
 </dd>
 </dl>
 <p>Example usage in SatSim configuration:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="s2">&quot;obs&quot;</span><span class="p">:</span> <span class="p">{</span>
     <span class="s2">&quot;generator&quot;</span><span class="p">:</span> <span class="p">{</span>
         <span class="s2">&quot;module&quot;</span><span class="p">:</span> <span class="s2">&quot;satsim.generator.obs.breakup&quot;</span><span class="p">,</span>
@@ -160,15 +161,15 @@
 <span class="p">}</span>
 </pre></div>
 </div>
 </dd></dl>
 
 <dl class="py function">
 <dt class="sig sig-object py" id="satsim.generator.obs.breakup.collision_from_tle">
-<span class="sig-prename descclassname"><span class="pre">satsim.generator.obs.breakup.</span></span><span class="sig-name descname"><span class="pre">collision_from_tle</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">tle</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">collision_time</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">radius</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">37.5</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">K</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0.5</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">attack_angle</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'random'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">attack_velocity</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">attack_velocity_scale</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">1.0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">n</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[100,</span> <span class="pre">100]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">target_mv_scale</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[0.5,</span> <span class="pre">2.0]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">rpo_mv_scale</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[0.5,</span> <span class="pre">2.0]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">target_mv</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">12.0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">rpo_mv</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">12.0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">offset</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[0.0,</span> <span class="pre">0.0]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">collision_time_offset</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0.0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">variable_brightness</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fragment_angle</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'random'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">scale_fragment_velocity</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.generator.obs.breakup.collision_from_tle" title="Permalink to this definition"></a></dt>
+<span class="sig-prename descclassname"><span class="pre">satsim.generator.obs.breakup.</span></span><span class="sig-name descname"><span class="pre">collision_from_tle</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">tle</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">collision_time</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">radius</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">37.5</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">K</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0.5</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">attack_angle</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'random'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">attack_velocity</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">attack_velocity_scale</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">1.0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">n</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[100,</span> <span class="pre">100]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">target_mv_scale</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[0.5,</span> <span class="pre">2.0]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">rpo_mv_scale</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[0.5,</span> <span class="pre">2.0]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">target_mv</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">12.0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">rpo_mv</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">12.0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">offset</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">[0.0,</span> <span class="pre">0.0]</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">collision_time_offset</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0.0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">variable_brightness</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">True</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fragment_angle</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'random'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">scale_fragment_velocity</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">brightness_model</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'mv'</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.generator.obs.breakup.collision_from_tle" title="Permalink to this definition"></a></dt>
 <dd><p>Generates a two object collision configuration from the input <cite>tle</cite>.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>tle</strong> – <cite>array</cite>, an array containing the SGP4 two line element set.</p></li>
 <li><p><strong>collision_time</strong> – <cite>array</cite>, UCT time as year, month, day, hour, minute, seconds.</p></li>
 <li><p><strong>radius</strong> – <cite>float</cite>, one sigma breakup cone radius in degrees. default=37.5</p></li>
@@ -182,14 +183,15 @@
 <li><p><strong>target_mv</strong> – <cite>float</cite>, brightness of target before collision in visual magnitude. default=12</p></li>
 <li><p><strong>rpo_mv</strong> – <cite>float</cite>, brightness of colliding object before collision in visual magnitude. default=12</p></li>
 <li><p><strong>offset</strong> – <cite>array</cite>, row column offset of target position on fpa in normalized coordinates. default=[0,0]</p></li>
 <li><p><strong>collision_time_offset</strong> – <cite>float</cite>, number of seconds to offset collision time from <cite>collision_time</cite>. default=0</p></li>
 <li><p><strong>variable_brightness</strong> – <cite>boolean</cite>, if True randomly assign sine variable brightness between 0 to 1 hz. default=True</p></li>
 <li><p><strong>fragment_angle</strong> – <cite>string</cite>, specified the fragment angle sampling. <cite>random</cite> or <cite>linspace</cite>. default=`random`</p></li>
 <li><p><strong>scale_fragment_velocity</strong> – <cite>boolean</cite>, if True scale the fragment velocity by cosine of the exit velocity. default=`false`</p></li>
+<li><p><strong>brightness_model</strong> – <cite>string</cite>, the model to use for brightness calculations. valid options <cite>mv</cite>, <cite>lambertian_sphere</cite> default=`mv`</p></li>
 </ul>
 </dd>
 </dl>
 <p>Example usage in SatSim configuration:</p>
 <div class="highlight-default notranslate"><div class="highlight"><pre><span></span><span class="s2">&quot;obs&quot;</span><span class="p">:</span> <span class="p">{</span>
     <span class="s2">&quot;generator&quot;</span><span class="p">:</span> <span class="p">{</span>
         <span class="s2">&quot;module&quot;</span><span class="p">:</span> <span class="s2">&quot;satsim.generator.obs.breakup&quot;</span><span class="p">,</span>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _S_a_t_S_i_m
-0.18.0
+0.19.0
 [q                   ]
 Contents:
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _U_s_a_g_e
     * _C_o_n_t_r_i_b_u_t_i_n_g
     * _A_P_I_ _D_o_c_u_m_e_n_t_a_t_i_o_n
           o _s_a_t_s_i_m_ _p_a_c_k_a_g_e
@@ -33,15 +33,16 @@
     * _V_i_e_w_ _p_a_g_e_ _s_o_u_r_c_e
 ===============================================================================
 ************ ssaattssiimm..ggeenneerraattoorr..oobbss ppaacckkaaggee_? ************
 ********** SSuubbmmoodduulleess_? **********
 ********** ssaattssiimm..ggeenneerraattoorr..oobbss..bbrreeaakkuupp mmoodduullee_? **********
   satsim.generator.obs.breakup.breakup_from_tle(ttllee, bbrreeaakkuupp__ttiimmee, rraaddiiuuss==3377..55,
   bbrreeaakkuupp__vveelloocciittyy==110088, nn==110000, ttaarrggeett__mmvv__ssccaallee==[[00..55,, 22..00]], ttaarrggeett__mmvv==1122..00,
-  ooffffsseett==[[00..00,, 00..00]], bbrreeaakkuupp__ttiimmee__ooffffsseett==00..00, vvaarriiaabbllee__bbrriigghhttnneessss==TTrruuee)_
+  ooffffsseett==[[00..00,, 00..00]], bbrreeaakkuupp__ttiimmee__ooffffsseett==00..00, vvaarriiaabbllee__bbrriigghhttnneessss==TTrruuee,
+  bbrriigghhttnneessss__mmooddeell==''mmvv'')_
       Generates a breakup configuration from the inputtle.
         Parameters:
                 * ttllee –array, an array containing the SGP4 two line element
                   set.
                 * bbrreeaakkuupp__ttiimmee –array, UCT time as year, month, day, hour,
                   minute, seconds.
                 * rraaddiiuuss –float, one sigma breakup cone radius in degrees.
@@ -54,14 +55,16 @@
                   on original target brightness. default=[0.5,2.0]
                 * ooffffsseett –array, row column offset of target position on fpa in
                   normalized coordinates. default=12
                 * bbrreeaakkuupp__ttiimmee__ooffffsseett –float, number of seconds to offset
                   breakup time frombreakup. default=[0,0]
                 * vvaarriiaabbllee__bbrriigghhttnneessss –boolean, if True randomly assign sine
                   variable brightness between 0 to 1 hz. default=True
+                * bbrriigghhttnneessss__mmooddeell –string, the model to use for brightness
+                  calculations. valid optionsmv,lambertian_spheredefault=`mv`
       Example usage in SatSim configuration:
       "obs": {
           "generator": {
               "module": "satsim.generator.obs.breakup",
               "function": "breakup_from_tle",
               "kwargs": {
                   "n": 39,
@@ -88,15 +91,15 @@
           }
       }
   satsim.generator.obs.breakup.collision_from_tle(ttllee, ccoolllliissiioonn__ttiimmee,
   rraaddiiuuss==3377..55, KK==00..55, aattttaacckk__aannggllee==''rraannddoomm'', aattttaacckk__vveelloocciittyy==NNoonnee,
   aattttaacckk__vveelloocciittyy__ssccaallee==11..00, nn==[[110000,, 110000]], ttaarrggeett__mmvv__ssccaallee==[[00..55,, 22..00]],
   rrppoo__mmvv__ssccaallee==[[00..55,, 22..00]], ttaarrggeett__mmvv==1122..00, rrppoo__mmvv==1122..00, ooffffsseett==[[00..00,, 00..00]],
   ccoolllliissiioonn__ttiimmee__ooffffsseett==00..00, vvaarriiaabbllee__bbrriigghhttnneessss==TTrruuee, ffrraaggmmeenntt__aannggllee==''rraannddoomm'',
-  ssccaallee__ffrraaggmmeenntt__vveelloocciittyy==FFaallssee)_
+  ssccaallee__ffrraaggmmeenntt__vveelloocciittyy==FFaallssee, bbrriigghhttnneessss__mmooddeell==''mmvv'')_
       Generates a two object collision configuration from the inputtle.
         Parameters:
                 * ttllee –array, an array containing the SGP4 two line element
                   set.
                 * ccoolllliissiioonn__ttiimmee –array, UCT time as year, month, day, hour,
                   minute, seconds.
                 * rraaddiiuuss –float, one sigma breakup cone radius in degrees.
@@ -128,14 +131,16 @@
                   collision time fromcollision_time. default=0
                 * vvaarriiaabbllee__bbrriigghhttnneessss –boolean, if True randomly assign sine
                   variable brightness between 0 to 1 hz. default=True
                 * ffrraaggmmeenntt__aannggllee –string, specified the fragment angle
                   sampling.randomorlinspace. default=`random`
                 * ssccaallee__ffrraaggmmeenntt__vveelloocciittyy –boolean, if True scale the fragment
                   velocity by cosine of the exit velocity. default=`false`
+                * bbrriigghhttnneessss__mmooddeell –string, the model to use for brightness
+                  calculations. valid optionsmv,lambertian_spheredefault=`mv`
       Example usage in SatSim configuration:
       "obs": {
           "generator": {
               "module": "satsim.generator.obs.breakup",
               "function": "collision_from_tle",
               "kwargs": {
                   "n": [
```

### Comparing `satsim-0.18.0/docs/_build/html/api/satsim.geometry.html` & `satsim-0.19.0/docs/_build/html/api/satsim.geometry.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.geometry package &mdash; SatSim 0.18.0 documentation</title>
+  <title>satsim.geometry package &mdash; SatSim 0.19.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.18.0
+                0.19.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -187,14 +187,32 @@
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>A <cite>Topos</cite> Skyfield object on the planet Earth</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py function">
+<dt class="sig sig-object py" id="satsim.geometry.astrometric.distance_between">
+<span class="sig-prename descclassname"><span class="pre">satsim.geometry.astrometric.</span></span><span class="sig-name descname"><span class="pre">distance_between</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">object_a</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">object_b</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">t</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.geometry.astrometric.distance_between" title="Permalink to this definition"></a></dt>
+<dd><p>Calculate the distance between <cite>object_a</cite> and <cite>object_b</cite> at time <cite>t</cite>.</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><strong>object_a</strong> – <cite>object</cite>, Skyfield object</p></li>
+<li><p><strong>object_b</strong> – <cite>object</cite>, Skyfield object</p></li>
+<li><p><strong>t</strong> – <cite>Time</cite>, Skyfield <cite>Time</cite></p></li>
+</ul>
+</dd>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
+<dd class="field-even"><p>A <cite>float</cite>, distance in km</p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py function">
 <dt class="sig sig-object py" id="satsim.geometry.astrometric.eci_to_ecr">
 <span class="sig-prename descclassname"><span class="pre">satsim.geometry.astrometric.</span></span><span class="sig-name descname"><span class="pre">eci_to_ecr</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">time</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">ra</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dec</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">roll</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.geometry.astrometric.eci_to_ecr" title="Permalink to this definition"></a></dt>
 <dd><p>Covert an Earth centered fixed sky coordinates to Earth centered rotating.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>ra</strong> – <cite>float</cite>, right ascension in degrees</p></li>
@@ -357,35 +375,14 @@
 <dt class="field-odd">Return type<span class="colon">:</span></dt>
 <dd class="field-odd"><p>A <cite>tuple</cite>, containing</p>
 </dd>
 </dl>
 </dd></dl>
 
 <dl class="py function">
-<dt class="sig sig-object py" id="satsim.geometry.astrometric.lambertian_sphere_to_mv">
-<span class="sig-prename descclassname"><span class="pre">satsim.geometry.astrometric.</span></span><span class="sig-name descname"><span class="pre">lambertian_sphere_to_mv</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">albedo</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">distance</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">radius</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">phase_angle</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.geometry.astrometric.lambertian_sphere_to_mv" title="Permalink to this definition"></a></dt>
-<dd><p>Applies lambertian sphere approximation to convert target brightness
-to visual magnitudes based on sun brightness of -26.74.</p>
-<dl class="field-list simple">
-<dt class="field-odd">Parameters<span class="colon">:</span></dt>
-<dd class="field-odd"><ul class="simple">
-<li><p><strong>albedo</strong> – <cite>float</cite>, The ratio of reflected light to incident light
-off of the object’s surface</p></li>
-<li><p><strong>distance</strong> – <cite>float</cite>, distance to object in meters</p></li>
-<li><p><strong>radius</strong> – <cite>float</cite>, radius of sphere in meters</p></li>
-<li><p><strong>phase_angle</strong> – <cite>float</cite>, the angle between observer, object, and sun in degrees</p></li>
-</ul>
-</dd>
-<dt class="field-even">Returns<span class="colon">:</span></dt>
-<dd class="field-even"><p>A <cite>float</cite>, calculated visual magnitude</p>
-</dd>
-</dl>
-</dd></dl>
-
-<dl class="py function">
 <dt class="sig sig-object py" id="satsim.geometry.astrometric.load_earth">
 <span class="sig-prename descclassname"><span class="pre">satsim.geometry.astrometric.</span></span><span class="sig-name descname"><span class="pre">load_earth</span></span><span class="sig-paren">(</span><span class="sig-paren">)</span><a class="headerlink" href="#satsim.geometry.astrometric.load_earth" title="Permalink to this definition"></a></dt>
 <dd><p>Loads a Skyfield Earth object using the planetary and lunar ephemeris,
 DE 421. The Earth object is loaded once and cached as a singleton in the
 variable <cite>SATSIM_EARTH</cite>.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Returns<span class="colon">:</span></dt>
@@ -763,14 +760,75 @@
 <dt class="field-even">Returns<span class="colon">:</span></dt>
 <dd class="field-even"><p>An <cite>EarthObservation</cite> object</p>
 </dd>
 </dl>
 </dd></dl>
 
 </section>
+<section id="module-satsim.geometry.photometric">
+<span id="satsim-geometry-photometric-module"></span><h2>satsim.geometry.photometric module<a class="headerlink" href="#module-satsim.geometry.photometric" title="Permalink to this heading"></a></h2>
+<dl class="py function">
+<dt class="sig sig-object py" id="satsim.geometry.photometric.lambertian_sphere_model_to_mv">
+<span class="sig-prename descclassname"><span class="pre">satsim.geometry.photometric.</span></span><span class="sig-name descname"><span class="pre">lambertian_sphere_model_to_mv</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">observer</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">target</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">model</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">time</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.geometry.photometric.lambertian_sphere_model_to_mv" title="Permalink to this definition"></a></dt>
+<dd><p>Calculates the phase angle between the observer, target, and sun.</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><strong>observer</strong> – <cite>object</cite>, observer as a Skyfield object</p></li>
+<li><p><strong>target</strong> – <cite>object</cite>, target as a Skyfield object</p></li>
+<li><p><strong>sun</strong> – <cite>object</cite>, Skyfield sun object</p></li>
+<li><p><strong>time</strong> – <cite>object</cite>, Skyfield time</p></li>
+</ul>
+</dd>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
+<dd class="field-even"><p>A <cite>float</cite>, the phase angle in degrees</p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py function">
+<dt class="sig sig-object py" id="satsim.geometry.photometric.lambertian_sphere_to_mv">
+<span class="sig-prename descclassname"><span class="pre">satsim.geometry.photometric.</span></span><span class="sig-name descname"><span class="pre">lambertian_sphere_to_mv</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">albedo</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">distance</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">radius</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">phase_angle</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.geometry.photometric.lambertian_sphere_to_mv" title="Permalink to this definition"></a></dt>
+<dd><p>Applies lambertian sphere approximation to convert target brightness
+to visual magnitudes based on sun brightness of -26.74.</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><strong>albedo</strong> – <cite>float</cite>, The ratio of reflected light to incident light
+off of the object’s surface</p></li>
+<li><p><strong>distance</strong> – <cite>float</cite>, distance to object in meters</p></li>
+<li><p><strong>radius</strong> – <cite>float</cite>, radius of sphere in meters</p></li>
+<li><p><strong>phase_angle</strong> – <cite>float</cite>, the angle between observer, object, and sun in degrees</p></li>
+</ul>
+</dd>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
+<dd class="field-even"><p>A <cite>float</cite>, calculated visual magnitude</p>
+</dd>
+</dl>
+</dd></dl>
+
+<dl class="py function">
+<dt class="sig sig-object py" id="satsim.geometry.photometric.model_to_mv">
+<span class="sig-prename descclassname"><span class="pre">satsim.geometry.photometric.</span></span><span class="sig-name descname"><span class="pre">model_to_mv</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">observer</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">target</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">model</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">time</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.geometry.photometric.model_to_mv" title="Permalink to this definition"></a></dt>
+<dd><p>Calculates the phase angle between the observer, target, and sun.</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><strong>observer</strong> – <cite>object</cite>, observer as a Skyfield object</p></li>
+<li><p><strong>target</strong> – <cite>object</cite>, target as a Skyfield object</p></li>
+<li><p><strong>time</strong> – <cite>object</cite>, Skyfield time</p></li>
+</ul>
+</dd>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
+<dd class="field-even"><p>A <cite>float</cite>, the phase angle in degrees</p>
+</dd>
+</dl>
+</dd></dl>
+
+</section>
 <section id="module-satsim.geometry.random">
 <span id="satsim-geometry-random-module"></span><h2>satsim.geometry.random module<a class="headerlink" href="#module-satsim.geometry.random" title="Permalink to this heading"></a></h2>
 <dl class="py function">
 <dt class="sig sig-object py" id="satsim.geometry.random.gen_random_points">
 <span class="sig-prename descclassname"><span class="pre">satsim.geometry.random.</span></span><span class="sig-name descname"><span class="pre">gen_random_points</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">height</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">width</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">y_fov</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">x_fov</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pe_bins</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">density</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">pad_mult</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">1</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.geometry.random.gen_random_points" title="Permalink to this definition"></a></dt>
 <dd><p>Generates random points in pixel coordinates of random brightnesses
 based on density bins. Typically used to inject a stationary target such as
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _S_a_t_S_i_m
-0.18.0
+0.19.0
 [q                   ]
 Contents:
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _U_s_a_g_e
     * _C_o_n_t_r_i_b_u_t_i_n_g
     * _A_P_I_ _D_o_c_u_m_e_n_t_a_t_i_o_n
           o _s_a_t_s_i_m_ _p_a_c_k_a_g_e
@@ -73,14 +73,22 @@
       place on the planet Earth.
         Parameters:
                 * llaatt –string or float, latitude in degrees
                 * lloonn –string or float, longitude in degrees
                 * aalltt –float, altitude in km
         Returns:
             AToposSkyfield object on the planet Earth
+  satsim.geometry.astrometric.distance_between(oobbjjeecctt__aa, oobbjjeecctt__bb, tt)_
+      Calculate the distance betweenobject_aandobject_bat timet.
+        Parameters:
+                * oobbjjeecctt__aa –object, Skyfield object
+                * oobbjjeecctt__bb –object, Skyfield object
+                * tt –Time, SkyfieldTime
+        Returns:
+            Afloat, distance in km
   satsim.geometry.astrometric.eci_to_ecr(ttiimmee, rraa, ddeecc, rroollll==00)_
       Covert an Earth centered fixed sky coordinates to Earth centered
       rotating.
         Parameters:
                 * rraa –float, right ascension in degrees
                 * ddeecc –float, declination in degrees
                 * rroollll –float, field rotation (ignored)
@@ -184,27 +192,14 @@
         Returns:
             ra: right ascension in degrees dec: declination in degrees d:
             distance between observer and target in km az: azimuth angle in
             degrees el: elevation angle in degrees icrf_los: LOS as skyfield
             ICRF object
         Return type:
             Atuple, containing
-  satsim.geometry.astrometric.lambertian_sphere_to_mv(aallbbeeddoo, ddiissttaannccee, rraaddiiuuss,
-  pphhaassee__aannggllee)_
-      Applies lambertian sphere approximation to convert target brightness to
-      visual magnitudes based on sun brightness of -26.74.
-        Parameters:
-                * aallbbeeddoo –float, The ratio of reflected light to incident light
-                  off of the object’s surface
-                * ddiissttaannccee –float, distance to object in meters
-                * rraaddiiuuss –float, radius of sphere in meters
-                * pphhaassee__aannggllee –float, the angle between observer, object, and
-                  sun in degrees
-        Returns:
-            Afloat, calculated visual magnitude
   satsim.geometry.astrometric.load_earth()_
       Loads a Skyfield Earth object using the planetary and lunar ephemeris, DE
       421. The Earth object is loaded once and cached as a singleton in the
       variableSATSIM_EARTH.
         Returns:
             TheplanetEarth Skyfield object
   satsim.geometry.astrometric.load_moon()_
@@ -434,14 +429,46 @@
                 * tt –Time, observation time as SkyfieldTime
                 * oobbsseerrvveerr –VectorFunction, Skyfield observer
                 * ttaarrggeett –VectorFunction, Skyfield target
                 * dd –float, distance to target in km iftargetis None
                 * nnaammee –string, object name
         Returns:
             AnEarthObservationobject
+********** ssaattssiimm..ggeeoommeettrryy..pphhoottoommeettrriicc mmoodduullee_? **********
+  satsim.geometry.photometric.lambertian_sphere_model_to_mv(oobbsseerrvveerr, ttaarrggeett,
+  mmooddeell, ttiimmee)_
+      Calculates the phase angle between the observer, target, and sun.
+        Parameters:
+                * oobbsseerrvveerr –object, observer as a Skyfield object
+                * ttaarrggeett –object, target as a Skyfield object
+                * ssuunn –object, Skyfield sun object
+                * ttiimmee –object, Skyfield time
+        Returns:
+            Afloat, the phase angle in degrees
+  satsim.geometry.photometric.lambertian_sphere_to_mv(aallbbeeddoo, ddiissttaannccee, rraaddiiuuss,
+  pphhaassee__aannggllee)_
+      Applies lambertian sphere approximation to convert target brightness to
+      visual magnitudes based on sun brightness of -26.74.
+        Parameters:
+                * aallbbeeddoo –float, The ratio of reflected light to incident light
+                  off of the object’s surface
+                * ddiissttaannccee –float, distance to object in meters
+                * rraaddiiuuss –float, radius of sphere in meters
+                * pphhaassee__aannggllee –float, the angle between observer, object, and
+                  sun in degrees
+        Returns:
+            Afloat, calculated visual magnitude
+  satsim.geometry.photometric.model_to_mv(oobbsseerrvveerr, ttaarrggeett, mmooddeell, ttiimmee)_
+      Calculates the phase angle between the observer, target, and sun.
+        Parameters:
+                * oobbsseerrvveerr –object, observer as a Skyfield object
+                * ttaarrggeett –object, target as a Skyfield object
+                * ttiimmee –object, Skyfield time
+        Returns:
+            Afloat, the phase angle in degrees
 ********** ssaattssiimm..ggeeoommeettrryy..rraannddoomm mmoodduullee_? **********
   satsim.geometry.random.gen_random_points(hheeiigghhtt, wwiiddtthh, yy__ffoovv, xx__ffoovv,
   ppee__bbiinnss, ddeennssiittyy, ppaadd__mmuulltt==11)_
       Generates random points in pixel coordinates of random brightnesses based
       on density bins. Typically used to inject a stationary target such as
       stars onto an oversampled image.
       Examples:
```

### Comparing `satsim-0.18.0/docs/_build/html/api/satsim.html` & `satsim-0.19.0/docs/_build/html/api/satsim.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim package &mdash; SatSim 0.18.0 documentation</title>
+  <title>satsim package &mdash; SatSim 0.19.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.18.0
+                0.19.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -157,21 +157,21 @@
 <li class="toctree-l2"><a class="reference internal" href="satsim.geometry.html#submodules">Submodules</a></li>
 <li class="toctree-l2"><a class="reference internal" href="satsim.geometry.html#module-satsim.geometry.astrometric">satsim.geometry.astrometric module</a><ul>
 <li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.astrometric.GreatCircle"><code class="docutils literal notranslate"><span class="pre">GreatCircle</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.astrometric.angle_between"><code class="docutils literal notranslate"><span class="pre">angle_between()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.astrometric.angle_from_los"><code class="docutils literal notranslate"><span class="pre">angle_from_los()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.astrometric.apparent"><code class="docutils literal notranslate"><span class="pre">apparent()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.astrometric.create_topocentric"><code class="docutils literal notranslate"><span class="pre">create_topocentric()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.astrometric.distance_between"><code class="docutils literal notranslate"><span class="pre">distance_between()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.astrometric.eci_to_ecr"><code class="docutils literal notranslate"><span class="pre">eci_to_ecr()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.astrometric.eci_to_radec"><code class="docutils literal notranslate"><span class="pre">eci_to_radec()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.astrometric.gen_track"><code class="docutils literal notranslate"><span class="pre">gen_track()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.astrometric.gen_track_from_wcs"><code class="docutils literal notranslate"><span class="pre">gen_track_from_wcs()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.astrometric.get_los"><code class="docutils literal notranslate"><span class="pre">get_los()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.astrometric.get_los_azel"><code class="docutils literal notranslate"><span class="pre">get_los_azel()</span></code></a></li>
-<li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.astrometric.lambertian_sphere_to_mv"><code class="docutils literal notranslate"><span class="pre">lambertian_sphere_to_mv()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.astrometric.load_earth"><code class="docutils literal notranslate"><span class="pre">load_earth()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.astrometric.load_moon"><code class="docutils literal notranslate"><span class="pre">load_moon()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.astrometric.load_sun"><code class="docutils literal notranslate"><span class="pre">load_sun()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.astrometric.query_by_los"><code class="docutils literal notranslate"><span class="pre">query_by_los()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.astrometric.radec_to_eci"><code class="docutils literal notranslate"><span class="pre">radec_to_eci()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.astrometric.wcs_from_observer_fixed"><code class="docutils literal notranslate"><span class="pre">wcs_from_observer_fixed()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.astrometric.wcs_from_observer_rate"><code class="docutils literal notranslate"><span class="pre">wcs_from_observer_rate()</span></code></a></li>
@@ -197,14 +197,20 @@
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="satsim.geometry.html#module-satsim.geometry.observation">satsim.geometry.observation module</a><ul>
 <li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.observation.EarthObservation"><code class="docutils literal notranslate"><span class="pre">EarthObservation</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.observation.create_observation"><code class="docutils literal notranslate"><span class="pre">create_observation()</span></code></a></li>
 </ul>
 </li>
+<li class="toctree-l2"><a class="reference internal" href="satsim.geometry.html#module-satsim.geometry.photometric">satsim.geometry.photometric module</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.photometric.lambertian_sphere_model_to_mv"><code class="docutils literal notranslate"><span class="pre">lambertian_sphere_model_to_mv()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.photometric.lambertian_sphere_to_mv"><code class="docutils literal notranslate"><span class="pre">lambertian_sphere_to_mv()</span></code></a></li>
+<li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.photometric.model_to_mv"><code class="docutils literal notranslate"><span class="pre">model_to_mv()</span></code></a></li>
+</ul>
+</li>
 <li class="toctree-l2"><a class="reference internal" href="satsim.geometry.html#module-satsim.geometry.random">satsim.geometry.random module</a><ul>
 <li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.random.gen_random_points"><code class="docutils literal notranslate"><span class="pre">gen_random_points()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="satsim.geometry.html#module-satsim.geometry.sgp4">satsim.geometry.sgp4 module</a><ul>
 <li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.sgp4.create_sgp4"><code class="docutils literal notranslate"><span class="pre">create_sgp4()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.geometry.html#satsim.geometry.sgp4.load_tle"><code class="docutils literal notranslate"><span class="pre">load_tle()</span></code></a></li>
@@ -404,14 +410,18 @@
 <li class="toctree-l2"><a class="reference internal" href="satsim.time.html#satsim.time.utc"><code class="docutils literal notranslate"><span class="pre">utc()</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="satsim.time.html#satsim.time.utc_from_list"><code class="docutils literal notranslate"><span class="pre">utc_from_list()</span></code></a></li>
 <li class="toctree-l2"><a class="reference internal" href="satsim.time.html#satsim.time.utc_from_list_or_scalar"><code class="docutils literal notranslate"><span class="pre">utc_from_list_or_scalar()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="satsim.util.html">satsim.util package</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="satsim.util.html#submodules">Submodules</a></li>
+<li class="toctree-l2"><a class="reference internal" href="satsim.util.html#module-satsim.util.python">satsim.util.python module</a><ul>
+<li class="toctree-l3"><a class="reference internal" href="satsim.util.html#satsim.util.python.merge_dicts"><code class="docutils literal notranslate"><span class="pre">merge_dicts()</span></code></a></li>
+</ul>
+</li>
 <li class="toctree-l2"><a class="reference internal" href="satsim.util.html#module-satsim.util.system">satsim.util.system module</a><ul>
 <li class="toctree-l3"><a class="reference internal" href="satsim.util.html#satsim.util.system.configure_eager"><code class="docutils literal notranslate"><span class="pre">configure_eager()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.util.html#satsim.util.system.configure_multi_gpu"><code class="docutils literal notranslate"><span class="pre">configure_multi_gpu()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.util.html#satsim.util.system.configure_single_gpu"><code class="docutils literal notranslate"><span class="pre">configure_single_gpu()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.util.html#satsim.util.system.get_semantic_version"><code class="docutils literal notranslate"><span class="pre">get_semantic_version()</span></code></a></li>
 <li class="toctree-l3"><a class="reference internal" href="satsim.util.html#satsim.util.system.is_tensorflow_running_on_cpu"><code class="docutils literal notranslate"><span class="pre">is_tensorflow_running_on_cpu()</span></code></a></li>
 </ul>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _S_a_t_S_i_m
-0.18.0
+0.19.0
 [q                   ]
 Contents:
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _U_s_a_g_e
     * _C_o_n_t_r_i_b_u_t_i_n_g
     * _A_P_I_ _D_o_c_u_m_e_n_t_a_t_i_o_n
           o _s_a_t_s_i_m_ _p_a_c_k_a_g_e
@@ -68,21 +68,21 @@
           o _S_u_b_m_o_d_u_l_e_s
           o _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._a_s_t_r_o_m_e_t_r_i_c_ _m_o_d_u_l_e
                 # _G_r_e_a_t_C_i_r_c_l_e
                 # _a_n_g_l_e___b_e_t_w_e_e_n_(_)
                 # _a_n_g_l_e___f_r_o_m___l_o_s_(_)
                 # _a_p_p_a_r_e_n_t_(_)
                 # _c_r_e_a_t_e___t_o_p_o_c_e_n_t_r_i_c_(_)
+                # _d_i_s_t_a_n_c_e___b_e_t_w_e_e_n_(_)
                 # _e_c_i___t_o___e_c_r_(_)
                 # _e_c_i___t_o___r_a_d_e_c_(_)
                 # _g_e_n___t_r_a_c_k_(_)
                 # _g_e_n___t_r_a_c_k___f_r_o_m___w_c_s_(_)
                 # _g_e_t___l_o_s_(_)
                 # _g_e_t___l_o_s___a_z_e_l_(_)
-                # _l_a_m_b_e_r_t_i_a_n___s_p_h_e_r_e___t_o___m_v_(_)
                 # _l_o_a_d___e_a_r_t_h_(_)
                 # _l_o_a_d___m_o_o_n_(_)
                 # _l_o_a_d___s_u_n_(_)
                 # _q_u_e_r_y___b_y___l_o_s_(_)
                 # _r_a_d_e_c___t_o___e_c_i_(_)
                 # _w_c_s___f_r_o_m___o_b_s_e_r_v_e_r___f_i_x_e_d_(_)
                 # _w_c_s___f_r_o_m___o_b_s_e_r_v_e_r___r_a_t_e_(_)
@@ -96,14 +96,18 @@
           o _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._e_p_h_e_m_e_r_i_s_ _m_o_d_u_l_e
                 # _E_p_h_e_m_e_r_i_s_O_b_j_e_c_t
                       # _E_p_h_e_m_e_r_i_s_O_b_j_e_c_t_._c_e_n_t_e_r
                 # _c_r_e_a_t_e___e_p_h_e_m_e_r_i_s___o_b_j_e_c_t_(_)
           o _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._o_b_s_e_r_v_a_t_i_o_n_ _m_o_d_u_l_e
                 # _E_a_r_t_h_O_b_s_e_r_v_a_t_i_o_n
                 # _c_r_e_a_t_e___o_b_s_e_r_v_a_t_i_o_n_(_)
+          o _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._p_h_o_t_o_m_e_t_r_i_c_ _m_o_d_u_l_e
+                # _l_a_m_b_e_r_t_i_a_n___s_p_h_e_r_e___m_o_d_e_l___t_o___m_v_(_)
+                # _l_a_m_b_e_r_t_i_a_n___s_p_h_e_r_e___t_o___m_v_(_)
+                # _m_o_d_e_l___t_o___m_v_(_)
           o _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._r_a_n_d_o_m_ _m_o_d_u_l_e
                 # _g_e_n___r_a_n_d_o_m___p_o_i_n_t_s_(_)
           o _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._s_g_p_4_ _m_o_d_u_l_e
                 # _c_r_e_a_t_e___s_g_p_4_(_)
                 # _l_o_a_d___t_l_e_(_)
           o _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._s_p_r_i_t_e_ _m_o_d_u_l_e
                 # _l_o_a_d___s_p_r_i_t_e___f_r_o_m___f_i_l_e_(_)
@@ -233,14 +237,16 @@
           o _t_o___a_s_t_r_o_p_y_(_)
           o _t_o___u_t_c___l_i_s_t_(_)
           o _u_t_c_(_)
           o _u_t_c___f_r_o_m___l_i_s_t_(_)
           o _u_t_c___f_r_o_m___l_i_s_t___o_r___s_c_a_l_a_r_(_)
     * _s_a_t_s_i_m_._u_t_i_l_ _p_a_c_k_a_g_e
           o _S_u_b_m_o_d_u_l_e_s
+          o _s_a_t_s_i_m_._u_t_i_l_._p_y_t_h_o_n_ _m_o_d_u_l_e
+                # _m_e_r_g_e___d_i_c_t_s_(_)
           o _s_a_t_s_i_m_._u_t_i_l_._s_y_s_t_e_m_ _m_o_d_u_l_e
                 # _c_o_n_f_i_g_u_r_e___e_a_g_e_r_(_)
                 # _c_o_n_f_i_g_u_r_e___m_u_l_t_i___g_p_u_(_)
                 # _c_o_n_f_i_g_u_r_e___s_i_n_g_l_e___g_p_u_(_)
                 # _g_e_t___s_e_m_a_n_t_i_c___v_e_r_s_i_o_n_(_)
                 # _i_s___t_e_n_s_o_r_f_l_o_w___r_u_n_n_i_n_g___o_n___c_p_u_(_)
           o _s_a_t_s_i_m_._u_t_i_l_._t_h_r_e_a_d_ _m_o_d_u_l_e
```

### Comparing `satsim-0.18.0/docs/_build/html/api/satsim.image.html` & `satsim-0.19.0/docs/_build/html/api/satsim.image.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.image package &mdash; SatSim 0.18.0 documentation</title>
+  <title>satsim.image package &mdash; SatSim 0.19.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.18.0
+                0.19.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _S_a_t_S_i_m
-0.18.0
+0.19.0
 [q                   ]
 Contents:
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _U_s_a_g_e
     * _C_o_n_t_r_i_b_u_t_i_n_g
     * _A_P_I_ _D_o_c_u_m_e_n_t_a_t_i_o_n
           o _s_a_t_s_i_m_ _p_a_c_k_a_g_e
```

### Comparing `satsim-0.18.0/docs/_build/html/api/satsim.io.html` & `satsim-0.19.0/docs/_build/html/api/satsim.io.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.io package &mdash; SatSim 0.18.0 documentation</title>
+  <title>satsim.io package &mdash; SatSim 0.19.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.18.0
+                0.19.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -189,15 +189,15 @@
 </dd></dl>
 
 </section>
 <section id="module-satsim.io.fits">
 <span id="satsim-io-fits-module"></span><h2>satsim.io.fits module<a class="headerlink" href="#module-satsim.io.fits" title="Permalink to this heading"></a></h2>
 <dl class="py function">
 <dt class="sig sig-object py" id="satsim.io.fits.save">
-<span class="sig-prename descclassname"><span class="pre">satsim.io.fits.</span></span><span class="sig-name descname"><span class="pre">save</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">filename</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fpa</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exposure_time</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dt_start</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">datetime.datetime(2024,</span> <span class="pre">3,</span> <span class="pre">23,</span> <span class="pre">7,</span> <span class="pre">33,</span> <span class="pre">44,</span> <span class="pre">552367)</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">header</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">{}</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">overwrite</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dtype</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'uint16'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">astrometrics</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.io.fits.save" title="Permalink to this definition"></a></dt>
+<span class="sig-prename descclassname"><span class="pre">satsim.io.fits.</span></span><span class="sig-name descname"><span class="pre">save</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">filename</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">fpa</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">exposure_time</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">0</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dt_start</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">datetime.datetime(2024,</span> <span class="pre">5,</span> <span class="pre">29,</span> <span class="pre">8,</span> <span class="pre">14,</span> <span class="pre">48,</span> <span class="pre">994133)</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">header</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">{}</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">overwrite</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">False</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">dtype</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">'uint16'</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">astrometrics</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">None</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.io.fits.save" title="Permalink to this definition"></a></dt>
 <dd><p>Save a SatNet compatible FITS file.</p>
 <dl class="field-list simple">
 <dt class="field-odd">Parameters<span class="colon">:</span></dt>
 <dd class="field-odd"><ul class="simple">
 <li><p><strong>filename</strong> – <cite>string</cite>, the FITS filename.</p></li>
 <li><p><strong>fpa</strong> – <cite>np.array</cite>, input image as a 2D numpy array.</p></li>
 <li><p><strong>exposure_time</strong> – <cite>float</cite>, exposure time for header.</p></li>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _S_a_t_S_i_m
-0.18.0
+0.19.0
 [q                   ]
 Contents:
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _U_s_a_g_e
     * _C_o_n_t_r_i_b_u_t_i_n_g
     * _A_P_I_ _D_o_c_u_m_e_n_t_a_t_i_o_n
           o _s_a_t_s_i_m_ _p_a_c_k_a_g_e
@@ -98,15 +98,15 @@
                 * sssspp –dict, SatSim input configuration.
                 * oobbss__ccaacchhee –list, list of SatSim Skyfield objects.
                 * ffiilleennaammee –str, if not None, save czml output. default=None
         Returns:
             Adict, the CZML output
 ********** ssaattssiimm..iioo..ffiittss mmoodduullee_? **********
   satsim.io.fits.save(ffiilleennaammee, ffppaa, eexxppoossuurree__ttiimmee==00,
-  ddtt__ssttaarrtt==ddaatteettiimmee..ddaatteettiimmee((22002244,, 33,, 2233,, 77,, 3333,, 4444,, 555522336677)), hheeaaddeerr=={{}},
+  ddtt__ssttaarrtt==ddaatteettiimmee..ddaatteettiimmee((22002244,, 55,, 2299,, 88,, 1144,, 4488,, 999944113333)), hheeaaddeerr=={{}},
   oovveerrwwrriittee==FFaallssee, ddttyyppee==''uuiinntt1166'', aassttrroommeettrriiccss==NNoonnee)_
       Save a SatNet compatible FITS file.
         Parameters:
                 * ffiilleennaammee –string, the FITS filename.
                 * ffppaa –np.array, input image as a 2D numpy array.
                 * eexxppoossuurree__ttiimmee –float, exposure time for header.
                 * ddtt__ssttaarrtt –datetime, datetime of start of exposure.
```

### Comparing `satsim-0.18.0/docs/_build/html/api/satsim.math.html` & `satsim-0.19.0/docs/_build/html/api/satsim.math.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.math package &mdash; SatSim 0.18.0 documentation</title>
+  <title>satsim.math package &mdash; SatSim 0.19.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.18.0
+                0.19.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _S_a_t_S_i_m
-0.18.0
+0.19.0
 [q                   ]
 Contents:
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _U_s_a_g_e
     * _C_o_n_t_r_i_b_u_t_i_n_g
     * _A_P_I_ _D_o_c_u_m_e_n_t_a_t_i_o_n
           o _s_a_t_s_i_m_ _p_a_c_k_a_g_e
```

### Comparing `satsim-0.18.0/docs/_build/html/api/satsim.pipeline.html` & `satsim-0.19.0/docs/_build/html/api/satsim.pipeline.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.pipeline package &mdash; SatSim 0.18.0 documentation</title>
+  <title>satsim.pipeline package &mdash; SatSim 0.19.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.18.0
+                0.19.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _S_a_t_S_i_m
-0.18.0
+0.19.0
 [q                   ]
 Contents:
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _U_s_a_g_e
     * _C_o_n_t_r_i_b_u_t_i_n_g
     * _A_P_I_ _D_o_c_u_m_e_n_t_a_t_i_o_n
           o _s_a_t_s_i_m_ _p_a_c_k_a_g_e
```

### Comparing `satsim-0.18.0/docs/_build/html/api/satsim.tfa.html` & `satsim-0.19.0/docs/_build/html/api/satsim.tfa.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.tfa package &mdash; SatSim 0.18.0 documentation</title>
+  <title>satsim.tfa package &mdash; SatSim 0.19.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.18.0
+                0.19.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _S_a_t_S_i_m
-0.18.0
+0.19.0
 [q                   ]
 Contents:
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _U_s_a_g_e
     * _C_o_n_t_r_i_b_u_t_i_n_g
     * _A_P_I_ _D_o_c_u_m_e_n_t_a_t_i_o_n
           o _s_a_t_s_i_m_ _p_a_c_k_a_g_e
```

### Comparing `satsim-0.18.0/docs/_build/html/api/satsim.tfa.image.html` & `satsim-0.19.0/docs/_build/html/api/satsim.tfa.image.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.tfa.image package &mdash; SatSim 0.18.0 documentation</title>
+  <title>satsim.tfa.image package &mdash; SatSim 0.19.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.18.0
+                0.19.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _S_a_t_S_i_m
-0.18.0
+0.19.0
 [q                   ]
 Contents:
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _U_s_a_g_e
     * _C_o_n_t_r_i_b_u_t_i_n_g
     * _A_P_I_ _D_o_c_u_m_e_n_t_a_t_i_o_n
           o _s_a_t_s_i_m_ _p_a_c_k_a_g_e
```

### Comparing `satsim-0.18.0/docs/_build/html/api/satsim.tfa.utils.html` & `satsim-0.19.0/docs/_build/html/api/satsim.tfa.utils.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.tfa.utils package &mdash; SatSim 0.18.0 documentation</title>
+  <title>satsim.tfa.utils package &mdash; SatSim 0.19.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.18.0
+                0.19.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _S_a_t_S_i_m
-0.18.0
+0.19.0
 [q                   ]
 Contents:
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _U_s_a_g_e
     * _C_o_n_t_r_i_b_u_t_i_n_g
     * _A_P_I_ _D_o_c_u_m_e_n_t_a_t_i_o_n
           o _s_a_t_s_i_m_ _p_a_c_k_a_g_e
```

### Comparing `satsim-0.18.0/docs/_build/html/api/satsim.time.html` & `satsim-0.19.0/docs/_build/html/api/satsim.time.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.time package &mdash; SatSim 0.18.0 documentation</title>
+  <title>satsim.time package &mdash; SatSim 0.19.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.18.0
+                0.19.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _S_a_t_S_i_m
-0.18.0
+0.19.0
 [q                   ]
 Contents:
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _U_s_a_g_e
     * _C_o_n_t_r_i_b_u_t_i_n_g
     * _A_P_I_ _D_o_c_u_m_e_n_t_a_t_i_o_n
           o _s_a_t_s_i_m_ _p_a_c_k_a_g_e
```

### Comparing `satsim-0.18.0/docs/_build/html/api/satsim.util.html` & `satsim-0.19.0/docs/_build/html/api/satsim.util.html`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.util package &mdash; SatSim 0.18.0 documentation</title>
+  <title>satsim.util package &mdash; SatSim 0.19.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.18.0
+                0.19.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -103,14 +103,46 @@
            <div itemprop="articleBody">
              
   <section id="module-satsim.util">
 <span id="satsim-util-package"></span><h1>satsim.util package<a class="headerlink" href="#module-satsim.util" title="Permalink to this heading"></a></h1>
 <section id="submodules">
 <h2>Submodules<a class="headerlink" href="#submodules" title="Permalink to this heading"></a></h2>
 </section>
+<section id="module-satsim.util.python">
+<span id="satsim-util-python-module"></span><h2>satsim.util.python module<a class="headerlink" href="#module-satsim.util.python" title="Permalink to this heading"></a></h2>
+<dl class="py function">
+<dt class="sig sig-object py" id="satsim.util.python.merge_dicts">
+<span class="sig-prename descclassname"><span class="pre">satsim.util.python.</span></span><span class="sig-name descname"><span class="pre">merge_dicts</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">d1</span></span></em>, <em class="sig-param"><span class="n"><span class="pre">d2</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.util.python.merge_dicts" title="Permalink to this definition"></a></dt>
+<dd><p>Recursively merges dictionary d2 into dictionary d1.</p>
+<p>If both dictionaries have a nested dictionary at the same key, this function
+will recursively merge those nested dictionaries. If there is a conflict
+where d1 has a dictionary and d2 has a non-dictionary value at the same key,
+the value from d2 will overwrite the one in d1.</p>
+<dl class="field-list simple">
+<dt class="field-odd">Parameters<span class="colon">:</span></dt>
+<dd class="field-odd"><ul class="simple">
+<li><p><strong>d1</strong> (<em>dict</em>) – The dictionary to be updated.</p></li>
+<li><p><strong>d2</strong> (<em>dict</em>) – The dictionary with updates to merge into d1.</p></li>
+</ul>
+</dd>
+<dt class="field-even">Returns<span class="colon">:</span></dt>
+<dd class="field-even"><p>The function updates d1 in place.</p>
+</dd>
+<dt class="field-odd">Return type<span class="colon">:</span></dt>
+<dd class="field-odd"><p>None</p>
+</dd>
+</dl>
+<p class="rubric">Example</p>
+<p>d1 = {‘a’: 1, ‘b’: {‘x’: 10}}
+d2 = {‘b’: {‘y’: 20}, ‘c’: 3}
+merge_dicts(d1, d2)
+# d1 is now {‘a’: 1, ‘b’: {‘x’: 10, ‘y’: 20}, ‘c’: 3}</p>
+</dd></dl>
+
+</section>
 <section id="module-satsim.util.system">
 <span id="satsim-util-system-module"></span><h2>satsim.util.system module<a class="headerlink" href="#module-satsim.util.system" title="Permalink to this heading"></a></h2>
 <dl class="py function">
 <dt class="sig sig-object py" id="satsim.util.system.configure_eager">
 <span class="sig-prename descclassname"><span class="pre">satsim.util.system.</span></span><span class="sig-name descname"><span class="pre">configure_eager</span></span><span class="sig-paren">(</span><em class="sig-param"><span class="n"><span class="pre">allow_growth</span></span><span class="o"><span class="pre">=</span></span><span class="default_value"><span class="pre">True</span></span></em><span class="sig-paren">)</span><a class="headerlink" href="#satsim.util.system.configure_eager" title="Permalink to this definition"></a></dt>
 <dd><p>Configure TensorFlow in eager mode.</p>
 <dl class="field-list simple">
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _S_a_t_S_i_m
-0.18.0
+0.19.0
 [q                   ]
 Contents:
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _U_s_a_g_e
     * _C_o_n_t_r_i_b_u_t_i_n_g
     * _A_P_I_ _D_o_c_u_m_e_n_t_a_t_i_o_n
           o _s_a_t_s_i_m_ _p_a_c_k_a_g_e
@@ -29,14 +29,31 @@
     * _A_P_I_ _D_o_c_u_m_e_n_t_a_t_i_o_n
     * _s_a_t_s_i_m_ _p_a_c_k_a_g_e
     * satsim.util package
     * _V_i_e_w_ _p_a_g_e_ _s_o_u_r_c_e
 ===============================================================================
 ************ ssaattssiimm..uuttiill ppaacckkaaggee_? ************
 ********** SSuubbmmoodduulleess_? **********
+********** ssaattssiimm..uuttiill..ppyytthhoonn mmoodduullee_? **********
+  satsim.util.python.merge_dicts(dd11, dd22)_
+      Recursively merges dictionary d2 into dictionary d1.
+      If both dictionaries have a nested dictionary at the same key, this
+      function will recursively merge those nested dictionaries. If there is a
+      conflict where d1 has a dictionary and d2 has a non-dictionary value at
+      the same key, the value from d2 will overwrite the one in d1.
+        Parameters:
+                * dd11 (ddiicctt) – The dictionary to be updated.
+                * dd22 (ddiicctt) – The dictionary with updates to merge into d1.
+        Returns:
+            The function updates d1 in place.
+        Return type:
+            None
+      Example
+      d1 = {‘a’: 1, ‘b’: {‘x’: 10}} d2 = {‘b’: {‘y’: 20}, ‘c’: 3} merge_dicts
+      (d1, d2) # d1 is now {‘a’: 1, ‘b’: {‘x’: 10, ‘y’: 20}, ‘c’: 3}
 ********** ssaattssiimm..uuttiill..ssyysstteemm mmoodduullee_? **********
   satsim.util.system.configure_eager(aallllooww__ggrroowwtthh==TTrruuee)_
       Configure TensorFlow in eager mode.
         Parameters:
             aallllooww__ggrroowwtthh –bool, enables memory growth
   satsim.util.system.configure_multi_gpu(ggppuu__iiddss, mmeemmoorryy==NNoonnee)_
       Configure multiple GPUs to be visible and limit their maximum memory
```

### Comparing `satsim-0.18.0/docs/_build/html/api/satsim.vecmath.html` & `satsim-0.19.0/docs/_build/html/api/satsim.vecmath.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>satsim.vecmath package &mdash; SatSim 0.18.0 documentation</title>
+  <title>satsim.vecmath package &mdash; SatSim 0.19.0 documentation</title>
       <link rel="stylesheet" href="../_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="../_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="../_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="../index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.18.0
+                0.19.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="../search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _S_a_t_S_i_m
-0.18.0
+0.19.0
 [q                   ]
 Contents:
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _U_s_a_g_e
     * _C_o_n_t_r_i_b_u_t_i_n_g
     * _A_P_I_ _D_o_c_u_m_e_n_t_a_t_i_o_n
           o _s_a_t_s_i_m_ _p_a_c_k_a_g_e
```

### Comparing `satsim-0.18.0/docs/_build/html/api.html` & `satsim-0.19.0/docs/_build/html/api.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>API Documentation &mdash; SatSim 0.18.0 documentation</title>
+  <title>API Documentation &mdash; SatSim 0.19.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.18.0
+                0.19.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -132,21 +132,21 @@
 <li class="toctree-l4"><a class="reference internal" href="api/satsim.geometry.html#submodules">Submodules</a></li>
 <li class="toctree-l4"><a class="reference internal" href="api/satsim.geometry.html#module-satsim.geometry.astrometric">satsim.geometry.astrometric module</a><ul>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.astrometric.GreatCircle"><code class="docutils literal notranslate"><span class="pre">GreatCircle</span></code></a></li>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.astrometric.angle_between"><code class="docutils literal notranslate"><span class="pre">angle_between()</span></code></a></li>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.astrometric.angle_from_los"><code class="docutils literal notranslate"><span class="pre">angle_from_los()</span></code></a></li>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.astrometric.apparent"><code class="docutils literal notranslate"><span class="pre">apparent()</span></code></a></li>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.astrometric.create_topocentric"><code class="docutils literal notranslate"><span class="pre">create_topocentric()</span></code></a></li>
+<li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.astrometric.distance_between"><code class="docutils literal notranslate"><span class="pre">distance_between()</span></code></a></li>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.astrometric.eci_to_ecr"><code class="docutils literal notranslate"><span class="pre">eci_to_ecr()</span></code></a></li>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.astrometric.eci_to_radec"><code class="docutils literal notranslate"><span class="pre">eci_to_radec()</span></code></a></li>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.astrometric.gen_track"><code class="docutils literal notranslate"><span class="pre">gen_track()</span></code></a></li>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.astrometric.gen_track_from_wcs"><code class="docutils literal notranslate"><span class="pre">gen_track_from_wcs()</span></code></a></li>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.astrometric.get_los"><code class="docutils literal notranslate"><span class="pre">get_los()</span></code></a></li>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.astrometric.get_los_azel"><code class="docutils literal notranslate"><span class="pre">get_los_azel()</span></code></a></li>
-<li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.astrometric.lambertian_sphere_to_mv"><code class="docutils literal notranslate"><span class="pre">lambertian_sphere_to_mv()</span></code></a></li>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.astrometric.load_earth"><code class="docutils literal notranslate"><span class="pre">load_earth()</span></code></a></li>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.astrometric.load_moon"><code class="docutils literal notranslate"><span class="pre">load_moon()</span></code></a></li>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.astrometric.load_sun"><code class="docutils literal notranslate"><span class="pre">load_sun()</span></code></a></li>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.astrometric.query_by_los"><code class="docutils literal notranslate"><span class="pre">query_by_los()</span></code></a></li>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.astrometric.radec_to_eci"><code class="docutils literal notranslate"><span class="pre">radec_to_eci()</span></code></a></li>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.astrometric.wcs_from_observer_fixed"><code class="docutils literal notranslate"><span class="pre">wcs_from_observer_fixed()</span></code></a></li>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.astrometric.wcs_from_observer_rate"><code class="docutils literal notranslate"><span class="pre">wcs_from_observer_rate()</span></code></a></li>
@@ -172,14 +172,20 @@
 </ul>
 </li>
 <li class="toctree-l4"><a class="reference internal" href="api/satsim.geometry.html#module-satsim.geometry.observation">satsim.geometry.observation module</a><ul>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.observation.EarthObservation"><code class="docutils literal notranslate"><span class="pre">EarthObservation</span></code></a></li>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.observation.create_observation"><code class="docutils literal notranslate"><span class="pre">create_observation()</span></code></a></li>
 </ul>
 </li>
+<li class="toctree-l4"><a class="reference internal" href="api/satsim.geometry.html#module-satsim.geometry.photometric">satsim.geometry.photometric module</a><ul>
+<li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.photometric.lambertian_sphere_model_to_mv"><code class="docutils literal notranslate"><span class="pre">lambertian_sphere_model_to_mv()</span></code></a></li>
+<li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.photometric.lambertian_sphere_to_mv"><code class="docutils literal notranslate"><span class="pre">lambertian_sphere_to_mv()</span></code></a></li>
+<li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.photometric.model_to_mv"><code class="docutils literal notranslate"><span class="pre">model_to_mv()</span></code></a></li>
+</ul>
+</li>
 <li class="toctree-l4"><a class="reference internal" href="api/satsim.geometry.html#module-satsim.geometry.random">satsim.geometry.random module</a><ul>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.random.gen_random_points"><code class="docutils literal notranslate"><span class="pre">gen_random_points()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l4"><a class="reference internal" href="api/satsim.geometry.html#module-satsim.geometry.sgp4">satsim.geometry.sgp4 module</a><ul>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.sgp4.create_sgp4"><code class="docutils literal notranslate"><span class="pre">create_sgp4()</span></code></a></li>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.geometry.html#satsim.geometry.sgp4.load_tle"><code class="docutils literal notranslate"><span class="pre">load_tle()</span></code></a></li>
@@ -405,14 +411,18 @@
 <li class="toctree-l4"><a class="reference internal" href="api/satsim.time.html#satsim.time.utc"><code class="docutils literal notranslate"><span class="pre">utc()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="api/satsim.time.html#satsim.time.utc_from_list"><code class="docutils literal notranslate"><span class="pre">utc_from_list()</span></code></a></li>
 <li class="toctree-l4"><a class="reference internal" href="api/satsim.time.html#satsim.time.utc_from_list_or_scalar"><code class="docutils literal notranslate"><span class="pre">utc_from_list_or_scalar()</span></code></a></li>
 </ul>
 </li>
 <li class="toctree-l3"><a class="reference internal" href="api/satsim.util.html">satsim.util package</a><ul>
 <li class="toctree-l4"><a class="reference internal" href="api/satsim.util.html#submodules">Submodules</a></li>
+<li class="toctree-l4"><a class="reference internal" href="api/satsim.util.html#module-satsim.util.python">satsim.util.python module</a><ul>
+<li class="toctree-l5"><a class="reference internal" href="api/satsim.util.html#satsim.util.python.merge_dicts"><code class="docutils literal notranslate"><span class="pre">merge_dicts()</span></code></a></li>
+</ul>
+</li>
 <li class="toctree-l4"><a class="reference internal" href="api/satsim.util.html#module-satsim.util.system">satsim.util.system module</a><ul>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.util.html#satsim.util.system.configure_eager"><code class="docutils literal notranslate"><span class="pre">configure_eager()</span></code></a></li>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.util.html#satsim.util.system.configure_multi_gpu"><code class="docutils literal notranslate"><span class="pre">configure_multi_gpu()</span></code></a></li>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.util.html#satsim.util.system.configure_single_gpu"><code class="docutils literal notranslate"><span class="pre">configure_single_gpu()</span></code></a></li>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.util.html#satsim.util.system.get_semantic_version"><code class="docutils literal notranslate"><span class="pre">get_semantic_version()</span></code></a></li>
 <li class="toctree-l5"><a class="reference internal" href="api/satsim.util.html#satsim.util.system.is_tensorflow_running_on_cpu"><code class="docutils literal notranslate"><span class="pre">is_tensorflow_running_on_cpu()</span></code></a></li>
 </ul>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _S_a_t_S_i_m
-0.18.0
+0.19.0
 [q                   ]
 Contents:
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _U_s_a_g_e
     * _C_o_n_t_r_i_b_u_t_i_n_g
     * _A_P_I_ _D_o_c_u_m_e_n_t_a_t_i_o_n
           o _s_a_t_s_i_m_ _p_a_c_k_a_g_e
@@ -42,21 +42,21 @@
                       # _S_u_b_m_o_d_u_l_e_s
                       # _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._a_s_t_r_o_m_e_t_r_i_c_ _m_o_d_u_l_e
                             # _G_r_e_a_t_C_i_r_c_l_e
                             # _a_n_g_l_e___b_e_t_w_e_e_n_(_)
                             # _a_n_g_l_e___f_r_o_m___l_o_s_(_)
                             # _a_p_p_a_r_e_n_t_(_)
                             # _c_r_e_a_t_e___t_o_p_o_c_e_n_t_r_i_c_(_)
+                            # _d_i_s_t_a_n_c_e___b_e_t_w_e_e_n_(_)
                             # _e_c_i___t_o___e_c_r_(_)
                             # _e_c_i___t_o___r_a_d_e_c_(_)
                             # _g_e_n___t_r_a_c_k_(_)
                             # _g_e_n___t_r_a_c_k___f_r_o_m___w_c_s_(_)
                             # _g_e_t___l_o_s_(_)
                             # _g_e_t___l_o_s___a_z_e_l_(_)
-                            # _l_a_m_b_e_r_t_i_a_n___s_p_h_e_r_e___t_o___m_v_(_)
                             # _l_o_a_d___e_a_r_t_h_(_)
                             # _l_o_a_d___m_o_o_n_(_)
                             # _l_o_a_d___s_u_n_(_)
                             # _q_u_e_r_y___b_y___l_o_s_(_)
                             # _r_a_d_e_c___t_o___e_c_i_(_)
                             # _w_c_s___f_r_o_m___o_b_s_e_r_v_e_r___f_i_x_e_d_(_)
                             # _w_c_s___f_r_o_m___o_b_s_e_r_v_e_r___r_a_t_e_(_)
@@ -70,14 +70,18 @@
                       # _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._e_p_h_e_m_e_r_i_s_ _m_o_d_u_l_e
                             # _E_p_h_e_m_e_r_i_s_O_b_j_e_c_t
                                   # _E_p_h_e_m_e_r_i_s_O_b_j_e_c_t_._c_e_n_t_e_r
                             # _c_r_e_a_t_e___e_p_h_e_m_e_r_i_s___o_b_j_e_c_t_(_)
                       # _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._o_b_s_e_r_v_a_t_i_o_n_ _m_o_d_u_l_e
                             # _E_a_r_t_h_O_b_s_e_r_v_a_t_i_o_n
                             # _c_r_e_a_t_e___o_b_s_e_r_v_a_t_i_o_n_(_)
+                      # _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._p_h_o_t_o_m_e_t_r_i_c_ _m_o_d_u_l_e
+                            # _l_a_m_b_e_r_t_i_a_n___s_p_h_e_r_e___m_o_d_e_l___t_o___m_v_(_)
+                            # _l_a_m_b_e_r_t_i_a_n___s_p_h_e_r_e___t_o___m_v_(_)
+                            # _m_o_d_e_l___t_o___m_v_(_)
                       # _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._r_a_n_d_o_m_ _m_o_d_u_l_e
                             # _g_e_n___r_a_n_d_o_m___p_o_i_n_t_s_(_)
                       # _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._s_g_p_4_ _m_o_d_u_l_e
                             # _c_r_e_a_t_e___s_g_p_4_(_)
                             # _l_o_a_d___t_l_e_(_)
                       # _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._s_p_r_i_t_e_ _m_o_d_u_l_e
                             # _l_o_a_d___s_p_r_i_t_e___f_r_o_m___f_i_l_e_(_)
@@ -226,14 +230,16 @@
                       # _t_o___a_s_t_r_o_p_y_(_)
                       # _t_o___u_t_c___l_i_s_t_(_)
                       # _u_t_c_(_)
                       # _u_t_c___f_r_o_m___l_i_s_t_(_)
                       # _u_t_c___f_r_o_m___l_i_s_t___o_r___s_c_a_l_a_r_(_)
                 # _s_a_t_s_i_m_._u_t_i_l_ _p_a_c_k_a_g_e
                       # _S_u_b_m_o_d_u_l_e_s
+                      # _s_a_t_s_i_m_._u_t_i_l_._p_y_t_h_o_n_ _m_o_d_u_l_e
+                            # _m_e_r_g_e___d_i_c_t_s_(_)
                       # _s_a_t_s_i_m_._u_t_i_l_._s_y_s_t_e_m_ _m_o_d_u_l_e
                             # _c_o_n_f_i_g_u_r_e___e_a_g_e_r_(_)
                             # _c_o_n_f_i_g_u_r_e___m_u_l_t_i___g_p_u_(_)
                             # _c_o_n_f_i_g_u_r_e___s_i_n_g_l_e___g_p_u_(_)
                             # _g_e_t___s_e_m_a_n_t_i_c___v_e_r_s_i_o_n_(_)
                             # _i_s___t_e_n_s_o_r_f_l_o_w___r_u_n_n_i_n_g___o_n___c_p_u_(_)
                       # _s_a_t_s_i_m_._u_t_i_l_._t_h_r_e_a_d_ _m_o_d_u_l_e
```

### Comparing `satsim-0.18.0/docs/_build/html/authors.html` & `satsim-0.19.0/docs/_build/html/authors.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Credits &mdash; SatSim 0.18.0 documentation</title>
+  <title>Credits &mdash; SatSim 0.19.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.18.0
+                0.19.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _S_a_t_S_i_m
-0.18.0
+0.19.0
 [q                   ]
 Contents:
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _U_s_a_g_e
     * _C_o_n_t_r_i_b_u_t_i_n_g
     * _A_P_I_ _D_o_c_u_m_e_n_t_a_t_i_o_n
     * _C_r_e_d_i_t_s
```

### Comparing `satsim-0.18.0/docs/_build/html/contributing.html` & `satsim-0.19.0/docs/_build/html/contributing.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Contributing &mdash; SatSim 0.18.0 documentation</title>
+  <title>Contributing &mdash; SatSim 0.19.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.18.0
+                0.19.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _S_a_t_S_i_m
-0.18.0
+0.19.0
 [q                   ]
 Contents:
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _U_s_a_g_e
     * _C_o_n_t_r_i_b_u_t_i_n_g
           o _G_e_t_t_i_n_g_ _S_t_a_r_t_e_d_ _f_o_r_ _D_e_v_e_l_o_p_e_r_s
           o _M_e_r_g_e_ _R_e_q_u_e_s_t_ _G_u_i_d_e_l_i_n_e_s
```

### Comparing `satsim-0.18.0/docs/_build/html/genindex.html` & `satsim-0.19.0/docs/_build/html/genindex.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Index &mdash; SatSim 0.18.0 documentation</title>
+  <title>Index &mdash; SatSim 0.19.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -26,15 +26,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.18.0
+                0.19.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -393,34 +393,36 @@
 
       <ul>
         <li><a href="api/satsim.vecmath.html#satsim.vecmath.Cartesian3.Cartesian3.distance">(satsim.vecmath.Cartesian3.Cartesian3 static method)</a>
 </li>
         <li><a href="api/satsim.vecmath.html#satsim.vecmath.Cartesian4.Cartesian4.distance">(satsim.vecmath.Cartesian4.Cartesian4 static method)</a>
 </li>
       </ul></li>
+      <li><a href="api/satsim.geometry.html#satsim.geometry.astrometric.distance_between">distance_between() (in module satsim.geometry.astrometric)</a>
+</li>
       <li><a href="api/satsim.vecmath.html#satsim.vecmath.Cartesian2.Cartesian2.distanceSquared">distanceSquared() (satsim.vecmath.Cartesian2.Cartesian2 static method)</a>
 
       <ul>
         <li><a href="api/satsim.vecmath.html#satsim.vecmath.Cartesian3.Cartesian3.distanceSquared">(satsim.vecmath.Cartesian3.Cartesian3 static method)</a>
 </li>
         <li><a href="api/satsim.vecmath.html#satsim.vecmath.Cartesian4.Cartesian4.distanceSquared">(satsim.vecmath.Cartesian4.Cartesian4 static method)</a>
 </li>
       </ul></li>
+  </ul></td>
+  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api/satsim.vecmath.html#satsim.vecmath.Cartesian2.Cartesian2.divideByScalar">divideByScalar() (satsim.vecmath.Cartesian2.Cartesian2 static method)</a>
 
       <ul>
         <li><a href="api/satsim.vecmath.html#satsim.vecmath.Cartesian3.Cartesian3.divideByScalar">(satsim.vecmath.Cartesian3.Cartesian3 static method)</a>
 </li>
         <li><a href="api/satsim.vecmath.html#satsim.vecmath.Cartesian4.Cartesian4.divideByScalar">(satsim.vecmath.Cartesian4.Cartesian4 static method)</a>
 </li>
         <li><a href="api/satsim.vecmath.html#satsim.vecmath.Quaternion.Quaternion.divideByScalar">(satsim.vecmath.Quaternion.Quaternion static method)</a>
 </li>
       </ul></li>
-  </ul></td>
-  <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api/satsim.vecmath.html#satsim.vecmath.Cartesian2.Cartesian2.divideComponents">divideComponents() (satsim.vecmath.Cartesian2.Cartesian2 static method)</a>
 
       <ul>
         <li><a href="api/satsim.vecmath.html#satsim.vecmath.Cartesian3.Cartesian3.divideComponents">(satsim.vecmath.Cartesian3.Cartesian3 static method)</a>
 </li>
         <li><a href="api/satsim.vecmath.html#satsim.vecmath.Cartesian4.Cartesian4.divideComponents">(satsim.vecmath.Cartesian4.Cartesian4 static method)</a>
 </li>
@@ -783,15 +785,17 @@
 </tr></table>
 
 <h2 id="L">L</h2>
 <table style="width: 100%" class="indextable genindextable"><tr>
   <td style="width: 33%; vertical-align: top;"><ul>
       <li><a href="api/satsim.math.html#satsim.math.interpolate.lagrange">lagrange() (in module satsim.math.interpolate)</a>
 </li>
-      <li><a href="api/satsim.geometry.html#satsim.geometry.astrometric.lambertian_sphere_to_mv">lambertian_sphere_to_mv() (in module satsim.geometry.astrometric)</a>
+      <li><a href="api/satsim.geometry.html#satsim.geometry.photometric.lambertian_sphere_model_to_mv">lambertian_sphere_model_to_mv() (in module satsim.geometry.photometric)</a>
+</li>
+      <li><a href="api/satsim.geometry.html#satsim.geometry.photometric.lambertian_sphere_to_mv">lambertian_sphere_to_mv() (in module satsim.geometry.photometric)</a>
 </li>
       <li><a href="api/satsim.vecmath.html#satsim.vecmath.Cartesian2.Cartesian2.lerp">lerp() (satsim.vecmath.Cartesian2.Cartesian2 static method)</a>
 
       <ul>
         <li><a href="api/satsim.vecmath.html#satsim.vecmath.Cartesian3.Cartesian3.lerp">(satsim.vecmath.Cartesian3.Cartesian3 static method)</a>
 </li>
         <li><a href="api/satsim.vecmath.html#satsim.vecmath.Cartesian4.Cartesian4.lerp">(satsim.vecmath.Cartesian4.Cartesian4 static method)</a>
@@ -801,18 +805,18 @@
       </ul></li>
       <li><a href="api/satsim.time.html#satsim.time.linspace">linspace() (in module satsim.time)</a>
 </li>
       <li><a href="api/satsim.geometry.html#satsim.geometry.astrometric.load_earth">load_earth() (in module satsim.geometry.astrometric)</a>
 </li>
       <li><a href="api/satsim.image.html#satsim.image.augment.load_from_file">load_from_file() (in module satsim.image.augment)</a>
 </li>
-      <li><a href="api/satsim.geometry.html#satsim.geometry.sstr7.load_index">load_index() (in module satsim.geometry.sstr7)</a>
-</li>
   </ul></td>
   <td style="width: 33%; vertical-align: top;"><ul>
+      <li><a href="api/satsim.geometry.html#satsim.geometry.sstr7.load_index">load_index() (in module satsim.geometry.sstr7)</a>
+</li>
       <li><a href="api/satsim.html#satsim.config.load_json">load_json() (in module satsim.config)</a>
 </li>
       <li><a href="api/satsim.geometry.html#satsim.geometry.astrometric.load_moon">load_moon() (in module satsim.geometry.astrometric)</a>
 </li>
       <li><a href="api/satsim.geometry.html#satsim.geometry.sprite.load_sprite_from_file">load_sprite_from_file() (in module satsim.geometry.sprite)</a>
 </li>
       <li><a href="api/satsim.geometry.html#satsim.geometry.sstr7.load_stars_for_zone">load_stars_for_zone() (in module satsim.geometry.sstr7)</a>
@@ -879,14 +883,16 @@
         <li><a href="api/satsim.vecmath.html#satsim.vecmath.Cartesian3.Cartesian3.maximumComponent">(satsim.vecmath.Cartesian3.Cartesian3 static method)</a>
 </li>
         <li><a href="api/satsim.vecmath.html#satsim.vecmath.Cartesian4.Cartesian4.maximumComponent">(satsim.vecmath.Cartesian4.Cartesian4 static method)</a>
 </li>
       </ul></li>
       <li><a href="api/satsim.math.html#satsim.math.angle.mean_degrees">mean_degrees() (in module satsim.math.angle)</a>
 </li>
+      <li><a href="api/satsim.util.html#satsim.util.python.merge_dicts">merge_dicts() (in module satsim.util.python)</a>
+</li>
       <li><a href="api/satsim.time.html#satsim.time.mid">mid() (in module satsim.time)</a>
 </li>
       <li><a href="api/satsim.vecmath.html#satsim.vecmath.Cartesian3.Cartesian3.midpoint">midpoint() (satsim.vecmath.Cartesian3.Cartesian3 static method)</a>
 </li>
       <li><a href="api/satsim.vecmath.html#satsim.vecmath.Cartesian2.Cartesian2.minimumByComponent">minimumByComponent() (satsim.vecmath.Cartesian2.Cartesian2 static method)</a>
 
       <ul>
@@ -899,14 +905,16 @@
 
       <ul>
         <li><a href="api/satsim.vecmath.html#satsim.vecmath.Cartesian3.Cartesian3.minimumComponent">(satsim.vecmath.Cartesian3.Cartesian3 static method)</a>
 </li>
         <li><a href="api/satsim.vecmath.html#satsim.vecmath.Cartesian4.Cartesian4.minimumComponent">(satsim.vecmath.Cartesian4.Cartesian4 static method)</a>
 </li>
       </ul></li>
+      <li><a href="api/satsim.geometry.html#satsim.geometry.photometric.model_to_mv">model_to_mv() (in module satsim.geometry.photometric)</a>
+</li>
       <li>
     module
 
       <ul>
         <li><a href="api/satsim.html#module-satsim">satsim</a>
 </li>
         <li><a href="api/satsim.html#module-satsim.cli">satsim.cli</a>
@@ -939,14 +947,16 @@
 </li>
         <li><a href="api/satsim.geometry.html#module-satsim.geometry.draw">satsim.geometry.draw</a>
 </li>
         <li><a href="api/satsim.geometry.html#module-satsim.geometry.ephemeris">satsim.geometry.ephemeris</a>
 </li>
         <li><a href="api/satsim.geometry.html#module-satsim.geometry.observation">satsim.geometry.observation</a>
 </li>
+        <li><a href="api/satsim.geometry.html#module-satsim.geometry.photometric">satsim.geometry.photometric</a>
+</li>
         <li><a href="api/satsim.geometry.html#module-satsim.geometry.random">satsim.geometry.random</a>
 </li>
         <li><a href="api/satsim.geometry.html#module-satsim.geometry.sgp4">satsim.geometry.sgp4</a>
 </li>
         <li><a href="api/satsim.geometry.html#module-satsim.geometry.sprite">satsim.geometry.sprite</a>
 </li>
         <li><a href="api/satsim.geometry.html#module-satsim.geometry.sstr7">satsim.geometry.sstr7</a>
@@ -1017,14 +1027,16 @@
 </li>
         <li><a href="api/satsim.tfa.utils.html#module-satsim.tfa.utils.types">satsim.tfa.utils.types</a>
 </li>
         <li><a href="api/satsim.time.html#module-satsim.time">satsim.time</a>
 </li>
         <li><a href="api/satsim.util.html#module-satsim.util">satsim.util</a>
 </li>
+        <li><a href="api/satsim.util.html#module-satsim.util.python">satsim.util.python</a>
+</li>
         <li><a href="api/satsim.util.html#module-satsim.util.system">satsim.util.system</a>
 </li>
         <li><a href="api/satsim.util.html#module-satsim.util.thread">satsim.util.thread</a>
 </li>
         <li><a href="api/satsim.util.html#module-satsim.util.timer">satsim.util.timer</a>
 </li>
         <li><a href="api/satsim.vecmath.html#module-satsim.vecmath">satsim.vecmath</a>
@@ -1403,14 +1415,21 @@
     satsim.geometry.observation
 
       <ul>
         <li><a href="api/satsim.geometry.html#module-satsim.geometry.observation">module</a>
 </li>
       </ul></li>
       <li>
+    satsim.geometry.photometric
+
+      <ul>
+        <li><a href="api/satsim.geometry.html#module-satsim.geometry.photometric">module</a>
+</li>
+      </ul></li>
+      <li>
     satsim.geometry.random
 
       <ul>
         <li><a href="api/satsim.geometry.html#module-satsim.geometry.random">module</a>
 </li>
       </ul></li>
       <li>
@@ -1678,14 +1697,21 @@
     satsim.util
 
       <ul>
         <li><a href="api/satsim.util.html#module-satsim.util">module</a>
 </li>
       </ul></li>
       <li>
+    satsim.util.python
+
+      <ul>
+        <li><a href="api/satsim.util.html#module-satsim.util.python">module</a>
+</li>
+      </ul></li>
+      <li>
     satsim.util.system
 
       <ul>
         <li><a href="api/satsim.util.html#module-satsim.util.system">module</a>
 </li>
       </ul></li>
       <li>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _S_a_t_S_i_m
-0.18.0
+0.19.0
 [q                   ]
 Contents:
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _U_s_a_g_e
     * _C_o_n_t_r_i_b_u_t_i_n_g
     * _A_P_I_ _D_o_c_u_m_e_n_t_a_t_i_o_n
     * _C_r_e_d_i_t_s
@@ -136,44 +136,39 @@
                                                                * _c_r_o_s_s_(_)_ 
                                                                  _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_2_._C_a_r_t_e_s_i_a_n_2
                                                                  _s_t_a_t_i_c_ _m_e_t_h_o_d_)
                                                                      o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_3_._C_a_r_t_e_s_i_a_n_3
                                                                        _s_t_a_t_i_c_ _m_e_t_h_o_d_)
                                                                * _C_Z_M_L_E_x_t_r_a_c_t_o_r_ _(_c_l_a_s_s_ _i_n_ _s_a_t_s_i_m_._i_o_._c_z_m_l_)
 ********** DD **********
-    * _d_e_l_t_a___s_e_c_(_)_ _(_i_n_ _m_o_d_u_l_e_ _s_a_t_s_i_m_._t_i_m_e_)             * _d_i_v_i_d_e_C_o_m_p_o_n_e_n_t_s_(_)_ 
+    * _d_e_l_t_a___s_e_c_(_)_ _(_i_n_ _m_o_d_u_l_e_ _s_a_t_s_i_m_._t_i_m_e_)             * _d_i_v_i_d_e_B_y_S_c_a_l_a_r_(_)_ 
     * _d_e_t_e_r_m_i_n_a_n_t_(_)_                                     _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_2_._C_a_r_t_e_s_i_a_n_2
       _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._M_a_t_r_i_x_3_._M_a_t_r_i_x_3_ _s_t_a_t_i_c            _s_t_a_t_i_c_ _m_e_t_h_o_d_)
       _m_e_t_h_o_d_)                                               o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_3_._C_a_r_t_e_s_i_a_n_3
     * _d_i_c_t___m_e_r_g_e_(_)_ _(_i_n_ _m_o_d_u_l_e_ _s_a_t_s_i_m_._c_o_n_f_i_g_)                  _s_t_a_t_i_c_ _m_e_t_h_o_d_)
     * _d_i_f_f___d_e_g_r_e_e_s_(_)_ _(_i_n_ _m_o_d_u_l_e                             o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_4_._C_a_r_t_e_s_i_a_n_4
       _s_a_t_s_i_m_._m_a_t_h_._a_n_g_l_e_)                                      _s_t_a_t_i_c_ _m_e_t_h_o_d_)
-    * _d_i_s_t_a_n_c_e_(_)_                                      * _d_o_t_(_)_ _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_2_._C_a_r_t_e_s_i_a_n_2
+    * _d_i_s_t_a_n_c_e_(_)_                                            o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._Q_u_a_t_e_r_n_i_o_n_._Q_u_a_t_e_r_n_i_o_n
+      _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_2_._C_a_r_t_e_s_i_a_n_2                   _s_t_a_t_i_c_ _m_e_t_h_o_d_)
+      _s_t_a_t_i_c_ _m_e_t_h_o_d_)                                  * _d_i_v_i_d_e_C_o_m_p_o_n_e_n_t_s_(_)_ 
+          o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_3_._C_a_r_t_e_s_i_a_n_3       _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_2_._C_a_r_t_e_s_i_a_n_2
+            _s_t_a_t_i_c_ _m_e_t_h_o_d_)                              _s_t_a_t_i_c_ _m_e_t_h_o_d_)
+          o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_4_._C_a_r_t_e_s_i_a_n_4           o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_3_._C_a_r_t_e_s_i_a_n_3
+            _s_t_a_t_i_c_ _m_e_t_h_o_d_)                                    _s_t_a_t_i_c_ _m_e_t_h_o_d_)
+    * _d_i_s_t_a_n_c_e___b_e_t_w_e_e_n_(_)_ _(_i_n_ _m_o_d_u_l_e                         o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_4_._C_a_r_t_e_s_i_a_n_4
+      _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._a_s_t_r_o_m_e_t_r_i_c_)                            _s_t_a_t_i_c_ _m_e_t_h_o_d_)
+    * _d_i_s_t_a_n_c_e_S_q_u_a_r_e_d_(_)_                               * _d_o_t_(_)_ _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_2_._C_a_r_t_e_s_i_a_n_2
       _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_2_._C_a_r_t_e_s_i_a_n_2             _s_t_a_t_i_c_ _m_e_t_h_o_d_)
       _s_t_a_t_i_c_ _m_e_t_h_o_d_)                                        o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_3_._C_a_r_t_e_s_i_a_n_3
           o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_3_._C_a_r_t_e_s_i_a_n_3             _s_t_a_t_i_c_ _m_e_t_h_o_d_)
             _s_t_a_t_i_c_ _m_e_t_h_o_d_)                                  o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_4_._C_a_r_t_e_s_i_a_n_4
           o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_4_._C_a_r_t_e_s_i_a_n_4             _s_t_a_t_i_c_ _m_e_t_h_o_d_)
             _s_t_a_t_i_c_ _m_e_t_h_o_d_)                                  o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._Q_u_a_t_e_r_n_i_o_n_._Q_u_a_t_e_r_n_i_o_n
-    * _d_i_s_t_a_n_c_e_S_q_u_a_r_e_d_(_)_                                       _s_t_a_t_i_c_ _m_e_t_h_o_d_)
-      _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_2_._C_a_r_t_e_s_i_a_n_2           * _d_o_w_n_s_a_m_p_l_e_(_)_ _(_i_n_ _m_o_d_u_l_e_ _s_a_t_s_i_m_._i_m_a_g_e_._f_p_a_)
-      _s_t_a_t_i_c_ _m_e_t_h_o_d_)
-          o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_3_._C_a_r_t_e_s_i_a_n_3
-            _s_t_a_t_i_c_ _m_e_t_h_o_d_)
-          o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_4_._C_a_r_t_e_s_i_a_n_4
-            _s_t_a_t_i_c_ _m_e_t_h_o_d_)
-    * _d_i_v_i_d_e_B_y_S_c_a_l_a_r_(_)_ 
-      _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_2_._C_a_r_t_e_s_i_a_n_2
-      _s_t_a_t_i_c_ _m_e_t_h_o_d_)
-          o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_3_._C_a_r_t_e_s_i_a_n_3
-            _s_t_a_t_i_c_ _m_e_t_h_o_d_)
-          o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_4_._C_a_r_t_e_s_i_a_n_4
-            _s_t_a_t_i_c_ _m_e_t_h_o_d_)
-          o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._Q_u_a_t_e_r_n_i_o_n_._Q_u_a_t_e_r_n_i_o_n
-            _s_t_a_t_i_c_ _m_e_t_h_o_d_)
+                                                              _s_t_a_t_i_c_ _m_e_t_h_o_d_)
+                                                      * _d_o_w_n_s_a_m_p_l_e_(_)_ _(_i_n_ _m_o_d_u_l_e_ _s_a_t_s_i_m_._i_m_a_g_e_._f_p_a_)
 ********** EE **********
     * _E_a_r_t_h_O_b_s_e_r_v_a_t_i_o_n_ _(_c_l_a_s_s_ _i_n                      * _e_q_u_a_l_s_E_p_s_i_l_o_n_(_)_ 
       _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._o_b_s_e_r_v_a_t_i_o_n_)                      _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_2_._C_a_r_t_e_s_i_a_n_2
     * _E_a_r_t_h_T_w_o_B_o_d_y_S_a_t_e_l_l_i_t_e_ _(_c_l_a_s_s_ _i_n                   _s_t_a_t_i_c_ _m_e_t_h_o_d_)
       _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._t_w_o_b_o_d_y_)                              o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_3_._C_a_r_t_e_s_i_a_n_3
     * _e_c_i___t_o___e_c_r_(_)_ _(_i_n_ _m_o_d_u_l_e                                 _s_t_a_t_i_c_ _m_e_t_h_o_d_)
       _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._a_s_t_r_o_m_e_t_r_i_c_)                          o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_4_._C_a_r_t_e_s_i_a_n_4
@@ -333,34 +328,35 @@
       _s_a_t_s_i_m_._i_o_._s_a_t_n_e_t_)                           _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._M_a_t_r_i_x_3_._M_a_t_r_i_x_3_ _s_t_a_t_i_c
     * _i_n_t_e_r_p___d_e_g_r_e_e_s_(_)_ _(_i_n_ _m_o_d_u_l_e                 _m_e_t_h_o_d_)
       _s_a_t_s_i_m_._m_a_t_h_._a_n_g_l_e_)                              o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._M_a_t_r_i_x_4_._M_a_t_r_i_x_4
                                                         _s_t_a_t_i_c_ _m_e_t_h_o_d_)
                                                 * _i_s___t_e_n_s_o_r_f_l_o_w___r_u_n_n_i_n_g___o_n___c_p_u_(_)_ _(_i_n_ _m_o_d_u_l_e
                                                   _s_a_t_s_i_m_._u_t_i_l_._s_y_s_t_e_m_)
 ********** LL **********
-    * _l_a_g_r_a_n_g_e_(_)_ _(_i_n_ _m_o_d_u_l_e                           * _l_o_a_d___j_s_o_n_(_)_ _(_i_n_ _m_o_d_u_l_e_ _s_a_t_s_i_m_._c_o_n_f_i_g_)
-      _s_a_t_s_i_m_._m_a_t_h_._i_n_t_e_r_p_o_l_a_t_e_)                        * _l_o_a_d___m_o_o_n_(_)_ _(_i_n_ _m_o_d_u_l_e
+    * _l_a_g_r_a_n_g_e_(_)_ _(_i_n_ _m_o_d_u_l_e                           * _l_o_a_d___i_n_d_e_x_(_)_ _(_i_n_ _m_o_d_u_l_e
+      _s_a_t_s_i_m_._m_a_t_h_._i_n_t_e_r_p_o_l_a_t_e_)                          _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._s_s_t_r_7_)
+    * _l_a_m_b_e_r_t_i_a_n___s_p_h_e_r_e___m_o_d_e_l___t_o___m_v_(_)_ _(_i_n_ _m_o_d_u_l_e      * _l_o_a_d___j_s_o_n_(_)_ _(_i_n_ _m_o_d_u_l_e_ _s_a_t_s_i_m_._c_o_n_f_i_g_)
+      _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._p_h_o_t_o_m_e_t_r_i_c_)                    * _l_o_a_d___m_o_o_n_(_)_ _(_i_n_ _m_o_d_u_l_e
     * _l_a_m_b_e_r_t_i_a_n___s_p_h_e_r_e___t_o___m_v_(_)_ _(_i_n_ _m_o_d_u_l_e              _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._a_s_t_r_o_m_e_t_r_i_c_)
-      _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._a_s_t_r_o_m_e_t_r_i_c_)                    * _l_o_a_d___s_p_r_i_t_e___f_r_o_m___f_i_l_e_(_)_ _(_i_n_ _m_o_d_u_l_e
+      _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._p_h_o_t_o_m_e_t_r_i_c_)                    * _l_o_a_d___s_p_r_i_t_e___f_r_o_m___f_i_l_e_(_)_ _(_i_n_ _m_o_d_u_l_e
     * _l_e_r_p_(_)_                                            _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._s_p_r_i_t_e_)
       _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_2_._C_a_r_t_e_s_i_a_n_2           * _l_o_a_d___s_t_a_r_s___f_o_r___z_o_n_e_(_)_ _(_i_n_ _m_o_d_u_l_e
       _s_t_a_t_i_c_ _m_e_t_h_o_d_)                                    _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._s_s_t_r_7_)
           o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_3_._C_a_r_t_e_s_i_a_n_3     * _l_o_a_d___s_u_n_(_)_ _(_i_n_ _m_o_d_u_l_e
             _s_t_a_t_i_c_ _m_e_t_h_o_d_)                              _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._a_s_t_r_o_m_e_t_r_i_c_)
           o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_4_._C_a_r_t_e_s_i_a_n_4     * _l_o_a_d___t_l_e_(_)_ _(_i_n_ _m_o_d_u_l_e
             _s_t_a_t_i_c_ _m_e_t_h_o_d_)                              _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._s_g_p_4_)
           o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._Q_u_a_t_e_r_n_i_o_n_._Q_u_a_t_e_r_n_i_o_n     * _l_o_a_d___y_a_m_l_(_)_ _(_i_n_ _m_o_d_u_l_e_ _s_a_t_s_i_m_._c_o_n_f_i_g_)
             _s_t_a_t_i_c_ _m_e_t_h_o_d_)                            * _l_o_a_d___z_o_n_e_(_)_ _(_i_n_ _m_o_d_u_l_e
     * _l_i_n_s_p_a_c_e_(_)_ _(_i_n_ _m_o_d_u_l_e_ _s_a_t_s_i_m_._t_i_m_e_)                _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._s_s_t_r_7_)
     * _l_o_a_d___e_a_r_t_h_(_)_ _(_i_n_ _m_o_d_u_l_e                         * _l_o_g_(_)_ 
       _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._a_s_t_r_o_m_e_t_r_i_c_)                      _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._Q_u_a_t_e_r_n_i_o_n_._Q_u_a_t_e_r_n_i_o_n
     * _l_o_a_d___f_r_o_m___f_i_l_e_(_)_ _(_i_n_ _m_o_d_u_l_e                       _s_t_a_t_i_c_ _m_e_t_h_o_d_)
       _s_a_t_s_i_m_._i_m_a_g_e_._a_u_g_m_e_n_t_)                           * _l_o_g_n_o_r_m_a_l_(_)_ _(_i_n_ _m_o_d_u_l_e
-    * _l_o_a_d___i_n_d_e_x_(_)_ _(_i_n_ _m_o_d_u_l_e                           _s_a_t_s_i_m_._m_a_t_h_._r_a_n_d_o_m_)
-      _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._s_s_t_r_7_)
+                                                        _s_a_t_s_i_m_._m_a_t_h_._r_a_n_d_o_m_)
 ********** MM **********
     * _m_ _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._M_a_t_r_i_x_4_._M_a_t_r_i_x_4               * _m_o_s_t_O_r_t_h_o_g_o_n_a_l_A_x_i_s_(_)_ 
       _a_t_t_r_i_b_u_t_e_)                                        _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_2_._C_a_r_t_e_s_i_a_n_2
     * _m_a_g_n_i_t_u_d_e_(_)_                                       _s_t_a_t_i_c_ _m_e_t_h_o_d_)
       _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_2_._C_a_r_t_e_s_i_a_n_2                 o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_3_._C_a_r_t_e_s_i_a_n_3
       _s_t_a_t_i_c_ _m_e_t_h_o_d_)                                          _s_t_a_t_i_c_ _m_e_t_h_o_d_)
           o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_3_._C_a_r_t_e_s_i_a_n_3           o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_4_._C_a_r_t_e_s_i_a_n_4
@@ -395,51 +391,56 @@
       _s_t_a_t_i_c_ _m_e_t_h_o_d_)                                          _s_t_a_t_i_c_ _m_e_t_h_o_d_)
           o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_3_._C_a_r_t_e_s_i_a_n_3           o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._M_a_t_r_i_x_4_._M_a_t_r_i_x_4
             _s_t_a_t_i_c_ _m_e_t_h_o_d_)                                    _s_t_a_t_i_c_ _m_e_t_h_o_d_)
           o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_4_._C_a_r_t_e_s_i_a_n_4           o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._Q_u_a_t_e_r_n_i_o_n_._Q_u_a_t_e_r_n_i_o_n
             _s_t_a_t_i_c_ _m_e_t_h_o_d_)                                    _s_t_a_t_i_c_ _m_e_t_h_o_d_)
     * _m_e_a_n___d_e_g_r_e_e_s_(_)_ _(_i_n_ _m_o_d_u_l_e                       * _m_u_l_t_i_p_l_y_B_y_S_c_a_l_e_(_)_ 
       _s_a_t_s_i_m_._m_a_t_h_._a_n_g_l_e_)                                _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._M_a_t_r_i_x_2_._M_a_t_r_i_x_2_ _s_t_a_t_i_c
-    * _m_i_d_(_)_ _(_i_n_ _m_o_d_u_l_e_ _s_a_t_s_i_m_._t_i_m_e_)                     _m_e_t_h_o_d_)
-    * _m_i_d_p_o_i_n_t_(_)_                                            o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._M_a_t_r_i_x_3_._M_a_t_r_i_x_3
+    * _m_e_r_g_e___d_i_c_t_s_(_)_ _(_i_n_ _m_o_d_u_l_e                          _m_e_t_h_o_d_)
+      _s_a_t_s_i_m_._u_t_i_l_._p_y_t_h_o_n_)                                   o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._M_a_t_r_i_x_3_._M_a_t_r_i_x_3
+    * _m_i_d_(_)_ _(_i_n_ _m_o_d_u_l_e_ _s_a_t_s_i_m_._t_i_m_e_)                           _s_t_a_t_i_c_ _m_e_t_h_o_d_)
+    * _m_i_d_p_o_i_n_t_(_)_                                            o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._M_a_t_r_i_x_4_._M_a_t_r_i_x_4
       _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_3_._C_a_r_t_e_s_i_a_n_3                   _s_t_a_t_i_c_ _m_e_t_h_o_d_)
-      _s_t_a_t_i_c_ _m_e_t_h_o_d_)                                        o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._M_a_t_r_i_x_4_._M_a_t_r_i_x_4
-    * _m_i_n_i_m_u_m_B_y_C_o_m_p_o_n_e_n_t_(_)_                                    _s_t_a_t_i_c_ _m_e_t_h_o_d_)
-      _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_2_._C_a_r_t_e_s_i_a_n_2           * _m_u_l_t_i_p_l_y_B_y_T_r_a_n_s_l_a_t_i_o_n_(_)_ 
-      _s_t_a_t_i_c_ _m_e_t_h_o_d_)                                    _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._M_a_t_r_i_x_4_._M_a_t_r_i_x_4_ _s_t_a_t_i_c
-          o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_3_._C_a_r_t_e_s_i_a_n_3       _m_e_t_h_o_d_)
-            _s_t_a_t_i_c_ _m_e_t_h_o_d_)                            * _m_u_l_t_i_p_l_y_B_y_U_n_i_f_o_r_m_S_c_a_l_e_(_)_ 
-          o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_4_._C_a_r_t_e_s_i_a_n_4       _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._M_a_t_r_i_x_2_._M_a_t_r_i_x_2_ _s_t_a_t_i_c
+      _s_t_a_t_i_c_ _m_e_t_h_o_d_)                                  * _m_u_l_t_i_p_l_y_B_y_T_r_a_n_s_l_a_t_i_o_n_(_)_ 
+    * _m_i_n_i_m_u_m_B_y_C_o_m_p_o_n_e_n_t_(_)_                              _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._M_a_t_r_i_x_4_._M_a_t_r_i_x_4_ _s_t_a_t_i_c
+      _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_2_._C_a_r_t_e_s_i_a_n_2             _m_e_t_h_o_d_)
+      _s_t_a_t_i_c_ _m_e_t_h_o_d_)                                  * _m_u_l_t_i_p_l_y_B_y_U_n_i_f_o_r_m_S_c_a_l_e_(_)_ 
+          o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_3_._C_a_r_t_e_s_i_a_n_3       _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._M_a_t_r_i_x_2_._M_a_t_r_i_x_2_ _s_t_a_t_i_c
             _s_t_a_t_i_c_ _m_e_t_h_o_d_)                              _m_e_t_h_o_d_)
-    * _m_i_n_i_m_u_m_C_o_m_p_o_n_e_n_t_(_)_                                    o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._M_a_t_r_i_x_3_._M_a_t_r_i_x_3
+          o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_4_._C_a_r_t_e_s_i_a_n_4           o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._M_a_t_r_i_x_3_._M_a_t_r_i_x_3
+            _s_t_a_t_i_c_ _m_e_t_h_o_d_)                                    _s_t_a_t_i_c_ _m_e_t_h_o_d_)
+    * _m_i_n_i_m_u_m_C_o_m_p_o_n_e_n_t_(_)_                                    o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._M_a_t_r_i_x_4_._M_a_t_r_i_x_4
       _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_2_._C_a_r_t_e_s_i_a_n_2                   _s_t_a_t_i_c_ _m_e_t_h_o_d_)
-      _s_t_a_t_i_c_ _m_e_t_h_o_d_)                                        o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._M_a_t_r_i_x_4_._M_a_t_r_i_x_4
-          o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_3_._C_a_r_t_e_s_i_a_n_3             _s_t_a_t_i_c_ _m_e_t_h_o_d_)
-            _s_t_a_t_i_c_ _m_e_t_h_o_d_)                            * _m_u_l_t_i_p_l_y_B_y_V_e_c_t_o_r_(_)_ 
-          o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_4_._C_a_r_t_e_s_i_a_n_4       _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._M_a_t_r_i_x_2_._M_a_t_r_i_x_2_ _s_t_a_t_i_c
+      _s_t_a_t_i_c_ _m_e_t_h_o_d_)                                  * _m_u_l_t_i_p_l_y_B_y_V_e_c_t_o_r_(_)_ 
+          o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_3_._C_a_r_t_e_s_i_a_n_3       _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._M_a_t_r_i_x_2_._M_a_t_r_i_x_2_ _s_t_a_t_i_c
             _s_t_a_t_i_c_ _m_e_t_h_o_d_)                              _m_e_t_h_o_d_)
-    * module                                                o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._M_a_t_r_i_x_3_._M_a_t_r_i_x_3
-          o _s_a_t_s_i_m                                            _s_t_a_t_i_c_ _m_e_t_h_o_d_)
-          o _s_a_t_s_i_m_._c_l_i                                      o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._M_a_t_r_i_x_4_._M_a_t_r_i_x_4
-          o _s_a_t_s_i_m_._c_o_n_f_i_g                                     _s_t_a_t_i_c_ _m_e_t_h_o_d_)
-          o _s_a_t_s_i_m_._d_a_t_a_s_e_t                            * _m_u_l_t_i_p_l_y_C_o_m_p_o_n_e_n_t_s_(_)_ 
-          o _s_a_t_s_i_m_._d_a_t_a_s_e_t_._a_u_g_m_e_n_t                      _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_2_._C_a_r_t_e_s_i_a_n_2
-          o _s_a_t_s_i_m_._g_e_n_e_r_a_t_o_r                            _s_t_a_t_i_c_ _m_e_t_h_o_d_)
-          o _s_a_t_s_i_m_._g_e_n_e_r_a_t_o_r_._o_b_s                            o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_3_._C_a_r_t_e_s_i_a_n_3
-          o _s_a_t_s_i_m_._g_e_n_e_r_a_t_o_r_._o_b_s_._b_r_e_a_k_u_p                      _s_t_a_t_i_c_ _m_e_t_h_o_d_)
-          o _s_a_t_s_i_m_._g_e_n_e_r_a_t_o_r_._o_b_s_._c_s_o                        o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_4_._C_a_r_t_e_s_i_a_n_4
-          o _s_a_t_s_i_m_._g_e_n_e_r_a_t_o_r_._o_b_s_._g_e_o_m_e_t_r_y                     _s_t_a_t_i_c_ _m_e_t_h_o_d_)
-          o _s_a_t_s_i_m_._g_e_n_e_r_a_t_o_r_._o_b_s_._i_o                   * _m_u_l_t_i_p_l_y_T_r_a_n_s_f_o_r_m_a_t_i_o_n_(_)_ 
-          o _s_a_t_s_i_m_._g_e_n_e_r_a_t_o_r_._o_b_s_._r_p_o                    _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._M_a_t_r_i_x_4_._M_a_t_r_i_x_4_ _s_t_a_t_i_c
-          o _s_a_t_s_i_m_._g_e_o_m_e_t_r_y                             _m_e_t_h_o_d_)
-          o _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._a_s_t_r_o_m_e_t_r_i_c               * _M_u_l_t_i_t_h_r_e_a_d_e_d_T_a_s_k_Q_u_e_u_e_ _(_c_l_a_s_s_ _i_n
-          o _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._c_s_v_s_c                       _s_a_t_s_i_m_._u_t_i_l_._t_h_r_e_a_d_)
-          o _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._d_r_a_w                      * _m_v___t_o___p_e_(_)_ _(_i_n_ _m_o_d_u_l_e_ _s_a_t_s_i_m_._i_m_a_g_e_._f_p_a_)
+          o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_4_._C_a_r_t_e_s_i_a_n_4           o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._M_a_t_r_i_x_3_._M_a_t_r_i_x_3
+            _s_t_a_t_i_c_ _m_e_t_h_o_d_)                                    _s_t_a_t_i_c_ _m_e_t_h_o_d_)
+    * _m_o_d_e_l___t_o___m_v_(_)_ _(_i_n_ _m_o_d_u_l_e                              o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._M_a_t_r_i_x_4_._M_a_t_r_i_x_4
+      _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._p_h_o_t_o_m_e_t_r_i_c_)                            _s_t_a_t_i_c_ _m_e_t_h_o_d_)
+    * module                                          * _m_u_l_t_i_p_l_y_C_o_m_p_o_n_e_n_t_s_(_)_ 
+          o _s_a_t_s_i_m                                      _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_2_._C_a_r_t_e_s_i_a_n_2
+          o _s_a_t_s_i_m_._c_l_i                                  _s_t_a_t_i_c_ _m_e_t_h_o_d_)
+          o _s_a_t_s_i_m_._c_o_n_f_i_g                                   o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_3_._C_a_r_t_e_s_i_a_n_3
+          o _s_a_t_s_i_m_._d_a_t_a_s_e_t                                    _s_t_a_t_i_c_ _m_e_t_h_o_d_)
+          o _s_a_t_s_i_m_._d_a_t_a_s_e_t_._a_u_g_m_e_n_t                          o _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_4_._C_a_r_t_e_s_i_a_n_4
+          o _s_a_t_s_i_m_._g_e_n_e_r_a_t_o_r                                  _s_t_a_t_i_c_ _m_e_t_h_o_d_)
+          o _s_a_t_s_i_m_._g_e_n_e_r_a_t_o_r_._o_b_s                      * _m_u_l_t_i_p_l_y_T_r_a_n_s_f_o_r_m_a_t_i_o_n_(_)_ 
+          o _s_a_t_s_i_m_._g_e_n_e_r_a_t_o_r_._o_b_s_._b_r_e_a_k_u_p                _(_s_a_t_s_i_m_._v_e_c_m_a_t_h_._M_a_t_r_i_x_4_._M_a_t_r_i_x_4_ _s_t_a_t_i_c
+          o _s_a_t_s_i_m_._g_e_n_e_r_a_t_o_r_._o_b_s_._c_s_o                    _m_e_t_h_o_d_)
+          o _s_a_t_s_i_m_._g_e_n_e_r_a_t_o_r_._o_b_s_._g_e_o_m_e_t_r_y             * _M_u_l_t_i_t_h_r_e_a_d_e_d_T_a_s_k_Q_u_e_u_e_ _(_c_l_a_s_s_ _i_n
+          o _s_a_t_s_i_m_._g_e_n_e_r_a_t_o_r_._o_b_s_._i_o                     _s_a_t_s_i_m_._u_t_i_l_._t_h_r_e_a_d_)
+          o _s_a_t_s_i_m_._g_e_n_e_r_a_t_o_r_._o_b_s_._r_p_o                  * _m_v___t_o___p_e_(_)_ _(_i_n_ _m_o_d_u_l_e_ _s_a_t_s_i_m_._i_m_a_g_e_._f_p_a_)
+          o _s_a_t_s_i_m_._g_e_o_m_e_t_r_y
+          o _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._a_s_t_r_o_m_e_t_r_i_c
+          o _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._c_s_v_s_c
+          o _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._d_r_a_w
           o _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._e_p_h_e_m_e_r_i_s
           o _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._o_b_s_e_r_v_a_t_i_o_n
+          o _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._p_h_o_t_o_m_e_t_r_i_c
           o _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._r_a_n_d_o_m
           o _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._s_g_p_4
           o _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._s_p_r_i_t_e
           o _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._s_s_t_r_7
           o _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._t_r_a_n_s_f_o_r_m
           o _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._t_w_o_b_o_d_y
           o _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._w_c_s
@@ -471,14 +472,15 @@
           o _s_a_t_s_i_m_._t_f_a_._i_m_a_g_e_._t_r_a_n_s_l_a_t_e___o_p_s
           o _s_a_t_s_i_m_._t_f_a_._i_m_a_g_e_._u_t_i_l_s
           o _s_a_t_s_i_m_._t_f_a_._u_t_i_l_s
           o _s_a_t_s_i_m_._t_f_a_._u_t_i_l_s_._t_e_s_t___u_t_i_l_s
           o _s_a_t_s_i_m_._t_f_a_._u_t_i_l_s_._t_y_p_e_s
           o _s_a_t_s_i_m_._t_i_m_e
           o _s_a_t_s_i_m_._u_t_i_l
+          o _s_a_t_s_i_m_._u_t_i_l_._p_y_t_h_o_n
           o _s_a_t_s_i_m_._u_t_i_l_._s_y_s_t_e_m
           o _s_a_t_s_i_m_._u_t_i_l_._t_h_r_e_a_d
           o _s_a_t_s_i_m_._u_t_i_l_._t_i_m_e_r
           o _s_a_t_s_i_m_._v_e_c_m_a_t_h
           o _s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_2
           o _s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_3
           o _s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_4
@@ -566,27 +568,29 @@
           o _m_o_d_u_l_e                            o _m_o_d_u_l_e
     * satsim.generator.obs.cso          * satsim.tfa.utils.types
           o _m_o_d_u_l_e                            o _m_o_d_u_l_e
     * satsim.generator.obs.geometry     * satsim.time
           o _m_o_d_u_l_e                            o _m_o_d_u_l_e
     * satsim.generator.obs.io           * satsim.util
           o _m_o_d_u_l_e                            o _m_o_d_u_l_e
-    * satsim.generator.obs.rpo          * satsim.util.system
+    * satsim.generator.obs.rpo          * satsim.util.python
+          o _m_o_d_u_l_e                            o _m_o_d_u_l_e
+    * satsim.geometry                   * satsim.util.system
           o _m_o_d_u_l_e                            o _m_o_d_u_l_e
-    * satsim.geometry                   * satsim.util.thread
+    * satsim.geometry.astrometric       * satsim.util.thread
           o _m_o_d_u_l_e                            o _m_o_d_u_l_e
-    * satsim.geometry.astrometric       * satsim.util.timer
+    * satsim.geometry.csvsc             * satsim.util.timer
           o _m_o_d_u_l_e                            o _m_o_d_u_l_e
-    * satsim.geometry.csvsc             * satsim.vecmath
+    * satsim.geometry.draw              * satsim.vecmath
           o _m_o_d_u_l_e                            o _m_o_d_u_l_e
-    * satsim.geometry.draw              * satsim.vecmath.Cartesian2
+    * satsim.geometry.ephemeris         * satsim.vecmath.Cartesian2
           o _m_o_d_u_l_e                            o _m_o_d_u_l_e
-    * satsim.geometry.ephemeris         * satsim.vecmath.Cartesian3
+    * satsim.geometry.observation       * satsim.vecmath.Cartesian3
           o _m_o_d_u_l_e                            o _m_o_d_u_l_e
-    * satsim.geometry.observation       * satsim.vecmath.Cartesian4
+    * satsim.geometry.photometric       * satsim.vecmath.Cartesian4
           o _m_o_d_u_l_e                            o _m_o_d_u_l_e
     * satsim.geometry.random            * satsim.vecmath.Matrix2
           o _m_o_d_u_l_e                            o _m_o_d_u_l_e
     * satsim.geometry.sgp4              * satsim.vecmath.Matrix3
           o _m_o_d_u_l_e                            o _m_o_d_u_l_e
     * satsim.geometry.sprite            * satsim.vecmath.Matrix4
           o _m_o_d_u_l_e                            o _m_o_d_u_l_e
```

### Comparing `satsim-0.18.0/docs/_build/html/history.html` & `satsim-0.19.0/docs/_build/html/history.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>History &mdash; SatSim 0.18.0 documentation</title>
+  <title>History &mdash; SatSim 0.19.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -28,15 +28,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.18.0
+                0.19.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -46,43 +46,44 @@
 <ul class="current">
 <li class="toctree-l1"><a class="reference internal" href="installation.html">Installation</a></li>
 <li class="toctree-l1"><a class="reference internal" href="usage.html">Usage</a></li>
 <li class="toctree-l1"><a class="reference internal" href="contributing.html">Contributing</a></li>
 <li class="toctree-l1"><a class="reference internal" href="api.html">API Documentation</a></li>
 <li class="toctree-l1"><a class="reference internal" href="authors.html">Credits</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">History</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="#id1">0.18.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id2">0.17.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id3">0.17.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id4">0.16.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id5">0.15.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id6">0.15.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id7">0.14.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id8">0.13.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id9">0.13.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id10">0.12.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id11">0.11.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id12">0.10.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id13">0.9.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id14">0.9.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id15">0.8.3</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id16">0.8.2</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id17">0.8.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id18">0.8.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id19">0.7.2</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id20">0.7.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id21">0.7.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id22">0.6.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id23">0.6.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id24">0.5.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id25">0.4.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id26">0.3.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id27">0.2.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id28">0.1.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="#id29">0.1.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id1">0.19.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id2">0.18.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id3">0.17.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id4">0.17.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id5">0.16.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id6">0.15.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id7">0.15.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id8">0.14.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id9">0.13.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id10">0.13.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id11">0.12.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id12">0.11.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id13">0.10.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id14">0.9.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id15">0.9.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id16">0.8.3</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id17">0.8.2</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id18">0.8.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id19">0.8.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id20">0.7.2</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id21">0.7.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id22">0.7.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id23">0.6.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id24">0.6.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id25">0.5.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id26">0.4.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id27">0.3.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id28">0.2.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id29">0.1.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="#id30">0.1.0</a></li>
 </ul>
 </li>
 </ul>
 
         </div>
       </div>
     </nav>
@@ -106,265 +107,271 @@
 </div>
           <div role="main" class="document" itemscope="itemscope" itemtype="http://schema.org/Article">
            <div itemprop="articleBody">
              
   <section id="history">
 <h1>History<a class="headerlink" href="#history" title="Permalink to this heading"></a></h1>
 <section id="id1">
-<h2>0.18.0<a class="headerlink" href="#id1" title="Permalink to this heading"></a></h2>
+<h2>0.19.0<a class="headerlink" href="#id1" title="Permalink to this heading"></a></h2>
+<ul class="simple">
+<li><p>Add lambertian sphere brightness model for objects. Set object key <cite>model</cite> <cite>mode</cite> to <cite>lambertian_sphere</cite> and set <cite>albedo</cite> and <cite>size</cite> (meters) parameters. For 2D simulations, <cite>distance</cite> (km) and <cite>phase_angle</cite> (degrees) parameters must also be specified.</p></li>
+</ul>
+</section>
+<section id="id2">
+<h2>0.18.0<a class="headerlink" href="#id2" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add turbulent atmosphere to POPPY PSF generation. Set with psf option <cite>turbulent_atmosphere</cite> and sim option <cite>psf_sample_frequency</cite>.</p></li>
 <li><p>Add star and object segmentation annotation. Set sim option <cite>save_segmentation</cite> to <cite>true</cite> and <cite>star_annotation_threshold</cite> to limit stars annotated.</p></li>
 </ul>
 </section>
-<section id="id2">
-<h2>0.17.1<a class="headerlink" href="#id2" title="Permalink to this heading"></a></h2>
+<section id="id3">
+<h2>0.17.1<a class="headerlink" href="#id3" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Copy useful TensorFlow Addon (TFA) functions into <cite>tfa</cite> as the TFA project is no longer maintained.</p></li>
 <li><p>Copy tests.</p></li>
 </ul>
 </section>
-<section id="id3">
-<h2>0.17.0<a class="headerlink" href="#id3" title="Permalink to this heading"></a></h2>
+<section id="id4">
+<h2>0.17.0<a class="headerlink" href="#id4" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add JSON schema definitions. See <cite>schema/v1/Document.json</cite> for root schema file.</p></li>
 <li><p>Add observation object type.</p></li>
 <li><p>Add support for cropped sensors.</p></li>
 <li><p>Add altitude to site object. Set site <cite>alt</cite> parameter in km. Default is 0.</p></li>
 </ul>
 </section>
-<section id="id4">
-<h2>0.16.0<a class="headerlink" href="#id4" title="Permalink to this heading"></a></h2>
+<section id="id5">
+<h2>0.16.0<a class="headerlink" href="#id5" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add option to annotate stars. Set sim option <cite>star_annotation_threshold</cite> to the minimum star brightness magnitude or <cite>false</cite> to disable. Disabled by default.</p></li>
 <li><p>Add option to show annotated stars in annotated images. Set sim option <cite>show_star_boxes</cite> to <cite>true</cite> to enable.</p></li>
 </ul>
 </section>
-<section id="id5">
-<h2>0.15.1<a class="headerlink" href="#id5" title="Permalink to this heading"></a></h2>
+<section id="id6">
+<h2>0.15.1<a class="headerlink" href="#id6" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Remove clipping of negative values in ground truth files by default.</p></li>
 <li><p>Fix missing dependencies for ground truth file generation.</p></li>
 </ul>
 </section>
-<section id="id6">
-<h2>0.15.0<a class="headerlink" href="#id6" title="Permalink to this heading"></a></h2>
+<section id="id7">
+<h2>0.15.0<a class="headerlink" href="#id7" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add support to save ground truth image data to the Annotations directory. Set sim option <cite>save_ground_truth</cite> to <cite>true</cite>.</p></li>
 <li><p>Add support for running on CPU with no GPU acceleration.</p></li>
 <li><p>Add CZML options for sensor visualization and object billboard image.</p></li>
 </ul>
 </section>
-<section id="id7">
-<h2>0.14.0<a class="headerlink" href="#id7" title="Permalink to this heading"></a></h2>
+<section id="id8">
+<h2>0.14.0<a class="headerlink" href="#id8" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add vector math library.</p></li>
 <li><p>Add CZML output for sensor visualization.</p></li>
 <li><p>Fix objects not updating properly when image renderer is off.</p></li>
 </ul>
 </section>
-<section id="id8">
-<h2>0.13.1<a class="headerlink" href="#id8" title="Permalink to this heading"></a></h2>
+<section id="id9">
+<h2>0.13.1<a class="headerlink" href="#id9" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add argument to set folder name in <cite>gen_multi</cite>.</p></li>
 <li><p>Add environment variable, <cite>SATSIM_SKYFIELD_LOAD_DIR</cite>, to specify location of Skyfield ephemeris files.</p></li>
 <li><p>Fix incorrect CZML output when image renderer is off.</p></li>
 </ul>
 </section>
-<section id="id9">
-<h2>0.13.0<a class="headerlink" href="#id9" title="Permalink to this heading"></a></h2>
+<section id="id10">
+<h2>0.13.0<a class="headerlink" href="#id10" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add ephemeris objects that are propagated with the Lagrange interpolator.</p></li>
 <li><p>Add Cesium CZML output. Set sim option <cite>save_czml</cite> to <cite>false</cite> to disable.</p></li>
 <li><p>Add CSV text file star catalog loader. This feature is useful for small catalogs such as Hipparcos and simulating wide FOV sensors.</p></li>
 <li><p>Add multiplier and clipping for radial cosine.</p></li>
 <li><p>Add option to skip image rendering. Set sim option <cite>mode</cite> to <cite>none</cite> to bypass image rendering.</p></li>
 <li><p>Update interfaces for newest version of Skyfield, Poliastro, POPPY, and AstroPy.</p></li>
 <li><p>Fix star renderer issue removing stars in field of view for non-square arrays.</p></li>
 </ul>
 </section>
-<section id="id10">
-<h2>0.12.0<a class="headerlink" href="#id10" title="Permalink to this heading"></a></h2>
+<section id="id11">
+<h2>0.12.0<a class="headerlink" href="#id11" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add augmentation of SatNet <cite>tf.data.Dataset</cite>. This feature allows injecting synthetic targets into real data during training.</p></li>
 <li><p>Add FFT convolution to <cite>add_patch</cite> sprite render and <cite>scatter_shift</cite> image augmenter for speed improvement.</p></li>
 <li><p>Add cache last PSF FFT to <cite>fftconv2p</cite> for speed improvement for static PSFs.</p></li>
 <li><p>Add two-body state vector as a trackable target.</p></li>
 <li><p>Add moon and sun model and misc methods to calculate phase angle and target brightness.</p></li>
 </ul>
 </section>
-<section id="id11">
-<h2>0.11.0<a class="headerlink" href="#id11" title="Permalink to this heading"></a></h2>
+<section id="id12">
+<h2>0.11.0<a class="headerlink" href="#id12" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add support to render star motion with FFT. Set sim option <cite>star_render_mode</cite> to <cite>fft</cite>.</p></li>
 <li><p>Add option to sample photon noise multiple times. Set sim option <cite>num_shot_noise_samples</cite> to integer number.</p></li>
 <li><p>Add support to render a satellite as a sprite. Set <cite>model</cite> option in obs.</p></li>
 <li><p>Add support to load and augment sprite model with <cite>$pipeline</cite> operator.</p></li>
 <li><p>Add cropped POPPY PSF generation.</p></li>
 <li><p>Fix GreatCircle propagator tracking offset.</p></li>
 <li><p>Fix runtime exception when site and track_mode are not defined.</p></li>
 <li><p>Add TensorFlow 2.6 and update TensorFlow 2.2 and 2.4 Docker build file.</p></li>
 </ul>
 </section>
-<section id="id12">
-<h2>0.10.0<a class="headerlink" href="#id12" title="Permalink to this heading"></a></h2>
+<section id="id13">
+<h2>0.10.0<a class="headerlink" href="#id13" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add support for piecewise rendering. Set sim option <cite>render_size</cite> to enable. For example, [256, 256].</p></li>
 <li><p>Add <cite>fixed</cite> tracking mode with mount azimuth and elevation.</p></li>
 <li><p>Add great circle propagator for targets.</p></li>
 <li><p>Add in-memory image generation. See generator function <cite>image_generator</cite>.</p></li>
 <li><p>Fix missing stars when FOV crosses zero degree RA.</p></li>
 <li><p>Add curved targets using bezier curve raster. Enabled by default. Set sim option <cite>num_target_samples</cite> to 2 to enable linear raster.</p></li>
 <li><p>Add LRU cache to star catalog reader.</p></li>
 <li><p>Add option to turn off SNR calculation. Set sim option <cite>calculate_snr</cite> to false will render targets and stars together.</p></li>
 <li><p>Handle unstable SGP4 TLEs.</p></li>
 <li><p>Add TensorFlow 2.4 Docker build file.</p></li>
 <li><p>Add debug output for pristine images of targets and stars.</p></li>
 </ul>
 </section>
-<section id="id13">
-<h2>0.9.1<a class="headerlink" href="#id13" title="Permalink to this heading"></a></h2>
+<section id="id14">
+<h2>0.9.1<a class="headerlink" href="#id14" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Calculate POPPY input wavefront resolution to avoid PSF aliasing.</p></li>
 <li><p>Add support for additional FITS image data types (<cite>int16</cite>, <cite>uint16</cite>, <cite>int32</cite>, <cite>uint32</cite>, <cite>float32</cite>).</p></li>
 <li><p>Add batch processing to <cite>transform_and_add_counts</cite> to support batch processing of stars.</p></li>
 <li><p>Add <cite>auto</cite> option to calculate temporal oversample factor based on star velocities.</p></li>
 <li><p>Add option to turn off serializing config data to pickle file (<cite>save_pickle</cite>).</p></li>
 <li><p>Add option to turn off png movie output (<cite>save_movie</cite>).</p></li>
 <li><p>Add <cite>crop_and_resize</cite> and <cite>flip</cite> image augmentation.</p></li>
 <li><p>Set pixels with values beyond the pixel data type’s capacity to the maximum value for that data type.</p></li>
 <li><p>Add <cite>lognormal</cite> function to generate a distribution with a true target mean.</p></li>
 <li><p>Fix issue with sidereal track.</p></li>
 <li><p>Fix issue with fragment velocity not being randomly sampled.</p></li>
 </ul>
 </section>
-<section id="id14">
-<h2>0.9.0<a class="headerlink" href="#id14" title="Permalink to this heading"></a></h2>
+<section id="id15">
+<h2>0.9.0<a class="headerlink" href="#id15" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add Physical Optics Propagation in Python (POPPY) PSF generation.</p></li>
 <li><p>Add PSF augmentation with <cite>$pipeline</cite> replacement key.</p></li>
 <li><p>Add <cite>$function</cite> and <cite>$compound</cite> replacement key.</p></li>
 <li><p>Add ability to generate stray light from a <cite>$function</cite> replacement key.</p></li>
 <li><p>Add built-in 2D polynomial image generator for stray light, <cite>polygrid2d</cite>.</p></li>
 <li><p>Add built-in cosine fourth image generator for irradiance falloff, <cite>radial_cos2d</cite>.</p></li>
 <li><p>Add built-in sine wave image generator for fix pattern noise, <cite>sin2d</cite>.</p></li>
 <li><p>Add built-in image generator from AstroPy model, <cite>astropy_model2d</cite>.</p></li>
 <li><p>Add built-in image augmentation, <cite>scatter_shift</cite> and <cite>scatter_shift_polar</cite>.</p></li>
 <li><p>Add <cite>$cache</cite> replacement key (caching works for PSF and <cite>$function</cite>).</p></li>
 </ul>
 </section>
-<section id="id15">
-<h2>0.8.3<a class="headerlink" href="#id15" title="Permalink to this heading"></a></h2>
+<section id="id16">
+<h2>0.8.3<a class="headerlink" href="#id16" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Fix new Skyfield incompatibility.</p></li>
 </ul>
 </section>
-<section id="id16">
-<h2>0.8.2<a class="headerlink" href="#id16" title="Permalink to this heading"></a></h2>
+<section id="id17">
+<h2>0.8.2<a class="headerlink" href="#id17" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Prefix replacement keys with <cite>$</cite> in SatSim configuration file.</p></li>
 <li><p>Add option to scale collision fragments by cosine of the exit angle.</p></li>
 </ul>
 </section>
-<section id="id17">
-<h2>0.8.1<a class="headerlink" href="#id17" title="Permalink to this heading"></a></h2>
+<section id="id18">
+<h2>0.8.1<a class="headerlink" href="#id18" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add astrometric metadata into FITS header</p></li>
 <li><p>Refactor WCS library</p></li>
 <li><p>Add option to flip images about x or y axis</p></li>
 <li><p>Add option to refresh stars for each frame</p></li>
 <li><p>Add RPO from TLE generator</p></li>
 </ul>
 </section>
-<section id="id18">
-<h2>0.8.0<a class="headerlink" href="#id18" title="Permalink to this heading"></a></h2>
+<section id="id19">
+<h2>0.8.0<a class="headerlink" href="#id19" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add two body propagator</p></li>
 <li><p>Add object <cite>create</cite>, <cite>delete</cite>, and <cite>update</cite> events</p></li>
 <li><p>Add collision generator</p></li>
 <li><p>Add breakup generator</p></li>
 <li><p>Add <cite>ref</cite> keyword to configuration</p></li>
 <li><p>Add <cite>key</cite> keyword to <cite>import</cite> configuration</p></li>
 <li><p>Refactor astrometric library</p></li>
 </ul>
 </section>
-<section id="id19">
-<h2>0.7.2<a class="headerlink" href="#id19" title="Permalink to this heading"></a></h2>
+<section id="id20">
+<h2>0.7.2<a class="headerlink" href="#id20" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add option to specify star and obs velocity in polar coordinates</p></li>
 </ul>
 </section>
-<section id="id20">
-<h2>0.7.1<a class="headerlink" href="#id20" title="Permalink to this heading"></a></h2>
+<section id="id21">
+<h2>0.7.1<a class="headerlink" href="#id21" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add option to turn off shot noise: <cite>sim.enable_shot_noise: true</cite></p></li>
 <li><p>Add option to turn off annotation boxes in image: <cite>sim.show_obs_boxes: true</cite></p></li>
 <li><p>Add option to specify velocity in arcseconds: <cite>sim.velocity_units: arcsec</cite></p></li>
 <li><p>Fix PNG output threading issue</p></li>
 </ul>
 </section>
-<section id="id21">
-<h2>0.7.0<a class="headerlink" href="#id21" title="Permalink to this heading"></a></h2>
+<section id="id22">
+<h2>0.7.0<a class="headerlink" href="#id22" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add function pipelines to support variable target brightness</p></li>
 </ul>
 </section>
-<section id="id22">
-<h2>0.6.1<a class="headerlink" href="#id22" title="Permalink to this heading"></a></h2>
+<section id="id23">
+<h2>0.6.1<a class="headerlink" href="#id23" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Fix built-in generators not included in distribution</p></li>
 <li><p>Add dockerfile</p></li>
 </ul>
 </section>
-<section id="id23">
-<h2>0.6.0<a class="headerlink" href="#id23" title="Permalink to this heading"></a></h2>
+<section id="id24">
+<h2>0.6.0<a class="headerlink" href="#id24" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add configuration import.</p></li>
 <li><p>Add configuration generator functions.</p></li>
 <li><p>Add built-in generator for breakups.</p></li>
 <li><p>Add built-in generator for CSOs.</p></li>
 <li><p>Add built-in generator for loading TLE files.</p></li>
 </ul>
 </section>
-<section id="id24">
-<h2>0.5.0<a class="headerlink" href="#id24" title="Permalink to this heading"></a></h2>
+<section id="id25">
+<h2>0.5.0<a class="headerlink" href="#id25" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Runtime optimization.</p></li>
 <li><p>Add parallel processing and multi-gpu utilization.</p></li>
 <li><p>Add option to limit gpu memory usage.</p></li>
 </ul>
 </section>
-<section id="id25">
-<h2>0.4.0<a class="headerlink" href="#id25" title="Permalink to this heading"></a></h2>
+<section id="id26">
+<h2>0.4.0<a class="headerlink" href="#id26" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add signal to noise calculation for target pixels.</p></li>
 </ul>
 </section>
-<section id="id26">
-<h2>0.3.0<a class="headerlink" href="#id26" title="Permalink to this heading"></a></h2>
+<section id="id27">
+<h2>0.3.0<a class="headerlink" href="#id27" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add support for two line element set SGP4 satellite propagator.</p></li>
 <li><p>Add support for rate and sidereal track from topocentric site.</p></li>
 </ul>
 </section>
-<section id="id27">
-<h2>0.2.0<a class="headerlink" href="#id27" title="Permalink to this heading"></a></h2>
+<section id="id28">
+<h2>0.2.0<a class="headerlink" href="#id28" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add support for SSTR7 star catalog.</p></li>
 </ul>
 </section>
-<section id="id28">
-<h2>0.1.1<a class="headerlink" href="#id28" title="Permalink to this heading"></a></h2>
+<section id="id29">
+<h2>0.1.1<a class="headerlink" href="#id29" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>Add target position to annotation file.</p></li>
 <li><p>Updates to run GitLab CI.</p></li>
 </ul>
 </section>
-<section id="id29">
-<h2>0.1.0<a class="headerlink" href="#id29" title="Permalink to this heading"></a></h2>
+<section id="id30">
+<h2>0.1.0<a class="headerlink" href="#id30" title="Permalink to this heading"></a></h2>
 <ul class="simple">
 <li><p>First release.</p></li>
 </ul>
 </section>
 </section>
```

#### html2text {}

```diff
@@ -1,17 +1,18 @@
 _S_a_t_S_i_m
-0.18.0
+0.19.0
 [q                   ]
 Contents:
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _U_s_a_g_e
     * _C_o_n_t_r_i_b_u_t_i_n_g
     * _A_P_I_ _D_o_c_u_m_e_n_t_a_t_i_o_n
     * _C_r_e_d_i_t_s
     * _H_i_s_t_o_r_y
+          o _0_._1_9_._0
           o _0_._1_8_._0
           o _0_._1_7_._1
           o _0_._1_7_._0
           o _0_._1_6_._0
           o _0_._1_5_._1
           o _0_._1_5_._0
           o _0_._1_4_._0
@@ -38,14 +39,19 @@
           o _0_._1_._1
           o _0_._1_._0
 _S_a_t_S_i_m
     * History
     * _V_i_e_w_ _p_a_g_e_ _s_o_u_r_c_e
 ===============================================================================
 ************ HHiissttoorryy_? ************
+********** 00..1199..00_? **********
+    * Add lambertian sphere brightness model for objects. Set object
+      keymodelmodetolambertian_sphereand setalbedoandsize(meters) parameters.
+      For 2D simulations,distance(km) andphase_angle(degrees) parameters must
+      also be specified.
 ********** 00..1188..00_? **********
     * Add turbulent atmosphere to POPPY PSF generation. Set with psf
       optionturbulent_atmosphereand sim optionpsf_sample_frequency.
     * Add star and object segmentation annotation. Set sim
       optionsave_segmentationtotrueandstar_annotation_thresholdto limit stars
       annotated.
 ********** 00..1177..11_? **********
```

### Comparing `satsim-0.18.0/docs/_build/html/index.html` & `satsim-0.19.0/docs/_build/html/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Documentation for SatSim &mdash; SatSim 0.18.0 documentation</title>
+  <title>Documentation for SatSim &mdash; SatSim 0.19.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -28,15 +28,15 @@
 
           
           
           <a href="#" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.18.0
+                0.19.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -106,43 +106,44 @@
 </li>
 <li class="toctree-l1"><a class="reference internal" href="authors.html">Credits</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="authors.html#development-lead">Development Lead</a></li>
 <li class="toctree-l2"><a class="reference internal" href="authors.html#contributors">Contributors</a></li>
 </ul>
 </li>
 <li class="toctree-l1"><a class="reference internal" href="history.html">History</a><ul>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id1">0.18.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id2">0.17.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id3">0.17.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id4">0.16.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id5">0.15.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id6">0.15.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id7">0.14.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id8">0.13.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id9">0.13.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id10">0.12.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id11">0.11.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id12">0.10.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id13">0.9.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id14">0.9.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id15">0.8.3</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id16">0.8.2</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id17">0.8.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id18">0.8.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id19">0.7.2</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id20">0.7.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id21">0.7.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id22">0.6.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id23">0.6.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id24">0.5.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id25">0.4.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id26">0.3.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id27">0.2.0</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id28">0.1.1</a></li>
-<li class="toctree-l2"><a class="reference internal" href="history.html#id29">0.1.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id1">0.19.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id2">0.18.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id3">0.17.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id4">0.17.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id5">0.16.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id6">0.15.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id7">0.15.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id8">0.14.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id9">0.13.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id10">0.13.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id11">0.12.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id12">0.11.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id13">0.10.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id14">0.9.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id15">0.9.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id16">0.8.3</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id17">0.8.2</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id18">0.8.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id19">0.8.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id20">0.7.2</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id21">0.7.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id22">0.7.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id23">0.6.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id24">0.6.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id25">0.5.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id26">0.4.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id27">0.3.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id28">0.2.0</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id29">0.1.1</a></li>
+<li class="toctree-l2"><a class="reference internal" href="history.html#id30">0.1.0</a></li>
 </ul>
 </li>
 </ul>
 </div>
 </section>
 <section id="indices-and-tables">
 <h1>Indices and tables<a class="headerlink" href="#indices-and-tables" title="Permalink to this heading"></a></h1>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _S_a_t_S_i_m
-0.18.0
+0.19.0
 [q                   ]
 Contents:
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _U_s_a_g_e
     * _C_o_n_t_r_i_b_u_t_i_n_g
     * _A_P_I_ _D_o_c_u_m_e_n_t_a_t_i_o_n
     * _C_r_e_d_i_t_s
@@ -29,14 +29,15 @@
           o _O_t_h_e_r_ _W_a_y_s_ _o_f_ _C_o_n_t_r_i_b_u_t_i_n_g
     * _A_P_I_ _D_o_c_u_m_e_n_t_a_t_i_o_n
           o _s_a_t_s_i_m_ _p_a_c_k_a_g_e
     * _C_r_e_d_i_t_s
           o _D_e_v_e_l_o_p_m_e_n_t_ _L_e_a_d
           o _C_o_n_t_r_i_b_u_t_o_r_s
     * _H_i_s_t_o_r_y
+          o _0_._1_9_._0
           o _0_._1_8_._0
           o _0_._1_7_._1
           o _0_._1_7_._0
           o _0_._1_6_._0
           o _0_._1_5_._1
           o _0_._1_5_._0
           o _0_._1_4_._0
```

### Comparing `satsim-0.18.0/docs/_build/html/installation.html` & `satsim-0.19.0/docs/_build/html/installation.html`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Installation &mdash; SatSim 0.18.0 documentation</title>
+  <title>Installation &mdash; SatSim 0.19.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.18.0
+                0.19.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _S_a_t_S_i_m
-0.18.0
+0.19.0
 [q                   ]
 Contents:
     * _I_n_s_t_a_l_l_a_t_i_o_n
           o _S_t_a_b_l_e_ _R_e_l_e_a_s_e
           o _F_r_o_m_ _S_o_u_r_c_e_s
     * _U_s_a_g_e
     * _C_o_n_t_r_i_b_u_t_i_n_g
```

### Comparing `satsim-0.18.0/docs/_build/html/py-modindex.html` & `satsim-0.19.0/docs/_build/html/py-modindex.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Python Module Index &mdash; SatSim 0.18.0 documentation</title>
+  <title>Python Module Index &mdash; SatSim 0.19.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.18.0
+                0.19.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
@@ -177,14 +177,19 @@
        <td></td>
        <td>&#160;&#160;&#160;
        <a href="api/satsim.geometry.html#module-satsim.geometry.observation"><code class="xref">satsim.geometry.observation</code></a></td><td>
        <em></em></td></tr>
      <tr class="cg-1">
        <td></td>
        <td>&#160;&#160;&#160;
+       <a href="api/satsim.geometry.html#module-satsim.geometry.photometric"><code class="xref">satsim.geometry.photometric</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
        <a href="api/satsim.geometry.html#module-satsim.geometry.random"><code class="xref">satsim.geometry.random</code></a></td><td>
        <em></em></td></tr>
      <tr class="cg-1">
        <td></td>
        <td>&#160;&#160;&#160;
        <a href="api/satsim.geometry.html#module-satsim.geometry.sgp4"><code class="xref">satsim.geometry.sgp4</code></a></td><td>
        <em></em></td></tr>
@@ -372,14 +377,19 @@
        <td></td>
        <td>&#160;&#160;&#160;
        <a href="api/satsim.util.html#module-satsim.util"><code class="xref">satsim.util</code></a></td><td>
        <em></em></td></tr>
      <tr class="cg-1">
        <td></td>
        <td>&#160;&#160;&#160;
+       <a href="api/satsim.util.html#module-satsim.util.python"><code class="xref">satsim.util.python</code></a></td><td>
+       <em></em></td></tr>
+     <tr class="cg-1">
+       <td></td>
+       <td>&#160;&#160;&#160;
        <a href="api/satsim.util.html#module-satsim.util.system"><code class="xref">satsim.util.system</code></a></td><td>
        <em></em></td></tr>
      <tr class="cg-1">
        <td></td>
        <td>&#160;&#160;&#160;
        <a href="api/satsim.util.html#module-satsim.util.thread"><code class="xref">satsim.util.thread</code></a></td><td>
        <em></em></td></tr>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _S_a_t_S_i_m
-0.18.0
+0.19.0
 [q                   ]
 Contents:
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _U_s_a_g_e
     * _C_o_n_t_r_i_b_u_t_i_n_g
     * _A_P_I_ _D_o_c_u_m_e_n_t_a_t_i_o_n
     * _C_r_e_d_i_t_s
@@ -29,14 +29,15 @@
         _s_a_t_s_i_m_._g_e_n_e_r_a_t_o_r_._o_b_s_._r_p_o
         _s_a_t_s_i_m_._g_e_o_m_e_t_r_y
         _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._a_s_t_r_o_m_e_t_r_i_c
         _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._c_s_v_s_c
         _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._d_r_a_w
         _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._e_p_h_e_m_e_r_i_s
         _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._o_b_s_e_r_v_a_t_i_o_n
+        _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._p_h_o_t_o_m_e_t_r_i_c
         _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._r_a_n_d_o_m
         _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._s_g_p_4
         _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._s_p_r_i_t_e
         _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._s_s_t_r_7
         _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._t_r_a_n_s_f_o_r_m
         _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._t_w_o_b_o_d_y
         _s_a_t_s_i_m_._g_e_o_m_e_t_r_y_._w_c_s
@@ -68,14 +69,15 @@
         _s_a_t_s_i_m_._t_f_a_._i_m_a_g_e_._t_r_a_n_s_l_a_t_e___o_p_s
         _s_a_t_s_i_m_._t_f_a_._i_m_a_g_e_._u_t_i_l_s
         _s_a_t_s_i_m_._t_f_a_._u_t_i_l_s
         _s_a_t_s_i_m_._t_f_a_._u_t_i_l_s_._t_e_s_t___u_t_i_l_s
         _s_a_t_s_i_m_._t_f_a_._u_t_i_l_s_._t_y_p_e_s
         _s_a_t_s_i_m_._t_i_m_e
         _s_a_t_s_i_m_._u_t_i_l
+        _s_a_t_s_i_m_._u_t_i_l_._p_y_t_h_o_n
         _s_a_t_s_i_m_._u_t_i_l_._s_y_s_t_e_m
         _s_a_t_s_i_m_._u_t_i_l_._t_h_r_e_a_d
         _s_a_t_s_i_m_._u_t_i_l_._t_i_m_e_r
         _s_a_t_s_i_m_._v_e_c_m_a_t_h
         _s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_2
         _s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_3
         _s_a_t_s_i_m_._v_e_c_m_a_t_h_._C_a_r_t_e_s_i_a_n_4
```

### Comparing `satsim-0.18.0/docs/_build/html/search.html` & `satsim-0.19.0/docs/_build/html/search.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" />
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Search &mdash; SatSim 0.18.0 documentation</title>
+  <title>Search &mdash; SatSim 0.19.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
     
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.18.0
+                0.19.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="#" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _S_a_t_S_i_m
-0.18.0
+0.19.0
 [q                   ]
 Contents:
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _U_s_a_g_e
     * _C_o_n_t_r_i_b_u_t_i_n_g
     * _A_P_I_ _D_o_c_u_m_e_n_t_a_t_i_o_n
     * _C_r_e_d_i_t_s
```

### Comparing `satsim-0.18.0/docs/_build/html/searchindex.js` & `satsim-0.19.0/docs/_build/html/searchindex.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -18,36 +18,36 @@
         "augment_satnet_with_satsim": [0, 1, 2],
         "gener": [0, 1, 5, 6, 7, 8, 13, 15, 18, 21],
         "ob": [0, 1, 3, 7, 18, 21],
         "breakup": [0, 1, 3, 18],
         "breakup_from_tl": [0, 3, 4],
         "collision_from_tl": [0, 3, 4],
         "cso": [0, 1, 3, 18],
-        "one": [0, 1, 3, 4, 6, 8, 11, 15],
+        "one": [0, 1, 3, 4, 6, 8, 11, 14, 15],
         "geometri": [0, 1, 3, 21],
         "circl": [0, 3, 4, 5, 18],
         "cone": [0, 3, 4, 21],
-        "sphere": [0, 3, 4, 5],
+        "sphere": [0, 3, 4, 5, 18],
         "io": [0, 1, 3],
         "tle_fil": [0, 3, 4],
         "rpo": [0, 1, 3, 18],
         "rpo_from_tl": [0, 3, 4],
         "astrometr": [0, 1, 7, 18],
         "greatcircl": [0, 1, 5, 18],
         "angle_between": [0, 1, 5],
         "angle_from_lo": [0, 1, 5],
         "appar": [0, 1, 5],
         "create_topocentr": [0, 1, 5],
+        "distance_between": [0, 1, 5],
         "eci_to_ecr": [0, 1, 5],
         "eci_to_radec": [0, 1, 5],
         "gen_track": [0, 1, 5],
         "gen_track_from_wc": [0, 1, 5],
         "get_lo": [0, 1, 5],
         "get_los_azel": [0, 1, 5],
-        "lambertian_sphere_to_mv": [0, 1, 5],
         "load_earth": [0, 1, 5],
         "load_moon": [0, 1, 5],
         "load_sun": [0, 1, 5],
         "query_by_lo": [0, 1, 5],
         "radec_to_eci": [0, 1, 5],
         "wcs_from_observer_fix": [0, 1, 5],
         "wcs_from_observer_r": [0, 1, 5],
@@ -60,14 +60,18 @@
         "ephemeri": [0, 1, 18],
         "ephemerisobject": [0, 1, 5],
         "center": [0, 1, 5, 6, 8, 15],
         "create_ephemeris_object": [0, 1, 5],
         "observ": [0, 1, 6, 15, 18, 21],
         "earthobserv": [0, 1, 5],
         "create_observ": [0, 1, 5],
+        "photometr": [0, 1],
+        "lambertian_sphere_model_to_mv": [0, 1, 5],
+        "lambertian_sphere_to_mv": [0, 1, 5],
+        "model_to_mv": [0, 1, 5],
         "random": [0, 1, 4, 6, 21],
         "gen_random_point": [0, 1, 5],
         "sgp4": [0, 1, 4, 18, 21],
         "create_sgp4": [0, 1, 5],
         "load_tl": [0, 1, 5],
         "sprite": [0, 1, 18],
         "load_sprite_from_fil": [0, 1, 5, 6],
@@ -106,15 +110,15 @@
         "analog_to_digit": [0, 1, 6],
         "crop": [0, 1, 6, 18],
         "downsampl": [0, 1, 6],
         "mv_to_p": [0, 1, 6],
         "pe_to_mv": [0, 1, 6],
         "transform_and_add_count": [0, 1, 6, 18],
         "transform_and_fft": [0, 1, 6],
-        "model": [0, 1, 18, 21],
+        "model": [0, 1, 4, 5, 18, 21],
         "astropy_model2d": [0, 1, 6, 18],
         "polygrid2d": [0, 1, 6, 18],
         "radial_cos2d": [0, 1, 6, 18],
         "sin2d": [0, 1, 6, 18],
         "nois": [0, 1, 2, 8, 18, 21],
         "add_photon_nois": [0, 1, 6],
         "add_read_nois": [0, 1, 6],
@@ -196,14 +200,16 @@
         "linspac": [0, 1, 4, 6, 13],
         "mid": [0, 1, 5, 13],
         "to_astropi": [0, 1, 13],
         "to_utc_list": [0, 1, 13],
         "utc": [0, 1, 13],
         "utc_from_list": [0, 1, 13],
         "utc_from_list_or_scalar": [0, 1, 13],
+        "python": [0, 1, 17, 18, 19, 20],
+        "merge_dict": [0, 1, 14],
         "system": [0, 1, 5, 6, 17],
         "configure_eag": [0, 1, 14],
         "configure_multi_gpu": [0, 1, 14],
         "configure_single_gpu": [0, 1, 14],
         "get_semantic_vers": [0, 1, 14],
         "is_tensorflow_running_on_cpu": [0, 1, 14],
         "thread": [0, 1, 18],
@@ -226,15 +232,15 @@
         "zero": [0, 1, 6, 8, 11, 15, 18],
         "ab": [0, 1, 15],
         "add": [0, 1, 5, 6, 7, 13, 14, 15, 17, 18],
         "anglebetween": [0, 1, 15],
         "clamp": [0, 1, 15],
         "clone": [0, 1, 15, 17, 20],
         "cross": [0, 1, 15, 18],
-        "distanc": [0, 1, 4, 5, 15],
+        "distanc": [0, 1, 4, 5, 15, 18],
         "distancesquar": [0, 1, 15],
         "dividebyscalar": [0, 1, 15],
         "dividecompon": [0, 1, 15],
         "dot": [0, 1, 15],
         "equal": [0, 1, 4, 5, 6, 11, 13, 15],
         "equalsepsilon": [0, 1, 15],
         "fromarrai": [0, 1, 15],
@@ -372,24 +378,24 @@
         "gen_imag": [0, 1],
         "gen_multi": [0, 1, 18, 21],
         "image_gener": [0, 1, 18],
         "top": [1, 5, 6, 15],
         "level": [1, 6, 11],
         "dct": 1,
         "merge_dct": 1,
-        "recurs": 1,
+        "recurs": [1, 14],
         "dict": [1, 2, 5, 6, 7, 8, 14, 15],
-        "merg": [1, 19],
+        "merg": [1, 14, 19],
         "inspir": 1,
-        "updat": [1, 17, 18],
+        "updat": [1, 14, 17, 18],
         "instead": [1, 15],
         "onli": [1, 5, 15, 21],
         "kei": [1, 8, 14, 18, 21],
         "down": [1, 5, 6],
-        "nest": 1,
+        "nest": [1, 14],
         "an": [1, 4, 5, 6, 7, 8, 11, 13, 14, 15, 17, 21],
         "arbitrari": [1, 6],
         "depth": 1,
         "The": [1, 2, 5, 6, 8, 11, 14, 15, 17, 20, 21],
         "i": [1, 2, 5, 6, 7, 8, 11, 13, 14, 15, 17, 18, 21],
         "param": [1, 6],
         "onto": [1, 2, 5, 15],
@@ -416,47 +422,47 @@
         "pars": [1, 5],
         "cach": [1, 5, 8, 18],
         "input": [1, 4, 5, 6, 7, 8, 11, 15, 18, 21],
         "argument": [1, 12, 14, 18, 21],
         "mai": [1, 11, 20, 21],
         "contain": [1, 4, 5, 6, 7, 8, 14, 15],
         "follow": [1, 17],
-        "valu": [1, 6, 7, 8, 9, 11, 12, 13, 15, 18, 21],
+        "valu": [1, 6, 7, 8, 9, 11, 12, 13, 14, 15, 18, 21],
         "describ": [1, 6],
         "run": [1, 12, 14, 17, 18, 20, 21],
         "For": [1, 6, 11, 18, 21],
         "exampl": [1, 2, 4, 5, 6, 8, 14, 18, 21],
-        "us": [1, 2, 5, 6, 7, 8, 11, 15, 17, 18, 21],
+        "us": [1, 2, 4, 5, 6, 7, 8, 11, 15, 17, 18, 21],
         "present": 1,
         "tupl": [1, 5, 6, 8, 11],
         "load": [1, 5, 6, 18, 21],
         "from": [1, 4, 5, 6, 7, 8, 13, 14, 15, 18, 19, 21],
         "avail": [1, 5, 21],
         "boolean": [1, 4, 5, 6, 7, 8, 15],
         "true": [1, 4, 5, 6, 7, 8, 14, 15, 18, 21],
         "fals": [1, 4, 5, 6, 7, 13, 15, 18],
         "otherwis": [1, 6, 15],
         "should": [1, 6, 8, 14, 17, 20],
         "my_modul": 1,
         "my_funct": 1,
         "kwarg": [1, 4, 6, 8, 12, 14, 21],
         "param_1": 1,
-        "10": [1, 2, 4, 5, 7, 8, 15, 19, 21],
+        "10": [1, 2, 4, 5, 7, 8, 14, 15, 19, 21],
         "0": [1, 2, 4, 5, 6, 7, 8, 9, 11, 12, 13, 14, 15, 19, 21],
         "param_2": 1,
         "astr": 1,
         "compar": [1, 11, 12, 15],
         "import": [1, 14, 18, 21],
         "lambda": 1,
         "encapsul": 1,
         "func": 1,
         "base": [1, 4, 5, 6, 7, 8, 13, 14, 15, 18, 21],
         "overrid": [1, 21],
         "string": [1, 2, 4, 5, 6, 7, 8, 14],
-        "option": [1, 18, 21],
+        "option": [1, 4, 18, 21],
         "dirnam": [1, 7],
         "none": [1, 4, 5, 6, 7, 8, 9, 11, 13, 14, 15, 16, 18, 20, 21],
         "run_gener": 1,
         "eval_python": 1,
         "run_compound": 1,
         "ani": [1, 6, 7, 15, 17, 20, 21],
         "children": 1,
@@ -481,27 +487,27 @@
         "numpi": [1, 5, 6, 7, 8, 12, 21],
         "p": [1, 5],
         "uniform": [1, 4, 8, 15, 21],
         "low": [1, 4, 6, 8, 21],
         "5": [1, 2, 4, 5, 6, 7, 8, 14, 15, 17, 19, 21],
         "high": [1, 4, 6, 8, 21],
         "22": [1, 21],
-        "x": [1, 4, 5, 6, 8, 9, 11, 15, 18],
+        "x": [1, 4, 5, 6, 8, 9, 11, 14, 15, 18],
         "between": [1, 4, 5, 6, 8, 13, 15, 21],
         "If": [1, 6, 7, 8, 11, 12, 14, 15, 17, 20, 21],
         "choic": 1,
         "chosen": 1,
         "1": [1, 4, 5, 6, 8, 9, 11, 14, 15, 19, 21],
         "2": [1, 2, 4, 5, 6, 7, 8, 11, 14, 15, 19, 21],
         "4": [1, 6, 8, 11, 15, 19, 21],
-        "8": [1, 4, 6, 11, 15, 19, 21],
+        "8": [1, 4, 6, 7, 11, 15, 19, 21],
         "length": [1, 4, 5, 6, 7, 8, 11, 15, 21],
         "randint": [1, 4, 21],
         "e": [1, 5, 6, 7, 8],
-        "7": [1, 4, 7, 15, 19, 21],
+        "7": [1, 4, 15, 19, 21],
         "number": [1, 2, 4, 5, 6, 7, 8, 13, 15, 18, 21],
         "disk": 1,
         "subsequ": 1,
         "call": [1, 8, 11, 12, 14, 15, 21],
         "output_dir": [1, 21],
         "write": [1, 7],
         "arrai": [1, 4, 5, 6, 7, 8, 12, 13, 14, 15, 18, 21],
@@ -509,19 +515,19 @@
         "configur": [1, 4, 6, 7, 8, 14, 18, 19],
         "stage": 1,
         "output": [1, 6, 7, 8, 11, 17, 18, 21],
         "save_pickl": [1, 7, 18],
         "item": 1,
         "serializ": 1,
         "binari": [1, 5],
-        "same": [1, 6, 8, 11],
+        "same": [1, 6, 8, 11, 14],
         "max_stag": 1,
         "with_debug": 1,
         "max_import": 1,
-        "20": [1, 8, 21],
+        "20": [1, 8, 14, 21],
         "max_ref": 1,
         "refer": [1, 6, 7, 14],
         "happen": 1,
         "two": [1, 4, 5, 6, 8, 12, 13, 15, 18, 21],
         "first": [1, 5, 12, 15, 16, 18],
         "second": [1, 4, 5, 6, 7, 12, 13, 14, 15, 21],
         "repeat": 1,
@@ -530,15 +536,15 @@
         "int": [1, 2, 4, 5, 6, 7, 8, 11, 13, 14, 15],
         "maximum": [1, 5, 6, 8, 14, 15, 18, 21],
         "equival": [1, 6, 11, 15],
         "onc": [1, 5, 20],
         "each": [1, 2, 4, 5, 6, 7, 8, 11, 18, 21],
         "after": [1, 4, 11, 14],
         "ref": [1, 4, 18, 20],
-        "place": [1, 5, 6, 7],
+        "place": [1, 5, 6, 7, 14],
         "ssp": [1, 7, 9, 21],
         "eager": [1, 14, 21],
         "sample_num": 1,
         "output_debug": 1,
         "queue": [1, 14],
         "set_nam": 1,
         "singl": [1, 5, 6, 11, 14, 21],
@@ -642,14 +648,15 @@
         "100": [4, 5, 8, 21],
         "target_mv_scal": 4,
         "target_mv": 4,
         "12": [4, 15, 19, 21],
         "offset": [4, 5, 6, 15, 18],
         "breakup_time_offset": 4,
         "variable_bright": 4,
+        "brightness_model": 4,
         "line": [4, 5, 18, 19],
         "element": [4, 5, 11, 12, 15, 18, 21],
         "uct": 4,
         "year": [4, 13, 21],
         "month": [4, 13, 21],
         "dai": [4, 13, 21],
         "hour": [4, 13, 21],
@@ -669,14 +676,17 @@
         "posit": [4, 5, 11, 15, 18],
         "coordin": [4, 5, 6, 7, 8, 11, 15, 18, 21],
         "randomli": [4, 6, 18, 21],
         "assign": [4, 14, 15],
         "sine": [4, 6, 18],
         "variabl": [4, 5, 6, 11, 18],
         "hz": 4,
+        "calcul": [4, 5, 6, 8, 18, 21],
+        "valid": [4, 5, 8, 21],
+        "lambertian_spher": [4, 18],
         "usag": [4, 18, 19],
         "39": 4,
         "site": [4, 18, 21],
         "track": [4, 5, 18, 21],
         "0256606954447602": 4,
         "01": [4, 5, 12, 21],
         "35": [4, 21],
@@ -731,15 +741,15 @@
         "95": 4,
         "02": 4,
         "t": [4, 5, 6, 9, 12, 13, 15, 20, 21],
         "eman": [4, 21],
         "point": [4, 5, 6, 7, 8, 11, 15, 21],
         "elaps": [4, 5, 14],
         "epoch": [4, 5, 6],
-        "3": [4, 5, 6, 7, 8, 11, 15, 17, 19, 21],
+        "3": [4, 5, 6, 8, 11, 14, 15, 17, 19, 21],
         "direct": [4, 5, 6, 15, 21],
         "30": [4, 5, 8, 21],
         "about": [4, 5, 6, 11, 15, 17, 18],
         "mean": [4, 6, 8, 18],
         "express": [4, 15],
         "min": [4, 5, 7, 8, 15],
         "max": [4, 5, 6, 7, 8, 15],
@@ -748,29 +758,28 @@
         "360": [4, 8, 21],
         "txt": [4, 5, 17],
         "delta_dist": 4,
         "delta_position_direct": 4,
         "delta_veloc": 4,
         "delta_velocity_direct": 4,
         "awai": 4,
-        "y": [4, 5, 6, 8, 11, 15, 18],
+        "y": [4, 5, 6, 8, 11, 14, 15, 18],
         "z": [4, 5, 15],
         "vector": [4, 5, 6, 11, 15, 18, 21],
         "delta": [4, 13],
         "001": [4, 12],
         "test": [5, 12, 15, 17, 18],
         "az": 5,
         "el": 5,
         "head": [5, 15, 20],
         "great": [5, 18],
         "propag": [5, 18],
         "skyfield": [5, 7, 13, 18],
         "object_a": 5,
         "object_b": 5,
-        "calcul": [5, 6, 8, 18, 21],
         "ra": [5, 18],
         "dec": 5,
         "sight": 5,
         "right": [5, 6, 15],
         "ascens": 5,
         "declin": 5,
         "deflect": 5,
@@ -846,49 +855,36 @@
         "elev": [5, 18],
         "rr": 5,
         "cc": 5,
         "dr": 5,
         "motion": [5, 18, 21],
         "along": [5, 11, 15],
         "dc": 5,
-        "b": [5, 11, 12, 15, 17],
+        "b": [5, 11, 12, 14, 15, 17],
         "wcs0": 5,
         "wcs1": 5,
         "astropi": [5, 6, 7, 13, 18],
         "world": [5, 15],
         "t_start": [5, 6],
         "corner": [5, 15],
         "get": [5, 6, 14, 15, 19],
         "adjust": 5,
         "icrf_lo": 5,
         "lo": 5,
         "icrf": 5,
-        "albedo": 5,
-        "phase_angl": 5,
-        "lambertian": 5,
-        "approxim": [5, 8],
-        "convert": [5, 6, 11, 13, 15, 21],
-        "sun": [5, 18],
-        "26": 5,
-        "74": 5,
-        "ratio": [5, 8, 15],
-        "reflect": [5, 6, 11],
-        "incid": [5, 6],
-        "off": [5, 15, 18],
-        "surfac": 5,
-        "meter": [5, 15],
         "planetari": 5,
         "lunar": 5,
         "de": 5,
         "421": 5,
         "singleton": 5,
         "satsim_earth": 5,
         "moon": [5, 18],
         "mon": 5,
         "satsim_moon": 5,
+        "sun": [5, 18],
         "satsim_sun": 5,
         "within": [5, 6],
         "plan": 5,
         "visibl": [5, 7, 14],
         "idx": 5,
         "indic": [5, 6, 7],
         "while": 5,
@@ -933,27 +929,41 @@
         "2500": 5,
         "457": 5,
         "6": [5, 15, 17, 19, 21],
         "618": 5,
         "534": 5,
         "quantiti": 5,
         "25000": 5,
+        "phase": [5, 18],
+        "albedo": [5, 18],
+        "phase_angl": [5, 18],
+        "lambertian": [5, 18],
+        "approxim": [5, 8],
+        "convert": [5, 6, 11, 13, 15, 21],
+        "26": 5,
+        "74": 5,
+        "ratio": [5, 8, 15],
+        "reflect": [5, 6, 11],
+        "incid": [5, 6],
+        "off": [5, 15, 18],
+        "surfac": 5,
+        "meter": [5, 15, 18],
         "pe_bin": 5,
         "densiti": [5, 8, 21],
         "bin": [5, 8, 17, 21],
         "stationari": 5,
         "200": [5, 6, 8],
         "vertic": [5, 6, 21],
         "view": [5, 6, 7, 15, 18, 21],
         "horizont": [5, 6, 21],
         "occurr": [5, 8],
         "squar": [5, 6, 15, 18],
         "2x": 5,
         "increas": [5, 6, 21],
-        "size": [5, 6, 7, 8, 11, 14],
+        "size": [5, 6, 7, 8, 11, 14, 18],
         "four": [5, 15],
         "area": 5,
         "tle1": [5, 21],
         "tle2": [5, 21],
         "earthsatellit": 5,
         "url": 5,
         "encod": 5,
@@ -1001,15 +1011,15 @@
         "byte": 5,
         "zoneindex": 5,
         "select": 5,
         "intersect": 5,
         "rectangular": 5,
         "encompass": 5,
         "r": [5, 6, 17],
-        "c": [5, 6, 11, 20],
+        "c": [5, 6, 11, 14, 20],
         "wrap_around": 5,
         "discret": [5, 6, 8],
         "smear": [5, 6, 21],
         "streak": [5, 6],
         "tempor": [5, 6, 18],
         "factor": [5, 6, 15, 18],
         "t_osf": [5, 6],
@@ -1028,15 +1038,14 @@
         "drift": [5, 21],
         "yy": 5,
         "xx": 5,
         "minu": 5,
         "vallado": 5,
         "initi": [5, 15],
         "u": [5, 17],
-        "valid": [5, 8, 21],
         "farnocchia": 5,
         "cowel": 5,
         "state": [5, 18],
         "y_ifov": [5, 6, 7],
         "x_ifov": [5, 6, 7],
         "ifov": 5,
         "cmin": 5,
@@ -1120,15 +1129,15 @@
         "useag": 6,
         "advantag": 6,
         "much": 6,
         "runtim": [6, 18],
         "when": [6, 11, 17, 18, 21],
         "mani": 6,
         "disadvantag": 6,
-        "have": [6, 8, 11, 12, 20, 21],
+        "have": [6, 8, 11, 12, 14, 20, 21],
         "advanc": 6,
         "scientif": 6,
         "lowest": 6,
         "seri": 6,
         "linearli": 6,
         "highest": 6,
         "coeffici": 6,
@@ -1322,20 +1331,20 @@
         "document": [7, 18],
         "obs_cach": 7,
         "scenario": 7,
         "exposure_tim": 7,
         "dt_start": 7,
         "datetim": 7,
         "2024": 7,
-        "23": 7,
-        "33": 7,
-        "44": [7, 21],
-        "552367": 7,
+        "29": 7,
+        "14": [7, 15, 19, 21],
+        "48": 7,
+        "994133": 7,
         "header": [7, 18],
-        "overwrit": 7,
+        "overwrit": [7, 14],
         "np": [7, 12],
         "exposur": [7, 21],
         "placehold": [7, 21],
         "implement": [7, 13, 15, 17],
         "exist": [7, 15],
         "int16": [7, 11, 18],
         "int32": [7, 11, 18],
@@ -1385,15 +1394,15 @@
         "tradit": 8,
         "convolut": [8, 18, 21],
         "kernel": 8,
         "complex64": 8,
         "complex128": 8,
         "fast": 8,
         "fourier": 8,
-        "must": [8, 11, 21],
+        "must": [8, 11, 18, 21],
         "cache_last_i": 8,
         "numer": [8, 21],
         "precis": 8,
         "l": 8,
         "last": [8, 11, 14, 18, 21],
         "improv": [8, 18],
         "perform": [8, 11, 14],
@@ -1546,25 +1555,31 @@
         "signatur": 12,
         "__hash__": 13,
         "dt": 13,
         "num": 13,
         "form": [13, 15],
         "t_list": 13,
         "default_t": 13,
+        "d1": 14,
+        "d2": 14,
+        "both": 14,
+        "those": 14,
+        "conflict": 14,
+        "non": [14, 15, 18],
+        "now": 14,
         "allow_growth": 14,
         "tensorflow": [14, 17, 18, 21],
         "growth": 14,
         "gpu_id": 14,
         "alloc": [14, 15, 21],
         "On": 14,
         "megabyt": 14,
         "logic": 14,
         "semat": 14,
         "version": [14, 17, 18, 20, 21],
-        "non": [14, 15, 18],
         "charact": 14,
         "ver": 14,
         "__version__": 14,
         "semant": 14,
         "cpu": [14, 18],
         "num_thread": 14,
         "round": 14,
@@ -1645,15 +1660,14 @@
         "schur": 15,
         "decomposit": 15,
         "largest": 15,
         "help": [15, 17, 21],
         "reduc": 15,
         "4x4": 15,
         "13": [15, 19, 21],
-        "14": [15, 19, 21],
         "infinit": 15,
         "perspect": 15,
         "below": 15,
         "abov": 15,
         "far": 15,
         "fovi": 15,
         "aspectratio": 15,
@@ -1709,15 +1723,14 @@
         "ai": [17, 20],
         "your": [17, 20],
         "instal": [17, 19],
         "instruct": 17,
         "virtualenvwrapp": 17,
         "mkvirtualenv": 17,
         "cd": 17,
-        "python": [17, 18, 19, 20],
         "pip": [17, 20],
         "requirements_dev": 17,
         "setup": [17, 20],
         "conda": 17,
         "activ": 17,
         "docker": [17, 18],
         "v": 17,
@@ -1783,14 +1796,15 @@
         "send": 17,
         "propos": 17,
         "explain": 17,
         "keep": 17,
         "scope": 17,
         "narrow": 17,
         "easier": 17,
+        "also": [18, 21],
         "turbul": 18,
         "atmospher": 18,
         "turbulent_atmospher": 18,
         "psf_sample_frequ": 18,
         "save_segment": 18,
         "star_annotation_threshold": 18,
         "longer": 18,
@@ -1816,15 +1830,14 @@
         "newest": 18,
         "poliastro": 18,
         "allow": [18, 21],
         "train": 18,
         "speed": 18,
         "trackabl": 18,
         "misc": [18, 21],
-        "phase": 18,
         "track_mod": 18,
         "piecewis": 18,
         "render_s": 18,
         "256": [18, 21],
         "mount": 18,
         "raster": 18,
         "num_target_sampl": 18,
@@ -1872,14 +1885,15 @@
         "tip": 19,
         "deploi": 19,
         "wai": 19,
         "api": 19,
         "credit": 19,
         "lead": 19,
         "contributor": 19,
+        "19": [19, 21],
         "18": [19, 21],
         "search": 19,
         "page": [19, 20],
         "pip3": 20,
         "Or": 20,
         "wheel": 20,
         "termin": 20,
@@ -1924,15 +1938,14 @@
         "a2d": 21,
         "100000": 21,
         "1500": 21,
         "ensquar": 21,
         "gap": 21,
         "num_fram": 21,
         "galact": 21,
-        "19": 21,
         "019444": 21,
         "0055556": 21,
         "016667": 21,
         "036111": 21,
         "038889": 21,
         "097222": 21,
         "66944": 21,
@@ -1944,14 +1957,15 @@
         "017": 21,
         "28": 21,
         "285": 21,
         "53": 21,
         "446": 21,
         "obj": 21,
         "2015": 21,
+        "44": 21,
         "746111": 21,
         "156": 21,
         "431667": 21,
         "gimbal": 21,
         "counter": 21,
         "36411u": 21,
         "10008a": 21,
@@ -1971,15 +1985,14 @@
         "6121": 21,
         "00266852": 21,
         "18866": 21,
         "45075343": 21,
         "custom": 21,
         "access": 21,
         "belong": 21,
-        "also": 21,
         "partial": 21,
         "extern": 21,
         "reus": 21,
         "common": 21,
         "random_raven_fpa": 21
     },
     "objects": {
@@ -2055,35 +2068,36 @@
         ],
         "satsim.geometry": [
             [5, 0, 0, "-", "astrometric"],
             [5, 0, 0, "-", "csvsc"],
             [5, 0, 0, "-", "draw"],
             [5, 0, 0, "-", "ephemeris"],
             [5, 0, 0, "-", "observation"],
+            [5, 0, 0, "-", "photometric"],
             [5, 0, 0, "-", "random"],
             [5, 0, 0, "-", "sgp4"],
             [5, 0, 0, "-", "sprite"],
             [5, 0, 0, "-", "sstr7"],
             [5, 0, 0, "-", "transform"],
             [5, 0, 0, "-", "twobody"],
             [5, 0, 0, "-", "wcs"]
         ],
         "satsim.geometry.astrometric": [
             [5, 2, 1, "", "GreatCircle"],
             [5, 1, 1, "", "angle_between"],
             [5, 1, 1, "", "angle_from_los"],
             [5, 1, 1, "", "apparent"],
             [5, 1, 1, "", "create_topocentric"],
+            [5, 1, 1, "", "distance_between"],
             [5, 1, 1, "", "eci_to_ecr"],
             [5, 1, 1, "", "eci_to_radec"],
             [5, 1, 1, "", "gen_track"],
             [5, 1, 1, "", "gen_track_from_wcs"],
             [5, 1, 1, "", "get_los"],
             [5, 1, 1, "", "get_los_azel"],
-            [5, 1, 1, "", "lambertian_sphere_to_mv"],
             [5, 1, 1, "", "load_earth"],
             [5, 1, 1, "", "load_moon"],
             [5, 1, 1, "", "load_sun"],
             [5, 1, 1, "", "query_by_los"],
             [5, 1, 1, "", "radec_to_eci"],
             [5, 1, 1, "", "wcs_from_observer_fixed"],
             [5, 1, 1, "", "wcs_from_observer_rate"],
@@ -2104,14 +2118,19 @@
         "satsim.geometry.ephemeris.EphemerisObject": [
             [5, 3, 1, "", "center"]
         ],
         "satsim.geometry.observation": [
             [5, 2, 1, "", "EarthObservation"],
             [5, 1, 1, "", "create_observation"]
         ],
+        "satsim.geometry.photometric": [
+            [5, 1, 1, "", "lambertian_sphere_model_to_mv"],
+            [5, 1, 1, "", "lambertian_sphere_to_mv"],
+            [5, 1, 1, "", "model_to_mv"]
+        ],
         "satsim.geometry.random": [
             [5, 1, 1, "", "gen_random_points"]
         ],
         "satsim.geometry.sgp4": [
             [5, 1, 1, "", "create_sgp4"],
             [5, 1, 1, "", "load_tle"]
         ],
@@ -2318,18 +2337,22 @@
             [13, 1, 1, "", "to_astropy"],
             [13, 1, 1, "", "to_utc_list"],
             [13, 1, 1, "", "utc"],
             [13, 1, 1, "", "utc_from_list"],
             [13, 1, 1, "", "utc_from_list_or_scalar"]
         ],
         "satsim.util": [
+            [14, 0, 0, "-", "python"],
             [14, 0, 0, "-", "system"],
             [14, 0, 0, "-", "thread"],
             [14, 0, 0, "-", "timer"]
         ],
+        "satsim.util.python": [
+            [14, 1, 1, "", "merge_dicts"]
+        ],
         "satsim.util.system": [
             [14, 1, 1, "", "configure_eager"],
             [14, 1, 1, "", "configure_multi_gpu"],
             [14, 1, 1, "", "configure_single_gpu"],
             [14, 1, 1, "", "get_semantic_version"],
             [14, 1, 1, "", "is_tensorflow_running_on_cpu"]
         ],
@@ -2731,14 +2754,15 @@
         "io": [4, 7],
         "rpo": 4,
         "astrometr": 5,
         "csvsc": 5,
         "draw": 5,
         "ephemeri": 5,
         "observ": 5,
+        "photometr": 5,
         "random": [5, 8],
         "sgp4": 5,
         "sprite": 5,
         "sstr7": 5,
         "transform": 5,
         "twobodi": 5,
         "wc": 5,
@@ -2762,14 +2786,15 @@
         "tfa": [10, 11, 12],
         "transform_op": 11,
         "translate_op": 11,
         "util": [11, 12, 14],
         "test_util": 12,
         "type": 12,
         "time": 13,
+        "python": [14, 21],
         "system": 14,
         "thread": 14,
         "timer": 14,
         "vecmath": 15,
         "cartesian2": 15,
         "cartesian3": 15,
         "cartesian4": 15,
@@ -2794,14 +2819,15 @@
         "report": 17,
         "bug": 17,
         "write": 17,
         "submit": 17,
         "feedback": 17,
         "histori": 18,
         "0": 18,
+        "19": 18,
         "18": 18,
         "17": 18,
         "1": 18,
         "16": 18,
         "15": 18,
         "14": 18,
         "13": 18,
@@ -2821,15 +2847,14 @@
         "tabl": 19,
         "instal": 20,
         "stabl": 20,
         "releas": 20,
         "from": 20,
         "sourc": 20,
         "usag": 21,
-        "python": 21,
         "command": 21,
         "line": 21,
         "interfac": 21,
         "paramet": 21,
         "configur": 21
     },
     "envversion": {
@@ -2920,14 +2945,17 @@
         ],
         "satsim.geometry.ephemeris module": [
             [5, "module-satsim.geometry.ephemeris"]
         ],
         "satsim.geometry.observation module": [
             [5, "module-satsim.geometry.observation"]
         ],
+        "satsim.geometry.photometric module": [
+            [5, "module-satsim.geometry.photometric"]
+        ],
         "satsim.geometry.random module": [
             [5, "module-satsim.geometry.random"]
         ],
         "satsim.geometry.sgp4 module": [
             [5, "module-satsim.geometry.sgp4"]
         ],
         "satsim.geometry.sprite module": [
@@ -3034,14 +3062,17 @@
         ],
         "satsim.time package": [
             [13, "module-satsim.time"]
         ],
         "satsim.util package": [
             [14, "module-satsim.util"]
         ],
+        "satsim.util.python module": [
+            [14, "module-satsim.util.python"]
+        ],
         "satsim.util.system module": [
             [14, "module-satsim.util.system"]
         ],
         "satsim.util.thread module": [
             [14, "module-satsim.util.thread"]
         ],
         "satsim.util.timer module": [
@@ -3106,101 +3137,104 @@
         ],
         "Submit Feedback": [
             [17, "submit-feedback"]
         ],
         "History": [
             [18, "history"]
         ],
-        "0.18.0": [
+        "0.19.0": [
             [18, "id1"]
         ],
-        "0.17.1": [
+        "0.18.0": [
             [18, "id2"]
         ],
-        "0.17.0": [
+        "0.17.1": [
             [18, "id3"]
         ],
-        "0.16.0": [
+        "0.17.0": [
             [18, "id4"]
         ],
-        "0.15.1": [
+        "0.16.0": [
             [18, "id5"]
         ],
-        "0.15.0": [
+        "0.15.1": [
             [18, "id6"]
         ],
-        "0.14.0": [
+        "0.15.0": [
             [18, "id7"]
         ],
-        "0.13.1": [
+        "0.14.0": [
             [18, "id8"]
         ],
-        "0.13.0": [
+        "0.13.1": [
             [18, "id9"]
         ],
-        "0.12.0": [
+        "0.13.0": [
             [18, "id10"]
         ],
-        "0.11.0": [
+        "0.12.0": [
             [18, "id11"]
         ],
-        "0.10.0": [
+        "0.11.0": [
             [18, "id12"]
         ],
-        "0.9.1": [
+        "0.10.0": [
             [18, "id13"]
         ],
-        "0.9.0": [
+        "0.9.1": [
             [18, "id14"]
         ],
-        "0.8.3": [
+        "0.9.0": [
             [18, "id15"]
         ],
-        "0.8.2": [
+        "0.8.3": [
             [18, "id16"]
         ],
-        "0.8.1": [
+        "0.8.2": [
             [18, "id17"]
         ],
-        "0.8.0": [
+        "0.8.1": [
             [18, "id18"]
         ],
-        "0.7.2": [
+        "0.8.0": [
             [18, "id19"]
         ],
-        "0.7.1": [
+        "0.7.2": [
             [18, "id20"]
         ],
-        "0.7.0": [
+        "0.7.1": [
             [18, "id21"]
         ],
-        "0.6.1": [
+        "0.7.0": [
             [18, "id22"]
         ],
-        "0.6.0": [
+        "0.6.1": [
             [18, "id23"]
         ],
-        "0.5.0": [
+        "0.6.0": [
             [18, "id24"]
         ],
-        "0.4.0": [
+        "0.5.0": [
             [18, "id25"]
         ],
-        "0.3.0": [
+        "0.4.0": [
             [18, "id26"]
         ],
-        "0.2.0": [
+        "0.3.0": [
             [18, "id27"]
         ],
-        "0.1.1": [
+        "0.2.0": [
             [18, "id28"]
         ],
-        "0.1.0": [
+        "0.1.1": [
             [18, "id29"]
         ],
+        "0.1.0": [
+            [18, "id30"]
+        ],
         "Documentation for SatSim": [
             [19, "documentation-for-satsim"]
         ],
         "Contents:": [
             [19, null]
         ],
         "Indices and tables": [
@@ -3266,14 +3300,15 @@
             [4, "module-satsim.generator.obs.rpo"],
             [5, "module-satsim.geometry"],
             [5, "module-satsim.geometry.astrometric"],
             [5, "module-satsim.geometry.csvsc"],
             [5, "module-satsim.geometry.draw"],
             [5, "module-satsim.geometry.ephemeris"],
             [5, "module-satsim.geometry.observation"],
+            [5, "module-satsim.geometry.photometric"],
             [5, "module-satsim.geometry.random"],
             [5, "module-satsim.geometry.sgp4"],
             [5, "module-satsim.geometry.sprite"],
             [5, "module-satsim.geometry.sstr7"],
             [5, "module-satsim.geometry.transform"],
             [5, "module-satsim.geometry.twobody"],
             [5, "module-satsim.geometry.wcs"],
@@ -3304,14 +3339,15 @@
             [11, "module-satsim.tfa.image.translate_ops"],
             [11, "module-satsim.tfa.image.utils"],
             [12, "module-satsim.tfa.utils"],
             [12, "module-satsim.tfa.utils.test_utils"],
             [12, "module-satsim.tfa.utils.types"],
             [13, "module-satsim.time"],
             [14, "module-satsim.util"],
+            [14, "module-satsim.util.python"],
             [14, "module-satsim.util.system"],
             [14, "module-satsim.util.thread"],
             [14, "module-satsim.util.timer"],
             [15, "module-satsim.vecmath"],
             [15, "module-satsim.vecmath.Cartesian2"],
             [15, "module-satsim.vecmath.Cartesian3"],
             [15, "module-satsim.vecmath.Cartesian4"],
@@ -3463,14 +3499,17 @@
         ],
         "create_twobody() (in module satsim.geometry.twobody)": [
             [5, "satsim.geometry.twobody.create_twobody"]
         ],
         "create_twobody_from_tle() (in module satsim.geometry.twobody)": [
             [5, "satsim.geometry.twobody.create_twobody_from_tle"]
         ],
+        "distance_between() (in module satsim.geometry.astrometric)": [
+            [5, "satsim.geometry.astrometric.distance_between"]
+        ],
         "eci_to_ecr() (in module satsim.geometry.astrometric)": [
             [5, "satsim.geometry.astrometric.eci_to_ecr"]
         ],
         "eci_to_radec() (in module satsim.geometry.astrometric)": [
             [5, "satsim.geometry.astrometric.eci_to_radec"]
         ],
         "gen_curve_from_points() (in module satsim.geometry.draw)": [
@@ -3502,16 +3541,19 @@
         ],
         "get_star_mv() (in module satsim.geometry.sstr7)": [
             [5, "satsim.geometry.sstr7.get_star_mv"]
         ],
         "get_wcs() (in module satsim.geometry.wcs)": [
             [5, "satsim.geometry.wcs.get_wcs"]
         ],
-        "lambertian_sphere_to_mv() (in module satsim.geometry.astrometric)": [
-            [5, "satsim.geometry.astrometric.lambertian_sphere_to_mv"]
+        "lambertian_sphere_model_to_mv() (in module satsim.geometry.photometric)": [
+            [5, "satsim.geometry.photometric.lambertian_sphere_model_to_mv"]
+        ],
+        "lambertian_sphere_to_mv() (in module satsim.geometry.photometric)": [
+            [5, "satsim.geometry.photometric.lambertian_sphere_to_mv"]
         ],
         "load_earth() (in module satsim.geometry.astrometric)": [
             [5, "satsim.geometry.astrometric.load_earth"]
         ],
         "load_index() (in module satsim.geometry.sstr7)": [
             [5, "satsim.geometry.sstr7.load_index"]
         ],
@@ -3529,14 +3571,17 @@
         ],
         "load_tle() (in module satsim.geometry.sgp4)": [
             [5, "satsim.geometry.sgp4.load_tle"]
         ],
         "load_zone() (in module satsim.geometry.sstr7)": [
             [5, "satsim.geometry.sstr7.load_zone"]
         ],
+        "model_to_mv() (in module satsim.geometry.photometric)": [
+            [5, "satsim.geometry.photometric.model_to_mv"]
+        ],
         "query_by_los() (in module satsim.geometry.astrometric)": [
             [5, "satsim.geometry.astrometric.query_by_los"]
         ],
         "query_by_los() (in module satsim.geometry.csvsc)": [
             [5, "satsim.geometry.csvsc.query_by_los"]
         ],
         "query_by_los() (in module satsim.geometry.sstr7)": [
@@ -3568,14 +3613,17 @@
         ],
         "satsim.geometry.ephemeris": [
             [5, "module-satsim.geometry.ephemeris"]
         ],
         "satsim.geometry.observation": [
             [5, "module-satsim.geometry.observation"]
         ],
+        "satsim.geometry.photometric": [
+            [5, "module-satsim.geometry.photometric"]
+        ],
         "satsim.geometry.random": [
             [5, "module-satsim.geometry.random"]
         ],
         "satsim.geometry.sgp4": [
             [5, "module-satsim.geometry.sgp4"]
         ],
         "satsim.geometry.sprite": [
@@ -3994,17 +4042,23 @@
         ],
         "has_tag() (satsim.util.thread.threadedtaskqueue method)": [
             [14, "satsim.util.thread.ThreadedTaskQueue.has_tag"]
         ],
         "is_tensorflow_running_on_cpu() (in module satsim.util.system)": [
             [14, "satsim.util.system.is_tensorflow_running_on_cpu"]
         ],
+        "merge_dicts() (in module satsim.util.python)": [
+            [14, "satsim.util.python.merge_dicts"]
+        ],
         "satsim.util": [
             [14, "module-satsim.util"]
         ],
+        "satsim.util.python": [
+            [14, "module-satsim.util.python"]
+        ],
         "satsim.util.system": [
             [14, "module-satsim.util.system"]
         ],
         "satsim.util.thread": [
             [14, "module-satsim.util.thread"]
         ],
         "satsim.util.timer": [
```

### Comparing `satsim-0.18.0/docs/_build/html/usage.html` & `satsim-0.19.0/docs/_build/html/usage.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 <!DOCTYPE html>
 <html class="writer-html5" lang="en" >
 <head>
   <meta charset="utf-8" /><meta name="generator" content="Docutils 0.18.1: http://docutils.sourceforge.net/" />
 
   <meta name="viewport" content="width=device-width, initial-scale=1.0" />
-  <title>Usage &mdash; SatSim 0.18.0 documentation</title>
+  <title>Usage &mdash; SatSim 0.19.0 documentation</title>
       <link rel="stylesheet" href="_static/pygments.css" type="text/css" />
       <link rel="stylesheet" href="_static/css/theme.css" type="text/css" />
   <!--[if lt IE 9]>
     <script src="_static/js/html5shiv.min.js"></script>
   <![endif]-->
   
         <script data-url_root="./" id="documentation_options" src="_static/documentation_options.js"></script>
@@ -29,15 +29,15 @@
 
           
           
           <a href="index.html" class="icon icon-home">
             SatSim
           </a>
               <div class="version">
-                0.18.0
+                0.19.0
               </div>
 <div role="search">
   <form id="rtd-search-form" class="wy-form" action="search.html" method="get">
     <input type="text" name="q" placeholder="Search docs" aria-label="Search docs" />
     <input type="hidden" name="check_keywords" value="yes" />
     <input type="hidden" name="area" value="default" />
   </form>
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 _S_a_t_S_i_m
-0.18.0
+0.19.0
 [q                   ]
 Contents:
     * _I_n_s_t_a_l_l_a_t_i_o_n
     * _U_s_a_g_e
           o _P_y_t_h_o_n_ _M_o_d_u_l_e
           o _C_o_m_m_a_n_d_ _L_i_n_e_ _I_n_t_e_r_f_a_c_e
           o _P_a_r_a_m_e_t_e_r_s_ _a_n_d_ _C_o_n_f_i_g_u_r_a_t_i_o_n
```

### Comparing `satsim-0.18.0/docs/api/satsim.generator.obs.rst` & `satsim-0.19.0/docs/api/satsim.generator.obs.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/api/satsim.geometry.rst` & `satsim-0.19.0/docs/api/satsim.geometry.rst`

 * *Files 8% similar despite different names*

```diff
@@ -45,14 +45,22 @@
 ----------------------------------
 
 .. automodule:: satsim.geometry.observation
    :members:
    :undoc-members:
    :show-inheritance:
 
+satsim.geometry.photometric module
+----------------------------------
+
+.. automodule:: satsim.geometry.photometric
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 satsim.geometry.random module
 -----------------------------
 
 .. automodule:: satsim.geometry.random
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `satsim-0.18.0/docs/api/satsim.image.rst` & `satsim-0.19.0/docs/api/satsim.image.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/api/satsim.io.rst` & `satsim-0.19.0/docs/api/satsim.io.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/api/satsim.math.rst` & `satsim-0.19.0/docs/api/satsim.math.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/api/satsim.rst` & `satsim-0.19.0/docs/api/satsim.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/api/satsim.tfa.image.rst` & `satsim-0.19.0/docs/api/satsim.tfa.image.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/api/satsim.util.rst` & `satsim-0.19.0/docs/api/satsim.util.rst`

 * *Files 10% similar despite different names*

```diff
@@ -5,14 +5,22 @@
    :members:
    :undoc-members:
    :show-inheritance:
 
 Submodules
 ----------
 
+satsim.util.python module
+-------------------------
+
+.. automodule:: satsim.util.python
+   :members:
+   :undoc-members:
+   :show-inheritance:
+
 satsim.util.system module
 -------------------------
 
 .. automodule:: satsim.util.system
    :members:
    :undoc-members:
    :show-inheritance:
```

### Comparing `satsim-0.18.0/docs/api/satsim.vecmath.rst` & `satsim-0.19.0/docs/api/satsim.vecmath.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/conf.py` & `satsim-0.19.0/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,24 +54,24 @@
 author = u"Alex Cabello"
 
 # The version info for the project you're documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The short X.Y version.
-version = '0.18.0'
+version = '0.19.0'
 # The full version, including alpha/beta/rc tags.
-release = '0.18.0'
+release = '0.19.0'
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
-language = None
+language = "en"
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
 # This patterns also effect to html_static_path and html_extra_path
 exclude_patterns = ['_build', 'Thumbs.db', '.DS_Store', 
     'api/satsim.cli.rst']
 
@@ -94,15 +94,15 @@
 # documentation.
 #
 # html_theme_options = {}
 
 # Add any paths that contain custom static files (such as style sheets) here,
 # relative to this directory. They are copied after the builtin static files,
 # so a file named "default.css" will overwrite the builtin "default.css".
-html_static_path = ['static']
+# html_static_path = ['static']
 
 
 # -- Options for HTMLHelp output ---------------------------------------
 
 # Output file base name for HTML help builder.
 htmlhelp_basename = 'satsimdoc'
```

### Comparing `satsim-0.18.0/docs/installation.rst` & `satsim-0.19.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/make.bat` & `satsim-0.19.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/docs/usage.rst` & `satsim-0.19.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/cli.py` & `satsim-0.19.0/satsim/cli.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/config.py` & `satsim-0.19.0/satsim/config.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/dataset/augment.py` & `satsim-0.19.0/satsim/dataset/augment.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/generator/obs/breakup.py` & `satsim-0.19.0/satsim/generator/obs/breakup.py`

 * *Files 15% similar despite different names*

```diff
@@ -16,29 +16,33 @@
     x_world = np.cross(z_world, y_world)
     y_world = np.cross(x_world, z_world)
     world = np.array([x_world, y_world, z_world])
     M = np.linalg.solve(local,world).T
     return M
 
 
-def _generate_random_mv(mv, scale, n, sigma=1.0):
-    ZP = 1.0
+def _generate_random_mv_or_size(mv_or_size, scale, n, sigma=1.0, brightness_model='mv'):
     # samples = np.abs(np.random.normal(0, sigma, n))
     samples = np.abs(np.random.lognormal(0, sigma, n))
-    samples = samples / np.sum(samples)
-    pe_target = mv_to_pe(ZP, mv)
-    pe_part = samples * pe_target
-    return pe_to_mv(ZP, pe_target * scale[0]), pe_to_mv(ZP, pe_part * scale[1])
+    samples = samples / np.sum(samples)  # normalize
+
+    if brightness_model == 'mv':
+        ZP = 1.0
+        pe_target = mv_to_pe(ZP, mv_or_size)
+        pe_part = samples * pe_target
+        return pe_to_mv(ZP, pe_target * scale[0]), pe_to_mv(ZP, pe_part * scale[1])
+    else:
+        return mv_or_size * scale[0], samples * mv_or_size * scale[1]
 
 
 def collision_from_tle(tle, collision_time, radius=37.5, K=0.5,
                        attack_angle='random', attack_velocity=None, attack_velocity_scale=1.0,
                        n=[100,100], target_mv_scale=[0.5, 2.0], rpo_mv_scale=[0.5, 2.0],
                        target_mv=12.0, rpo_mv=12.0, offset=[0.0, 0.0], collision_time_offset=0.0, variable_brightness=True,
-                       fragment_angle='random', scale_fragment_velocity=False):
+                       fragment_angle='random', scale_fragment_velocity=False, brightness_model='mv'):
     """Generates a two object collision configuration from the input `tle`.
 
     Args:
         tle: `array`, an array containing the SGP4 two line element set.
         collision_time: `array`, UCT time as year, month, day, hour, minute, seconds.
         radius: `float`, one sigma breakup cone radius in degrees. default=37.5
         K: `array or `float`, one sigma velocity transfer multiplier from colliding object. default=0.5
@@ -51,14 +55,15 @@
         target_mv: `float`, brightness of target before collision in visual magnitude. default=12
         rpo_mv: `float`, brightness of colliding object before collision in visual magnitude. default=12
         offset: `array`, row column offset of target position on fpa in normalized coordinates. default=[0,0]
         collision_time_offset: `float`, number of seconds to offset collision time from `collision_time`. default=0
         variable_brightness: `boolean`, if True randomly assign sine variable brightness between 0 to 1 hz. default=True
         fragment_angle: `string`, specified the fragment angle sampling. `random` or `linspace`. default=`random`
         scale_fragment_velocity: `boolean`, if True scale the fragment velocity by cosine of the exit velocity. default=`false`
+        brightness_model: `string`, the model to use for brightness calculations. valid options `mv`, `lambertian_sphere` default=`mv`
 
     Example usage in SatSim configuration::
 
         "obs": {
             "generator": {
                 "module": "satsim.generator.obs.breakup",
                 "function": "collision_from_tle",
@@ -105,18 +110,18 @@
         K = [K, K]
 
     sat = EarthSatellite(tle[0], tle[1])
     t = time.utc_from_list(collision_time, collision_time_offset)
     collision_time = time.to_utc_list(t)
 
     # brightness calculations
-    target_mv_after, target_particles_mv = _generate_random_mv(target_mv, target_mv_scale, n[0], np.random.uniform(0.0,1.0))
+    target_mv_after, target_particles_mv = _generate_random_mv_or_size(target_mv, target_mv_scale, n[0], np.random.uniform(0.0,1.0), brightness_model=brightness_model)
 
     if rpo_mv is not None:
-        rpo_mv_after, rpo_particles_mv = _generate_random_mv(rpo_mv, rpo_mv_scale, n[1], np.random.uniform(0.0,1.0))
+        rpo_mv_after, rpo_particles_mv = _generate_random_mv_or_size(rpo_mv, rpo_mv_scale, n[1], np.random.uniform(0.0,1.0), brightness_model=brightness_model)
     else:
         rpo_mv_after, rpo_particles_mv = (None, [])
 
     # get state vector at time t
     position, velocity0, _, _ = sat._at(t)
     position *= AU_KM
     velocity0 *= AU_KM
@@ -180,113 +185,154 @@
 
     # scale and rotate for target1
     M1 = _rotation_from_vectors(dv0 / dv0_mag)
     vv[ndiv2:,:] *= np.random.normal(0, dv0_mag * K[1], n)[ndiv2:, np.newaxis]
     vv[ndiv2:,2] = np.abs(vv[ndiv2:,2])
     vv[ndiv2:,:] = M1.dot(vv[ndiv2:,:].T).T + velocity1
 
-    if variable_brightness is True:
-        def mv_func(mv_in):
-            return {
-                "$pipeline": [
-                    {
-                        "module": "satsim.pipeline",
-                        "function": "constant",
-                        "kwargs": {
-                            "value": mv_in
-                        }
-                    },
-                    {
-                        "module": "satsim.pipeline",
-                        "function": "sin_add",
-                        "kwargs": {
-                            "freq": np.random.normal(0, 1.0),
-                            "mag_scale": np.random.uniform(0, 7.0)
-                        }
-                    }
-                ]
-            }
-    else:
-        def mv_func(mv_in):
-            return mv_in
-
     obs = {
         "mode": "list",
         "list": [{
             "mode": "twobody",
             "position": list(position),
             "velocity": list(v),
             "epoch": collision_time,
-            "mv": mv_func(m),
             "offset": offset,
             "events": {
                 "create": collision_time
             }
         } for v, m in zip(vv, np.concatenate([target_particles_mv, rpo_particles_mv]))]
     }
 
+    target_obs = None
     if target_mv is not None:
-        obs['list'].append({
+        target_obs = {
             "mode": "twobody",
             "position": list(position),
             "velocity": list(velocity0),
             "epoch": collision_time,
-            "mv": target_mv,
             "offset": offset,
             "events": {
                 "update": [
                     {
                         "time": collision_time,
                         "values": {
-                            "mv": mv_func(target_mv_after)
                         }
                     }
                 ]
             }
-        })
+        }
+        obs['list'].append(target_obs)
 
+    rpo_obs = None
     if rpo_mv is not None:
-        obs['list'].append({
+        rpo_obs = {
             "mode": "twobody",
             "position": list(position),
             "velocity": list(velocity1),
             "epoch": collision_time,
-            "mv": rpo_mv,
             "offset": offset,
             "events": {
                 "update": [
                     {
                         "time": collision_time,
                         "values": {
-                            "mv": mv_func(rpo_mv_after)
                         }
                     }
                 ]
             }
-        })
+        }
+        obs['list'].append(rpo_obs)
+
+    if variable_brightness is True:
+        def mv_func(mv_in):
+            return {
+                "$pipeline": [
+                    {
+                        "module": "satsim.pipeline",
+                        "function": "constant",
+                        "kwargs": {
+                            "value": mv_in
+                        }
+                    },
+                    {
+                        "module": "satsim.pipeline",
+                        "function": "sin_add",
+                        "kwargs": {
+                            "freq": np.random.normal(0, 1.0),
+                            "mag_scale": np.random.uniform(0, 7.0)
+                        }
+                    }
+                ]
+            }
+    else:
+        def mv_func(mv_in):
+            return mv_in
+
+    if brightness_model == 'mv':
+
+        for i, m in enumerate(np.concatenate([target_particles_mv, rpo_particles_mv])):
+            obs['list'][i]['mv'] = mv_func(m)
+
+        if target_obs is not None:
+            target_obs['mv'] = mv_func(target_mv_after)
+            target_obs['events']['update'][-1]['values']['mv'] = mv_func(target_mv_after)
+        if rpo_obs is not None:
+            rpo_obs['mv'] = mv_func(rpo_mv_after)
+            rpo_obs['events']['update'][-1]['values']['mv'] = mv_func(rpo_mv_after)
+
+    else:
+        albedo = 0.3  # TODO: make this a parameter
+        for i, m in enumerate(np.concatenate([target_particles_mv, rpo_particles_mv])):
+            obs['list'][i]['model'] = {
+                'mode': brightness_model,
+                'albedo': albedo,
+                'size': m
+            }
+
+        if target_obs is not None:
+            target_obs['model'] = {
+                'mode': brightness_model,
+                'albedo': albedo,
+                'size': target_mv
+            }
+            target_obs['events']['update'][-1]['values']['model'] = {
+                'size': target_mv_after
+            }
+
+        if rpo_obs is not None:
+            rpo_obs['model'] = {
+                'mode': brightness_model,
+                'albedo': albedo,
+                'size': rpo_mv
+            }
+            rpo_obs['events']['update'][-1]['values']['model'] = {
+                'size': rpo_mv_after
+            }
 
     return obs
 
 
 def breakup_from_tle(tle, breakup_time, radius=37.5, breakup_velocity=108,
                      n=100, target_mv_scale=[0.5, 2.0], target_mv=12.0,
                      offset=[0.0, 0.0], breakup_time_offset=0.0,
-                     variable_brightness=True):
+                     variable_brightness=True, brightness_model='mv'):
     """Generates a breakup configuration from the input `tle`.
 
     Args:
         tle: `array`, an array containing the SGP4 two line element set.
         breakup_time: `array`, UCT time as year, month, day, hour, minute, seconds.
         radius: `float`, one sigma breakup cone radius in degrees. default=37.5
         breakup_velocity: `float`, the relative velocity of generated particles in km/s. default=108
         n: `array`, number of particles to generate. default=100
         target_mv_scale: `array`, brightness of target and total brightness of generated particles after breakup. scale based on original target brightness. default=[0.5,2.0]
         offset: `array`, row column offset of target position on fpa in normalized coordinates. default=12
         breakup_time_offset: `float`, number of seconds to offset breakup time from `breakup`. default=[0,0]
         variable_brightness: `boolean`, if True randomly assign sine variable brightness between 0 to 1 hz. default=True
+        brightness_model: `string`, the model to use for brightness calculations. valid options `mv`, `lambertian_sphere` default=`mv`
 
     Example usage in SatSim configuration::
 
         "obs": {
             "generator": {
                 "module": "satsim.generator.obs.breakup",
                 "function": "breakup_from_tle",
@@ -315,10 +361,10 @@
             }
         }
     """
     obs = collision_from_tle(tle, breakup_time, radius=radius, K=1.0,
                              attack_angle='random', attack_velocity=breakup_velocity, attack_velocity_scale=1.0,
                              n=n, target_mv_scale=target_mv_scale, rpo_mv_scale=None, target_mv=target_mv, rpo_mv=None,
                              offset=offset, collision_time_offset=breakup_time_offset, variable_brightness=variable_brightness,
-                             scale_fragment_velocity=False)
+                             scale_fragment_velocity=False, brightness_model=brightness_model)
 
     return obs
```

### Comparing `satsim-0.18.0/satsim/generator/obs/cso.py` & `satsim-0.19.0/satsim/generator/obs/cso.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/generator/obs/geometry.py` & `satsim-0.19.0/satsim/generator/obs/geometry.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/generator/obs/io.py` & `satsim-0.19.0/satsim/generator/obs/io.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/generator/obs/rpo.py` & `satsim-0.19.0/satsim/generator/obs/rpo.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/geometry/astrometric.py` & `satsim-0.19.0/satsim/geometry/astrometric.py`

 * *Files 2% similar despite different names*

```diff
@@ -512,14 +512,31 @@
     o = observer.at(t)
     a = o.observe(object_a).apparent()
     b = o.observe(object_b).apparent()
 
     return a.separation_from(b).degrees
 
 
+def distance_between(object_a, object_b, t):
+    """Calculate the distance between `object_a` and `object_b` at time `t`.
+
+    Args:
+        object_a: `object`, Skyfield object
+        object_b: `object`, Skyfield object
+        t: `Time`, Skyfield `Time`
+
+    Returns:
+        A `float`, distance in km
+    """
+    a = object_a.at(t)
+    b = object_b.at(t)
+
+    return (a - b).distance().km
+
+
 def angle_from_los(observer, object_a, ra, dec, t):
     """Calculate the angle between `observer` to `object_a` and `observer`
     to a line of sight in `ra` and `dec`. Angle is returned in degrees.
 
     Args:
         observer: `object`, Skyfield object
         object_a: `object`, Skyfield object
@@ -531,42 +548,14 @@
         A `float`, angle in degrees
     """
     s = Star(ra=Angle(degrees=ra), dec=Angle(degrees=dec))
 
     return angle_between(observer, s, object_a, t)
 
 
-def lambertian_sphere_to_mv(albedo, distance, radius, phase_angle):
-    """Applies lambertian sphere approximation to convert target brightness
-    to visual magnitudes based on sun brightness of -26.74.
-
-    Args:
-        albedo: `float`, The ratio of reflected light to incident light
-            off of the object's surface
-        distance: `float`, distance to object in meters
-        radius: `float`, radius of sphere in meters
-        phase_angle: `float`, the angle between observer, object, and sun in degrees
-
-    Returns:
-        A `float`, calculated visual magnitude
-    """
-    phase_angle = np.deg2rad(phase_angle)
-
-    mv_sun = -26.74
-
-    # Lambertian sphere approximation.
-    phase_factor = np.sin(phase_angle) + (np.pi - phase_angle) * np.cos(phase_angle)
-    intensity = phase_factor * (2 * albedo * (radius * radius)) / (3 * np.pi * (distance * distance))
-
-    # Convert intensities to magnitudes
-    mvVector = mv_sun - 2.5 * np.log10(intensity)
-
-    return mvVector
-
-
 def eci_to_ecr(time, ra, dec, roll=0):
     """Covert an Earth centered fixed sky coordinates to Earth centered rotating.
 
     Args:
         ra: `float`, right ascension in degrees
         dec: `float`, declination in degrees
         roll: `float`, field rotation (ignored)
```

### Comparing `satsim-0.18.0/satsim/geometry/csvsc.py` & `satsim-0.19.0/satsim/geometry/csvsc.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/geometry/draw.py` & `satsim-0.19.0/satsim/geometry/draw.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/geometry/ephemeris.py` & `satsim-0.19.0/satsim/geometry/ephemeris.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/geometry/observation.py` & `satsim-0.19.0/satsim/geometry/observation.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/geometry/random.py` & `satsim-0.19.0/satsim/geometry/random.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/geometry/sgp4.py` & `satsim-0.19.0/satsim/geometry/sgp4.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/geometry/sprite.py` & `satsim-0.19.0/satsim/geometry/sprite.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/geometry/sstr7.py` & `satsim-0.19.0/satsim/geometry/sstr7.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/geometry/transform.py` & `satsim-0.19.0/satsim/geometry/transform.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/geometry/twobody.py` & `satsim-0.19.0/satsim/geometry/twobody.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         # self.target_name = name
 
     def _at(self, t):
         """Compute this satellite's GCRS position and velocity at time `t`."""
         tt = _to_astropy(t)
         td = tt - self.epoch['time']
 
-        if td.size > 1:
+        if td.ndim > 0:
             rGCRS = np.zeros((3, td.size))
             vGCRS = np.zeros((3, td.size))
             for i in range(td.size):
                 o = self.orbit.propagate(td[i], method=self.method)
                 r, v = o.rv()
                 rGCRS[:, i] = r.to(u.km).value
                 vGCRS[:, i] = v.to(u.km / u.s).value
```

### Comparing `satsim-0.18.0/satsim/geometry/wcs.py` & `satsim-0.19.0/satsim/geometry/wcs.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/image/augment.py` & `satsim-0.19.0/satsim/image/augment.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/image/fpa.py` & `satsim-0.19.0/satsim/image/fpa.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/image/model.py` & `satsim-0.19.0/satsim/image/model.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/image/noise.py` & `satsim-0.19.0/satsim/image/noise.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/image/psf.py` & `satsim-0.19.0/satsim/image/psf.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/image/render.py` & `satsim-0.19.0/satsim/image/render.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/io/czml.py` & `satsim-0.19.0/satsim/io/czml.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/io/fits.py` & `satsim-0.19.0/satsim/io/fits.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/io/image.py` & `satsim-0.19.0/satsim/io/image.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/io/satnet.py` & `satsim-0.19.0/satsim/io/satnet.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/math/angle.py` & `satsim-0.19.0/satsim/math/angle.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/math/const.py` & `satsim-0.19.0/satsim/math/const.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/math/conv.py` & `satsim-0.19.0/satsim/math/conv.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/math/fft.py` & `satsim-0.19.0/satsim/math/fft.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/math/interpolate.py` & `satsim-0.19.0/satsim/math/interpolate.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/math/random.py` & `satsim-0.19.0/satsim/math/random.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/math/stats.py` & `satsim-0.19.0/satsim/math/stats.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/pipeline/__init__.py` & `satsim-0.19.0/satsim/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/satsim.py` & `satsim-0.19.0/satsim/satsim.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,22 +26,23 @@
 from satsim.geometry.draw import gen_line, gen_line_from_endpoints, gen_curve_from_points
 from satsim.geometry.random import gen_random_points
 from satsim.geometry.sstr7 import query_by_los
 from satsim.geometry.csvsc import query_by_los as csvsc_query_by_los
 from satsim.geometry.sgp4 import create_sgp4
 from satsim.geometry.ephemeris import create_ephemeris_object
 from satsim.geometry.astrometric import create_topocentric, gen_track, get_los, get_los_azel, GreatCircle
+from satsim.geometry.photometric import model_to_mv
 from satsim.geometry.twobody import create_twobody
 from satsim.geometry.observation import create_observation
 from satsim.io.satnet import write_frame, set_frame_annotation, init_annotation
 from satsim.io.image import save_apng
 from satsim.io.czml import save_czml
-from satsim.util import tic, toc, MultithreadedTaskQueue, configure_eager, configure_single_gpu
+from satsim.util import tic, toc, MultithreadedTaskQueue, configure_eager, configure_single_gpu, merge_dicts
 from satsim.config import transform, save_debug, _transform, save_cache
-from satsim.pipeline import _delta_t
+from satsim.pipeline import _delta_t, _avg_t
 from satsim import time
 
 logger = logging.getLogger(__name__)
 
 
 def gen_multi(ssp, eager=True, output_dir='./', input_dir='./', device=None, memory=None, pid=0, output_debug=False, folder_name=None):
     """Generates multiple sets of images. Number of sets is based on the
@@ -925,36 +926,40 @@
     ts_mid = time.utc_from_list(tt, t_start + 0.5 * (t_end - t_start))
     ts_end = time.utc_from_list(tt, t_end)
 
     for i, o in enumerate(obs):
 
         # TODO support in frame events
         updated = False
+        target = None
         if 'events' in o:
             if 'create' in o['events']:
                 ts_start_ob = time.utc_from_list_or_scalar(o['events']['create'], default_t=tt)
                 if ts_end.tt <= ts_start_ob.tt:
                     continue
             if 'delete' in o['events']:
                 ts_end_ob = time.utc_from_list_or_scalar(o['events']['delete'], default_t=tt)
                 if ts_end.tt >= ts_end_ob.tt:
                     continue
             if 'update' in o['events']:
                 for eu in o['events']['update']:
                     ts_start_ob = time.utc_from_list_or_scalar(eu['time'], default_t=tt)
                     if ts_end.tt >= ts_start_ob.tt:
-                        o.update(eu['values'])
+                        merge_dicts(o, eu['values'])
                         updated = True
 
         if 'mv' in o:
             ope = mv_to_pe(zeropoint, o['mv']) if not callable(o['mv']) else 0.0
             pe_func = (lambda x, t: x) if not callable(o['mv']) else (lambda x, t: mv_to_pe(zeropoint, o['mv'](x, t)) * _delta_t(t))
         elif 'pe' in o:
             ope = o['pe'] if not callable(o['pe']) else 0.0
             pe_func = (lambda x, t: x) if not callable(o['pe']) else (lambda x, t: o['pe'](x, t) * _delta_t(t))
+        else:
+            ope = 0.0
+            pe_func = (lambda x, t: x)
 
         if o['mode'] == 'line':
             ovrc = [o['velocity'][0] / y_to_pix * s_osf, o['velocity'][1] / x_to_pix * s_osf]
             epoch = o['epoch'] if 'epoch' in o else 0
             (orr, occ, opp, ott) = gen_line(h_fpa_os, w_fpa_os, o['origin'], ovrc, ope, t_start + epoch, t_end + epoch)
         elif o['mode'] == 'line-polar':
             o_vel_angle = o['velocity'][0] * math.pi / 180
@@ -988,19 +993,19 @@
             if ssp['sim']['mode'] == 'none':
                 continue
 
             o_offset = [0.0, 0.0]
             if 'offset' in o:
                 o_offset = [o['offset'][0] * h_fpa_os, o['offset'][1] * w_fpa_os]
 
-            sat = obs_cache[i]
+            target = obs_cache[i][0]
             az, el = _calculate_az_el(tc_start, tc_end, [ts_start, ts_mid, ts_end], track_az, track_el)
 
             try:
-                [rr0, rr1, rr2], [cc0, cc1, cc2], _, _, _ = gen_track(h_fpa_os, w_fpa_os, y_fov, x_fov, observer, track, sat, [ope], tc_start, [ts_start, ts_mid, ts_end], star_rot, 1, track_mode, offset=o_offset, flipud=ssp['fpa']['flip_up_down'], fliplr=ssp['fpa']['flip_left_right'], az=az, el=el)
+                [rr0, rr1, rr2], [cc0, cc1, cc2], _, _, _ = gen_track(h_fpa_os, w_fpa_os, y_fov, x_fov, observer, track, [target], [ope], tc_start, [ts_start, ts_mid, ts_end], star_rot, 1, track_mode, offset=o_offset, flipud=ssp['fpa']['flip_up_down'], fliplr=ssp['fpa']['flip_left_right'], az=az, el=el)
             except Exception:
                 logger.exception("Error propagating target. {}".format(o))
                 continue
 
             if len(rr0) > 0 and not math.isnan(rr0[0]) and not math.isnan(cc0[0]) and not math.isnan(rr2[0]) and not math.isnan(cc2[0]):
 
                 if rr0[0] < -h_pad_os and rr2[0] < -h_pad_os:
@@ -1017,33 +1022,40 @@
                 else:
                     (orr, occ, opp, ott) = gen_curve_from_points(rr0[0], cc0[0], rr1[0], cc1[0], rr2[0], cc2[0], ope, t_start, t_end)
             else:
                 continue
         elif o['mode'] == 'none':
             continue
 
+        # non-sprite based brightness models
+        has_brightness_model = 'model' in o and not callable(o['model']) and 'mode' in o['model'] and o['model']['mode'] != 'sprite'
+        if has_brightness_model:
+            pe_func = (lambda x, t: mv_to_pe(zeropoint, model_to_mv(observer, target, o['model'], time.utc_from_list(tt, _avg_t(t)))) * _delta_t(t))
+
         opp = pe_func(opp, ott)
         avg_pe = np.sum(opp) / (t_end - t_start)
         avg_mv = pe_to_mv(zeropoint, avg_pe)
 
         logger.debug('Average brightness for target: {:.2f} mv, {:.2f} pix.'.format(avg_mv, len(opp) / s_osf))
 
-        if 'model' in o:
+        # TODO generalize `model`
+        # sprint based brightness models
+        if 'model' in o and not has_brightness_model:
             if render_mode != 'piecewise':
-                if not callable(o['model']):
-                    patch = load_sprite_from_file(filename=o['model']['filename']) if 'mode' in o['model'] else o['model']
-                    fpa_os_clear = tf.zeros([h_fpa_pad_os, w_fpa_pad_os], tf.float32)
-                    fpa_os_w_targets = add_patch(fpa_os_clear, orr, occ, opp, patch, h_pad_os_div2, w_pad_os_div2)
-                    obs_model.append(fpa_os_w_targets)
-                else:
+                if callable(o['model']):
                     fpa_os_w_targets = tf.zeros([h_fpa_pad_os, w_fpa_pad_os], tf.float32)
                     patch = o['model'](x=None, t=ott[0])
                     fpa_os_w_targets = add_patch(fpa_os_w_targets, orr, occ, opp, patch, h_pad_os_div2, w_pad_os_div2)
                     obs_model.append(fpa_os_w_targets)
                     # TODO support sub-sample patching
+                elif o['model']['mode'] == 'sprite':
+                    patch = load_sprite_from_file(filename=o['model']['filename']) if 'mode' in o['model'] else o['model']
+                    fpa_os_clear = tf.zeros([h_fpa_pad_os, w_fpa_pad_os], tf.float32)
+                    fpa_os_w_targets = add_patch(fpa_os_clear, orr, occ, opp, patch, h_pad_os_div2, w_pad_os_div2)
+                    obs_model.append(fpa_os_w_targets)
             else:
                 logger.warning('Sprite models not supported for piecewise rendering.')
         else:
             orrr = np.concatenate((orrr, orr))
             occc = np.concatenate((occc, occ))
             oppp = np.concatenate((oppp, opp))
```

### Comparing `satsim-0.18.0/satsim/tfa/image/__init__.py` & `satsim-0.19.0/satsim/tfa/image/__init__.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/tfa/image/transform_ops.py` & `satsim-0.19.0/satsim/tfa/image/transform_ops.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/tfa/image/translate_ops.py` & `satsim-0.19.0/satsim/tfa/image/translate_ops.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/tfa/image/utils.py` & `satsim-0.19.0/satsim/tfa/image/utils.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/tfa/utils/test_utils.py` & `satsim-0.19.0/satsim/tfa/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/tfa/utils/types.py` & `satsim-0.19.0/satsim/tfa/utils/types.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/time/__init__.py` & `satsim-0.19.0/satsim/time/__init__.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/util/system.py` & `satsim-0.19.0/satsim/util/system.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/util/thread.py` & `satsim-0.19.0/satsim/util/thread.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/util/timer.py` & `satsim-0.19.0/satsim/util/timer.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/vecmath/Cartesian2.py` & `satsim-0.19.0/satsim/vecmath/Cartesian2.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/vecmath/Cartesian3.py` & `satsim-0.19.0/satsim/vecmath/Cartesian3.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/vecmath/Cartesian4.py` & `satsim-0.19.0/satsim/vecmath/Cartesian4.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/vecmath/Matrix2.py` & `satsim-0.19.0/satsim/vecmath/Matrix2.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/vecmath/Matrix3.py` & `satsim-0.19.0/satsim/vecmath/Matrix3.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/vecmath/Matrix4.py` & `satsim-0.19.0/satsim/vecmath/Matrix4.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim/vecmath/Quaternion.py` & `satsim-0.19.0/satsim/vecmath/Quaternion.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/satsim.egg-info/PKG-INFO` & `satsim-0.19.0/satsim.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,46 @@
 Metadata-Version: 2.1
 Name: satsim
-Version: 0.18.0
+Version: 0.19.0
 Summary: Satellite observation and scene simulator.
 Home-page: https://github.com/ssc-ai/satsim
 Author: Alex Cabello
 Author-email: alexander.cabello@algoritics.com
-License: UNKNOWN
 Keywords: satsim
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta 
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: AUTHORS.rst
+Requires-Dist: Click>=8.1
+Requires-Dist: Cython>=0.29.0
+Requires-Dist: scikit-image>=0.19.3
+Requires-Dist: Pillow<10.0,>=9.0
+Requires-Dist: numpy>=1.21.0
+Requires-Dist: PyYAML>=6.0
+Requires-Dist: matplotlib>=3.7.0
+Requires-Dist: astropy<6,>=5.2.1
+Requires-Dist: apng>=0.3.4
+Requires-Dist: scipy>=1.10
+Requires-Dist: tensorflow>=2.4
+Requires-Dist: skyfield>=1.45
+Requires-Dist: sgp4>=2.21
+Requires-Dist: poliastro>=0.17.0
+Requires-Dist: poppy>=1.0.3
+Requires-Dist: diskcache>=5.0.3
+Requires-Dist: pydash>=4.9.0
+Requires-Dist: asdf<3,>=2.14.3
+Requires-Dist: pygc>=1.3.0
+Requires-Dist: numba>=0.56.0
+Requires-Dist: pooch>=1.6.0
+Requires-Dist: czmlpy>=0.9.0
+Requires-Dist: tifffile>=2023.4.12
+Requires-Dist: imagecodecs>=2023.3.16
 
 SatSim
 ======
 
 **SatSim source code was developed under contract with ARFL/RDSM, and is approved for public release under Public Affairs release approval
 #AFRL-2022-1116.**
 
@@ -37,14 +59,20 @@
 --------
 
 * [History](HISTORY.md)
 
 History
 =======
 
+0.19.0
+---------------------
+
+* Add lambertian sphere brightness model for objects. Set object key `model` `mode` to `lambertian_sphere` and set `albedo` and `size` (meters) parameters. For 2D simulations, `distance` (km) and `phase_angle` (degrees) parameters must also be specified.
+
+
 0.18.0
 ---------------------
 
 * Add turbulent atmosphere to POPPY PSF generation. Set with psf option `turbulent_atmosphere` and sim option `psf_sample_frequency`.
 * Add star and object segmentation annotation. Set sim option `save_segmentation` to `true` and `star_annotation_threshold` to limit stars annotated.
 
 
@@ -291,9 +319,7 @@
 * Updates to run GitLab CI.
 
 
 0.1.0
 ---------------------
 
 * First release.
-
-
```

### Comparing `satsim-0.18.0/satsim.egg-info/SOURCES.txt` & `satsim-0.19.0/satsim.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,15 @@
 satsim/generator/obs/rpo.py
 satsim/geometry/__init__.py
 satsim/geometry/astrometric.py
 satsim/geometry/csvsc.py
 satsim/geometry/draw.py
 satsim/geometry/ephemeris.py
 satsim/geometry/observation.py
+satsim/geometry/photometric.py
 satsim/geometry/random.py
 satsim/geometry/sgp4.py
 satsim/geometry/sprite.py
 satsim/geometry/sstr7.py
 satsim/geometry/transform.py
 satsim/geometry/twobody.py
 satsim/geometry/wcs.py
@@ -137,14 +138,15 @@
 satsim/tfa/image/translate_ops.py
 satsim/tfa/image/utils.py
 satsim/tfa/utils/__init__.py
 satsim/tfa/utils/test_utils.py
 satsim/tfa/utils/types.py
 satsim/time/__init__.py
 satsim/util/__init__.py
+satsim/util/python.py
 satsim/util/system.py
 satsim/util/thread.py
 satsim/util/timer.py
 satsim/vecmath/Cartesian2.py
 satsim/vecmath/Cartesian3.py
 satsim/vecmath/Cartesian4.py
 satsim/vecmath/Matrix2.py
@@ -186,14 +188,15 @@
 tests/test_generator.py
 tests/test_image.py
 tests/test_io.py
 tests/test_math.py
 tests/test_matrix.py
 tests/test_noise.py
 tests/test_observation.py
+tests/test_photometric.py
 tests/test_pipeline.py
 tests/test_psf.py
 tests/test_random.py
 tests/test_render.py
 tests/test_satnet.py
 tests/test_satsim.py
 tests/test_sgp4.py
```

### Comparing `satsim-0.18.0/setup.cfg` & `satsim-0.19.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.18.0
+current_version = 0.19.0
 commit = True
 tag = True
 
 [bumpversion:file:setup.py]
 search = version='{current_version}'
 replace = version='{new_version}'
```

### Comparing `satsim-0.18.0/setup.py` & `satsim-0.19.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,10 +65,10 @@
     keywords='satsim',
     name='satsim',
     packages=find_packages(include=['satsim', 'satsim.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ssc-ai/satsim',
-    version='0.18.0',
+    version='0.19.0',
     zip_safe=False,
 )
```

### Comparing `satsim-0.18.0/tests/config.yml` & `satsim-0.19.0/tests/config.yml`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/config_dynamic.json` & `satsim-0.19.0/tests/config_dynamic.json`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/config_dynamic_legacy.json` & `satsim-0.19.0/tests/config_dynamic_legacy.json`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/config_dynamic_sstr7.json` & `satsim-0.19.0/tests/config_dynamic_sstr7.json`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/config_function.json` & `satsim-0.19.0/tests/config_function.json`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/config_generator.json` & `satsim-0.19.0/tests/config_generator.json`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/config_generator_legacy.json` & `satsim-0.19.0/tests/config_generator_legacy.json`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/config_import.json` & `satsim-0.19.0/tests/config_import.json`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/config_none.json` & `satsim-0.19.0/tests/config_none.json`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/config_piecewise.json` & `satsim-0.19.0/tests/config_piecewise.json`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/config_pipeline.json` & `satsim-0.19.0/tests/config_pipeline.json`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/config_poppy.json` & `satsim-0.19.0/tests/config_poppy.json`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/config_static.json` & `satsim-0.19.0/tests/config_static.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999375%*

 * *Differences: {"'geometry'": "{'obs': {'list': {insert: [(9, OrderedDict([('mode', 'line'), ('origin', [0.1, "*

 * *               "0.1]), ('velocity', [1.0, 1.0]), ('model', OrderedDict([('mode', "*

 * *               "'lambertian_sphere'), ('diameter', 10.0), ('albedo', 0.2), ('phase_angle', 0.0), "*

 * *               "('distance', 400000)])), ('mv_truth', 14.96310309343897)]))]}}}"}*

```diff
@@ -169,14 +169,33 @@
                     "velocity": [
                         0.0,
                         0.0
                     ]
                 },
                 {
                     "mode": "none"
+                },
+                {
+                    "mode": "line",
+                    "model": {
+                        "albedo": 0.2,
+                        "diameter": 10.0,
+                        "distance": 400000,
+                        "mode": "lambertian_sphere",
+                        "phase_angle": 0.0
+                    },
+                    "mv_truth": 14.96310309343897,
+                    "origin": [
+                        0.1,
+                        0.1
+                    ],
+                    "velocity": [
+                        1.0,
+                        1.0
+                    ]
                 }
             ],
             "mode": "list"
         },
         "stars": {
             "mode": "bins",
             "motion": {
```

### Comparing `satsim-0.18.0/tests/config_static_sttr7_sgp4.json` & `satsim-0.19.0/tests/config_static_sttr7_sgp4.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999375%*

 * *Differences: {"'geometry'": "{'obs': {'list': {insert: [(4, OrderedDict([('mode', 'twobody'), ('position', "*

 * *               "[-35204.34419132078, -23217.077089991137, 92.97508204470279]), ('velocity', "*

 * *               "[1.692918281515607, -2.5661652062418896, 0.0011262853330114807]), ('epoch', 6), "*

 * *               "('model', OrderedDict([('mode', 'lambertian_sphere'), ('diameter', 5.0), "*

 * *               "('albedo', 0.2)])), ('events', OrderedDict([('update', [OrderedDict([('time', 10), "*

 * *               "('values', Order […]*

```diff
@@ -112,14 +112,45 @@
                         92.97508204470279
                     ],
                     "velocity": [
                         1.692918281515607,
                         -2.5661652062418896,
                         0.0011262853330114807
                     ]
+                },
+                {
+                    "epoch": 6,
+                    "events": {
+                        "update": [
+                            {
+                                "time": 10,
+                                "values": {
+                                    "model": {
+                                        "albedo": 0.3
+                                    }
+                                }
+                            }
+                        ]
+                    },
+                    "mode": "twobody",
+                    "model": {
+                        "albedo": 0.2,
+                        "diameter": 5.0,
+                        "mode": "lambertian_sphere"
+                    },
+                    "position": [
+                        -35204.34419132078,
+                        -23217.077089991137,
+                        92.97508204470279
+                    ],
+                    "velocity": [
+                        1.692918281515607,
+                        -2.5661652062418896,
+                        0.0011262853330114807
+                    ]
                 }
             ],
             "mode": "list"
         },
         "site": {
             "alt": 0.3,
             "gimbal": {
```

### Comparing `satsim-0.18.0/tests/geo.txt` & `satsim-0.19.0/tests/geo.txt`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/sprite.fits` & `satsim-0.19.0/tests/sprite.fits`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/stray_light.asdf` & `satsim-0.19.0/tests/stray_light.asdf`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_astrometric.py` & `satsim-0.19.0/tests/test_astrometric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Tests for `satsim.geometry.transform` package."""
 from dateutil import parser
 
 import numpy as np
 
 from satsim.geometry.sgp4 import create_sgp4
-from satsim.geometry.astrometric import apparent, load_earth, load_sun, load_moon, create_topocentric, get_los, gen_track, query_by_los, GreatCircle, get_los_azel, angle_between, lambertian_sphere_to_mv, angle_from_los, eci_to_radec, radec_to_eci
+from satsim.geometry.astrometric import apparent, load_earth, load_sun, load_moon, create_topocentric, get_los, gen_track, query_by_los, GreatCircle, get_los_azel, angle_between, angle_from_los, eci_to_radec, radec_to_eci
+from satsim.geometry.photometric import lambertian_sphere_to_mv
 from satsim import time
 
 
 def test_load_earth():
 
     earth = load_earth()
```

### Comparing `satsim-0.18.0/tests/test_cartesian.py` & `satsim-0.19.0/tests/test_cartesian.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_cli.py` & `satsim-0.19.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_config.py` & `satsim-0.19.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_csvsc.py` & `satsim-0.19.0/tests/test_csvsc.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_czml.py` & `satsim-0.19.0/tests/test_czml.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_dataset.py` & `satsim-0.19.0/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_draw.py` & `satsim-0.19.0/tests/test_draw.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_ephemeris.py` & `satsim-0.19.0/tests/test_ephemeris.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_fpa.py` & `satsim-0.19.0/tests/test_fpa.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_generator.py` & `satsim-0.19.0/tests/test_generator.py`

 * *Files 19% similar despite different names*

```diff
@@ -94,14 +94,30 @@
     breakup_velocity = 0.05
     radius = 45.0
 
     output = breakup.breakup_from_tle(tle, collision_time, breakup_velocity, radius, n)
 
     assert(len(output['list']) == n + 1)
 
+    target_size = 12.0
+    target_scale = [0.5, 2.0]
+    output = breakup.breakup_from_tle(tle, collision_time, breakup_velocity, radius, n, target_scale, target_size, brightness_model='lambertian_sphere')
+    assert(len(output['list']) == n + 1)
+
+    total_size = 0.0
+    for item in output['list']:
+        model = item.get('model')
+        size = model.get('size')
+        total_size += size
+
+    expected_size = target_size + target_size * target_scale[1]
+
+    np.testing.assert_almost_equal(total_size, expected_size)
+    np.testing.assert_almost_equal(output['list'][-1]['events']['update'][0]['values']['model']['size'], target_size * target_scale[0])
+
 
 def test_collision():
 
     n = 50
     tle = [
         "1 36411U 10008A   15115.45079343  .00000069  00000-0  00000+0 0  9992",
         "2 36411 000.0719 125.6855 0001927 217.7585 256.6121 01.00266852 18866"
@@ -121,14 +137,35 @@
     output = breakup.collision_from_tle(tle, collision_time, radius, K, attach_angle, attack_velocity, attack_velocity_scale, n)
     assert(len(output['list']) == n * 2 + 2)
 
     output = breakup.collision_from_tle(tle, collision_time, radius, K, attach_angle, attack_velocity, attack_velocity_scale,
                                         [10, 20], fragment_angle='linspace', scale_fragment_velocity=True, variable_brightness=False)
     assert(len(output['list']) == 10 + 20 + 2)
 
+    target_size = 12.0
+    target_scale = [0.5, 2.0]
+    rpo_size = 6.0
+    rpo_scale = [0.5, 2.0]
+    output = breakup.collision_from_tle(tle, collision_time, radius, K, attach_angle, attack_velocity, attack_velocity_scale,
+                                        [10, 20], target_scale, rpo_scale, target_size, rpo_size,
+                                        fragment_angle='linspace', scale_fragment_velocity=True, variable_brightness=False, brightness_model='lambertian_sphere')
+    assert(len(output['list']) == 10 + 20 + 2)
+
+    total_size = 0.0
+    for item in output['list']:
+        model = item.get('model')
+        size = model.get('size')
+        total_size += size
+
+    expected_size = target_size + target_size * target_scale[1] + rpo_size + rpo_size * rpo_scale[1]
+
+    np.testing.assert_almost_equal(total_size, expected_size)
+    np.testing.assert_almost_equal(output['list'][-2]['events']['update'][0]['values']['model']['size'], target_size * target_scale[0])
+    np.testing.assert_almost_equal(output['list'][-1]['events']['update'][0]['values']['model']['size'], rpo_size * rpo_scale[0])
+
 
 def test_rpo():
 
     tle = [
         "1 36411U 10008A   15115.45079343  .00000069  00000-0  00000+0 0  9992",
         "2 36411 000.0719 125.6855 0001927 217.7585 256.6121 01.00266852 18866"
     ]
```

### Comparing `satsim-0.18.0/tests/test_image.py` & `satsim-0.19.0/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_io.py` & `satsim-0.19.0/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_math.py` & `satsim-0.19.0/tests/test_math.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_matrix.py` & `satsim-0.19.0/tests/test_matrix.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_noise.py` & `satsim-0.19.0/tests/test_noise.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_observation.py` & `satsim-0.19.0/tests/test_observation.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_pipeline.py` & `satsim-0.19.0/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_psf.py` & `satsim-0.19.0/tests/test_psf.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_random.py` & `satsim-0.19.0/tests/test_random.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_render.py` & `satsim-0.19.0/tests/test_render.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_satnet.py` & `satsim-0.19.0/tests/test_satnet.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_satsim.py` & `satsim-0.19.0/tests/test_satsim.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,20 +124,21 @@
 
     dirname = gen_images(ssp, eager=True, output_dir='./.images', output_debug=True)
 
     if render_size is None:
         with open(os.path.join(dirname, 'Debug', 'fpa_os_0.pickle'), 'rb') as f:
             fpa_os_1 = pickle.load(f)
 
-        np.testing.assert_approx_equal(np.sum(fpa_os_0.flatten()) * 2, np.sum(fpa_os_1.flatten()), significant=7)
+        np.testing.assert_approx_equal(np.sum(fpa_os_0.flatten()) * 2, np.sum(fpa_os_1.flatten()), significant=6)
 
     with open(os.path.join(dirname, 'Debug', 'metadata_0.json'), 'r') as f:
         metadata_1 = json.load(f)
 
-    for a, b in zip(ssp['geometry']['obs']['list'], metadata_1['data']['objects']):
+    filtered_obs = [item for item in ssp['geometry']['obs']['list'] if item.get('mode') != 'none']
+    for a, b in zip(filtered_obs, metadata_1['data']['objects']):
         if 'mv_truth' in a:
             assert(a['mv_truth'] == b['magnitude'])
         if 'pe_truth' in a:
             assert(a['pe_truth'] == b['pe_per_sec'])
 
 
 def _test_target_centroid(render_size=None):
```

### Comparing `satsim-0.18.0/tests/test_sgp4.py` & `satsim-0.19.0/tests/test_sgp4.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_sprite.py` & `satsim-0.19.0/tests/test_sprite.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_sstr7.py` & `satsim-0.19.0/tests/test_sstr7.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_tfa_transform_ops.py` & `satsim-0.19.0/tests/test_tfa_transform_ops.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_tfa_translate_ops.py` & `satsim-0.19.0/tests/test_tfa_translate_ops.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_tfa_utils_test.py` & `satsim-0.19.0/tests/test_tfa_utils_test.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_time.py` & `satsim-0.19.0/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_transform.py` & `satsim-0.19.0/tests/test_transform.py`

 * *Files identical despite different names*

### Comparing `satsim-0.18.0/tests/test_twobody.py` & `satsim-0.19.0/tests/test_twobody.py`

 * *Files identical despite different names*

