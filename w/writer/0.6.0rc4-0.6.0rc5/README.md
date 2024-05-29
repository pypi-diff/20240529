# Comparing `tmp/writer-0.6.0rc4.tar.gz` & `tmp/writer-0.6.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "writer-0.6.0rc4.tar", max compression
+gzip compressed data, was "writer-0.6.0rc5.tar", max compression
```

## Comparing `writer-0.6.0rc4.tar` & `writer-0.6.0rc5.tar`

### file list

```diff
@@ -1,173 +1,173 @@
--rw-r--r--   0        0        0    11323 2024-05-24 15:58:15.731534 writer-0.6.0rc4/LICENSE.txt
--rw-r--r--   0        0        0     4027 2024-05-24 15:58:15.731534 writer-0.6.0rc4/README.md
--rw-r--r--   0        0        0     2293 2024-05-24 15:58:15.843535 writer-0.6.0rc4/pyproject.toml
--rw-r--r--   0        0        0     3712 2024-05-24 15:58:15.851535 writer-0.6.0rc4/src/writer/__init__.py
--rw-r--r--   0        0        0    20078 2024-05-24 15:58:15.851535 writer-0.6.0rc4/src/writer/ai.py
--rw-r--r--   0        0        0    30304 2024-05-24 15:58:15.851535 writer-0.6.0rc4/src/writer/app_runner.py
--rw-r--r--   0        0        0      115 2024-05-24 15:58:15.731534 writer-0.6.0rc4/src/writer/app_templates/ai-starter/README.md
--rw-r--r--   0        0        0      296 2024-05-24 15:58:15.731534 writer-0.6.0rc4/src/writer/app_templates/ai-starter/main.py
--rw-r--r--   0        0        0      309 2024-05-24 15:58:15.731534 writer-0.6.0rc4/src/writer/app_templates/ai-starter/pyproject.toml
--rw-r--r--   0        0        0      416 2024-05-24 15:58:15.731534 writer-0.6.0rc4/src/writer/app_templates/ai-starter/static/README.md
--rw-r--r--   0        0        0      889 2024-05-24 15:58:15.731534 writer-0.6.0rc4/src/writer/app_templates/ai-starter/static/favicon.png
--rw-r--r--   0        0        0     1536 2024-05-24 15:58:15.731534 writer-0.6.0rc4/src/writer/app_templates/ai-starter/ui.json
--rw-r--r--   0        0        0      115 2024-05-24 15:58:15.731534 writer-0.6.0rc4/src/writer/app_templates/default/README.md
--rw-r--r--   0        0        0     1044 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/default/main.py
--rw-r--r--   0        0        0      309 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/default/pyproject.toml
--rw-r--r--   0        0        0      416 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/default/static/README.md
--rw-r--r--   0        0        0      889 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/default/static/favicon.png
--rw-r--r--   0        0        0     5171 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/default/ui.json
--rw-r--r--   0        0        0      115 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/hello/README.md
--rw-r--r--   0        0        0     1250 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/hello/assets/main_df.csv
--rw-r--r--   0        0        0     2666 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/hello/assets/story.txt
--rw-r--r--   0        0        0     4564 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/hello/main.py
--rw-r--r--   0        0        0      307 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/hello/pyproject.toml
--rw-r--r--   0        0        0      628 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/hello/static/README.md
--rw-r--r--   0        0        0      889 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/hello/static/favicon.png
--rw-r--r--   0        0        0   152314 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/hello/static/pigeon1.jpg
--rw-r--r--   0        0        0     1494 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/hello/test_app.py
--rw-r--r--   0        0        0    39757 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/hello/ui.json
--rw-r--r--   0        0        0      115 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/product-description-generator/README.md
--rw-r--r--   0        0        0      463 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/product-description-generator/main.py
--rw-r--r--   0        0        0     3351 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/product-description-generator/prompts.py
--rw-r--r--   0        0        0      309 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/product-description-generator/pyproject.toml
--rw-r--r--   0        0        0      416 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/product-description-generator/static/README.md
--rw-r--r--   0        0        0      889 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/product-description-generator/static/favicon.png
--rw-r--r--   0        0        0     4940 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/product-description-generator/ui.json
--rw-r--r--   0        0        0      115 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/quickstart/README.md
--rw-r--r--   0        0        0     2849 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/quickstart/main.py
--rw-r--r--   0        0        0      309 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/quickstart/pyproject.toml
--rw-r--r--   0        0        0       20 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/quickstart/requirements.txt
--rw-r--r--   0        0        0      628 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/quickstart/static/README.md
--rw-r--r--   0        0        0      889 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/quickstart/static/favicon.png
--rw-r--r--   0        0        0     5538 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/quickstart/ui.json
--rw-r--r--   0        0        0      115 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/text-demo/README.md
--rw-r--r--   0        0        0      928 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/text-demo/main.py
--rw-r--r--   0        0        0      309 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/text-demo/pyproject.toml
--rw-r--r--   0        0        0      416 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/text-demo/static/README.md
--rw-r--r--   0        0        0      889 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/text-demo/static/favicon.png
--rw-r--r--   0        0        0     4466 2024-05-24 15:58:15.735534 writer-0.6.0rc4/src/writer/app_templates/text-demo/ui.json
--rw-r--r--   0        0        0     9183 2024-05-24 15:58:15.851535 writer-0.6.0rc4/src/writer/auth.py
--rw-r--r--   0        0        0     5979 2024-05-24 15:58:15.851535 writer-0.6.0rc4/src/writer/command_line.py
--rw-r--r--   0        0        0    52678 2024-05-24 15:58:15.851535 writer-0.6.0rc4/src/writer/core.py
--rw-r--r--   0        0        0    14612 2024-05-24 15:58:15.851535 writer-0.6.0rc4/src/writer/core_ui.py
--rw-r--r--   0        0        0     3757 2024-05-24 15:58:15.851535 writer-0.6.0rc4/src/writer/deploy.py
--rw-r--r--   0        0        0       30 2024-05-24 15:58:15.851535 writer-0.6.0rc4/src/writer/mypy.ini
--rw-r--r--   0        0        0        0 2024-05-24 15:58:15.851535 writer-0.6.0rc4/src/writer/py.typed
--rw-r--r--   0        0        0    21550 2024-05-24 15:58:15.851535 writer-0.6.0rc4/src/writer/serve.py
--rw-r--r--   0        0        0     3599 2024-05-24 15:58:15.851535 writer-0.6.0rc4/src/writer/ss_types.py
--rw-r--r--   0        0        0     8966 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/Arrow.dom-C52_vrWm.js
--rw-r--r--   0        0        0  3288135 2024-05-24 16:00:26.701193 writer-0.6.0rc4/src/writer/static/assets/BuilderApp-DakBH-QB.js
--rw-r--r--   0        0        0   280997 2024-05-24 16:00:26.489190 writer-0.6.0rc4/src/writer/static/assets/BuilderApp-DjkgRMd3.css
--rw-r--r--   0        0        0    13237 2024-05-24 16:00:26.489190 writer-0.6.0rc4/src/writer/static/assets/ComponentRenderer-BnXm57ig.css
--rw-r--r--   0        0        0     7856 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/ComponentRenderer-PYR7CN9R.js
--rw-r--r--   0        0        0    14409 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/abap-D8nrxEjS.js
--rw-r--r--   0        0        0     4198 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/apex-BrXDlLUW.js
--rw-r--r--   0        0        0     1094 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/azcli-CElzELwZ.js
--rw-r--r--   0        0        0     2091 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/bat-CUsyEhik.js
--rw-r--r--   0        0        0     2782 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/bicep-BtxyJn6H.js
--rw-r--r--   0        0        0     2431 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/cameligo-ClBCoF8h.js
--rw-r--r--   0        0        0     9889 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/clojure-B9TqLHAk.js
--rw-r--r--   0        0        0    79568 2024-05-24 16:00:26.489190 writer-0.6.0rc4/src/writer/static/assets/codicon-BA2IlpFX.ttf
--rw-r--r--   0        0        0     3836 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/coffee-DYsfeylR.js
--rw-r--r--   0        0        0     5680 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/cpp-VVGvvgir.js
--rw-r--r--   0        0        0     4770 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/csharp-Z6z2stHy.js
--rw-r--r--   0        0        0     1665 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/csp-DgZoLDI1.js
--rw-r--r--   0        0        0     4756 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/css-KqQ96-gC.js
--rw-r--r--   0        0        0   984347 2024-05-24 16:00:26.657193 writer-0.6.0rc4/src/writer/static/assets/css.worker-DvNUQFd1.js
--rw-r--r--   0        0        0    33713 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/cssMode-BjK5GHby.js
--rw-r--r--   0        0        0     3631 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/cypher-CYoSlgTu.js
--rw-r--r--   0        0        0     4496 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/dart-BGDl7St1.js
--rw-r--r--   0        0        0     2115 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/dockerfile-CuCtxA7T.js
--rw-r--r--   0        0        0     5588 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/ecl-BCTFAUpS.js
--rw-r--r--   0        0        0   210242 2024-05-24 16:00:26.629192 writer-0.6.0rc4/src/writer/static/assets/editor.worker-BVwmgLrR.js
--rw-r--r--   0        0        0    10503 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/elixir-C7hRTYZ9.js
--rw-r--r--   0        0        0     2056 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/flow9-Bi_qi707.js
--rw-r--r--   0        0        0    16478 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/freemarker2-i8lRH5rw.js
--rw-r--r--   0        0        0     3229 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/fsharp-CxaaEKKi.js
--rw-r--r--   0        0        0     2903 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/go-DUImKuGY.js
--rw-r--r--   0        0        0     2506 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/graphql-D5sGVkLV.js
--rw-r--r--   0        0        0     7156 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/handlebars-C-M0xH-3.js
--rw-r--r--   0        0        0     3836 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/hcl-zD_CCkZ1.js
--rw-r--r--   0        0        0     5396 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/html-D4h1E1bc.js
--rw-r--r--   0        0        0   648041 2024-05-24 16:00:26.657193 writer-0.6.0rc4/src/writer/static/assets/html.worker-BJMlcbMU.js
--rw-r--r--   0        0        0    34264 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/htmlMode-B2YRTiG6.js
--rw-r--r--   0        0        0  1798722 2024-05-24 16:00:26.677193 writer-0.6.0rc4/src/writer/static/assets/index-BaC5au8C.js
--rw-r--r--   0        0        0     5725 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/index-DMFOqlrb.js
--rw-r--r--   0        0        0   201777 2024-05-24 16:00:26.593192 writer-0.6.0rc4/src/writer/static/assets/index-DaNZqg5r.js
--rw-r--r--   0        0        0   345034 2024-05-24 16:00:26.489190 writer-0.6.0rc4/src/writer/static/assets/index-XEiBUN1q.css
--rw-r--r--   0        0        0   314372 2024-05-24 16:00:26.609192 writer-0.6.0rc4/src/writer/static/assets/index-cJO61pFl.js
--rw-r--r--   0        0        0     1347 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/ini-8kKHd4ZL.js
--rw-r--r--   0        0        0     3467 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/java-De1axCfe.js
--rw-r--r--   0        0        0     1292 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/javascript-BYM0Yx4u.js
--rw-r--r--   0        0        0   339023 2024-05-24 16:00:26.633192 writer-0.6.0rc4/src/writer/static/assets/json.worker-BwvX8PuZ.js
--rw-r--r--   0        0        0    39790 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/jsonMode-B8RZLFyl.js
--rw-r--r--   0        0        0     7395 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/julia-D3ApGBxz.js
--rw-r--r--   0        0        0     3685 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/kotlin-GbSrCElU.js
--rw-r--r--   0        0        0     4144 2024-05-24 16:00:26.489190 writer-0.6.0rc4/src/writer/static/assets/less-DNUaDNdz.js
--rw-r--r--   0        0        0     2683 2024-05-24 16:00:26.489190 writer-0.6.0rc4/src/writer/static/assets/lexon-Bg9QKxBu.js
--rw-r--r--   0        0        0     4342 2024-05-24 16:00:26.489190 writer-0.6.0rc4/src/writer/static/assets/liquid-ktIne1h-.js
--rw-r--r--   0        0        0     2369 2024-05-24 16:00:26.489190 writer-0.6.0rc4/src/writer/static/assets/lua-Crkvc3mc.js
--rw-r--r--   0        0        0     3063 2024-05-24 16:00:26.489190 writer-0.6.0rc4/src/writer/static/assets/m3-DsrzVyM1.js
--rw-r--r--   0        0        0  1289773 2024-05-24 16:00:26.665192 writer-0.6.0rc4/src/writer/static/assets/mapbox-gl-FST67qaq.js
--rw-r--r--   0        0        0     4034 2024-05-24 16:00:26.489190 writer-0.6.0rc4/src/writer/static/assets/markdown-CY5IOZuu.js
--rw-r--r--   0        0        0    35703 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/marked.esm-273vDTCT.js
--rw-r--r--   0        0        0     5247 2024-05-24 16:00:26.489190 writer-0.6.0rc4/src/writer/static/assets/mdx-Bi1uxJs7.js
--rw-r--r--   0        0        0     2825 2024-05-24 16:00:26.489190 writer-0.6.0rc4/src/writer/static/assets/mips-BE8RsGBA.js
--rw-r--r--   0        0        0     5158 2024-05-24 16:00:26.489190 writer-0.6.0rc4/src/writer/static/assets/msdax-N5ajIiFQ.js
--rw-r--r--   0        0        0    11520 2024-05-24 16:00:26.489190 writer-0.6.0rc4/src/writer/static/assets/mysql-DRxbB97D.js
--rw-r--r--   0        0        0     2648 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/objective-c-BHUZy23s.js
--rw-r--r--   0        0        0     3241 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/pascal-BemVzBTY.js
--rw-r--r--   0        0        0     2246 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/pascaligo-BACCcnx_.js
--rw-r--r--   0        0        0     8501 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/perl-CuU66Ptk.js
--rw-r--r--   0        0        0    13710 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/pgsql-CQ6TMH2r.js
--rw-r--r--   0        0        0     8273 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/php-BvyzZa65.js
--rw-r--r--   0        0        0     1929 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/pla-DrIuu9u1.js
--rw-r--r--   0        0        0  3704067 2024-05-24 16:00:26.709193 writer-0.6.0rc4/src/writer/static/assets/plotly.min-Bn62pPWj.js
--rw-r--r--   0        0        0     8102 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/postiats-BR_hrfni.js
--rw-r--r--   0        0        0    17185 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/powerquery-CKDUeRmd.js
--rw-r--r--   0        0        0     3515 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/powershell-Dsa4rhA_.js
--rw-r--r--   0        0        0     9292 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/protobuf-CGsvhooB.js
--rw-r--r--   0        0        0     5074 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/pug-D2p3uOX2.js
--rw-r--r--   0        0        0     4006 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/python-DGmW9UMq.js
--rw-r--r--   0        0        0     3181 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/qsharp-B7F3HtPF.js
--rw-r--r--   0        0        0     3377 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/r-3aLoi2fs.js
--rw-r--r--   0        0        0     9160 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/razor-NRqESbyQ.js
--rw-r--r--   0        0        0     3802 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/redis-jqFeRM5s.js
--rw-r--r--   0        0        0    12046 2024-05-24 16:00:26.489190 writer-0.6.0rc4/src/writer/static/assets/redshift-BriwQgXR.js
--rw-r--r--   0        0        0   163200 2024-05-24 16:00:26.489190 writer-0.6.0rc4/src/writer/static/assets/remixicon-BVOYbT3K.woff2
--rw-r--r--   0        0        0   525572 2024-05-24 16:00:26.489190 writer-0.6.0rc4/src/writer/static/assets/remixicon-D9ZyeRwQ.ttf
--rw-r--r--   0        0        0   525744 2024-05-24 16:00:26.489190 writer-0.6.0rc4/src/writer/static/assets/remixicon-DUK49BtM.eot
--rw-r--r--   0        0        0   224116 2024-05-24 16:00:26.489190 writer-0.6.0rc4/src/writer/static/assets/remixicon-DfzPQSMi.woff
--rw-r--r--   0        0        0  2460531 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/remixicon-ncU_JTfY.svg
--rw-r--r--   0        0        0     4139 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/restructuredtext-hbBFZ0w9.js
--rw-r--r--   0        0        0     8750 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/ruby-ByThyB2Q.js
--rw-r--r--   0        0        0     4406 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/rust-DIEZMp5R.js
--rw-r--r--   0        0        0     2075 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/sb-C6Gjjw_x.js
--rw-r--r--   0        0        0     7564 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/scala-DZNw3jJB.js
--rw-r--r--   0        0        0     2013 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/scheme-55eqh71t.js
--rw-r--r--   0        0        0     6655 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/scss-D-OVkc4F.js
--rw-r--r--   0        0        0   202255 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/serialization-DDqLB4lR.js
--rw-r--r--   0        0        0     3319 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/shell-DSpi8_qN.js
--rw-r--r--   0        0        0    18843 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/solidity-BHddiNFS.js
--rw-r--r--   0        0        0     3010 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/sophia-D6taVZFb.js
--rw-r--r--   0        0        0     2798 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/sparql-LA0C7mUc.js
--rw-r--r--   0        0        0    10543 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/sql-C3-3IcFM.js
--rw-r--r--   0        0        0     7645 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/st-C4g7059C.js
--rw-r--r--   0        0        0     5417 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/swift-DNI1vH3h.js
--rw-r--r--   0        0        0     7849 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/systemverilog-DL_FVbcQ.js
--rw-r--r--   0        0        0     3817 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/tcl-DVJXmIwd.js
--rw-r--r--   0        0        0  4847810 2024-05-24 16:00:26.717193 writer-0.6.0rc4/src/writer/static/assets/ts.worker-CwG1rUES.js
--rw-r--r--   0        0        0    22645 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/tsMode-CjGd3dCD.js
--rw-r--r--   0        0        0     6219 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/twig-BVWDLtw5.js
--rw-r--r--   0        0        0     5789 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/typescript-8g2Igz_p.js
--rw-r--r--   0        0        0     6037 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/vb-Btz91-7U.js
--rw-r--r--   0        0        0   839306 2024-05-24 16:00:26.649192 writer-0.6.0rc4/src/writer/static/assets/vega-embed.module-CxKUxoHf.js
--rw-r--r--   0        0        0     7592 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/wgsl-D8V_buCG.js
--rw-r--r--   0        0        0     2790 2024-05-24 16:00:26.493190 writer-0.6.0rc4/src/writer/static/assets/xml-Cey2x9G0.js
--rw-r--r--   0        0        0     4397 2024-05-24 16:00:26.497191 writer-0.6.0rc4/src/writer/static/assets/yaml-DiYkW6--.js
--rw-r--r--   0        0        0      889 2024-05-24 16:00:23.561154 writer-0.6.0rc4/src/writer/static/favicon.png
--rw-r--r--   0        0        0     2787 2024-05-24 16:00:26.637192 writer-0.6.0rc4/src/writer/static/index.html
--rw-r--r--   0        0        0      432 2024-05-24 15:58:15.851535 writer-0.6.0rc4/src/writer/templates/auth_unauthorized.html
--rw-r--r--   0        0        0    59105 2024-05-24 15:59:12.252257 writer-0.6.0rc4/src/writer/ui.py
--rw-r--r--   0        0        0     7896 2024-05-24 15:58:15.851535 writer-0.6.0rc4/src/writer/ui_manager.py
--rw-r--r--   0        0        0     5436 1970-01-01 00:00:00.000000 writer-0.6.0rc4/PKG-INFO
+-rw-r--r--   0        0        0    10752 2024-05-29 09:08:49.039499 writer-0.6.0rc5/LICENSE.txt
+-rw-r--r--   0        0        0     4027 2024-05-29 09:08:49.039499 writer-0.6.0rc5/README.md
+-rw-r--r--   0        0        0     2298 2024-05-29 09:08:49.151501 writer-0.6.0rc5/pyproject.toml
+-rw-r--r--   0        0        0     3712 2024-05-29 09:08:49.159501 writer-0.6.0rc5/src/writer/__init__.py
+-rw-r--r--   0        0        0    20151 2024-05-29 09:08:49.159501 writer-0.6.0rc5/src/writer/ai.py
+-rw-r--r--   0        0        0    30304 2024-05-29 09:08:49.159501 writer-0.6.0rc5/src/writer/app_runner.py
+-rw-r--r--   0        0        0      115 2024-05-29 09:08:49.039499 writer-0.6.0rc5/src/writer/app_templates/ai-starter/README.md
+-rw-r--r--   0        0        0      296 2024-05-29 09:08:49.039499 writer-0.6.0rc5/src/writer/app_templates/ai-starter/main.py
+-rw-r--r--   0        0        0      309 2024-05-29 09:08:49.039499 writer-0.6.0rc5/src/writer/app_templates/ai-starter/pyproject.toml
+-rw-r--r--   0        0        0      416 2024-05-29 09:08:49.039499 writer-0.6.0rc5/src/writer/app_templates/ai-starter/static/README.md
+-rw-r--r--   0        0        0      889 2024-05-29 09:08:49.039499 writer-0.6.0rc5/src/writer/app_templates/ai-starter/static/favicon.png
+-rw-r--r--   0        0        0     1536 2024-05-29 09:08:49.039499 writer-0.6.0rc5/src/writer/app_templates/ai-starter/ui.json
+-rw-r--r--   0        0        0      115 2024-05-29 09:08:49.039499 writer-0.6.0rc5/src/writer/app_templates/default/README.md
+-rw-r--r--   0        0        0     1044 2024-05-29 09:08:49.039499 writer-0.6.0rc5/src/writer/app_templates/default/main.py
+-rw-r--r--   0        0        0      309 2024-05-29 09:08:49.039499 writer-0.6.0rc5/src/writer/app_templates/default/pyproject.toml
+-rw-r--r--   0        0        0      416 2024-05-29 09:08:49.039499 writer-0.6.0rc5/src/writer/app_templates/default/static/README.md
+-rw-r--r--   0        0        0      889 2024-05-29 09:08:49.039499 writer-0.6.0rc5/src/writer/app_templates/default/static/favicon.png
+-rw-r--r--   0        0        0     5171 2024-05-29 09:08:49.039499 writer-0.6.0rc5/src/writer/app_templates/default/ui.json
+-rw-r--r--   0        0        0      115 2024-05-29 09:08:49.039499 writer-0.6.0rc5/src/writer/app_templates/hello/README.md
+-rw-r--r--   0        0        0     1250 2024-05-29 09:08:49.039499 writer-0.6.0rc5/src/writer/app_templates/hello/assets/main_df.csv
+-rw-r--r--   0        0        0     2666 2024-05-29 09:08:49.039499 writer-0.6.0rc5/src/writer/app_templates/hello/assets/story.txt
+-rw-r--r--   0        0        0     4564 2024-05-29 09:08:49.039499 writer-0.6.0rc5/src/writer/app_templates/hello/main.py
+-rw-r--r--   0        0        0      307 2024-05-29 09:08:49.039499 writer-0.6.0rc5/src/writer/app_templates/hello/pyproject.toml
+-rw-r--r--   0        0        0      628 2024-05-29 09:08:49.039499 writer-0.6.0rc5/src/writer/app_templates/hello/static/README.md
+-rw-r--r--   0        0        0      889 2024-05-29 09:08:49.039499 writer-0.6.0rc5/src/writer/app_templates/hello/static/favicon.png
+-rw-r--r--   0        0        0   152314 2024-05-29 09:08:49.039499 writer-0.6.0rc5/src/writer/app_templates/hello/static/pigeon1.jpg
+-rw-r--r--   0        0        0     1494 2024-05-29 09:08:49.039499 writer-0.6.0rc5/src/writer/app_templates/hello/test_app.py
+-rw-r--r--   0        0        0    39757 2024-05-29 09:08:49.043500 writer-0.6.0rc5/src/writer/app_templates/hello/ui.json
+-rw-r--r--   0        0        0      115 2024-05-29 09:08:49.043500 writer-0.6.0rc5/src/writer/app_templates/pdg-tutorial/README.md
+-rw-r--r--   0        0        0      463 2024-05-29 09:08:49.043500 writer-0.6.0rc5/src/writer/app_templates/pdg-tutorial/main.py
+-rw-r--r--   0        0        0     3351 2024-05-29 09:08:49.043500 writer-0.6.0rc5/src/writer/app_templates/pdg-tutorial/prompts.py
+-rw-r--r--   0        0        0      309 2024-05-29 09:08:49.043500 writer-0.6.0rc5/src/writer/app_templates/pdg-tutorial/pyproject.toml
+-rw-r--r--   0        0        0      416 2024-05-29 09:08:49.043500 writer-0.6.0rc5/src/writer/app_templates/pdg-tutorial/static/README.md
+-rw-r--r--   0        0        0      889 2024-05-29 09:08:49.043500 writer-0.6.0rc5/src/writer/app_templates/pdg-tutorial/static/favicon.png
+-rw-r--r--   0        0        0     4940 2024-05-29 09:08:49.043500 writer-0.6.0rc5/src/writer/app_templates/pdg-tutorial/ui.json
+-rw-r--r--   0        0        0      115 2024-05-29 09:08:49.043500 writer-0.6.0rc5/src/writer/app_templates/quickstart/README.md
+-rw-r--r--   0        0        0     2849 2024-05-29 09:08:49.043500 writer-0.6.0rc5/src/writer/app_templates/quickstart/main.py
+-rw-r--r--   0        0        0      309 2024-05-29 09:08:49.043500 writer-0.6.0rc5/src/writer/app_templates/quickstart/pyproject.toml
+-rw-r--r--   0        0        0       20 2024-05-29 09:08:49.043500 writer-0.6.0rc5/src/writer/app_templates/quickstart/requirements.txt
+-rw-r--r--   0        0        0      628 2024-05-29 09:08:49.043500 writer-0.6.0rc5/src/writer/app_templates/quickstart/static/README.md
+-rw-r--r--   0        0        0      889 2024-05-29 09:08:49.043500 writer-0.6.0rc5/src/writer/app_templates/quickstart/static/favicon.png
+-rw-r--r--   0        0        0     5538 2024-05-29 09:08:49.043500 writer-0.6.0rc5/src/writer/app_templates/quickstart/ui.json
+-rw-r--r--   0        0        0      115 2024-05-29 09:08:49.043500 writer-0.6.0rc5/src/writer/app_templates/text-demo/README.md
+-rw-r--r--   0        0        0      928 2024-05-29 09:08:49.043500 writer-0.6.0rc5/src/writer/app_templates/text-demo/main.py
+-rw-r--r--   0        0        0      309 2024-05-29 09:08:49.043500 writer-0.6.0rc5/src/writer/app_templates/text-demo/pyproject.toml
+-rw-r--r--   0        0        0      416 2024-05-29 09:08:49.043500 writer-0.6.0rc5/src/writer/app_templates/text-demo/static/README.md
+-rw-r--r--   0        0        0      889 2024-05-29 09:08:49.043500 writer-0.6.0rc5/src/writer/app_templates/text-demo/static/favicon.png
+-rw-r--r--   0        0        0     4466 2024-05-29 09:08:49.043500 writer-0.6.0rc5/src/writer/app_templates/text-demo/ui.json
+-rw-r--r--   0        0        0     9183 2024-05-29 09:08:49.159501 writer-0.6.0rc5/src/writer/auth.py
+-rw-r--r--   0        0        0     5979 2024-05-29 09:08:49.159501 writer-0.6.0rc5/src/writer/command_line.py
+-rw-r--r--   0        0        0    52678 2024-05-29 09:08:49.159501 writer-0.6.0rc5/src/writer/core.py
+-rw-r--r--   0        0        0    14612 2024-05-29 09:08:49.159501 writer-0.6.0rc5/src/writer/core_ui.py
+-rw-r--r--   0        0        0     3757 2024-05-29 09:08:49.159501 writer-0.6.0rc5/src/writer/deploy.py
+-rw-r--r--   0        0        0       30 2024-05-29 09:08:49.159501 writer-0.6.0rc5/src/writer/mypy.ini
+-rw-r--r--   0        0        0        0 2024-05-29 09:08:49.159501 writer-0.6.0rc5/src/writer/py.typed
+-rw-r--r--   0        0        0    21550 2024-05-29 09:08:49.159501 writer-0.6.0rc5/src/writer/serve.py
+-rw-r--r--   0        0        0     3599 2024-05-29 09:08:49.159501 writer-0.6.0rc5/src/writer/ss_types.py
+-rw-r--r--   0        0        0     8966 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/Arrow.dom-C52_vrWm.js
+-rw-r--r--   0        0        0  3288135 2024-05-29 09:10:53.564837 writer-0.6.0rc5/src/writer/static/assets/BuilderApp-DakBH-QB.js
+-rw-r--r--   0        0        0   280997 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/BuilderApp-DjkgRMd3.css
+-rw-r--r--   0        0        0    13237 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/ComponentRenderer-BnXm57ig.css
+-rw-r--r--   0        0        0     7856 2024-05-29 09:10:53.560837 writer-0.6.0rc5/src/writer/static/assets/ComponentRenderer-PYR7CN9R.js
+-rw-r--r--   0        0        0    14409 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/abap-D8nrxEjS.js
+-rw-r--r--   0        0        0     4198 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/apex-BrXDlLUW.js
+-rw-r--r--   0        0        0     1094 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/azcli-CElzELwZ.js
+-rw-r--r--   0        0        0     2091 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/bat-CUsyEhik.js
+-rw-r--r--   0        0        0     2782 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/bicep-BtxyJn6H.js
+-rw-r--r--   0        0        0     2431 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/cameligo-ClBCoF8h.js
+-rw-r--r--   0        0        0     9889 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/clojure-B9TqLHAk.js
+-rw-r--r--   0        0        0    79568 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/codicon-BA2IlpFX.ttf
+-rw-r--r--   0        0        0     3836 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/coffee-DYsfeylR.js
+-rw-r--r--   0        0        0     5680 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/cpp-VVGvvgir.js
+-rw-r--r--   0        0        0     4770 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/csharp-Z6z2stHy.js
+-rw-r--r--   0        0        0     1665 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/csp-DgZoLDI1.js
+-rw-r--r--   0        0        0     4756 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/css-KqQ96-gC.js
+-rw-r--r--   0        0        0   984347 2024-05-29 09:10:53.564837 writer-0.6.0rc5/src/writer/static/assets/css.worker-DvNUQFd1.js
+-rw-r--r--   0        0        0    33713 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/cssMode-BjK5GHby.js
+-rw-r--r--   0        0        0     3631 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/cypher-CYoSlgTu.js
+-rw-r--r--   0        0        0     4496 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/dart-BGDl7St1.js
+-rw-r--r--   0        0        0     2115 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/dockerfile-CuCtxA7T.js
+-rw-r--r--   0        0        0     5588 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/ecl-BCTFAUpS.js
+-rw-r--r--   0        0        0   210242 2024-05-29 09:10:53.560837 writer-0.6.0rc5/src/writer/static/assets/editor.worker-BVwmgLrR.js
+-rw-r--r--   0        0        0    10503 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/elixir-C7hRTYZ9.js
+-rw-r--r--   0        0        0     2056 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/flow9-Bi_qi707.js
+-rw-r--r--   0        0        0    16478 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/freemarker2-i8lRH5rw.js
+-rw-r--r--   0        0        0     3229 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/fsharp-CxaaEKKi.js
+-rw-r--r--   0        0        0     2903 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/go-DUImKuGY.js
+-rw-r--r--   0        0        0     2506 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/graphql-D5sGVkLV.js
+-rw-r--r--   0        0        0     7156 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/handlebars-C-M0xH-3.js
+-rw-r--r--   0        0        0     3836 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/hcl-zD_CCkZ1.js
+-rw-r--r--   0        0        0     5396 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/html-D4h1E1bc.js
+-rw-r--r--   0        0        0   648041 2024-05-29 09:10:53.564837 writer-0.6.0rc5/src/writer/static/assets/html.worker-BJMlcbMU.js
+-rw-r--r--   0        0        0    34264 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/htmlMode-B2YRTiG6.js
+-rw-r--r--   0        0        0  1798722 2024-05-29 09:10:53.564837 writer-0.6.0rc5/src/writer/static/assets/index-BaC5au8C.js
+-rw-r--r--   0        0        0     5725 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/index-DMFOqlrb.js
+-rw-r--r--   0        0        0   201777 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/index-DaNZqg5r.js
+-rw-r--r--   0        0        0   345034 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/index-XEiBUN1q.css
+-rw-r--r--   0        0        0   314372 2024-05-29 09:10:53.560837 writer-0.6.0rc5/src/writer/static/assets/index-cJO61pFl.js
+-rw-r--r--   0        0        0     1347 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/ini-8kKHd4ZL.js
+-rw-r--r--   0        0        0     3467 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/java-De1axCfe.js
+-rw-r--r--   0        0        0     1292 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/javascript-BYM0Yx4u.js
+-rw-r--r--   0        0        0   339023 2024-05-29 09:10:53.560837 writer-0.6.0rc5/src/writer/static/assets/json.worker-BwvX8PuZ.js
+-rw-r--r--   0        0        0    39790 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/jsonMode-B8RZLFyl.js
+-rw-r--r--   0        0        0     7395 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/julia-D3ApGBxz.js
+-rw-r--r--   0        0        0     3685 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/kotlin-GbSrCElU.js
+-rw-r--r--   0        0        0     4144 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/less-DNUaDNdz.js
+-rw-r--r--   0        0        0     2683 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/lexon-Bg9QKxBu.js
+-rw-r--r--   0        0        0     4342 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/liquid-ktIne1h-.js
+-rw-r--r--   0        0        0     2369 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/lua-Crkvc3mc.js
+-rw-r--r--   0        0        0     3063 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/m3-DsrzVyM1.js
+-rw-r--r--   0        0        0  1289773 2024-05-29 09:10:53.564837 writer-0.6.0rc5/src/writer/static/assets/mapbox-gl-FST67qaq.js
+-rw-r--r--   0        0        0     4034 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/markdown-CY5IOZuu.js
+-rw-r--r--   0        0        0    35703 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/marked.esm-273vDTCT.js
+-rw-r--r--   0        0        0     5247 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/mdx-Bi1uxJs7.js
+-rw-r--r--   0        0        0     2825 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/mips-BE8RsGBA.js
+-rw-r--r--   0        0        0     5158 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/msdax-N5ajIiFQ.js
+-rw-r--r--   0        0        0    11520 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/mysql-DRxbB97D.js
+-rw-r--r--   0        0        0     2648 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/objective-c-BHUZy23s.js
+-rw-r--r--   0        0        0     3241 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/pascal-BemVzBTY.js
+-rw-r--r--   0        0        0     2246 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/pascaligo-BACCcnx_.js
+-rw-r--r--   0        0        0     8501 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/perl-CuU66Ptk.js
+-rw-r--r--   0        0        0    13710 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/pgsql-CQ6TMH2r.js
+-rw-r--r--   0        0        0     8273 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/php-BvyzZa65.js
+-rw-r--r--   0        0        0     1929 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/pla-DrIuu9u1.js
+-rw-r--r--   0        0        0  3704067 2024-05-29 09:10:53.568837 writer-0.6.0rc5/src/writer/static/assets/plotly.min-Bn62pPWj.js
+-rw-r--r--   0        0        0     8102 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/postiats-BR_hrfni.js
+-rw-r--r--   0        0        0    17185 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/powerquery-CKDUeRmd.js
+-rw-r--r--   0        0        0     3515 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/powershell-Dsa4rhA_.js
+-rw-r--r--   0        0        0     9292 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/protobuf-CGsvhooB.js
+-rw-r--r--   0        0        0     5074 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/pug-D2p3uOX2.js
+-rw-r--r--   0        0        0     4006 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/python-DGmW9UMq.js
+-rw-r--r--   0        0        0     3181 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/qsharp-B7F3HtPF.js
+-rw-r--r--   0        0        0     3377 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/r-3aLoi2fs.js
+-rw-r--r--   0        0        0     9160 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/razor-NRqESbyQ.js
+-rw-r--r--   0        0        0     3802 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/redis-jqFeRM5s.js
+-rw-r--r--   0        0        0    12046 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/redshift-BriwQgXR.js
+-rw-r--r--   0        0        0   163200 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/remixicon-BVOYbT3K.woff2
+-rw-r--r--   0        0        0   525572 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/remixicon-D9ZyeRwQ.ttf
+-rw-r--r--   0        0        0   525744 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/remixicon-DUK49BtM.eot
+-rw-r--r--   0        0        0   224116 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/remixicon-DfzPQSMi.woff
+-rw-r--r--   0        0        0  2460531 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/remixicon-ncU_JTfY.svg
+-rw-r--r--   0        0        0     4139 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/restructuredtext-hbBFZ0w9.js
+-rw-r--r--   0        0        0     8750 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/ruby-ByThyB2Q.js
+-rw-r--r--   0        0        0     4406 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/rust-DIEZMp5R.js
+-rw-r--r--   0        0        0     2075 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/sb-C6Gjjw_x.js
+-rw-r--r--   0        0        0     7564 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/scala-DZNw3jJB.js
+-rw-r--r--   0        0        0     2013 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/scheme-55eqh71t.js
+-rw-r--r--   0        0        0     6655 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/scss-D-OVkc4F.js
+-rw-r--r--   0        0        0   202255 2024-05-29 09:10:53.520836 writer-0.6.0rc5/src/writer/static/assets/serialization-DDqLB4lR.js
+-rw-r--r--   0        0        0     3319 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/shell-DSpi8_qN.js
+-rw-r--r--   0        0        0    18843 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/solidity-BHddiNFS.js
+-rw-r--r--   0        0        0     3010 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/sophia-D6taVZFb.js
+-rw-r--r--   0        0        0     2798 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/sparql-LA0C7mUc.js
+-rw-r--r--   0        0        0    10543 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/sql-C3-3IcFM.js
+-rw-r--r--   0        0        0     7645 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/st-C4g7059C.js
+-rw-r--r--   0        0        0     5417 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/swift-DNI1vH3h.js
+-rw-r--r--   0        0        0     7849 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/systemverilog-DL_FVbcQ.js
+-rw-r--r--   0        0        0     3817 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/tcl-DVJXmIwd.js
+-rw-r--r--   0        0        0  4847810 2024-05-29 09:10:53.568837 writer-0.6.0rc5/src/writer/static/assets/ts.worker-CwG1rUES.js
+-rw-r--r--   0        0        0    22645 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/tsMode-CjGd3dCD.js
+-rw-r--r--   0        0        0     6219 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/twig-BVWDLtw5.js
+-rw-r--r--   0        0        0     5789 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/typescript-8g2Igz_p.js
+-rw-r--r--   0        0        0     6037 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/vb-Btz91-7U.js
+-rw-r--r--   0        0        0   839306 2024-05-29 09:10:53.560837 writer-0.6.0rc5/src/writer/static/assets/vega-embed.module-CxKUxoHf.js
+-rw-r--r--   0        0        0     7592 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/wgsl-D8V_buCG.js
+-rw-r--r--   0        0        0     2790 2024-05-29 09:10:53.512836 writer-0.6.0rc5/src/writer/static/assets/xml-Cey2x9G0.js
+-rw-r--r--   0        0        0     4397 2024-05-29 09:10:53.516837 writer-0.6.0rc5/src/writer/static/assets/yaml-DiYkW6--.js
+-rw-r--r--   0        0        0      889 2024-05-29 09:10:50.644809 writer-0.6.0rc5/src/writer/static/favicon.png
+-rw-r--r--   0        0        0     2789 2024-05-29 09:10:53.560837 writer-0.6.0rc5/src/writer/static/index.html
+-rw-r--r--   0        0        0      432 2024-05-29 09:08:49.159501 writer-0.6.0rc5/src/writer/templates/auth_unauthorized.html
+-rw-r--r--   0        0        0    59105 2024-05-29 09:09:39.628110 writer-0.6.0rc5/src/writer/ui.py
+-rw-r--r--   0        0        0     7896 2024-05-29 09:08:49.159501 writer-0.6.0rc5/src/writer/ui_manager.py
+-rw-r--r--   0        0        0     5423 1970-01-01 00:00:00.000000 writer-0.6.0rc5/PKG-INFO
```

### Comparing `writer-0.6.0rc4/LICENSE.txt` & `writer-0.6.0rc5/LICENSE.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Apache License
+                             Apache License
                            Version 2.0, January 2004
                         http://www.apache.org/licenses/
 
    TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
 
    1. Definitions.
 
@@ -171,26 +171,15 @@
       of any other Contributor, and only if You agree to indemnify,
       defend, and hold each Contributor harmless for any liability
       incurred by, or claims asserted against, such Contributor by reason
       of your accepting any such warranty or additional liability.
 
    END OF TERMS AND CONDITIONS
 
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
+   Copyright 2024 Writer, Inc.
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `writer-0.6.0rc4/README.md` & `writer-0.6.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/pyproject.toml` & `writer-0.6.0rc5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "writer"
-version = "0.6.0rc4"
-description = "Writer Framework helps you create performant data apps, via Python code and its built-in visual UI editor."
-authors = ["Writer, Inc. <dev-feedback@writer.com>"]
+version = "0.6.0rc5"
+description = "An open-source, Python framework for building feature-rich apps that are fully integrated with the Writer platform."
+authors = ["Writer, Inc."]
 readme = "README.md"
 homepage = "https://www.writer.com"
 repository = "https://www.github.com/streamsync-cloud/streamsync"
-documentation = "https://www.streamsync.cloud/getting-started.html"
-keywords = ["data apps", "gui", "ui"]
+documentation = "https://developer.writer.com/framework"
+keywords = ["data apps", "gui", "ui", "framework", "writer framework"]
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Development Status :: 4 - Beta"
 ]
@@ -41,15 +41,15 @@
 python = ">=3.9.2, <4.0"
 python-dateutil = "^2.9.0.post0"
 pytz = "^2024.1"
 requests = "^2.31.0"
 uvicorn = ">= 0.20.0, < 1"
 watchdog = ">= 3.0.0, < 4"
 websockets = ">= 12, < 13"
-writer-sdk = "0.1.0a2"
+writer-sdk = "0.1.0a3"
 
 
 [tool.poetry.group.build]
 optional = true
 
 [tool.poetry.group.build.dependencies]
 alfred-cli = "^2.2.7"
```

### Comparing `writer-0.6.0rc4/src/writer/__init__.py` & `writer-0.6.0rc5/src/writer/__init__.py`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/ai.py` & `writer-0.6.0rc5/src/writer/ai.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,19 +92,22 @@
     def acquire_instance(cls) -> 'WriterAIManager':
         """
         Retrieve the existing instance of WriterAIManager from the current app process.
         If no instance was previously initialized, creates a new one and attaches it to the current app process.
 
         :returns: The current instance of the manager.
         """
+        instance: WriterAIManager
         current_process = get_app_process()
 
         # If instance was not created explicitly, we initialize a new one
-        instance: WriterAIManager = \
-            getattr(current_process, 'ai_manager', cls())
+        try:
+            instance = getattr(current_process, 'ai_manager')
+        except AttributeError:
+            instance = cls()
         return instance
 
     @classmethod
     def authorize(cls, token: str):
         """
         Authorize the WriterAIManager with a new token.
         This can be done as an alternative to setting up an environment variable, or to override the token that was already provided before.
```

### Comparing `writer-0.6.0rc4/src/writer/app_runner.py` & `writer-0.6.0rc5/src/writer/app_runner.py`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/app_templates/ai-starter/static/favicon.png` & `writer-0.6.0rc5/src/writer/app_templates/ai-starter/static/favicon.png`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/app_templates/ai-starter/ui.json` & `writer-0.6.0rc5/src/writer/app_templates/ai-starter/ui.json`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/app_templates/default/main.py` & `writer-0.6.0rc5/src/writer/app_templates/default/main.py`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/app_templates/default/static/favicon.png` & `writer-0.6.0rc5/src/writer/app_templates/default/static/favicon.png`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/app_templates/default/ui.json` & `writer-0.6.0rc5/src/writer/app_templates/default/ui.json`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/app_templates/hello/assets/main_df.csv` & `writer-0.6.0rc5/src/writer/app_templates/hello/assets/main_df.csv`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/app_templates/hello/assets/story.txt` & `writer-0.6.0rc5/src/writer/app_templates/hello/assets/story.txt`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/app_templates/hello/main.py` & `writer-0.6.0rc5/src/writer/app_templates/hello/main.py`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/app_templates/hello/static/README.md` & `writer-0.6.0rc5/src/writer/app_templates/hello/static/README.md`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/app_templates/hello/static/favicon.png` & `writer-0.6.0rc5/src/writer/app_templates/hello/static/favicon.png`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/app_templates/hello/static/pigeon1.jpg` & `writer-0.6.0rc5/src/writer/app_templates/hello/static/pigeon1.jpg`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/app_templates/hello/test_app.py` & `writer-0.6.0rc5/src/writer/app_templates/hello/test_app.py`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/app_templates/hello/ui.json` & `writer-0.6.0rc5/src/writer/app_templates/hello/ui.json`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/app_templates/product-description-generator/prompts.py` & `writer-0.6.0rc5/src/writer/app_templates/pdg-tutorial/prompts.py`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/app_templates/product-description-generator/static/favicon.png` & `writer-0.6.0rc5/src/writer/app_templates/pdg-tutorial/static/favicon.png`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/app_templates/product-description-generator/ui.json` & `writer-0.6.0rc5/src/writer/app_templates/pdg-tutorial/ui.json`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/app_templates/quickstart/main.py` & `writer-0.6.0rc5/src/writer/app_templates/quickstart/main.py`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/app_templates/quickstart/static/README.md` & `writer-0.6.0rc5/src/writer/app_templates/quickstart/static/README.md`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/app_templates/quickstart/static/favicon.png` & `writer-0.6.0rc5/src/writer/app_templates/quickstart/static/favicon.png`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/app_templates/quickstart/ui.json` & `writer-0.6.0rc5/src/writer/app_templates/quickstart/ui.json`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/app_templates/text-demo/main.py` & `writer-0.6.0rc5/src/writer/app_templates/text-demo/main.py`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/app_templates/text-demo/static/favicon.png` & `writer-0.6.0rc5/src/writer/app_templates/text-demo/static/favicon.png`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/app_templates/text-demo/ui.json` & `writer-0.6.0rc5/src/writer/app_templates/text-demo/ui.json`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/auth.py` & `writer-0.6.0rc5/src/writer/auth.py`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/command_line.py` & `writer-0.6.0rc5/src/writer/command_line.py`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/core.py` & `writer-0.6.0rc5/src/writer/core.py`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/core_ui.py` & `writer-0.6.0rc5/src/writer/core_ui.py`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/deploy.py` & `writer-0.6.0rc5/src/writer/deploy.py`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/serve.py` & `writer-0.6.0rc5/src/writer/serve.py`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/ss_types.py` & `writer-0.6.0rc5/src/writer/ss_types.py`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/Arrow.dom-C52_vrWm.js` & `writer-0.6.0rc5/src/writer/static/assets/Arrow.dom-C52_vrWm.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/BuilderApp-DakBH-QB.js` & `writer-0.6.0rc5/src/writer/static/assets/BuilderApp-DakBH-QB.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/BuilderApp-DjkgRMd3.css` & `writer-0.6.0rc5/src/writer/static/assets/BuilderApp-DjkgRMd3.css`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/ComponentRenderer-BnXm57ig.css` & `writer-0.6.0rc5/src/writer/static/assets/ComponentRenderer-BnXm57ig.css`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/ComponentRenderer-PYR7CN9R.js` & `writer-0.6.0rc5/src/writer/static/assets/ComponentRenderer-PYR7CN9R.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/abap-D8nrxEjS.js` & `writer-0.6.0rc5/src/writer/static/assets/abap-D8nrxEjS.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/apex-BrXDlLUW.js` & `writer-0.6.0rc5/src/writer/static/assets/apex-BrXDlLUW.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/azcli-CElzELwZ.js` & `writer-0.6.0rc5/src/writer/static/assets/azcli-CElzELwZ.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/bat-CUsyEhik.js` & `writer-0.6.0rc5/src/writer/static/assets/bat-CUsyEhik.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/bicep-BtxyJn6H.js` & `writer-0.6.0rc5/src/writer/static/assets/bicep-BtxyJn6H.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/cameligo-ClBCoF8h.js` & `writer-0.6.0rc5/src/writer/static/assets/cameligo-ClBCoF8h.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/clojure-B9TqLHAk.js` & `writer-0.6.0rc5/src/writer/static/assets/clojure-B9TqLHAk.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/codicon-BA2IlpFX.ttf` & `writer-0.6.0rc5/src/writer/static/assets/codicon-BA2IlpFX.ttf`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/coffee-DYsfeylR.js` & `writer-0.6.0rc5/src/writer/static/assets/coffee-DYsfeylR.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/cpp-VVGvvgir.js` & `writer-0.6.0rc5/src/writer/static/assets/cpp-VVGvvgir.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/csharp-Z6z2stHy.js` & `writer-0.6.0rc5/src/writer/static/assets/csharp-Z6z2stHy.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/csp-DgZoLDI1.js` & `writer-0.6.0rc5/src/writer/static/assets/csp-DgZoLDI1.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/css-KqQ96-gC.js` & `writer-0.6.0rc5/src/writer/static/assets/css-KqQ96-gC.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/css.worker-DvNUQFd1.js` & `writer-0.6.0rc5/src/writer/static/assets/css.worker-DvNUQFd1.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/cssMode-BjK5GHby.js` & `writer-0.6.0rc5/src/writer/static/assets/cssMode-BjK5GHby.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/cypher-CYoSlgTu.js` & `writer-0.6.0rc5/src/writer/static/assets/cypher-CYoSlgTu.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/dart-BGDl7St1.js` & `writer-0.6.0rc5/src/writer/static/assets/dart-BGDl7St1.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/dockerfile-CuCtxA7T.js` & `writer-0.6.0rc5/src/writer/static/assets/dockerfile-CuCtxA7T.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/ecl-BCTFAUpS.js` & `writer-0.6.0rc5/src/writer/static/assets/ecl-BCTFAUpS.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/editor.worker-BVwmgLrR.js` & `writer-0.6.0rc5/src/writer/static/assets/editor.worker-BVwmgLrR.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/elixir-C7hRTYZ9.js` & `writer-0.6.0rc5/src/writer/static/assets/elixir-C7hRTYZ9.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/flow9-Bi_qi707.js` & `writer-0.6.0rc5/src/writer/static/assets/flow9-Bi_qi707.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/freemarker2-i8lRH5rw.js` & `writer-0.6.0rc5/src/writer/static/assets/freemarker2-i8lRH5rw.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/fsharp-CxaaEKKi.js` & `writer-0.6.0rc5/src/writer/static/assets/fsharp-CxaaEKKi.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/go-DUImKuGY.js` & `writer-0.6.0rc5/src/writer/static/assets/go-DUImKuGY.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/graphql-D5sGVkLV.js` & `writer-0.6.0rc5/src/writer/static/assets/graphql-D5sGVkLV.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/handlebars-C-M0xH-3.js` & `writer-0.6.0rc5/src/writer/static/assets/handlebars-C-M0xH-3.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/hcl-zD_CCkZ1.js` & `writer-0.6.0rc5/src/writer/static/assets/hcl-zD_CCkZ1.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/html-D4h1E1bc.js` & `writer-0.6.0rc5/src/writer/static/assets/html-D4h1E1bc.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/html.worker-BJMlcbMU.js` & `writer-0.6.0rc5/src/writer/static/assets/html.worker-BJMlcbMU.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/htmlMode-B2YRTiG6.js` & `writer-0.6.0rc5/src/writer/static/assets/htmlMode-B2YRTiG6.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/index-BaC5au8C.js` & `writer-0.6.0rc5/src/writer/static/assets/index-BaC5au8C.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/index-DMFOqlrb.js` & `writer-0.6.0rc5/src/writer/static/assets/index-DMFOqlrb.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/index-DaNZqg5r.js` & `writer-0.6.0rc5/src/writer/static/assets/index-DaNZqg5r.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/index-XEiBUN1q.css` & `writer-0.6.0rc5/src/writer/static/assets/index-XEiBUN1q.css`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/index-cJO61pFl.js` & `writer-0.6.0rc5/src/writer/static/assets/index-cJO61pFl.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/ini-8kKHd4ZL.js` & `writer-0.6.0rc5/src/writer/static/assets/ini-8kKHd4ZL.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/java-De1axCfe.js` & `writer-0.6.0rc5/src/writer/static/assets/java-De1axCfe.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/javascript-BYM0Yx4u.js` & `writer-0.6.0rc5/src/writer/static/assets/javascript-BYM0Yx4u.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/json.worker-BwvX8PuZ.js` & `writer-0.6.0rc5/src/writer/static/assets/json.worker-BwvX8PuZ.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/jsonMode-B8RZLFyl.js` & `writer-0.6.0rc5/src/writer/static/assets/jsonMode-B8RZLFyl.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/julia-D3ApGBxz.js` & `writer-0.6.0rc5/src/writer/static/assets/julia-D3ApGBxz.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/kotlin-GbSrCElU.js` & `writer-0.6.0rc5/src/writer/static/assets/kotlin-GbSrCElU.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/less-DNUaDNdz.js` & `writer-0.6.0rc5/src/writer/static/assets/less-DNUaDNdz.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/lexon-Bg9QKxBu.js` & `writer-0.6.0rc5/src/writer/static/assets/lexon-Bg9QKxBu.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/liquid-ktIne1h-.js` & `writer-0.6.0rc5/src/writer/static/assets/liquid-ktIne1h-.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/lua-Crkvc3mc.js` & `writer-0.6.0rc5/src/writer/static/assets/lua-Crkvc3mc.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/m3-DsrzVyM1.js` & `writer-0.6.0rc5/src/writer/static/assets/m3-DsrzVyM1.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/mapbox-gl-FST67qaq.js` & `writer-0.6.0rc5/src/writer/static/assets/mapbox-gl-FST67qaq.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/markdown-CY5IOZuu.js` & `writer-0.6.0rc5/src/writer/static/assets/markdown-CY5IOZuu.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/marked.esm-273vDTCT.js` & `writer-0.6.0rc5/src/writer/static/assets/marked.esm-273vDTCT.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/mdx-Bi1uxJs7.js` & `writer-0.6.0rc5/src/writer/static/assets/mdx-Bi1uxJs7.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/mips-BE8RsGBA.js` & `writer-0.6.0rc5/src/writer/static/assets/mips-BE8RsGBA.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/msdax-N5ajIiFQ.js` & `writer-0.6.0rc5/src/writer/static/assets/msdax-N5ajIiFQ.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/mysql-DRxbB97D.js` & `writer-0.6.0rc5/src/writer/static/assets/mysql-DRxbB97D.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/objective-c-BHUZy23s.js` & `writer-0.6.0rc5/src/writer/static/assets/objective-c-BHUZy23s.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/pascal-BemVzBTY.js` & `writer-0.6.0rc5/src/writer/static/assets/pascal-BemVzBTY.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/pascaligo-BACCcnx_.js` & `writer-0.6.0rc5/src/writer/static/assets/pascaligo-BACCcnx_.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/perl-CuU66Ptk.js` & `writer-0.6.0rc5/src/writer/static/assets/perl-CuU66Ptk.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/pgsql-CQ6TMH2r.js` & `writer-0.6.0rc5/src/writer/static/assets/pgsql-CQ6TMH2r.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/php-BvyzZa65.js` & `writer-0.6.0rc5/src/writer/static/assets/php-BvyzZa65.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/pla-DrIuu9u1.js` & `writer-0.6.0rc5/src/writer/static/assets/pla-DrIuu9u1.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/plotly.min-Bn62pPWj.js` & `writer-0.6.0rc5/src/writer/static/assets/plotly.min-Bn62pPWj.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/postiats-BR_hrfni.js` & `writer-0.6.0rc5/src/writer/static/assets/postiats-BR_hrfni.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/powerquery-CKDUeRmd.js` & `writer-0.6.0rc5/src/writer/static/assets/powerquery-CKDUeRmd.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/powershell-Dsa4rhA_.js` & `writer-0.6.0rc5/src/writer/static/assets/powershell-Dsa4rhA_.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/protobuf-CGsvhooB.js` & `writer-0.6.0rc5/src/writer/static/assets/protobuf-CGsvhooB.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/pug-D2p3uOX2.js` & `writer-0.6.0rc5/src/writer/static/assets/pug-D2p3uOX2.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/python-DGmW9UMq.js` & `writer-0.6.0rc5/src/writer/static/assets/python-DGmW9UMq.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/qsharp-B7F3HtPF.js` & `writer-0.6.0rc5/src/writer/static/assets/qsharp-B7F3HtPF.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/r-3aLoi2fs.js` & `writer-0.6.0rc5/src/writer/static/assets/r-3aLoi2fs.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/razor-NRqESbyQ.js` & `writer-0.6.0rc5/src/writer/static/assets/razor-NRqESbyQ.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/redis-jqFeRM5s.js` & `writer-0.6.0rc5/src/writer/static/assets/redis-jqFeRM5s.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/redshift-BriwQgXR.js` & `writer-0.6.0rc5/src/writer/static/assets/redshift-BriwQgXR.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/remixicon-BVOYbT3K.woff2` & `writer-0.6.0rc5/src/writer/static/assets/remixicon-BVOYbT3K.woff2`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/remixicon-D9ZyeRwQ.ttf` & `writer-0.6.0rc5/src/writer/static/assets/remixicon-D9ZyeRwQ.ttf`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/remixicon-DUK49BtM.eot` & `writer-0.6.0rc5/src/writer/static/assets/remixicon-DUK49BtM.eot`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/remixicon-DfzPQSMi.woff` & `writer-0.6.0rc5/src/writer/static/assets/remixicon-DfzPQSMi.woff`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/remixicon-ncU_JTfY.svg` & `writer-0.6.0rc5/src/writer/static/assets/remixicon-ncU_JTfY.svg`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/restructuredtext-hbBFZ0w9.js` & `writer-0.6.0rc5/src/writer/static/assets/restructuredtext-hbBFZ0w9.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/ruby-ByThyB2Q.js` & `writer-0.6.0rc5/src/writer/static/assets/ruby-ByThyB2Q.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/rust-DIEZMp5R.js` & `writer-0.6.0rc5/src/writer/static/assets/rust-DIEZMp5R.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/sb-C6Gjjw_x.js` & `writer-0.6.0rc5/src/writer/static/assets/sb-C6Gjjw_x.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/scala-DZNw3jJB.js` & `writer-0.6.0rc5/src/writer/static/assets/scala-DZNw3jJB.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/scheme-55eqh71t.js` & `writer-0.6.0rc5/src/writer/static/assets/scheme-55eqh71t.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/scss-D-OVkc4F.js` & `writer-0.6.0rc5/src/writer/static/assets/scss-D-OVkc4F.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/serialization-DDqLB4lR.js` & `writer-0.6.0rc5/src/writer/static/assets/serialization-DDqLB4lR.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/shell-DSpi8_qN.js` & `writer-0.6.0rc5/src/writer/static/assets/shell-DSpi8_qN.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/solidity-BHddiNFS.js` & `writer-0.6.0rc5/src/writer/static/assets/solidity-BHddiNFS.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/sophia-D6taVZFb.js` & `writer-0.6.0rc5/src/writer/static/assets/sophia-D6taVZFb.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/sparql-LA0C7mUc.js` & `writer-0.6.0rc5/src/writer/static/assets/sparql-LA0C7mUc.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/sql-C3-3IcFM.js` & `writer-0.6.0rc5/src/writer/static/assets/sql-C3-3IcFM.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/st-C4g7059C.js` & `writer-0.6.0rc5/src/writer/static/assets/st-C4g7059C.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/swift-DNI1vH3h.js` & `writer-0.6.0rc5/src/writer/static/assets/swift-DNI1vH3h.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/systemverilog-DL_FVbcQ.js` & `writer-0.6.0rc5/src/writer/static/assets/systemverilog-DL_FVbcQ.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/tcl-DVJXmIwd.js` & `writer-0.6.0rc5/src/writer/static/assets/tcl-DVJXmIwd.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/ts.worker-CwG1rUES.js` & `writer-0.6.0rc5/src/writer/static/assets/ts.worker-CwG1rUES.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/tsMode-CjGd3dCD.js` & `writer-0.6.0rc5/src/writer/static/assets/tsMode-CjGd3dCD.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/twig-BVWDLtw5.js` & `writer-0.6.0rc5/src/writer/static/assets/twig-BVWDLtw5.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/typescript-8g2Igz_p.js` & `writer-0.6.0rc5/src/writer/static/assets/typescript-8g2Igz_p.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/vb-Btz91-7U.js` & `writer-0.6.0rc5/src/writer/static/assets/vb-Btz91-7U.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/vega-embed.module-CxKUxoHf.js` & `writer-0.6.0rc5/src/writer/static/assets/vega-embed.module-CxKUxoHf.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/wgsl-D8V_buCG.js` & `writer-0.6.0rc5/src/writer/static/assets/wgsl-D8V_buCG.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/xml-Cey2x9G0.js` & `writer-0.6.0rc5/src/writer/static/assets/xml-Cey2x9G0.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/assets/yaml-DiYkW6--.js` & `writer-0.6.0rc5/src/writer/static/assets/yaml-DiYkW6--.js`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/favicon.png` & `writer-0.6.0rc5/src/writer/static/favicon.png`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/static/index.html` & `writer-0.6.0rc5/src/writer/static/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 <!DOCTYPE html>
 <html lang="en">
 	<head>
 		<meta charset="UTF-8" />
-		<link rel="icon" type="image/png" href="./static/favicon.png" />
+		<link rel="icon" type="image/png" href="./static/favicon.png?2" />
 		<link rel="preconnect" href="https://fonts.googleapis.com">
 		<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
 		<link href="https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,100;0,200;0,300;0,400;0,500;0,600;0,700;0,800;0,900;1,100;1,200;1,300;1,400;1,500;1,600;1,700;1,800;1,900&display=swap" rel="stylesheet">
 		<link href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined" rel="stylesheet" />
 		<meta name="viewport" content="width=device-width, initial-scale=1.0" />
 		<title>Writer Framework</title>
 		<style>
```

### Comparing `writer-0.6.0rc4/src/writer/ui.py` & `writer-0.6.0rc5/src/writer/ui.py`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/src/writer/ui_manager.py` & `writer-0.6.0rc5/src/writer/ui_manager.py`

 * *Files identical despite different names*

### Comparing `writer-0.6.0rc4/PKG-INFO` & `writer-0.6.0rc5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: writer
-Version: 0.6.0rc4
-Summary: Writer Framework helps you create performant data apps, via Python code and its built-in visual UI editor.
+Version: 0.6.0rc5
+Summary: An open-source, Python framework for building feature-rich apps that are fully integrated with the Writer platform.
 Home-page: https://www.writer.com
-Keywords: data apps,gui,ui
+Keywords: data apps,gui,ui,framework,writer framework
 Author: Writer, Inc.
-Author-email: dev-feedback@writer.com
 Requires-Python: >=3.9.2,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.9
@@ -23,16 +22,16 @@
 Requires-Dist: pydantic (>=2.6.0,<3)
 Requires-Dist: python-dateutil (>=2.9.0.post0,<3.0.0)
 Requires-Dist: pytz (>=2024.1,<2025.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: uvicorn (>=0.20.0,<1)
 Requires-Dist: watchdog (>=3.0.0,<4)
 Requires-Dist: websockets (>=12,<13)
-Requires-Dist: writer-sdk (==0.1.0a2)
-Project-URL: Documentation, https://www.streamsync.cloud/getting-started.html
+Requires-Dist: writer-sdk (==0.1.0a3)
+Project-URL: Documentation, https://developer.writer.com/framework
 Project-URL: Repository, https://www.github.com/streamsync-cloud/streamsync
 Description-Content-Type: text/markdown
 
 ## What is Streamsync?
 
 [![PyPi](https://img.shields.io/pypi/v/streamsync.svg?label=Version)](https://pypi.org/project/streamsync/)
 [![CI](https://github.com/streamsync-cloud/streamsync/actions/workflows/ci.yml/badge.svg)](https://github.com/streamsync-cloud/streamsync/actions/workflows/ci.yml)
```

