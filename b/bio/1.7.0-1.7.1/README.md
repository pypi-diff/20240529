# Comparing `tmp/bio-1.7.0.tar.gz` & `tmp/bio-1.7.1.tar.gz`

## Comparing `bio-1.7.0.tar` & `bio-1.7.1.tar`

### file list

```diff
@@ -1,366 +1,119 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 bio-1.7.0/MANIFEST.in
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 bio-1.7.0/Makefile
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 bio-1.7.0/.venv/.gitignore
--rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 bio-1.7.0/.venv/pyvenv.cfg
--rw-r--r--   0        0        0     2232 2020-02-02 00:00:00.000000 bio-1.7.0/.venv/bin/activate
--rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 bio-1.7.0/.venv/bin/activate.csh
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 bio-1.7.0/.venv/bin/activate.fish
--rw-r--r--   0        0        0     2747 2020-02-02 00:00:00.000000 bio-1.7.0/.venv/bin/activate.nu
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 bio-1.7.0/.venv/bin/activate.ps1
--rw-r--r--   0        0        0     1337 2020-02-02 00:00:00.000000 bio-1.7.0/.venv/bin/activate_this.py
--rwxr-xr-x   0        0        0      235 2020-02-02 00:00:00.000000 bio-1.7.0/.venv/bin/bio
--rwxr-xr-x   0        0        0      238 2020-02-02 00:00:00.000000 bio-1.7.0/.venv/bin/coverage
--rwxr-xr-x   0        0        0      238 2020-02-02 00:00:00.000000 bio-1.7.0/.venv/bin/coverage-3.12
--rwxr-xr-x   0        0        0      238 2020-02-02 00:00:00.000000 bio-1.7.0/.venv/bin/coverage3
--rwxr-xr-x   0        0        0      239 2020-02-02 00:00:00.000000 bio-1.7.0/.venv/bin/f2py
--rwxr-xr-x   0        0        0      247 2020-02-02 00:00:00.000000 bio-1.7.0/.venv/bin/fasta_filter.py
--rwxr-xr-x   0        0        0      256 2020-02-02 00:00:00.000000 bio-1.7.0/.venv/bin/normalizer
--rwxr-xr-x   0        0        0      244 2020-02-02 00:00:00.000000 bio-1.7.0/.venv/bin/pip
--rwxr-xr-x   0        0        0      244 2020-02-02 00:00:00.000000 bio-1.7.0/.venv/bin/pip-3.12
--rwxr-xr-x   0        0        0      244 2020-02-02 00:00:00.000000 bio-1.7.0/.venv/bin/pip3
--rwxr-xr-x   0        0        0      244 2020-02-02 00:00:00.000000 bio-1.7.0/.venv/bin/pip3.12
--rwxr-xr-x   0        0        0      244 2020-02-02 00:00:00.000000 bio-1.7.0/.venv/bin/py.test
--rwxr-xr-x   0        0        0      244 2020-02-02 00:00:00.000000 bio-1.7.0/.venv/bin/pytest
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bio-1.7.0/.venv/bin/python -> /Users/ialbert/Library/Application Support/hatch/env/virtual/.pythons/3.12/python/bin/python3.12
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bio-1.7.0/.venv/bin/python3 -> python
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bio-1.7.0/.venv/bin/python3.12 -> python
--rwxr-xr-x   0        0        0      230 2020-02-02 00:00:00.000000 bio-1.7.0/.venv/bin/tqdm
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.gitignore
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 bio-1.7.0/docs/_bookdown.yml
--rw-r--r--   0        0        0      376 2020-02-02 00:00:00.000000 bio-1.7.0/docs/_output.yml
--rw-r--r--   0        0        0     5288 2020-02-02 00:00:00.000000 bio-1.7.0/docs/bio-align.md
--rw-r--r--   0        0        0     2013 2020-02-02 00:00:00.000000 bio-1.7.0/docs/bio-comm.md
--rw-r--r--   0        0        0     3626 2020-02-02 00:00:00.000000 bio-1.7.0/docs/bio-explain.md
--rw-r--r--   0        0        0     4688 2020-02-02 00:00:00.000000 bio-1.7.0/docs/bio-fasta.md
--rw-r--r--   0        0        0     4434 2020-02-02 00:00:00.000000 bio-1.7.0/docs/bio-fetch.md
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 bio-1.7.0/docs/bio-format.md
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bio-1.7.0/docs/bio-gff.md
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 bio-1.7.0/docs/bio-install.md
--rw-r--r--   0        0        0     5555 2020-02-02 00:00:00.000000 bio-1.7.0/docs/bio-intro.md
--rw-r--r--   0        0        0      785 2020-02-02 00:00:00.000000 bio-1.7.0/docs/bio-meta.md
--rw-r--r--   0        0        0     6622 2020-02-02 00:00:00.000000 bio-1.7.0/docs/bio-mygene.md
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 bio-1.7.0/docs/bio-part-info.md
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 bio-1.7.0/docs/bio-part-tasks.md
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 bio-1.7.0/docs/bio-part-utilities.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bio-1.7.0/docs/bio-part1.md
--rw-r--r--   0        0        0     4173 2020-02-02 00:00:00.000000 bio-1.7.0/docs/bio-related.md
--rw-r--r--   0        0        0     1125 2020-02-02 00:00:00.000000 bio-1.7.0/docs/bio-runinfo.md
--rw-r--r--   0        0        0    13016 2020-02-02 00:00:00.000000 bio-1.7.0/docs/bio-search.md
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 bio-1.7.0/docs/bio-table.md
--rw-r--r--   0        0        0     7784 2020-02-02 00:00:00.000000 bio-1.7.0/docs/bio-taxonomy.md
--rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 bio-1.7.0/docs/bio-tips.md
--rw-r--r--   0        0        0     1183 2020-02-02 00:00:00.000000 bio-1.7.0/docs/bio-uniq.md
--rw-r--r--   0        0        0      538 2020-02-02 00:00:00.000000 bio-1.7.0/docs/bio-usage.md
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 bio-1.7.0/docs/google-sdk.md
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 bio-1.7.0/docs/index.Rmd
--rw-r--r--   0        0        0     1325 2020-02-02 00:00:00.000000 bio-1.7.0/docs/old.md
--rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 bio-1.7.0/docs/removed-todo.txt
--rw-r--r--   0        0        0      157 2020-02-02 00:00:00.000000 bio-1.7.0/docs/upload_prebuilt_data.sh
--rw-r--r--   0        0        0     6865 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/404.html
--rw-r--r--   0        0        0    18097 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/bio-align.html
--rw-r--r--   0        0        0    11173 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/bio-comm.html
--rw-r--r--   0        0        0    12956 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/bio-examples.html
--rw-r--r--   0        0        0    12497 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/bio-explain.html
--rw-r--r--   0        0        0    16595 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/bio-fasta.html
--rw-r--r--   0        0        0    13005 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/bio-fetch.html
--rw-r--r--   0        0        0    10658 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/bio-format.html
--rw-r--r--   0        0        0     9552 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/bio-gff.html
--rw-r--r--   0        0        0     9873 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/bio-install.html
--rw-r--r--   0        0        0     8062 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/bio-meta-obtain-viral-metadata.html
--rw-r--r--   0        0        0    24780 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/bio-search.html
--rw-r--r--   0        0        0     8583 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/bio-table.html
--rw-r--r--   0        0        0    17809 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/bio-taxonomy.html
--rw-r--r--   0        0        0    11557 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/bio-tips.html
--rw-r--r--   0        0        0     9281 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/bio-uniq.html
--rw-r--r--   0        0        0    14694 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/index.html
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/reference-keys.txt
--rw-r--r--   0        0        0    61949 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/search_index.json
--rw-r--r--   0        0        0    50722 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/assets/asciinema-player.css
--rw-r--r--   0        0        0   582376 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/assets/asciinema-player.js
--rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/assets/bio.css
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/assets/favicon.ico
--rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/assets/prism.css
--rw-r--r--   0        0        0    13060 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/assets/prism.js
--rw-r--r--   0        0        0    14568 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/images/gff-model-bio.png
--rw-r--r--   0        0        0   453687 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/images/igv-index.png
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/libs/anchor-sections-1.1.0/anchor-sections-hash.css
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/libs/anchor-sections-1.1.0/anchor-sections.css
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/libs/anchor-sections-1.1.0/anchor-sections.js
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/libs/gitbook-2.6.7/css/plugin-bookdown.css
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/libs/gitbook-2.6.7/css/plugin-clipboard.css
--rw-r--r--   0        0        0     8787 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/libs/gitbook-2.6.7/css/plugin-fontsettings.css
--rw-r--r--   0        0        0    30762 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/libs/gitbook-2.6.7/css/plugin-highlight.css
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/libs/gitbook-2.6.7/css/plugin-search.css
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/libs/gitbook-2.6.7/css/plugin-table.css
--rw-r--r--   0        0        0    48663 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/libs/gitbook-2.6.7/css/style.css
--rw-r--r--   0        0        0   165548 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/libs/gitbook-2.6.7/css/fontawesome/fontawesome-webfont.ttf
--rw-r--r--   0        0        0   146237 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/libs/gitbook-2.6.7/js/app.min.js
--rw-r--r--   0        0        0    10754 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/libs/gitbook-2.6.7/js/clipboard.min.js
--rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/libs/gitbook-2.6.7/js/jquery.highlight.js
--rw-r--r--   0        0        0     8991 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/libs/gitbook-2.6.7/js/plugin-bookdown.js
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/libs/gitbook-2.6.7/js/plugin-clipboard.js
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/libs/gitbook-2.6.7/js/plugin-fontsettings.js
--rw-r--r--   0        0        0     9078 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/libs/gitbook-2.6.7/js/plugin-search.js
--rw-r--r--   0        0        0     4027 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/libs/gitbook-2.6.7/js/plugin-sharing.js
--rw-r--r--   0        0        0    89501 2020-02-02 00:00:00.000000 bio-1.7.0/docs/.book/libs/jquery-3.6.0/jquery-3.6.0.min.js
--rw-r--r--   0        0        0    50722 2020-02-02 00:00:00.000000 bio-1.7.0/docs/assets/asciinema-player.css
--rw-r--r--   0        0        0   582376 2020-02-02 00:00:00.000000 bio-1.7.0/docs/assets/asciinema-player.js
--rw-r--r--   0        0        0     5596 2020-02-02 00:00:00.000000 bio-1.7.0/docs/assets/bio.css
--rw-r--r--   0        0        0    15406 2020-02-02 00:00:00.000000 bio-1.7.0/docs/assets/favicon.ico
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 bio-1.7.0/docs/assets/footer.html
--rw-r--r--   0        0        0      447 2020-02-02 00:00:00.000000 bio-1.7.0/docs/assets/header.html
--rw-r--r--   0        0        0     3162 2020-02-02 00:00:00.000000 bio-1.7.0/docs/assets/prism.css
--rw-r--r--   0        0        0    13060 2020-02-02 00:00:00.000000 bio-1.7.0/docs/assets/prism.js
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 bio-1.7.0/docs/code/align1.txt
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 bio-1.7.0/docs/code/align10.txt
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 bio-1.7.0/docs/code/align2.txt
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bio-1.7.0/docs/code/align3.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 bio-1.7.0/docs/code/align4.txt
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 bio-1.7.0/docs/code/align5.txt
--rw-r--r--   0        0        0      418 2020-02-02 00:00:00.000000 bio-1.7.0/docs/code/align6.txt
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 bio-1.7.0/docs/code/align7.txt
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 bio-1.7.0/docs/code/align8.txt
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 bio-1.7.0/docs/code/align9.txt
--rw-r--r--   0        0        0    61015 2020-02-02 00:00:00.000000 bio-1.7.0/docs/code/aligned.fa
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 bio-1.7.0/docs/code/code.sh
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 bio-1.7.0/docs/code/format1.txt
--rw-r--r--   0        0        0      197 2020-02-02 00:00:00.000000 bio-1.7.0/docs/code/format2.txt
--rw-r--r--   0        0        0      522 2020-02-02 00:00:00.000000 bio-1.7.0/docs/code/format3.txt
--rw-r--r--   0        0        0    60966 2020-02-02 00:00:00.000000 bio-1.7.0/docs/code/genomes.fa
--rw-r--r--   0        0        0   135014 2020-02-02 00:00:00.000000 bio-1.7.0/docs/code/genomes.gb
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 bio-1.7.0/docs/code/table1.txt
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bio-1.7.0/docs/code/table2.txt
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 bio-1.7.0/docs/code/table3.txt
--rw-r--r--   0        0        0    14568 2020-02-02 00:00:00.000000 bio-1.7.0/docs/images/gff-model-bio.png
--rw-r--r--   0        0        0    10837 2020-02-02 00:00:00.000000 bio-1.7.0/docs/images/gff-model-ncbi.png
--rw-r--r--   0        0        0   453687 2020-02-02 00:00:00.000000 bio-1.7.0/docs/images/igv-index.png
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 bio-1.7.0/sandbox/gff/README.md
--rw-r--r--   0        0        0    79645 2020-02-02 00:00:00.000000 bio-1.7.0/sandbox/gff/bp_genbank2gff3
--rw-r--r--   0        0        0    10340 2020-02-02 00:00:00.000000 bio-1.7.0/sandbox/gff/convert_genbank_to_gff3.py
--rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 bio-1.7.0/sandbox/gff/fixit.py
--rw-r--r--   0        0        0  6583092 2020-02-02 00:00:00.000000 bio-1.7.0/sandbox/gff/gb2gff.jar
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 bio-1.7.0/sandbox/gff/genbank_to_gff.py
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 bio-1.7.0/sandbox/gff/runall.sh
--rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/__about__.py
--rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/__init__.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/__main__.py
--rw-r--r--   0        0        0     7599 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/align.py
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/code.py
--rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/combine.py
--rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/comm.py
--rw-r--r--   0        0        0    10917 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/convert.py
--rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/enrichr.py
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/fasta.py
--rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/fetch.py
--rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/format.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/gff.py
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/gprof.py
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/gtf.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/jsonrec.py
--rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/main.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/mart.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/meta.py
--rw-r--r--   0        0        0     9986 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/models.py
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/mygene.py
--rw-r--r--   0        0        0    13618 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/ontology.py
--rw-r--r--   0        0        0    11322 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/parser.py
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/patterns.py
--rw-r--r--   0        0        0    11125 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/search.py
--rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/table.py
--rw-r--r--   0        0        0    15408 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/taxon.py
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/test.py
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/uniq.py
--rw-r--r--   0        0        0    12175 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/variant.py
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/vcf2fasta.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/api/__init__.py
--rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/api/ena_fastq.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/api/ncbi_datasets.py
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/BLASTN
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/alias.txt
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/align_default.diff
--rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/align_default.txt
--rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/align_default.vcf
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/align_global.txt
--rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/align_input.fa
--rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/align_input.vcf
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/align_local.txt
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/align_pile1.txt
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/align_s.tsv
--rw-r--r--   0        0        0     4050 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/align_s.txt
--rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/align_s.vcf
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/comm0.txt
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/comm1.txt
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/comm2.txt
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/explain_exon.txt
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/explain_food.txt
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/explain_neutral.txt
--rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/fasta_alias1.fa
--rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/fasta_all1.fa
--rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/fasta_all2.fa
--rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/fasta_all3.fa
--rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/fasta_cds.fa
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/fasta_frame.fa
--rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/fasta_ids.fa
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/fasta_match.fa
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/fasta_multi.fa
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/fasta_olap1.fa
--rw-r--r--   0        0        0    26397 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/fasta_protein.fa
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/fasta_rename1.fa
--rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/fasta_s.fa
--rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/fasta_start.fa
--rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/fasta_stop.fa
--rw-r--r--   0        0        0    26419 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/fasta_translate.fa
--rw-r--r--   0        0        0   193482 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/fetch_enst.txt
--rw-r--r--   0        0        0    14719 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/fetch_gff.gff
--rw-r--r--   0        0        0     9137 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/fetch_prot.fa
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/file1.txt
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/file2.txt
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/format_mafft1.diff.txt
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/format_mafft1.txt
--rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/format_mafft1.vcf
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/genomes.fa
--rw-r--r--   0        0        0   135161 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/genomes.gb
--rw-r--r--   0        0        0   161771 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/genomes.json
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/gff_CDS.gff
--rw-r--r--   0        0        0     7872 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/gff_all.gff
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/gff_olap1.gff
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/gff_slice.gff
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/ids.txt
--rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/lineage.txt
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/mafft.fa
--rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/meta.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/nodiff.txt
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/search_assembly.json
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/search_mygene.json
--rw-r--r--   0        0        0     6873 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/search_prjn.json
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/search_prjn.txt
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/search_srr.json
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/table_1.txt
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/table_2.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/taxids.txt
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/taxon1.txt
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/uniq0.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/uniq1.txt
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/uniq3.txt
--rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/usage.sh
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/data/weird.fa
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/libs/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/libs/__init__.py
--rw-r--r--   0        0        0    15874 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/libs/placlib.py
--rw-r--r--   0        0        0    20944 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/libs/sqlitedict.py
--rw-r--r--   0        0        0    19058 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/libs/xmltodict.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/scripts/__init__.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/scripts/fasta_filter.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 bio-1.7.0/src/biorun/tests/__init__.py
--rw-r--r--   0        0        0     1066 2020-02-02 00:00:00.000000 bio-1.7.0/test/README.md
--rw-r--r--   0        0        0     2430 2020-02-02 00:00:00.000000 bio-1.7.0/test/compare.py
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/CDS.gff
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/alias.txt -> ../data/alias.txt
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/align-s-pairwise.txt
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/align-s-table.txt
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/align-s.vcf
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/align_input.fa -> ../data/align_input.fa
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/align_input.vcf
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/aln1.fa
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/cds.fa
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/comm0.txt
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/comm1.txt
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/comm2.txt
--rw-r--r--   0        0        0   193482 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/enst.txt
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/file1.txt -> ../data/file1.txt
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/file2.txt -> ../data/file2.txt
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/frame.fa
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/gattaca.vcf
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/gattaca1.txt
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/gattaca2.txt
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/gattaca3.txt
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/genomes.alias.fa
--rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/genomes.fa
--rw-r--r--   0        0        0   135014 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/genomes.gb
--rw-r--r--   0        0        0     7872 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/genomes.gff
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/go.txt
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/in1.fa
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/in2.fa
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/mafft.fa -> ../data/mafft.fa
--rw-r--r--   0        0        0      810 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/mafft.vcf
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/meta.txt
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/prjn.txt
--rw-r--r--   0        0        0    25084 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/protein.fa
--rw-r--r--   0        0        0     2662 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/s.fa
--rw-r--r--   0        0        0    78471 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/sars2.gb
--rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/search.txt
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/slice.gff
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/so.txt
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/srr.txt
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/start.fa
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/stop.fa
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/taxonomy.txt
--rw-r--r--   0        0        0    25106 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/translate.fa
--rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/uniq0.txt
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/uniq1.txt
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 bio-1.7.0/test/run/uniq3.txt
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 bio-1.7.0/work/demo.py
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/Test.mk
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/data/._barton_counts.csv
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/data/README.md
--rw-r--r--   0        0        0  2690542 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/data/barton_counts.csv
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/data/barton_design.csv
--rw-r--r--   0        0        0     3198 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/data/golden_counts.csv
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/data/golden_design.csv
--rwxr-xr-x   0        0        0     5094 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/r/combine_salmon.r
--rwxr-xr-x   0        0        0     2100 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/r/create_tx2gene.r
--rwxr-xr-x   0        0        0     7565 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/r/deseq2.r
--rwxr-xr-x   0        0        0     9094 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/r/edger.r
--rwxr-xr-x   0        0        0     3839 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/r/evaluate_results.r
--rwxr-xr-x   0        0        0     2662 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/r/format_featurecounts.r
--rwxr-xr-x   0        0        0     5068 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/r/plot_heatmap.r
--rwxr-xr-x   0        0        0     4869 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/r/plot_pca.r
--rwxr-xr-x   0        0        0     4794 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/r/simulate_counts.r
--rwxr-xr-x   0        0        0     2810 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/r/simulate_null.r
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/recipes/download-data.mk
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/recipes/genome-assembly.mk
--rw-r--r--   0        0        0     2139 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/recipes/rnaseq-with-hisat.mk
--rw-r--r--   0        0        0     1991 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/recipes/rnaseq-with-salmon.mk
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/recipes/short-read-alignments.mk
--rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/recipes/variant-calling.mk
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/run/aria.mk
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/run/bcftools.mk
--rw-r--r--   0        0        0     2274 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/run/bcftools_parallel.mk
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/run/bgzip.mk
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/run/bioproject.mk
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/run/bowtie2.mk
--rw-r--r--   0        0        0     3060 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/run/bwa.mk
--rw-r--r--   0        0        0     1295 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/run/curl.mk
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/run/deepvariant.mk
--rw-r--r--   0        0        0     2096 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/run/fastp.mk
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/run/freebayes.mk
--rw-r--r--   0        0        0     3252 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/run/gatk.mk
--rw-r--r--   0        0        0     1846 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/run/genbank.mk
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/run/hisat2.mk
--rw-r--r--   0        0        0     1723 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/run/ivar.mk
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/run/minimap2.mk
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/run/refgenie.mk
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/run/rsync.mk
--rw-r--r--   0        0        0     2350 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/run/salmon.mk
--rw-r--r--   0        0        0     2036 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/run/snpeff.mk
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/run/splitchrom.mk
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/run/sra.mk
--rw-r--r--   0        0        0     3565 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/run/star.mk
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/run/tester.mk
--rwxr-xr-x   0        0        0     1801 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/run/time.sh
--rw-r--r--   0        0        0     1624 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/run/wiggle.mk
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/setup/README.md
--rwxr-xr-x   0        0        0      803 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/setup/doctor.r
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/setup/init-rstudio.r
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/setup/init-stats.sh
--rw-r--r--   0        0        0     3875 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/workflows/airway.mk
--rw-r--r--   0        0        0     8579 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/workflows/benchmark.mk
--rw-r--r--   0        0        0     1375 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/workflows/presenilin.mk
--rw-r--r--   0        0        0     2832 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/workflows/snpcall.mk
--rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 bio-1.7.0/work/src/workflows/snpeval.mk
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 bio-1.7.0/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 bio-1.7.0/LICENSE
--rw-r--r--   0        0        0     4796 2020-02-02 00:00:00.000000 bio-1.7.0/README.md
--rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 bio-1.7.0/pyproject.toml
--rw-r--r--   0        0        0     5599 2020-02-02 00:00:00.000000 bio-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0      134 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/__about__.py
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/__init__.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/__main__.py
+-rw-r--r--   0        0        0     7599 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/align.py
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/code.py
+-rw-r--r--   0        0        0     2533 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/combine.py
+-rw-r--r--   0        0        0     3403 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/comm.py
+-rw-r--r--   0        0        0    10913 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/convert.py
+-rw-r--r--   0        0        0     3271 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/enrichr.py
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/fasta.py
+-rw-r--r--   0        0        0    10244 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/fetch.py
+-rw-r--r--   0        0        0     1913 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/format.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/gff.py
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/gprof.py
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/gtf.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/jsonrec.py
+-rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/main.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/mart.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/meta.py
+-rw-r--r--   0        0        0     9986 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/models.py
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/mygene.py
+-rw-r--r--   0        0        0    13618 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/ontology.py
+-rw-r--r--   0        0        0    11322 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/parser.py
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/patterns.py
+-rw-r--r--   0        0        0    11124 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/search.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/search2.py
+-rw-r--r--   0        0        0      992 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/table.py
+-rw-r--r--   0        0        0    15408 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/taxon.py
+-rw-r--r--   0        0        0     2752 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/test.py
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/uniq.py
+-rw-r--r--   0        0        0    12175 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/variant.py
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/vcf2fasta.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/api/__init__.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/api/ena.py
+-rw-r--r--   0        0        0     1842 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/api/ena_fastq.py
+-rw-r--r--   0        0        0      161 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/api/ncbi_datasets.py
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/BLASTN
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/alias.txt
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/align_default.diff
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/align_default.txt
+-rw-r--r--   0        0        0      383 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/align_default.vcf
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/align_global.txt
+-rw-r--r--   0        0        0      395 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/align_input.fa
+-rw-r--r--   0        0        0      762 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/align_input.vcf
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/align_local.txt
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/align_pile1.txt
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/align_s.tsv
+-rw-r--r--   0        0        0     4050 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/align_s.txt
+-rw-r--r--   0        0        0     2008 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/align_s.vcf
+-rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/comm0.txt
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/comm1.txt
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/comm2.txt
+-rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/explain_exon.txt
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/explain_food.txt
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/explain_neutral.txt
+-rw-r--r--   0        0        0      405 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/fasta_alias1.fa
+-rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/fasta_all1.fa
+-rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/fasta_all2.fa
+-rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/fasta_all3.fa
+-rw-r--r--   0        0        0     2379 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/fasta_cds.fa
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/fasta_frame.fa
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/fasta_ids.fa
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/fasta_match.fa
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/fasta_multi.fa
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/fasta_olap1.fa
+-rw-r--r--   0        0        0    26397 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/fasta_protein.fa
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/fasta_rename1.fa
+-rw-r--r--   0        0        0     2776 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/fasta_s.fa
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/fasta_start.fa
+-rw-r--r--   0        0        0     2225 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/fasta_stop.fa
+-rw-r--r--   0        0        0    26419 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/fasta_translate.fa
+-rw-r--r--   0        0        0   193482 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/fetch_enst.txt
+-rw-r--r--   0        0        0    14719 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/fetch_gff.gff
+-rw-r--r--   0        0        0     9137 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/fetch_prot.fa
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/file1.txt
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/file2.txt
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/format_mafft1.diff.txt
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/format_mafft1.txt
+-rw-r--r--   0        0        0      760 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/format_mafft1.vcf
+-rw-r--r--   0        0        0      369 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/genomes.fa
+-rw-r--r--   0        0        0   135161 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/genomes.gb
+-rw-r--r--   0        0        0   161771 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/genomes.json
+-rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/gff_CDS.gff
+-rw-r--r--   0        0        0     7872 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/gff_all.gff
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/gff_olap1.gff
+-rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/gff_slice.gff
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/ids.txt
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/lineage.txt
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/mafft.fa
+-rw-r--r--   0        0        0     2044 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/meta.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/nodiff.txt
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/search_assembly.json
+-rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/search_mygene.json
+-rw-r--r--   0        0        0     6873 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/search_prjn.json
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/search_prjn.txt
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/search_srr.json
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/table_1.txt
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/table_2.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/taxids.txt
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/taxon1.txt
+-rw-r--r--   0        0        0        8 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/uniq0.txt
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/uniq1.txt
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/uniq3.txt
+-rw-r--r--   0        0        0     4614 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/usage.sh
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/data/weird.fa
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/libs/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/libs/__init__.py
+-rw-r--r--   0        0        0    15874 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/libs/placlib.py
+-rw-r--r--   0        0        0    20944 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/libs/sqlitedict.py
+-rw-r--r--   0        0        0    19058 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/libs/xmltodict.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/scripts/__init__.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/scripts/fasta_filter.py
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 bio-1.7.1/biorun/tests/__init__.py
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 bio-1.7.1/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 bio-1.7.1/LICENSE
+-rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 bio-1.7.1/README.md
+-rw-r--r--   0        0        0     2170 2020-02-02 00:00:00.000000 bio-1.7.1/pyproject.toml
+-rw-r--r--   0        0        0     5683 2020-02-02 00:00:00.000000 bio-1.7.1/PKG-INFO
```

### Comparing `bio-1.7.0/docs/code/genomes.gb` & `bio-1.7.1/biorun/data/genomes.gb`

 * *Files 0% similar despite different names*

```diff
@@ -1,811 +1,20 @@
-LOCUS       MN996532               29855 bp    RNA     linear   VRL 24-NOV-2020
-DEFINITION  Bat coronavirus RaTG13, complete genome.
-ACCESSION   MN996532
-VERSION     MN996532.2
-KEYWORDS    .
-SOURCE      Bat coronavirus RaTG13
-  ORGANISM  Bat coronavirus RaTG13
-            Viruses; Riboviria; Orthornavirae; Pisuviricota; Pisoniviricetes;
-            Nidovirales; Cornidovirineae; Coronaviridae; Orthocoronavirinae;
-            Betacoronavirus; Sarbecovirus.
-REFERENCE   1  (bases 1 to 29855)
-  AUTHORS   Zhou,P., Yang,X.-L., Wang,X.-G., Hu,B., Zhang,L., Zhang,W.,
-            Si,H.-R., Zhu,Y., Li,B., Huang,C.-L., Chen,H.-D., Chen,J., Luo,Y.,
-            Guo,H., Jiang,R.-D., Liu,M.-Q., Chen,Y., Shen,X.-R., Wang,X.,
-            Zheng,X.-S., Zhao,K., Chen,Q.-J., Deng,F., Liu,L.-L., Yan,B.,
-            Zhan,F.-X., Wang,Y.-Y., Xiao,G.-F. and Shi,Z.-L.
-  TITLE     A pneumonia outbreak associated with a new coronavirus of probable
-            bat origin
-  JOURNAL   Nature 579 (7798), 270-273 (2020)
-  REMARK    DOI: 10.1038/s41586-020-2012-7
-REFERENCE   2  (bases 1 to 29855)
-  AUTHORS   Zhu,Y., Yu,P., Li,B., Hu,B., Si,H.R., Yang,X.L., Zhou,P. and
-            Shi,Z.L.
-  TITLE     Direct Submission
-  JOURNAL   Submitted (27-JAN-2020) CAS Key Laboratory of Special Pathogens,
-            Wuhan Institute of Virology, Center for Biosafety Mega-Science,
-            Chinese Academy of Sciences, No. 44 Xiao Hong Shan, Wuhan, Hubei
-            430071, China
-COMMENT     On Oct 13, 2020 this sequence version replaced MN996532.1.
-            
-            ##Assembly-Data-START##
-            Assembly Method       :: CLC Genomics Workbench v. 12.0
-            Sequencing Technology :: Illumina
-            ##Assembly-Data-END##
-FEATURES             Location/Qualifiers
-     source          1..29855
-                     /organism="Bat coronavirus RaTG13"
-                     /mol_type="genomic RNA"
-                     /isolate="RaTG13"
-                     /isolation_source="fecal swab"
-                     /host="Rhinolophus affinis"
-                     /db_xref="taxon:2709072"
-                     /country="China"
-                     /collection_date="24-Jul-2013"
-                     /note="former lab designation: Bat coronavirus Ra4991"
-     gene            266..21552
-                     /gene="orf1ab"
-     CDS             join(266..13465,13465..21552)
-                     /gene="orf1ab"
-                     /ribosomal_slippage
-                     /codon_start=1
-                     /product="orf1ab polyprotein"
-                     /protein_id="QHR63299.2"
-                     /translation="MESLVPGFNEKTHVQLSLPVLQVRDVLVRGFGDSVEEALSEARQ
-                     HLKDGTCGLVEVEKGVLPQLEQPYVFIKRSDARTAPHGHVMVELVAELNGIQYGRSGE
-                     TLGVLVPYVGETPVVYRKVLLRKNGNKGAGGHSYGADLKSFDLGDELGTDPYEDFQEN
-                     WNTKHSSGVTRDLMRELNGGAYTRYVDNNFCGPDGYPLECIKDLLARAGKASCTLSEQ
-                     LDFIDTKRGVYCCREHEHEIAWYTERSEKSYELQTPFEIKLAKKFDTFNGECPNFVFP
-                     LNSTIKTIQPRVEKKKLDGFMGRIRSVYPVASPNECNQMCLSTLMKCDHCGETSWQTG
-                     DFVKATCEFCGTENLTKEGATTCGYLPQNAVVKIYCPACHNPEVGPEHSLAEYHNESG
-                     LKPILRKGGRTIAFGGCVFSYVGCYNKCAYWIPRASANIGCNHTGVVGEGSEGLNDNL
-                     LEILQKEKVNINIVGDFKLNEEIAIILASFSASTSAFVETVKGLDYKTFKQIVESCGN
-                     FKVTKGKAKKGAWNIGEQKSILSPLYAFASEAARVVRSIFSRTLETAQNSVRALQKAA
-                     ITILDGISQYSLRLIDAMMFTSDLVTNNLVVMAYITGGVVQLTSQWLTNIFGTVYEKL
-                     KPVLDWLEEKFKEGVEFLRDGWEIVKFISTCACEIVGGQIVTCAKEIKESVQTFFKLV
-                     NKFLALCADSIIIGGAKLKALNLGETFVTHSKGLYRKCVKPKEETGLLMPLKAPKEII
-                     FLEGETLPTEVLTEEVVLKTGDLQPLEQPTSEAVEAPLVGTPVCINGLMLLEIKDTEK
-                     YCALAPNMMVTNNTFTLKGGAPTKVTFGDDTVIEVQGYKSVNITFELDERIDKVLNEK
-                     CSTYTVELGTEVNEFACVVADAVIKTLQPVSELLIPLGIDLDEWGMATYYLFDESGEF
-                     KLASHMYCSFYPPDEDEEEGDCEEEDFEPPTQYEYGTEDDYQGKSLEFGATSVTPQPE
-                     EELEEDWLDDDSQQTVVQEDDSEVNQTTITQSIAEVQPQLEMEPTPVVQTEVNSFSGY
-                     LKLTDNVYIKNADIVEEAKKVKPTIVVNAANVYLKHGGGVAGALNKATNNAMQVESDH
-                     YIATNGPLKVGGGCVLSGHNLAKNCLHVVGPNVNRGEDIQLLKSAYENFNQHDVLLAP
-                     LLSAGIFGADPVHSLRVCVDTVRTNVYLAVFDKNLYDKLVSSFLEMKSEKQVEQKTAE
-                     IPKEEVKSSITESKLSVEQRQQVDKKIKACVEEVTTTLEETKFLTENLLLYIDINGNL
-                     HPDSATLVNDIDITFLKKDAPYIVGDVVQEGVLTAVVIPTKKAGGTTEMLTKALRKVP
-                     TDNYITTYPGQGLNGYTVEEARTVLKKCKSAFYILPSIISNEKQEILGTVSWNLREML
-                     AHAEETRKLMPVCMETKAIVSTIQRKYKGIKIQEGVVDYGARFYFYTSKTTVASLINT
-                     LNDLNETLVTMPLGYVTHGLNLEEAARYMRSLKVPATVSVSSPDAVTAYNGYLTSSSK
-                     TPEEHFIETISLAGSYKDWSYSGQSTQLGIEFLKRGDKSVYYTSNPITFHLDGEVITF
-                     DNLKILLSLKEVRTIKVFTTVDNINLHTQVVDMSMTYGQQFGPTYLDGADVTKIKPHN
-                     SHEGKTFYVLPNDDTLRAEAFEYYHTTDPSFLGRYMSALNHTKKWKYPQVNGLTSIKW
-                     ADNNCYLATALLTLQQIELKFNPPALQDAYYRARAGEAANFCALILAYCNKTVGELGD
-                     VRETMNYLFQHANLDSCKRVLNVVCKTCGQQQTTLKGVEAVMYMGTLSYEQLKKGVQI
-                     PCTCGKQATQYLVQQESPFVMMSAPPAQYELKHGTFICASEYTGNYQCGHYKHITSKE
-                     TLYCIDGALLTKSSEYKGPITDIFYKENSYITTIKPVIYKLDGVVCTEIDPKLDNYYK
-                     KDNSYFTEQPIDLVPNQPYPNASFDNFKFVCDNIKLADDLNQLTGYKKPASREFKVTF
-                     FPDLNGDVVAIDYKHYTPSFKKGAKLLHKPIVWHVNNATNKATYKPNTWCIRCLWNTK
-                     PVETSNSFDVLKSEDTQGMDNLACEDLKPVSEEVVENPTIQKDILECNVKTTEVVGDI
-                     ILKPANDGLKITEEVGHTDLMAAYVDNSSLTIKKPNELSRVLGLKTLVTHGLAAVNSV
-                     PWDTIANYAKPFLNKVVSTTTNIVTRCLNRVCTNYMPYFFTLLLQLCTFTRSTNSRIK
-                     ASMPTTIAKNTVKSVGKFCLEASFNYLKSPNFFKLINIIIWFLLLSVCLGSLIYSTAA
-                     LGVLMSNLGMPSYCTGYREGYLNSTNVTTAIYCTGSIPCSVCLSGLDSLDTYPSLETI
-                     QITISSFKWDLTAFGLVAEWFLAYILFTRFFYVLGLAAIMQLFFSYFAVHFISNSWLM
-                     WLIINLVQMAPISAMVRMYIFFASFYYVWKSYVHVVDGCTSSTCMMCYKRNRATRVEC
-                     TTIVNGVRRSFYVYANGGKGFCKLHNWNCVNCDTFCAGSTFISDEVARDLSLQFKRPI
-                     NPTDQSSYIVDSVTVKNGSIHLYFDKAGQKTYERHSLSHFVNLDNLRASNTKGSLPIN
-                     VIVFDGKSKCEESSAKSASVYYSQLMCQPILLLDQALVSDVGDSTEVAVKMFDAYVNT
-                     FSSTFNVPMEKLKTLVATAEAELAKNVSLDNVLSTFISAARQGFVDSDVETKDVVECL
-                     KLSHQSDIEVTGDSCNNYMLTYNKVENMTPRDLGACIDCSARHINAQVAKSHNIALIW
-                     NVKDFMSLSEQLRKQIRSAAKKNNLPFKLTCATTRQVVNVVTTKIALKGGKIVNNWLK
-                     QLIKVTLVFLFVAAIFYLITPVHVMSKHTDFSSEIIGYKAIDGGVTRDIASTDTCFAN
-                     KHADFDTWFSQRGGSYTNDKACPLIAAVITREVGFVVPGLPGTILRTTNGDFLHFLPR
-                     VFSAVGNICYTPSKLIEYTDFATSACVLAAECTIFKDASGKPVPYCYDTNVLEGSVAY
-                     ESLRPDTRYVLMDGSIIQFPNTYLEGSVRVVTTFDSEYCRHGTCERSEAGVCVSTSGR
-                     WVLNNDYYRSLPGVFCGVDAVNLLTNMFTPLIQPIGALDISASIVAGGIVAIVVTCLA
-                     YYFMRFRRAFGEYSHVVAFNTLLFLMSFTVLCLTPVYSFLPGVYSVIYLYLTFYLTND
-                     VSFLAHIQWMVMFTPLVPFWITIVYVICISTKHFYWFFSNYLKRRVVFNGVSFSTFEE
-                     AALCTFLLNKEMYLKLRSDVLLPLTQYNRYLALYNKYKYFSGAMDTTSYREAACCHLA
-                     KALNDFSNSGSDVLYQPPQTSITSAVLQSGFRKMAFPSGKVEGCMVQVTCGTTTLNGL
-                     WLDDVVYCPRHVICTSEDMLNPNYEDLLIRKSNHNFLVQAGNVQLRVIGHSMQNCVLK
-                     LKVDTANTKTPKYKFVRIQPGQTFSVLACYNGSPSGVYQCAMRPNFTIKGSFLNGSCG
-                     SVGFNIDYDCVSFCYMHHMELPTGVHAGTDLEGTFYGPFVDRQTAQAAGTDTTITVNV
-                     LAWLYAAVINGDRWFLNRFTTTLNDFNLVAMKYNYEPLTQDHVDILGPLSAQTGIAVL
-                     DMCASLKELLQNGMNGRTILGSALLEDEFTPFDVVRQCSGVTFQSAVKRTIKGTHHWL
-                     LLTILTSLLVLVQSTQWSLFFFVYENAFLPFAMGIIAMSAFAMMFVKHKHAFLCLFLL
-                     PSLATVAYFNMVYMPASWVMRIMTWLDMVDTSLSGFKLKDCVMYASAVVLLILMTART
-                     VYDDGARRVWTLMNVLTLVYKVYYGNALDQAISMWALIISVTSNYSGVVTTVMFLARG
-                     IVFMCVEYCPIFFITGNTLQCIMLVYCFLGYFCTCYFGLFCLLNRYFRLTLGVYDYLV
-                     STQEFRYMNSQGLLPPKNSIDAFKLNIKLLGVGGKPCIKVATVQSKMSDVKCTSVVLL
-                     SVLQQLRVESSSKLWAQCVQLHNDILLAKDTTEAFEKMVSLLSVLLSMQGAVDINKLC
-                     EEMLDNRATLQAIASEFSSLPSYAAFATAQEAYEQAVANGDSEVVLKKLKKSLNVAKS
-                     EFDRDAAMQRKLEKMADQAMTQMYKQARSEDKRAKVTSAMQTMLFTMLRKLDNDALNN
-                     IINNARDGCVPLNIIPLTTAAKLMVVIPDYNTYKNTCDGTTFTYASALWEIQQVVDAD
-                     SKIVQLSEISMDNSPNLAWPLIVTALRANSAVKLQNNELSPVALRQMSCAAGTTQTAC
-                     TDDNALAYYNTTKGGRFVLALLSDLQDLKWARFPKSDGTGTIYTELEPPCRFVTDTPK
-                     GPKVKYLYFIKGLNNLNRGMVLGSLAATVRLQAGNATEVPANSTVLSFCAFAVDAAKA
-                     YKDYLASGGQPITNCVKMLCTHTGTGQAITVTPEANMDQESFGGASCCLYCRCHIDHP
-                     NPKGFCDLKGKYVQIPTTCANDPVGFTLKNTVCTVCGMWKGYGCSCDQLREPMLQSAD
-                     AQSFLNRVCGVSAARLTPCGTGTSTDVVYRAFDIYNDKVAGFAKFLKTNCCRFQEKDE
-                     DDNLIDSYFVVKRHTFSNYQHEETIYNLLKDCPAVAKHDFFKFRIDGDMVPHISRQRL
-                     TKYTMADLVYALRHFDEGNCDTLREILVTYNCCDDDYFNKKDWYDFVENPDILRVYAN
-                     LGERVRQALLKTVQFCDAMRDAGIVGVLTLDNQDLNGNWYDFGDFIQTTPGSGVPIVD
-                     SYYSLLMPILTLTRALTAESHVDTDLTKPYIKWDLLKYDFTEERLKLFDRYFKYWDQT
-                     YHPNCVNCLDDRCILHCANFNVLFSTVFPPTSFGPLVRKIFVDGVPFVVSTGYHFREL
-                     GVVHNQDVNLHSSRLSFKELLVYAADPAMHAASGNLLLDKRTTCFSVAALTNNVAFQT
-                     VKPGNFNKDFYDFAVSKGFFKEGSSVELKHFFFAQDGNAAISDYDYYRYNLPTMCDIR
-                     QLLFVVEVVDKYFDCYDGGCINANQVIVNNLDKSAGFPFNKWGKARLYYDSMSYEDQD
-                     ALFAYTKRNVIPTITQMNLKYAISAKNRARTVAGVSICSTMTNRQFHQKLLKSIAATR
-                     GATVVIGTSKFYGGWHNMLKTVYSDVENPHLMGWDYPKCDRAMPNMLRIMASLVLARK
-                     HTTCCSLSHRFYRLANECAQVLSEMVMCGGSLYVKPGGTSSGDATTAYANSVFNICQA
-                     VTANVNALLSTDGNKIADKHVRNLQHRLYECLYRNRDVDTDFVNEFYAYLRKHFSMMI
-                     LSDDAVVCFNSTYASQGLVASIKNFKSVLYYQNNVFMSEAKCWTETDLTKGPHEFCSQ
-                     HTMLVKQGDDYVYLPYPDPSRILGAGCFVDDIVKTDGTLMIERFVSLAIDAYPLTKHP
-                     NQEYADVFHLYLQYIRKLHDELTGHMLDMYSVMLTNDNTSRYWEPEFYEAMYTPHTVL
-                     QAVGACVLCNSQTSLRCGACIRRPFLCCKCCYDHVISTSHKLVLSVNPYVCNAPGCDV
-                     TDVTQLYLGGMSYYCKSHKPPISFPLCANGQVFGLYKNTCVGSDNVTDFNAIATCDWT
-                     NAGDYILANTCTERLKLFAAETLKATEETFKLSYGIATVREVLSDRELHLSWEVGKPR
-                     PPLNRNYVFTGYRVTKNSKVQIGEYTFEKGDYGDAVVYRGTTTYKLNVGDYFVLTSHT
-                     VMPLSAPTLVPQEHYVRITGLYPTLNISDEFSSNVANYQKVGMQKYSTLQGPPGTGKS
-                     HFAIGLALYYPSARIVYTACSHAAVDALCEKALKYLPIDKCSRIIPARARVECFDKFK
-                     VNSTLEQYVFCTVNALPETTADIVVFDEISMATNYDLSVVNARLRAKHYVYIGDPAQL
-                     PAPRTLLTKGTLEPEYFNSVCRLMKTIGPDMFLGTCRRCPAEIVDTVSALVYDNKLKA
-                     HKDKSAQCFKMFYKGVITHDVSSAINRPQIGVVREFLTRNPTWRKAVFISPYNSQNAV
-                     ASKILGLPTQTVDSSQGSEYDYVIFTQTTETAHSCNVNRFNVAITRAKVGILCIMSDR
-                     DLYDKLQFTSLEIPRRNVATLQAENVTGLFKDCSKVITGLHPTQAPTHLSVDTKFKTE
-                     GLCVDIPGIPKDMTYRRLISMMGFKMNYQVNGYPNMFITREEAVRHVRAWIGFDVEGC
-                     HATREAIGTNLPLQLGFSTGVNLVAVPTGYVDTPNNTDFSRVSAKPPPGDQFKHLIPL
-                     MYKGLPWNVVRIKIVQMLSDTLKNLSDRVVFVLWAHGFELTSMKYFVKIGPERTCCLC
-                     DKRATCFSTASDTYACWHHSIGFDYVYNPFMIDVQQWGFTGNLQSNHDLYCQVHGNAH
-                     VASCDAIMTRCLAVHECFVKRVDWTIEYPIIGDELKINAACRKVQHMVVKAALLADKF
-                     PVLHDIGNPKAIKCVPQADVEWKFYDAQPCSDKAYKIEELFYSYATHSDKFTDGVCLF
-                     WNCNVDRYPANSIVCRFDTRVLSNLNLPGCDGGSLYVNKHAFHTPAFDKSAFVNLKQL
-                     PFFYYSDSPCESHGKQVVSDIDYVPLKSATCITRCNLGGAVCRHHANEYRLYLDAYNM
-                     MISAGFSLWVYKQFDTYNLWNTFTRLQSLENVAFNVVNKGHFDGQQGEVPVSIINNTV
-                     YTKVDGVDVELFENKTTLPVNVAFELWAKRNIKPVPEVKILNNLGVDIAANTVIWDYK
-                     RDAPAHISTIGVCSMTDIAKKPTENICAPLTVFFDGRVNGQVDLFRNARNGVLITEGS
-                     VKGLQPSVGPKQASLNGVTLIGEALKTQFNYYKKVNGVVQQLPETYFTQSRNLKEFKP
-                     RSQMEIDFLELAMDEFIERYKLEGYAFEHIVYGDFSHRQLGGLHLLIGLAKRSKESPL
-                     ELEDFIPMDSTVKNYFITDAQTGSSKCVCSVIDLLLDDFVEIIKSQDLSVVSKVVKVT
-                     IDYTEISFMLWCKDGHVETFYPKLQSSQAWQPGVAMPNLYKMQRMLLEKCDLQNYGDS
-                     ATLPKGIMMNVAKYTQLCQYLNTLTLAVPYNMRVIHFGAGSDKGVAPGTAVLRQWLPT
-                     GTLLVDSDLNDFVSDADSTLIGDCATVHTANKWDLIISDMYDPKTKNVTKENDSKEGF
-                     FTYICGFIQQKLALGGSVAIKITEHSWNADLYKLMGHFAWWTAFVTNVNASSSEAFLI
-                     GCNYLGKPREQIDGYVMHANYIFWRNTNPIQLSSYSLFDMSKFPLKLRGTAVMSLKEG
-                     QINDMILSLLSKGRLIIRENNRVVISSDVLVNN"
-     gene            21560..25369
-                     /gene="S"
-     CDS             21560..25369
-                     /gene="S"
-                     /codon_start=1
-                     /product="spike glycoprotein"
-                     /protein_id="QHR63300.2"
-                     /translation="MFVFLVLLPLVSSQCVNLTTRTQLPPAYTNSSTRGVYYPDKVFR
-                     SSVLHLTQDLFLPFFSNVTWFHAIHVSGTNGIKRFDNPVLPFNDGVYFASTEKSNIIR
-                     GWIFGTTLDSKTQSLLIVNNATNVVIKVCEFQFCNDPFLGVYYHKNNKSWMESEFRVY
-                     SSANNCTFEYVSQPFLMDLEGKQGNFKNLREFVFKNIDGYFKIYSKHTPINLVRDLPP
-                     GFSALEPLVDLPIGINITRFQTLLALHRSYLTPGDSSSGWTAGAAAYYVGYLQPRTFL
-                     LKYNENGTITDAVDCALDPLSETKCTLKSFTVEKGIYQTSNFRVQPTDSIVRFPNITN
-                     LCPFGEVFNATTFASVYAWNRKRISNCVADYSVLYNSTSFSTFKCYGVSPTKLNDLCF
-                     TNVYADSFVITGDEVRQIAPGQTGKIADYNYKLPDDFTGCVIAWNSKHIDAKEGGNFN
-                     YLYRLFRKANLKPFERDISTEIYQAGSKPCNGQTGLNCYYPLYRYGFYPTDGVGHQPY
-                     RVVVLSFELLNAPATVCGPKKSTNLVKNKCVNFNFNGLTGTGVLTESNKKFLPFQQFG
-                     RDIADTTDAVRDPQTLEILDITPCSFGGVSVITPGTNASNQVAVLYQDVNCTEVPVAI
-                     HADQLTPTWRVYSTGSNVFQTRAGCLIGAEHVNNSYECDIPIGAGICASYQTQTNSRS
-                     VASQSIIAYTMSLGAENSVAYSNNSIAIPTNFTISVTTEILPVSMTKTSVDCTMYICG
-                     DSTECSNLLLQYGSFCTQLNRALTGIAVEQDKNTQEVFAQVKQIYKTPPIKDFGGFNF
-                     SQILPDPSKPSKRSFIEDLLFNKVTLADAGFIKQYGDCLGDIAARDLICAQKFNGLTV
-                     LPPLLTDEMIAQYTSALLAGTITSGWTFGAGAALQIPFAMQMAYRFNGIGVTQNVLYE
-                     NQKLIANQFNSAIGKIQDSLSSTASALGKLQDVVNQNAQALNTLVKQLSSNFGAISSV
-                     LNDILSRLDKVEAEVQIDRLITGRLQSLQTYVTQQLIRAAEIRASANLAATKMSECVL
-                     GQSKRVDFCGKGYHLMSFPQSAPHGVVFLHVTYVPAQEKNFTTAPAICHDGKAHFPRE
-                     GVFVSNGTHWFVTQRNFYEPQIITTDNTFVSGSCDVVIGIVNNTVYDPLQPELDSFKE
-                     ELDKYFKNHTSPDVDLGDISGINASVVNIQKEIDRLNEVAKNLNESLIDLQELGKYEQ
-                     YIKWPWYIWLGFIAGLIAIIMVTIMLCCMTSCCSCLKGCCSCGSCCKFDEDDSEPVLK
-                     GVKLHYT"
-     gene            25378..26205
-                     /gene="NS3"
-     CDS             25378..26205
-                     /gene="NS3"
-                     /codon_start=1
-                     /product="nonstructural protein NS3"
-                     /protein_id="QHR63301.1"
-                     /translation="MDLFMRIFTLGTVTLKQGEIKDATPSDSVRATATIPIQASLPFG
-                     WLIVGVAFLAVFQSASKIITLKKRWQLALSKGIHFICNLLLLFVTVYSHLLLVAAGLE
-                     APFLYLYALVYFLQSINFVRIIMRLWLCWKCRSKNPLLYDANYFLCWHTNCYDYCIPY
-                     NSVTSSIVITSGDGTTSPISEHDYQIGGYTEKWESGVKDCVVLHSYFTSDYYQLYSTQ
-                     LSTDTGVEHVTFFIYNKIVDEPEEHVQIHTIDGSSGVVNPAMEPIYDEPTTTTSVPL"
-     gene            26230..26457
-                     /gene="E"
-     CDS             26230..26457
-                     /gene="E"
-                     /codon_start=1
-                     /product="envelope protein"
-                     /protein_id="QHR63302.1"
-                     /translation="MYSFVSEETGTLIVNSVLLFLAFVVFLLVTLAILTALRLCAYCC
-                     NIVNVSLVKPSFYVYSRVKNLNSSRVPDLLV"
-     gene            26508..27173
-                     /gene="M"
-     CDS             26508..27173
-                     /gene="M"
-                     /codon_start=1
-                     /product="membrane protein"
-                     /protein_id="QHR63303.1"
-                     /translation="MADNGTITVEELKKLLEQWNLVIGFLFLTWICLLQFAYANRNRF
-                     LYIIKLIFLWLLWPVTLACFVLAAVYRINWITGGIAIAMACLVGLMWLSYFIASFRLF
-                     ARTRSMWSFNPETNILLNVPLHGTILTRPLLESELVIGAVILRGHLRIAGHHLGRCDI
-                     KDLPKEITVATSRTLSYYKLGASQRVAGDSGFAAYSRYRIGNYKLNTDHSSSSDNIAL
-                     LVQ"
-     gene            27184..27369
-                     /gene="NS6"
-     CDS             27184..27369
-                     /gene="NS6"
-                     /codon_start=1
-                     /product="nonstructural protein NS6"
-                     /protein_id="QHR63304.1"
-                     /translation="MFHLVDFQVTIAEILLIIMRTFKVSIWNLDYIINLIIKNLSKSL
-                     TENKYSQLDEEQPMEID"
-     gene            27375..27740
-                     /gene="NS7a"
-     CDS             27375..27740
-                     /gene="NS7a"
-                     /codon_start=1
-                     /product="nonstructural protein NS7a"
-                     /protein_id="QHR63305.1"
-                     /translation="MKIILFLVLVTLATCELYHYQECVRGTTVLLKEPCSSGTYEGNS
-                     PFHPLADNKFALTCFSTQFAFACPDGVKHVYQLRARSVSPKLFIRQEEVQELYSPIFL
-                     IIAAIVFITLCFTLKRKTE"
-     gene            27737..27868
-                     /gene="NS7b"
-     CDS             27737..27868
-                     /gene="NS7b"
-                     /codon_start=1
-                     /product="nonstructural protein NS7b"
-                     /protein_id="QHR63306.1"
-                     /translation="MSELSLIDFYLCFLAFLLFLVLIMLIIFWFSLELQDHNETCHA"
-     gene            27875..28240
-                     /gene="NS8"
-     CDS             27875..28240
-                     /gene="NS8"
-                     /codon_start=1
-                     /product="nonstructural protein NS8"
-                     /protein_id="QHR63307.1"
-                     /translation="MKLLVFLGILTTVTAFHQECSLQSCAQHQPYVVDDPCPIHFYSK
-                     WYIRVGARKSAPLIELCVDEVGSKSPIQYIDIGNYTVSCSPFTINCQEPKLGSLVVRC
-                     SFYEDFLEYHDVRVVLDFI"
-     gene            28255..29514
-                     /gene="N"
-     CDS             28255..29514
-                     /gene="N"
-                     /codon_start=1
-                     /product="nucleocapsid protein"
-                     /protein_id="QHR63308.1"
-                     /translation="MSDNGPQNQRNAPRITFGGPSDSTGSNQNGERSGARPKQRRPQG
-                     LPNNTASWFTALTQHGKEDLKFPRGQGVPINTNSSPDDQIGYYRRATRRIRGGDGKMK
-                     DLSPRWYFYYLGTGPEAGLPYGANKDGIIWVATEGALNTPKDHIGTRNPANNAAIVLQ
-                     LPQGTTLPKGFYAEGSRGGSQASSRSSSRSRNSSRNSTPGSSRGTSPARMAGNGSDAA
-                     LALLLLDRLNQLESKMSGKGQQQQSQTVTKKSAAEASKKPRQKRTATKQYNVTQAFGR
-                     RGPEQTQGNFGDQELIRQGTDYKHWPQIAQFAPSASAFFGMSRIGMEVTPSGTWLTYT
-                     GAIKLDDKDPNFKDQVILLNKHIDAYKTFPPTEPKKDKKKKADETQALPQRQKKQQTV
-                     TLLPAADLDDFSKQLQQSMSSADSTQA"
-ORIGIN      
-        1 attaaaggtt tatacctttc caggtaacaa accaacgaac tctcgatctc ttgtagatct
-       61 gttctctaaa cgaactttaa aatctgtgtg actgtcactc ggctgcatgc ttagtgcact
-      121 cacgcagtat aattaataac taattactgt cgttgacagg acacgagtaa ctcatctatc
-      181 ttctgcaggt tgcttacggt ttcgtccgtg ttgcagccga tcatcagcac atctaggttt
-      241 cgtccgggtg tgaccgaaag gtaagatgga gagccttgtc cctggtttca acgagaaaac
-      301 acacgtccaa ctcagtttgc ctgtcttaca ggttcgcgac gtgctcgtac gtggctttgg
-      361 agactccgtg gaggaggctt tatcagaggc acgtcaacat cttaaagatg gcacttgtgg
-      421 cttagtagaa gttgaaaaag gtgttttgcc tcaacttgaa cagccctatg tgttcatcaa
-      481 acgttctgat gctcgaactg cacctcatgg ccatgttatg gttgagctgg tagcagaact
-      541 taatggcatt cagtatggtc gtagtggtga gacactcggt gtccttgtcc cttatgtggg
-      601 cgaaacacca gtggtttacc gcaaggttct tcttcgtaag aacggtaata aaggagctgg
-      661 tggccatagt tacggcgctg atctaaagtc gtttgactta ggcgacgagc ttggcactga
-      721 tccttatgaa gattttcaag aaaactggaa cactaaacat agcagtggtg tcacccgtga
-      781 tctcatgcgt gagcttaatg gaggagcata cactcgctat gtcgataaca acttctgtgg
-      841 ccctgatggc taccctcttg agtgcattaa agaccttcta gctcgtgctg gtaaagcttc
-      901 atgcactttg tccgaacaac tggactttat tgacactaaa agaggtgtat actgctgtcg
-      961 tgaacatgag catgagattg cttggtacac ggaacgttct gaaaagagct atgaattgca
-     1021 gacacctttt gaaattaaat tggcaaagaa atttgacaca tttaatgggg aatgtccaaa
-     1081 ttttgtattc cccctaaatt ccacaatcaa gactattcaa ccaagggttg aaaagaaaaa
-     1141 gcttgatggc tttatgggta gaattcgatc tgtctatcca gttgcttcac caaatgaatg
-     1201 caaccaaatg tgcctttcaa ctctcatgaa gtgtgatcat tgtggtgaaa cttcatggca
-     1261 gacaggcgat tttgttaaag ccacttgtga attttgtggc actgaaaatt tgactaaaga
-     1321 gggtgccact acttgtggtt acctacccca aaatgctgtt gtcaaaattt attgtccagc
-     1381 atgtcataat ccagaagtag gacctgagca tagtcttgct gaatatcata atgaatctgg
-     1441 cttgaaaccc attcttcgta agggtggtcg cactattgct tttggaggct gtgtgttctc
-     1501 ctatgttggt tgctacaata agtgtgccta ttggattcca cgtgctagcg ccaacatagg
-     1561 ttgcaatcat acaggtgttg ttggagaagg ttctgaaggt cttaatgata accttcttga
-     1621 aatacttcaa aaagagaaag tcaacatcaa tattgttggt gactttaaac ttaatgaaga
-     1681 gatcgccatt attttggcat ctttttctgc ttctacaagt gcttttgtgg aaactgtgaa
-     1741 aggtttggat tataaaacat tcaaacaaat tgttgaatcc tgcggtaact ttaaagttac
-     1801 aaaggggaag gcaaagaaag gtgcttggaa cattggtgaa caaaaatcaa tattgagtcc
-     1861 tctttatgca tttgcgtcag aggctgctcg tgttgttcga tcaattttct cccgcactct
-     1921 tgaaactgct caaaattccg tgcgtgcctt acagaaggcc gctataacaa tactagatgg
-     1981 aatttcacag tactcactga gactcattga tgctatgatg ttcacatctg atttggttac
-     2041 taacaatctg gttgtaatgg cttacattac aggtggtgtt gttcagttga cttcacagtg
-     2101 gctaacaaat atctttggca ctgtttatga gaaactcaaa cctgttcttg attggctcga
-     2161 agagaaattc aaggaaggtg tagagtttct tagagatggt tgggaaattg ttaaatttat
-     2221 ctcaacttgt gcttgtgaaa ttgtcggtgg acaaattgtc acctgtgcaa aggaaattaa
-     2281 agagagtgtt cagacattct ttaagcttgt aaacaaattt ttggctttat gtgctgactc
-     2341 catcatcatt ggtggagcta aacttaaagc cttgaattta ggtgaaacat ttgtcacaca
-     2401 ctcaaaggga ttgtatagaa agtgtgttaa acccaaagaa gaaactggct tactcatgcc
-     2461 tctgaaagct ccaaaagaaa ttattttctt agagggagaa acacttccta cagaagtgtt
-     2521 aacagaggaa gttgtcttga aaactggtga tttacaacca ttagaacaac ctactagtga
-     2581 agctgttgaa gccccattgg ttggtacacc agtttgcatt aacgggctca tgttgctcga
-     2641 aattaaagac acagaaaagt actgtgccct tgcacctaat atgatggtaa caaacaatac
-     2701 cttcacactt aaaggcggtg caccaacaaa agttactttt ggtgatgaca ctgtgattga
-     2761 agtgcaaggt tataagagtg tgaatatcac ttttgaactt gacgaaagga ttgataaggt
-     2821 acttaacgag aagtgctcta cctatacagt tgaactcggt acagaagtaa atgagtttgc
-     2881 ttgtgttgta gcagatgctg tcataaaaac tttacaacca gtatctgaat tacttatacc
-     2941 actgggcatt gatttagatg agtggggtat ggctacatac tacttatttg atgagtctgg
-     3001 tgaatttaaa ttggcttcac atatgtactg ttctttttat cctccagatg aggatgagga
-     3061 agaaggtgat tgtgaagaag aagattttga accaccaact caatatgagt atggtactga
-     3121 agatgattac caaggtaaat ctttggaatt tggtgccact tctgtcactc ctcaacctga
-     3181 agaagagcta gaagaagatt ggttagatga tgatagtcaa caaactgtcg ttcaagaaga
-     3241 tgacagtgaa gttaatcaga caactatcac tcaatcaatt gctgaggttc aacctcagtt
-     3301 agagatggaa cctacaccag ttgttcagac tgaagtgaat agctttagtg gttatttaaa
-     3361 acttactgac aatgtataca ttaaaaatgc agacattgtg gaagaagcta aaaaggtaaa
-     3421 accaacaata gttgtcaacg cagccaatgt ttaccttaaa catggaggag gtgttgcggg
-     3481 agctttaaat aaggctacta ataatgccat gcaagttgaa tcagatcatt acatagccac
-     3541 caatggacca cttaaagtgg gtggtggctg tgttttgagt ggacacaatc ttgctaaaaa
-     3601 ctgtcttcat gttgttggtc caaatgttaa cagaggtgaa gatattcaac ttcttaagag
-     3661 tgcttatgaa aattttaatc agcacgatgt tctactcgca ccactattat cagccggtat
-     3721 ttttggtgct gaccctgtac attctttaag agtttgtgta gacactgttc gcacaaatgt
-     3781 ctacctagct gtctttgata aaaatctcta tgacaaactt gtttcaagct ttttagaaat
-     3841 gaagagtgaa aagcaagttg aacaaaagac tgctgaaatt cctaaagagg aagttaagtc
-     3901 atctattact gaaagtaaac tttcagttga gcagagacaa caagttgata agaaaatcaa
-     3961 agcttgtgtt gaagaagtta caacaactct ggaagaaact aagtttctca cagaaaattt
-     4021 gttactctat attgacatta atggcaatct tcatccagat tctgccactc ttgttaatga
-     4081 cattgacatc actttcttaa agaaagatgc tccctatata gtgggtgatg ttgttcaaga
-     4141 gggtgtttta actgctgtag ttatacctac taaaaaggct ggtggtacta ctgaaatgct
-     4201 aacgaaagcc ttgagaaaag tgccaacaga taactatata accacttacc caggccaggg
-     4261 tttaaatggt tatactgtag aagaggcaag gacagtgctt aaaaagtgta aaagtgcctt
-     4321 ttacattcta ccatctatta tctctaatga gaagcaagaa attcttggaa ctgtttcttg
-     4381 gaatttgcga gaaatgcttg cacatgcaga ggaaactcgt aaattaatgc ctgtctgtat
-     4441 ggaaactaaa gctatagttt caactataca gcgtaaatac aagggtatta aaatacaaga
-     4501 gggtgtggtt gattatggtg ccagatttta cttttatacc agtaaaacaa ctgtagcatc
-     4561 acttatcaat acactcaacg atctaaatga gactcttgtt acaatgccac ttggctatgt
-     4621 aacacatggt ttaaatttgg aagaagctgc tcggtatatg agatctctca aagtgccagc
-     4681 tacagtttct gtttcttcac ctgatgctgt tacagcgtat aatggttacc ttacttcttc
-     4741 ttctaaaaca cctgaagaac attttattga aaccatctca cttgctggct cttacaaaga
-     4801 ttggtcctat tctggacagt ctacacaact aggtatagaa tttcttaaga gaggtgataa
-     4861 aagtgtgtat tacactagta accctattac atttcaccta gatggtgaag ttatcacctt
-     4921 tgacaatctt aagatacttc tctctttgaa agaagttagg actattaagg tgtttacaac
-     4981 agtagacaac attaaccttc acacgcaagt tgtggacatg tcaatgacat atggacaaca
-     5041 gtttggccca acttatttgg atggagctga tgttactaaa ataaaacctc ataattcaca
-     5101 tgaaggtaaa acgttttatg ttttgcctaa tgatgacact ttacgtgctg aggcttttga
-     5161 gtactaccac acaactgatc ctagttttct gggtaggtac atgtcagcat taaatcacac
-     5221 taaaaagtgg aaatacccac aagtcaatgg tttaacttct attaaatggg cagataacaa
-     5281 ctgttatctt gccactgcat tattaacact acagcaaata gagttgaaat ttaacccacc
-     5341 tgctttacaa gatgcctact acagggcaag agctggtgaa gctgctaatt tttgtgcact
-     5401 tatcttagcc tactgtaaca agacagtagg tgagttaggt gatgttagag aaacaatgaa
-     5461 ttatttgttt caacatgcca atttagattc ttgcaaaaga gtcttgaatg tggtgtgtaa
-     5521 aacttgtgga caacagcaga ctactcttaa gggtgtagaa gctgttatgt acatgggcac
-     5581 actttcttat gaacaactta agaagggtgt tcagatacct tgtacttgtg gtaaacaagc
-     5641 tacacaatat ctagtacaac aagagtcacc ttttgttatg atgtcggcac cacctgctca
-     5701 gtatgaactt aagcatggta catttatttg tgctagtgag tacactggta attaccagtg
-     5761 tggtcactat aaacatataa cttctaaaga aactttgtat tgcatagacg gtgctttact
-     5821 tacaaagtcc tctgagtaca aaggtcctat tacggatatt ttctacaaag aaaatagcta
-     5881 tataacaacc ataaaaccag ttatttataa attggatggt gttgtttgta cagaaattga
-     5941 tcctaagttg gacaattatt ataagaaaga caattcttat ttcacagagc aaccaattga
-     6001 tcttgtgcca aaccaacctt atccgaatgc aagcttcgat aatttcaagt ttgtatgtga
-     6061 taacatcaaa cttgctgatg atttaaacca gttaactggt tacaagaaac ctgcttcaag
-     6121 agagtttaaa gttacattct tccctgactt aaatggtgat gtggtggcta ttgattataa
-     6181 acactacaca ccttctttta agaaaggagc taaattgtta cataaaccta ttgtctggca
-     6241 tgttaacaat gcaactaaca aagctacgta taaaccaaac acttggtgta tacgctgtct
-     6301 ttggaacaca aaaccagttg aaacatcaaa ctcttttgat gtactgaaat cagaggacac
-     6361 gcagggaatg gataatcttg cctgcgaaga tctaaaacca gtctctgaag aagtagtgga
-     6421 aaatcctacc atacagaaag acattcttga gtgtaatgtg aaaactaccg aagttgtagg
-     6481 agacattata cttaaaccag caaatgatgg tttgaaaatt acagaggagg ttggtcacac
-     6541 agatctaatg gctgcttatg tagacaattc tagtcttact attaagaaac ctaatgaatt
-     6601 atctagagta ctaggtttga aaacccttgt tactcatggt ttagctgctg ttaatagtgt
-     6661 tccgtgggat actatagcta attatgctaa gccttttctt aataaagttg ttagcacaac
-     6721 tactaatata gtcacacggt gtttaaaccg tgtttgtact aattatatgc cttatttctt
-     6781 tactttattg ctacaattgt gtacttttac tagaagtaca aattctagaa ttaaagcatc
-     6841 tatgccgact actatagcaa agaatactgt taagagtgtt ggtaaatttt gcctagaggc
-     6901 ttcatttaat tacctgaagt cacctaattt ttttaaattg attaatatta taatttggtt
-     6961 tttactatta agtgtttgtt taggttcttt aatctactca accgctgctc taggtgtttt
-     7021 aatgtctaat ttaggcatgc cttcttactg tactggctac agagaaggct atttgaactc
-     7081 tactaatgtc actacagcaa tctactgtac tggttctata ccttgtagtg tttgtcttag
-     7141 tggtttagat tctttagata cctatccttc tttagaaact atacaaatta ccatttcatc
-     7201 ttttaaatgg gatttaactg cttttggctt agttgcagag tggtttttgg catatattct
-     7261 ttttactagg ttcttctatg tacttggatt ggctgcaatt atgcaattgt ttttcagcta
-     7321 ttttgcagta cattttatta gtaattcttg gcttatgtgg ttaataatta atcttgtaca
-     7381 aatggcccca atttcagcta tggttaggat gtacattttc tttgcatcat tttattatgt
-     7441 atggaaaagt tatgtgcatg ttgtagatgg ttgtacttca tcaacttgta tgatgtgtta
-     7501 caaacgtaat agagcaacaa gagttgaatg tacaactatt gttaatggtg ttagaaggtc
-     7561 cttttatgtc tatgctaatg gaggtaaagg cttttgcaaa ctacataatt ggaattgtgt
-     7621 taattgtgac acattctgtg ctggtagtac atttattagt gatgaagttg cgagagactt
-     7681 gtcactacag tttaaaagac caataaatcc tactgaccag tcttcctaca ttgttgacag
-     7741 tgttacagtg aagaatggtt ccatccatct ttactttgat aaagctggtc aaaagactta
-     7801 tgaaagacat tctctctctc attttgttaa cttagacaat ttgagagcta gtaacactaa
-     7861 aggttcattg cctattaatg ttatagtttt tgatggtaaa tcaaaatgtg aagaatcatc
-     7921 tgcaaaatca gcgtctgttt attacagtca gcttatgtgt caacctatac tgttactaga
-     7981 tcaggcatta gtgtctgatg ttggtgatag tacagaagtt gcagttaaaa tgtttgatgc
-     8041 ttacgttaat acgttttcat caacttttaa cgttccaatg gaaaaactaa aaacactagt
-     8101 tgcaactgca gaagctgaac ttgcaaagaa tgtgtcctta gacaatgtct tatccacctt
-     8161 tatttcagca gctcggcaag ggtttgttga ttcagatgta gaaactaaag atgttgttga
-     8221 atgtcttaaa ttgtcacatc aatctgacat agaagttact ggtgatagtt gtaataacta
-     8281 tatgctcacc tataacaaag ttgaaaacat gacacctcgt gaccttggtg cttgtattga
-     8341 ctgtagtgcg cgtcatatta atgcgcaggt agcaaaaagt cacaatattg cgttgatatg
-     8401 gaacgttaaa gattttatgt cactgtctga acaactacga aaacaaatac gtagtgctgc
-     8461 caaaaagaac aacttgcctt tcaagttgac atgtgcaact actagacaag ttgttaatgt
-     8521 tgtaacaaca aaaatagcac ttaagggtgg taaaattgtt aataattggt tgaagcagtt
-     8581 aattaaagtt acactcgtgt tcctttttgt tgctgctatc ttctatttaa taacacctgt
-     8641 tcatgtcatg tctaaacata ctgacttttc aagtgaaatt atagggtaca aggctatcga
-     8701 tggtggtgtc actcgtgaca tagcatctac agatacttgt tttgctaaca aacatgctga
-     8761 ttttgacaca tggtttagtc agcgtggtgg tagttatact aatgacaaag cttgtccatt
-     8821 gattgctgca gtcataacaa gagaagtggg ttttgtcgtg cctggtcttc ctggtacgat
-     8881 attacgcaca actaatggtg actttttgca tttcttacct agagttttta gtgcagttgg
-     8941 taacatctgc tatacaccat caaaacttat agagtacact gactttgcaa cttcagcttg
-     9001 tgttttggct gctgaatgta caatttttaa agatgcttct ggtaagccag taccatattg
-     9061 ttatgatact aatgtactag aaggttctgt tgcatatgaa agtctacgtc ctgatacacg
-     9121 ttatgtactc atggatggct ctattattca atttcctaac acctaccttg aaggttctgt
-     9181 tagagtggta acaacttttg attctgagta ttgtagacac ggtacttgtg aaagatcaga
-     9241 agctggtgtt tgtgtatcta ctagtggtag atgggtactt aataatgatt attacagatc
-     9301 tttaccagga gttttttgtg gtgtagatgc tgtaaattta cttactaata tgttcacacc
-     9361 actaattcaa cctatcggtg ctttggacat atcagcatct attgtagccg gcggtattgt
-     9421 tgctatcgta gtaacatgcc ttgcctacta ctttatgagg tttagaagag cttttggtga
-     9481 atacagccat gtagttgcct ttaatacttt actattcctt atgtcattca ctgtactctg
-     9541 tttaacacca gtttactcat ttttacctgg cgtttattct gttatttact tgtacttgac
-     9601 attttatctt actaatgatg tttctttctt agcacatatc cagtggatgg ttatgttcac
-     9661 acctttagta cctttctgga taacaattgt ttatgtcatt tgtatttcca caaagcattt
-     9721 ttactggttc tttagtaact acctaaaaag gcgtgtagtc tttaatggtg tttcctttag
-     9781 tacttttgaa gaagctgcgt tatgcacttt cttattaaat aaggaaatgt atctaaaatt
-     9841 gcgtagtgat gtacttctac ctcttacgca atataataga tatttagccc tttataataa
-     9901 gtacaagtat tttagtggag ccatggatac aactagctac agagaagctg cttgttgtca
-     9961 tcttgcaaaa gctctcaatg atttcagtaa ttcaggttct gatgttcttt atcaaccacc
-    10021 acaaacctct atcacctcgg ctgttttgca gagtggtttt agaaaaatgg cattcccatc
-    10081 aggtaaagtt gagggttgca tggtacaagt tacttgtggt acaaccacac ttaatggtct
-    10141 ttggcttgat gatgtagtct actgtccaag acatgtgatc tgcacctctg aagacatgct
-    10201 taatcctaat tatgaagact tacttatccg caagtctaat cataatttct tggtacaggc
-    10261 tggtaatgtc caacttagag ttattggaca ttctatgcaa aattgtgtgc ttaagcttaa
-    10321 ggtagatact gccaatacta agacgcctaa gtataagttt gttcgcattc aacctggaca
-    10381 gactttttca gtgttagctt gttacaatgg ttcaccatct ggtgtttacc agtgtgctat
-    10441 gagacctaac tttacaatta agggttcatt ccttaatggt tcttgtggta gtgttggttt
-    10501 taacatagat tatgactgtg tctctttttg ttacatgcac catatggaat taccaactgg
-    10561 agttcatgct ggcacagact tagaaggtac cttctatgga ccttttgttg acagacaaac
-    10621 agcacaagca gctggtacgg acacaactat cacagtcaat gttttagctt ggttgtacgc
-    10681 tgctgttata aatggagaca ggtggtttct caatcgattt accacaactc ttaatgattt
-    10741 taacctcgtg gctatgaagt acaattatga acctctaaca caggaccatg ttgacatact
-    10801 aggacctctt tctgctcaaa ccggaattgc cgttttagat atgtgtgctt cactaaaaga
-    10861 attactgcaa aatggtatga atggacgtac catattgggt agtgctttat tagaagatga
-    10921 atttacacct tttgatgttg ttagacaatg ctcaggtgtt actttccaaa gtgcagtaaa
-    10981 aagaacaatc aagggcacac accattggtt gttacttaca attttgactt cacttttagt
-    11041 tttagtccag agtactcaat ggtctttgtt cttttttgtg tatgaaaatg cctttttgcc
-    11101 ttttgctatg ggtattattg ctatgtctgc ttttgcaatg atgtttgtta aacataagca
-    11161 tgcattcctc tgtttgttct tgttaccttc tcttgctact gtagcttact ttaatatggt
-    11221 ctatatgcct gctagttggg tgatgcgcat tatgacatgg ttggatatgg ttgatactag
-    11281 tttgtctggt ttcaagctaa aagactgtgt tatgtatgca tcagccgtag tgttactaat
-    11341 ccttatgaca gcaagaactg tgtatgatga tggtgctagg agggtgtgga cacttatgaa
-    11401 tgtcttgaca ctcgtctata aagtttatta tggtaatgct ttagatcaag ctatttccat
-    11461 gtgggctctt ataatctctg ttacttctaa ctactcgggt gtagttacaa ctgtcatgtt
-    11521 cttggccaga ggtattgttt ttatgtgtgt tgagtattgc cctattttct tcataactgg
-    11581 taatacactt cagtgtataa tgctagttta ttgtttctta ggctatttct gtacttgtta
-    11641 ctttggtctc ttttgtttac tcaaccgtta ctttagactg actcttggtg tttatgatta
-    11701 tttggtttcc acacaagagt ttaggtatat gaattcacag ggattgctcc caccaaagaa
-    11761 tagcatagat gcctttaaac tcaacatcaa attgttgggt gttggaggta aaccttgtat
-    11821 taaagtagcc actgtacagt ctaaaatgtc agatgtaaag tgcacgtcag tagtcttact
-    11881 ctcagttttg caacaactta gagtagaatc atcatctaaa ttgtgggctc aatgtgttca
-    11941 gttacacaat gacatactct tagctaaaga tactactgaa gcctttgaaa aaatggtttc
-    12001 actactttct gtcttgcttt ccatgcaggg tgctgtagac ataaacaagc tttgtgaaga
-    12061 aatgcttgac aacagggcaa ccttacaagc tatagcctca gagtttagtt ctcttccatc
-    12121 atatgcagct tttgctaccg ctcaagaagc ttatgagcag gctgttgcta atggtgactc
-    12181 tgaagttgtc cttaaaaagt tgaagaagtc tttgaatgtg gctaaatctg aatttgaccg
-    12241 tgatgcagcc atgcaacgca agttggaaaa gatggctgat caagctatga cccaaatgta
-    12301 taaacaggct agatctgaag acaagagggc aaaagttact agtgctatgc agacaatgct
-    12361 tttcactatg cttagaaagt tggataatga tgcactcaac aacattatca acaatgcaag
-    12421 agatggttgt gttccattga acataatacc tcttacaaca gcagccaaat taatggttgt
-    12481 cataccagac tataacacat ataaaaatac gtgtgatggt acaacattta cttatgcatc
-    12541 ggcattgtgg gaaatccaac aggttgttga tgcagatagt aaaattgttc aacttagtga
-    12601 aattagcatg gacaattcac ctaatttagc atggcctctt attgtaacag ctttaagggc
-    12661 caattctgct gtcaaattac agaataatga gcttagtcct gttgcactac gacagatgtc
-    12721 ttgtgctgcc ggtactacac aaactgcttg cactgatgac aatgcgttag cttactacaa
-    12781 cacaacaaag ggaggtaggt ttgtacttgc attgttatcc gatttacagg atttgaaatg
-    12841 ggctagattc cctaagagtg atggaactgg tactatctat acagaactgg aaccaccttg
-    12901 taggtttgtt acagacacac ctaaaggtcc taaagtgaag tatttatact ttattaaagg
-    12961 attaaacaat ctaaatagag gtatggtact tggtagttta gctgctacag tacgtttaca
-    13021 agctggtaat gcaacagaag tgcctgccaa ttcaactgta ctatctttct gtgcttttgc
-    13081 tgtagatgcc gctaaagcgt acaaagacta tctagctagt gggggacaac caatcactaa
-    13141 ttgtgttaag atgttgtgta cacacactgg tactggtcag gcaataacag ttacaccaga
-    13201 agccaatatg gatcaagaat cctttggtgg tgcatcgtgt tgtctgtact gtcgttgcca
-    13261 catagatcat ccaaatccta aaggattttg tgacttaaaa ggtaagtatg tacaaatacc
-    13321 tacgacttgt gctaatgacc ctgtgggttt tacacttaaa aacacagtct gtaccgtctg
-    13381 cggtatgtgg aaaggttatg gctgtagttg tgatcaactc cgcgaaccca tgcttcagtc
-    13441 agctgatgca caatcgtttt taaacgggtt tgcggtgtaa gtgcagcccg tcttacaccg
-    13501 tgcggcacag gcactagcac tgatgtcgtg tacagggctt ttgacatcta caatgataaa
-    13561 gtagctggtt ttgctaaatt cttaaaaact aattgttgtc gcttccaaga aaaagacgag
-    13621 gatgacaatt taattgattc ttactttgta gttaagagac acactttctc taactaccaa
-    13681 catgaagaaa caatttataa tttacttaag gattgtccag ctgttgctaa acacgacttc
-    13741 tttaagttta gaatagacgg tgacatggta ccacatatat cacgtcaacg tcttactaaa
-    13801 tacacaatgg cagacctcgt ctatgcttta aggcattttg acgaaggcaa ttgtgataca
-    13861 ttaagagaaa tacttgtcac atacaattgt tgtgacgatg attatttcaa taaaaaagac
-    13921 tggtatgatt ttgtagaaaa cccagatata ttacgcgtat acgccaactt aggtgaacgt
-    13981 gtacgccaag ctttgttaaa aacagtacaa ttctgtgatg ccatgcgaga tgctggtatt
-    14041 gtaggtgtac taacattaga taatcaagat ctcaatggta actggtatga tttcggtgac
-    14101 ttcatacaaa ccactccagg tagtggagtt cctattgtag attcttatta ttcattgtta
-    14161 atgcctatac taactttaac tagggcatta actgcagagt cacatgttga cactgactta
-    14221 acaaagccct acattaagtg ggatttgtta aaatatgact ttacggaaga gaggttaaaa
-    14281 ctctttgacc gttattttaa atattgggat cagacatacc acccaaattg tgttaactgt
-    14341 ttggatgaca gatgcattct gcattgtgca aactttaacg ttttattctc tacagtgttc
-    14401 ccacctacaa gttttggacc tctagtgaga aaaatatttg ttgatggtgt tccatttgta
-    14461 gtttcaactg gataccactt cagggagcta ggtgttgtac ataatcagga tgtaaactta
-    14521 catagctcta gacttagttt taaggaatta cttgtgtatg ctgctgaccc tgctatgcac
-    14581 gctgcttctg gtaatttatt actagataaa cgcactacgt gcttctcagt agctgcactt
-    14641 actaacaatg ttgcttttca aactgtcaaa cccggtaatt ttaacaaaga cttctatgac
-    14701 tttgctgtgt ctaagggttt ctttaaggaa ggaagttctg ttgaattaaa acacttcttc
-    14761 tttgctcagg atggtaatgc tgccatcagc gattatgact actatcgtta taatctacca
-    14821 acaatgtgtg atatcagaca actcctattt gtagttgaag ttgttgataa gtactttgat
-    14881 tgttacgatg gtggctgtat taatgctaac caagtcatcg tcaacaacct agacaaatca
-    14941 gctggttttc catttaataa atggggtaag gctagactct attacgattc aatgagttac
-    15001 gaggatcaag atgcactttt cgcatataca aaacgtaatg tcatccctac tataactcaa
-    15061 atgaatctta agtatgccat tagtgcaaag aatagagctc gcaccgtagc tggtgtctct
-    15121 atctgtagta ctatgaccaa tagacagttt catcaaaaat tattgaaatc aatagccgcc
-    15181 actagaggag ctactgtagt aatcggaaca agcaaatttt atggtggttg gcataacatg
-    15241 ttaaaaactg tttacagtga tgtagaaaac cctcatctta tgggttggga ttaccctaaa
-    15301 tgtgatagag ccatgcctaa catgcttaga attatggcct cacttgttct tgctcgcaaa
-    15361 catacaacgt gctgtagctt gtcacaccgt ttctatagat tagctaatga gtgtgctcaa
-    15421 gtattgagtg aaatggtcat gtgtggcggt tcactatatg ttaaaccagg tggaacctca
-    15481 tcaggagatg ccacaactgc ttatgctaat agtgtcttta acatttgtca agctgttacg
-    15541 gccaatgtta atgcactttt atctactgat ggtaacaaaa ttgccgataa gcacgtccgc
-    15601 aatttacaac acagacttta tgagtgtctc tatagaaata gagatgttga cacagacttt
-    15661 gtgaatgagt tttacgcata tttgcgtaaa catttctcaa tgatgatact ttctgatgat
-    15721 gctgttgtgt gtttcaatag cacttatgca tctcaaggtc tagtggctag cataaagaac
-    15781 tttaaatcag ttctttacta tcaaaacaac gtttttatgt ctgaagcaaa atgttggact
-    15841 gagactgacc ttactaaagg acctcatgaa ttttgctctc aacatacaat gctagttaaa
-    15901 cagggtgatg attatgtgta cctcccttac ccggatccat cacgaatctt aggggctggc
-    15961 tgttttgtag atgatatcgt aaaaacagat ggtacactga tgattgaacg gtttgtgtct
-    16021 ttagctatag atgcttaccc acttactaaa catcctaatc aggagtatgc tgatgtcttt
-    16081 cacttgtact tacaatacat aagaaagtta catgatgagt taacaggaca tatgttagac
-    16141 atgtattctg ttatgcttac taatgataac acttcaaggt attgggaacc tgagttttat
-    16201 gaggctatgt acacaccgca tacagtctta caggctgttg gggcttgtgt tctttgcaat
-    16261 tcacagactt cattaagatg tggtgcttgc atacgtagac cattcttatg ctgtaaatgc
-    16321 tgttacgacc acgtcatatc tacatcacat aaattagtct tgtctgttaa tccgtatgtt
-    16381 tgcaatgctc caggttgtga tgtcacagat gtgactcaac tttacttagg aggtatgagc
-    16441 tattattgta aatcacataa accacccatt agttttccgt tgtgtgctaa tggacaagtt
-    16501 tttggtttat ataagaatac atgtgttggt agcgataatg ttactgactt taacgcaatt
-    16561 gcaacatgtg attggacaaa tgctggtgat tacattttag ctaacacctg tactgaaaga
-    16621 ctcaagcttt tcgcagcaga aacgctcaaa gctactgagg agacatttaa actgtcttat
-    16681 ggtattgcca ctgtacgtga agtgctgtct gacagagaat tgcatctttc atgggaagtt
-    16741 ggtaaaccta gaccaccact taaccgaaat tatgtcttta ctggttatcg tgtaactaaa
-    16801 aacagtaaag tacaaatagg agagtacacc tttgaaaaag gtgactatgg tgatgctgtt
-    16861 gtctaccgag gtacaacaac ttacaaacta aatgttggtg actattttgt gctgacatca
-    16921 catacagtaa tgccattaag tgcacctaca ctagtgccac aagagcacta tgttagaatt
-    16981 actggcttat acccaacact caatatttca gatgagtttt ctagcaatgt tgcaaattat
-    17041 caaaaggttg gtatgcaaaa gtattctaca ctccaaggac cacctggtac tggtaagagt
-    17101 cattttgcta ttggcttagc tctctactac ccttctgctc gcatagtgta cacagcttgc
-    17161 tctcatgccg ctgttgatgc actatgtgag aaggcattaa aatatttgcc tatagataaa
-    17221 tgtagtagaa ttatacctgc acgtgctcgt gtagagtgtt ttgataaatt caaagtgaat
-    17281 tcaacattag aacagtacgt cttttgtact gtaaatgcat tgcctgagac gactgcagat
-    17341 atagttgtct ttgatgaaat ttcaatggct acaaattatg atttgagtgt tgtcaatgct
-    17401 agattacgtg ctaagcacta tgtgtacatt ggcgaccctg ctcaattacc agcaccacgc
-    17461 acattgctaa ctaagggcac actagaacca gaatatttca attcagtgtg tagactcatg
-    17521 aaaactatag gtccagacat gttccttgga acttgtcggc gttgtcctgc tgaaattgtt
-    17581 gacactgtga gtgctttggt ttatgataat aagctgaaag cacataaaga caaatcagct
-    17641 caatgcttta aaatgtttta taagggtgtt attactcatg atgtttcatc tgcaattaac
-    17701 aggccacaaa taggcgtggt aagagaattt cttacacgta atcctacttg gagaaaagct
-    17761 gtcttcattt caccttataa ttcacagaat gctgtagcct caaagatttt gggactacca
-    17821 actcaaactg ttgattcatc acagggttca gaatatgact atgtcatatt cactcaaacc
-    17881 actgagacag ctcactcttg taatgtaaac agatttaatg ttgctattac tagagcaaaa
-    17941 gtaggcatac tttgcataat gtctgataga gacctttatg acaagttgca atttacaagt
-    18001 cttgagattc cacgtaggaa tgtggcaact ttacaagctg aaaatgtaac aggacttttt
-    18061 aaggattgta gtaaggtaat cactgggtta cacccaacac aggcacctac acacctcagt
-    18121 gttgacacta aattcaaaac tgaaggttta tgtgttgaca tacctggtat acctaaggac
-    18181 atgacctata gaagactcat ctctatgatg ggtttcaaaa tgaattacca agttaatggt
-    18241 taccctaata tgtttatcac ccgtgaggaa gccgtaagac atgtacgtgc atggattggc
-    18301 tttgatgtcg aggggtgtca tgctactaga gaagctattg gtactaattt acctttacag
-    18361 ctaggctttt ctacaggtgt taacctagtt gctgtaccta caggctatgt tgatacacct
-    18421 aataatacag atttttccag agttagtgct aaaccaccac ctggagatca gtttaaacat
-    18481 cttataccac ttatgtataa aggacttcct tggaatgtag tgcgtataaa gattgtacaa
-    18541 atgttaagtg atacacttaa aaatctctct gacagagtcg tgtttgtctt atgggcacat
-    18601 ggctttgaat taacatctat gaagtatttt gtgaaaatag gacctgagcg cacttgttgt
-    18661 ctatgtgata aacgtgccac atgcttttcc actgcttcag acacttatgc ctgttggcat
-    18721 cattctattg gatttgatta tgtctataat ccgtttatga ttgatgttca acaatggggt
-    18781 tttacaggta acctacaaag caaccatgat ctgtattgtc aggttcatgg taatgcacat
-    18841 gtagctagtt gtgatgcaat catgactaga tgtctagctg tccacgagtg ctttgttaag
-    18901 cgtgttgact ggactattga ataccctata attggtgatg aactgaagat taatgcggct
-    18961 tgtagaaagg ttcaacacat ggttgttaaa gctgcattat tagcagacaa atttccagtt
-    19021 cttcatgaca ttggtaaccc taaagctatt aagtgtgtac ctcaagctga tgtagaatgg
-    19081 aagttctatg acgcacagcc ttgtagtgac aaagcttata aaatagaaga attattctat
-    19141 tcttatgcca cacattctga caaattcaca gatggtgtat gcctattttg gaattgcaat
-    19201 gtcgatagat atcctgctaa ttccattgtt tgtagatttg acactagagt gctatctaac
-    19261 cttaacttgc ctggttgtga tggtggcagt ttgtatgtaa ataaacatgc attccacaca
-    19321 ccagcttttg ataaaagtgc ttttgttaat ttaaaacaat taccattttt ctattactct
-    19381 gacagtccat gtgagtctca tggaaaacaa gtagtgtcag atatagacta tgtaccacta
-    19441 aagtctgcta cgtgcataac acgttgcaat ttaggtggtg ctgtctgtag acatcatgct
-    19501 aatgagtaca gattgtatct tgatgcttac aacatgatga tctcagctgg ctttagcttg
-    19561 tgggtttaca aacaatttga tacttacaac ctctggaata cttttacaag acttcagagt
-    19621 ttagaaaatg tggcttttaa tgttgtaaat aaaggacact ttgatggaca acagggtgaa
-    19681 gtaccagttt ccatcattaa taacactgtt tacacaaaag ttgatggtgt tgatgtagaa
-    19741 ctatttgaaa ataaaacaac attacctgtt aatgtagcat ttgagctctg ggctaagcgc
-    19801 aatattaaac cagtaccaga ggtgaaaata ctcaataatt tgggtgtgga cattgctgct
-    19861 aatactgtga tttgggacta caaaagagat gctccagcac atatatctac tattggtgtt
-    19921 tgttctatga ctgacatagc caagaaacca actgaaaata tttgtgcacc actcactgtc
-    19981 tttttcgatg gtagagtcaa tggtcaagta gacttgttta gaaatgcccg taatggtgtt
-    20041 cttattacag aaggtagtgt taaaggttta caaccatctg taggtcctaa acaagccagt
-    20101 cttaatggag tcacattgat tggagaagcc ttaaaaacac agttcaatta ttacaagaaa
-    20161 gttaatggtg ttgttcaaca actacctgaa acttacttta cccaaagtag aaatttaaaa
-    20221 gaattcaaac ccaggagtca aatggaaatt gatttcttag aattagctat ggatgaattc
-    20281 attgaacggt ataaactaga aggttatgcc ttcgaacata tcgtctatgg agattttagt
-    20341 cataggcagt taggtggttt acatctactg attggactag ctaaacgttc taaggaatca
-    20401 cctcttgaat tagaagattt tattcctatg gacagtacag ttaaaaatta cttcataaca
-    20461 gatgcgcaaa caggttcatc taagtgtgtg tgttctgtta ttgatttatt acttgatgat
-    20521 tttgttgaaa taataaaatc gcaggattta tctgtagttt ctaaggtggt caaagtgacc
-    20581 attgactata cagaaatttc atttatgctt tggtgtaaag atggacatgt tgaaacattt
-    20641 tacccaaaat tacaatctag tcaagcgtgg caaccgggtg ttgctatgcc taatctctac
-    20701 aaaatgcaaa gaatgttact agaaaagtgt gaccttcaaa attatggtga tagtgcaaca
-    20761 ttacctaaag gcataatgat gaatgtcgca aaatatactc aactgtgtca gtatttaaat
-    20821 acacttactt tagctgtacc ctataatatg agggttatac attttggtgc tggttctgat
-    20881 aaaggagttg cacctggtac agctgtttta agacagtggt tgcctacggg tacactactt
-    20941 gtcgattcag atcttaatga ctttgtctct gatgcagatt caactttgat tggtgattgt
-    21001 gcaactgtac atacagctaa taaatgggat ctcattatta gtgatatgta cgatcctaag
-    21061 actaaaaatg ttacaaaaga aaatgattcc aaagagggat ttttcactta catttgtgga
-    21121 tttatacaac aaaagctagc ccttggaggt tctgtagcta taaagataac agagcattct
-    21181 tggaatgccg atctttataa gcttatggga catttcgcat ggtggactgc ttttgttact
-    21241 aatgtaaatg catcttcatc tgaagcattt ttaattgggt gtaattacct tggcaaaccg
-    21301 cgtgaacaga tagatggtta tgtcatgcat gcaaattaca tattttggag gaatacaaac
-    21361 ccaattcagt tgtcttccta ttctttattt gacatgagta aattccccct taaattaagg
-    21421 ggtactgcag ttatgtcttt gaaagaaggt caaatcaatg atatgatttt atctcttctt
-    21481 agtaaaggta gacttataat tagagaaaac aatagagttg ttatttctag tgatgttctt
-    21541 gttaacaact aaacgaacca tgtttgtttt tcttgtttta ttgccactag tttctagtca
-    21601 gtgtgttaat ctaacaacta gaactcagtt acctcctgca tacaccaact catccacccg
-    21661 tggtgtctat taccctgaca aagttttcag atcttcagtt ttacatttaa ctcaggattt
-    21721 gtttttacct ttcttctcca atgtgacctg gttccatgct atacatgttt cagggaccaa
-    21781 tggtattaaa aggtttgata acccagttct gccattcaac gatggcgtct attttgcttc
-    21841 cactgagaag tctaatataa taagaggatg gatttttggt actaccttag attcgaagac
-    21901 ccagtctcta cttattgtta ataacgctac taatgttgtt attaaagtct gtgaatttca
-    21961 attttgtaat gatccatttt tgggtgttta ttaccacaaa aacaacaaaa gttggatgga
-    22021 aagtgagttc agagtttact ctagtgcgaa taattgcact tttgagtatg tctctcagcc
-    22081 ttttcttatg gaccttgaag gaaaacaggg taatttcaaa aatcttaggg aattcgtgtt
-    22141 taagaatatt gatggttatt tcaaaatata ttctaaacat acgcctatta atttagtgcg
-    22201 tgatcttccc cctggttttt cagctttaga accattggta gatctgccaa taggtattaa
-    22261 catcactagg tttcaaactt tacttgcttt acatagaagc tatttgactc ctggtgattc
-    22321 ttcttcaggt tggacagctg gtgctgcagc ttattatgtg ggttatcttc aaccaaggac
-    22381 ttttctacta aaatataatg agaatggaac cattacagat gctgtagact gtgcacttga
-    22441 ccctctttca gaaacaaagt gtacgttaaa atccttcact gttgaaaaag gaatttatca
-    22501 aacctctaac tttagagtcc aaccaacaga ttctattgtt agattcccaa atattacaaa
-    22561 cttatgtcct tttggtgaag tttttaacgc caccacattc gcatcagttt atgcttggaa
-    22621 cagaaagaga attagcaact gtgttgctga ttactctgtc ctatataatt ccacttcatt
-    22681 ttctaccttt aaatgttatg gagtgtctcc tactaaatta aatgatctct gctttactaa
-    22741 tgtttatgca gactcatttg tgattacagg tgatgaagtc agacaaattg cgccaggaca
-    22801 aactggaaag attgctgact acaattataa actaccagat gattttactg gttgtgttat
-    22861 agcttggaat tctaagcata ttgatgcaaa agagggcggt aattttaact atctttaccg
-    22921 tctctttaga aaagctaatc ttaaaccctt tgagagggat atctcaactg aaatttacca
-    22981 agcaggcagc aaaccttgta atggtcaaac tggtctaaat tgctactacc cactttatag
-    23041 atatggattt taccctactg atggtgttgg tcaccaacct tatagggtag tagtactttc
-    23101 ttttgaactt ctaaatgcac cagcaactgt ttgtggacct aagaagtcta ctaacttggt
-    23161 taaaaataaa tgtgtcaatt tcaactttaa tggtttaact ggcacaggtg tcctcacaga
-    23221 gtctaataaa aagtttctac ctttccaaca atttggtaga gacattgcag acactactga
-    23281 tgccgtccgt gatccacaga cacttgagat tcttgacatt acaccatgtt cttttggtgg
-    23341 tgtcagtgtt ataacacctg gaacaaatgc ctctaaccag gttgctgttc tttatcagga
-    23401 tgttaactgc acagaagtcc ctgttgctat ccatgcagac caacttactc ccacttggcg
-    23461 tgtttactcc acaggttcta atgtttttca aacacgtgca ggttgtttaa taggggctga
-    23521 acatgtcaat aactcgtatg agtgtgacat acctattggt gcaggaatat gcgccagtta
-    23581 tcagactcaa actaattcac gtagtgtggc cagtcaatct attattgcct acactatgtc
-    23641 acttggtgca gaaaattcag ttgcttattc taataactct attgccatac ctacaaattt
-    23701 tactattagt gtgaccactg aaattctacc tgtgtctatg acaaagacat cggtagactg
-    23761 tacaatgtat atttgtggtg attcaactga gtgcagcaac cttttgttgc aatatggtag
-    23821 tttttgcaca caattaaatc gtgctttaac tggaatagct gttgaacagg acaaaaatac
-    23881 tcaagaagtt tttgctcaag ttaaacaaat ttataagaca ccaccaatta aagattttgg
-    23941 tggtttcaat ttttcacaaa tattaccaga tccatcaaaa ccaagcaaga ggtcatttat
-    24001 tgaggattta cttttcaata aagtgacact tgctgatgct ggcttcatca aacaatatgg
-    24061 tgattgcctt ggtgatattg ctgctaggga tcttatttgt gctcaaaagt tcaatggcct
-    24121 tactgttctg ccacctttgc tcacagatga aatgatcgct caatacactt ctgcactatt
-    24181 agcaggtaca atcacttctg gttggacttt tggtgcaggt gctgctttac aaataccatt
-    24241 tgccatgcaa atggcttata ggtttaatgg tattggagtt acacagaatg ttctctatga
-    24301 gaaccaaaaa ttgattgcca accagtttaa tagtgctatt ggcaaaattc aagactcact
-    24361 ttcttctaca gcaagtgcac ttggaaaact tcaagatgtt gtcaaccaaa atgcacaagc
-    24421 tttaaacacg cttgttaaac aacttagctc caattttgga gctatttcta gcgtgttaaa
-    24481 tgatatcctt tcacgtctcg acaaagttga ggctgaagtg cagattgaca ggttgatcac
-    24541 aggcagactt caaagcttgc agacatatgt gactcaacaa ttaattagag ctgcagaaat
-    24601 cagagcttct gccaatcttg ctgctactaa aatgtcagag tgtgtactcg gacaatcaaa
-    24661 aagagttgat ttttgtggaa aaggctatca tcttatgtct ttccctcagt cagcacctca
-    24721 tggtgtagtc ttcttgcatg tgacatatgt ccctgcacaa gaaaagaact tcacaactgc
-    24781 tcctgccatt tgtcatgatg gaaaagcaca ctttccacgt gaaggtgttt tcgtttcaaa
-    24841 tggcacacac tggtttgtta cacaaaggaa tttttatgaa ccacaaatta ttacaacaga
-    24901 caacacattt gtctctggta gctgtgatgt tgtaatagga attgtcaaca acacagttta
-    24961 tgatcctttg caaccagaac ttgattcatt caaggaggag ttggataaat actttaaaaa
-    25021 tcatacatca cctgatgtag atttaggtga catttctggc attaatgctt cagttgtcaa
-    25081 tattcaaaag gaaattgacc gcctcaatga ggttgccaaa aatctaaatg aatctctcat
-    25141 cgatctccaa gaacttggaa agtatgaaca gtatataaaa tggccatggt acatttggct
-    25201 aggttttata gctggcttga ttgccataat aatggtcacg attatgcttt gctgtatgac
-    25261 cagttgctgc agttgtctca agggctgttg ttcttgcgga tcttgctgca aatttgatga
-    25321 agacgactct gagccagtgc tcaaaggagt caaattacat tacacataaa cgaacttatg
-    25381 gatttgttta tgagaatttt cacacttgga actgtaactt tgaaacaagg tgaaattaag
-    25441 gatgctactc cttcagattc tgttcgcgct actgcaacga taccgataca agcctcactc
-    25501 cctttcggat ggcttattgt tggcgttgca tttcttgctg tttttcaaag cgcttccaag
-    25561 atcataaccc ttaaaaagag atggcaacta gcactctcta agggtattca ctttatttgc
-    25621 aacttgctgc tgctgtttgt aacagtttac tcacatcttt tgctcgttgc tgctggtctt
-    25681 gaagccccat tcctctacct ctacgcttta gtctacttct tgcagagtat aaactttgta
-    25741 agaataataa tgaggctttg gctttgctgg aaatgccgtt ccaaaaaccc attactctat
-    25801 gatgctaact acttcctttg ttggcatact aattgttatg actattgtat accttacaat
-    25861 agtgtaactt cttcaattgt cattacttca ggtgatggca caacaagtcc tatttctgaa
-    25921 catgactacc agattggtgg ttatactgaa aaatgggagt ctggagtaaa agactgtgtt
-    25981 gtattacaca gttacttcac ttcagattat taccagctgt actcaactca attgagcaca
-    26041 gacactggtg ttgaacatgt taccttcttc atctacaata aaattgttga tgagcctgaa
-    26101 gaacatgtcc aaattcacac aatcgacggt tcatccggag ttgttaatcc agcaatggaa
-    26161 ccaatttatg atgaaccgac gacgactact agcgtgcctt tgtaagcaca agctgatgag
-    26221 tacgaactta tgtactcatt cgtttcggaa gagacaggta cgttaatagt taatagcgta
-    26281 cttctttttc ttgctttcgt ggtattcttg ctagtcacac tagccatcct tactgcgctt
-    26341 cgattgtgtg cgtactgctg caatattgtt aacgtgagtc ttgtaaaacc ttctttttac
-    26401 gtttactctc gtgttaaaaa tctgaattct tctagagttc ctgatcttct ggtctaaacg
-    26461 aactaaatat tatattagtt tttctgtttg gaactttaat tttagccatg gcagataacg
-    26521 gtactattac cgttgaagag ctgaaaaagc tccttgaaca gtggaatcta gtaataggat
-    26581 tcctatttct tacatggatt tgtcttctac aatttgccta tgccaacagg aataggtttt
-    26641 tgtatataat taagttaatt ttcctctggc tgctttggcc agtaacttta gcctgctttg
-    26701 tgcttgctgc tgtttacaga ataaattgga tcactggagg aatcgctatc gcaatggctt
-    26761 gtcttgtagg cttgatgtgg ctgagctact tcattgcttc tttcaggcta tttgcacgta
-    26821 cgcgttccat gtggtcattc aatccagaaa ctaacatttt gctcaacgtg ccactccatg
-    26881 gcactatttt gaccagaccg cttctagaga gtgaacttgt aatcggagct gtcatccttc
-    26941 gtggacatct tcgtattgct ggacaccatc taggacgctg tgacatcaag gacctgccca
-    27001 aagaaatcac tgttgctaca tcacgaacgc tttcttatta caaattggga gcttcacagc
-    27061 gtgtagcagg tgattcaggt tttgctgcat acagtcgcta caggattgga aactacaaat
-    27121 taaacacaga ccattccagt agcagtgaca atattgcttt gcttgtacag taagtgacaa
-    27181 cagatgtttc atctcgttga ctttcaggtt actatagcag agatattact aattattatg
-    27241 aggactttca aagtttccat ttggaacctt gattacatca taaaccttat aattaaaaat
-    27301 ttatctaagt cactaactga gaataaatat tctcaattag atgaagagca accaatggag
-    27361 attgattaac gaacatgaaa attattcttt tcttggtact ggtaacactt gctacttgtg
-    27421 agctttatca ctaccaagag tgtgttagag gtacaacagt acttctaaaa gaaccttgct
-    27481 cttctggaac gtatgaaggc aattcaccat tccatcctct agctgataat aaatttgcac
-    27541 tgacttgctt tagcactcaa tttgcttttg cttgtcctga cggcgtgaaa cacgtctatc
-    27601 agttacgtgc cagatcagtt tcacccaaac tgttcatcag acaagaggaa gttcaagaac
-    27661 tttactcacc aatttttctt atcattgcag caatagtgtt tataacactt tgcttcacac
-    27721 tcaaaagaaa aacagaatga gtgaactttc attaattgac ttctatttgt gctttttagc
-    27781 ctttctgcta ttccttgttt taattatgct tattatcttt tggttctcac ttgaactgca
-    27841 agatcataat gaaacttgtc acgcctaaac gaacatgaaa cttcttgttt tcttaggaat
-    27901 cctcacaaca gtaactgcat ttcaccaaga atgtagttta cagtcatgtg ctcaacacca
-    27961 accatatgta gttgatgacc cgtgtcctat tcacttctat tctaaatggt acattagagt
-    28021 aggagctaga aaatcagcac ctttaattga attgtgcgtg gatgaggttg gttctaaatc
-    28081 acccattcag tacatcgata tcggcaatta tacagtttcc tgttcacctt ttacaattaa
-    28141 ttgccaggag cctaaattgg gtagtcttgt agtgcgttgt tcgttctatg aagacttttt
-    28201 agagtatcat gacgttcgtg ttgttttaga tttcatctaa acgaacaaac taaaatgtct
-    28261 gataatggac cccaaaacca acgaaatgca ccccgcatta cgtttggtgg accctcagat
-    28321 tcaactggca gtaaccagaa tggagaacgc agtggagcac gaccaaaaca acgtcggcct
-    28381 caaggtttac ccaataatac tgcgtcttgg ttcaccgctc tcactcaaca tggcaaggaa
-    28441 gaccttaaat tccctcgagg acaaggcgtt ccgattaata ccaatagcag tccagatgac
-    28501 caaattggct actaccgaag agctaccaga cgaattcgtg gtggtgacgg taaaatgaaa
-    28561 gatctcagtc caagatggta cttttactac ctaggaactg ggccagaagc tggacttccc
-    28621 tatggtgcta acaaagacgg catcatatgg gttgcaactg agggagcctt gaatacacca
-    28681 aaagatcaca ttggcacccg caatcctgct aacaatgctg caatcgtgct acaacttcct
-    28741 caaggaacaa cattgccaaa aggcttctac gcagaaggga gcagaggtgg cagtcaagct
-    28801 tcttctcgct cttcatcacg tagtcgcaac agttcaagaa actcaactcc aggcagcagt
-    28861 aggggaactt cccctgctag gatggctggc aatggcagtg atgctgctct tgctttgctg
-    28921 ctgcttgaca gattgaacca gcttgagagc aaaatgtctg gtaaaggcca acaacaacag
-    28981 agccaaactg tcactaagaa atctgctgca gaggcttcta agaaacctcg gcaaaaacgt
-    29041 actgccacca aacaatacaa tgtaacacaa gcttttggca gacgtggtcc agaacaaacc
-    29101 caaggaaact ttggggatca agaactaatc aggcaaggaa ctgattacaa acattggccg
-    29161 caaattgcac aattcgctcc cagcgcttca gcattcttcg gaatgtcgcg cattggcatg
-    29221 gaagtcacac cttcgggaac gtggttgacc tatacaggtg ccattaaatt ggatgacaaa
-    29281 gatccaaatt tcaaagatca agtcattttg ctgaataagc acattgacgc atacaaaaca
-    29341 ttcccaccaa cagagcctaa aaaggacaaa aagaaaaagg ctgatgaaac tcaagcctta
-    29401 ccgcagagac agaagaaaca gcaaactgtg actcttcttc ctgctgcaga tttggatgac
-    29461 ttctccaaac aattgcaaca atccatgagc agtgctgatt caactcaggc ctaaactcat
-    29521 gcagaccaca caaggcagat gggctatata aacgttttcg cttttccgtt tacgatatat
-    29581 agtctactct tgtgcagaat gaattctcgt aactacatag cacaagtaga tgtagttaac
-    29641 cttaatctca catagcaatc tttaatcagt gtgtaacatt agggaggact tgaaagagcc
-    29701 accacatttt caccgaggcc acgcggagta cgatcgaggg tacagtgaat aatgctaggg
-    29761 agagctgcct atatggaaga gccctaatgt gtaaaattaa ttttagtagt gctatcccat
-    29821 gtgattttaa tagcttctta ggagaatgac aaaaa
-//
-
 LOCUS       NC_045512              29903 bp ss-RNA     linear   VRL 18-JUL-2020
 DEFINITION  Severe acute respiratory syndrome coronavirus 2 isolate Wuhan-Hu-1,
             complete genome.
 ACCESSION   NC_045512
 VERSION     NC_045512.2
 DBLINK      BioProject: PRJNA485481
 KEYWORDS    RefSeq.
 SOURCE      Severe acute respiratory syndrome coronavirus 2 (SARS-CoV-2)
   ORGANISM  Severe acute respiratory syndrome coronavirus 2
             Viruses; Riboviria; Orthornavirae; Pisuviricota; Pisoniviricetes;
             Nidovirales; Cornidovirineae; Coronaviridae; Orthocoronavirinae;
-            Betacoronavirus; Sarbecovirus.
+            Betacoronavirus; Sarbecovirus; Severe acute respiratory
+            syndrome-related coronavirus.
 REFERENCE   1  (bases 1 to 29903)
   AUTHORS   Wu,F., Zhao,S., Yu,B., Chen,Y.M., Wang,W., Song,Z.G., Hu,Y.,
             Tao,Z.W., Tian,J.H., Pei,Y.Y., Yuan,M.L., Zhang,Y.L., Dai,F.H.,
             Liu,Y., Wang,Q.M., Zheng,J.J., Xu,L., Holmes,E.C. and Zhang,Y.Z.
   TITLE     A new coronavirus associated with human respiratory disease in
             China
   JOURNAL   Nature 579 (7798), 265-269 (2020)
@@ -841,14 +50,15 @@
             Dai,F.-H., Liu,Y., Wang,Q.-M., Zheng,J.-J., Xu,L., Holmes,E.C. and
             Zhang,Y.-Z.
   TITLE     Direct Submission
   JOURNAL   Submitted (05-JAN-2020) Shanghai Public Health Clinical Center &
             School of Public Health, Fudan University, Shanghai, China
 COMMENT     REVIEWED REFSEQ: This record has been curated by NCBI staff. The
             reference sequence is identical to MN908947.
+            
             On Jan 17, 2020 this sequence version replaced NC_045512.1.
             Annotation was added using homology to SARSr-CoV NC_004718.3. ###
             Formerly called 'Wuhan seafood market pneumonia virus.' If you have
             questions or suggestions, please email us at info@ncbi.nlm.nih.gov
             and include the accession number NC_045512.### Protein structures
             can be found at
             https://www.ncbi.nlm.nih.gov/structure/?term=sars-cov-2.### Find
@@ -1977,7 +1187,800 @@
     29641 acaagtagat gtagttaact ttaatctcac atagcaatct ttaatcagtg tgtaacatta
     29701 gggaggactt gaaagagcca ccacattttc accgaggcca cgcggagtac gatcgagtgt
     29761 acagtgaaca atgctaggga gagctgccta tatggaagag ccctaatgtg taaaattaat
     29821 tttagtagtg ctatccccat gtgattttaa tagcttctta ggagaatgac aaaaaaaaaa
     29881 aaaaaaaaaa aaaaaaaaaa aaa
 //
 
+LOCUS       MN996532               29855 bp    RNA     linear   VRL 24-NOV-2020
+DEFINITION  Bat coronavirus RaTG13, complete genome.
+ACCESSION   MN996532
+VERSION     MN996532.2
+KEYWORDS    .
+SOURCE      Bat coronavirus RaTG13
+  ORGANISM  Bat coronavirus RaTG13
+            Viruses; Riboviria; Orthornavirae; Pisuviricota; Pisoniviricetes;
+            Nidovirales; Cornidovirineae; Coronaviridae; Orthocoronavirinae;
+            Betacoronavirus; Sarbecovirus; Severe acute respiratory
+            syndrome-related coronavirus.
+REFERENCE   1  (bases 1 to 29855)
+  AUTHORS   Zhou,P., Yang,X.-L., Wang,X.-G., Hu,B., Zhang,L., Zhang,W.,
+            Si,H.-R., Zhu,Y., Li,B., Huang,C.-L., Chen,H.-D., Chen,J., Luo,Y.,
+            Guo,H., Jiang,R.-D., Liu,M.-Q., Chen,Y., Shen,X.-R., Wang,X.,
+            Zheng,X.-S., Zhao,K., Chen,Q.-J., Deng,F., Liu,L.-L., Yan,B.,
+            Zhan,F.-X., Wang,Y.-Y., Xiao,G.-F. and Shi,Z.-L.
+  TITLE     A pneumonia outbreak associated with a new coronavirus of probable
+            bat origin
+  JOURNAL   Nature 579 (7798), 270-273 (2020)
+  REMARK    DOI: 10.1038/s41586-020-2012-7
+REFERENCE   2  (bases 1 to 29855)
+  AUTHORS   Zhu,Y., Yu,P., Li,B., Hu,B., Si,H.R., Yang,X.L., Zhou,P. and
+            Shi,Z.L.
+  TITLE     Direct Submission
+  JOURNAL   Submitted (27-JAN-2020) CAS Key Laboratory of Special Pathogens,
+            Wuhan Institute of Virology, Center for Biosafety Mega-Science,
+            Chinese Academy of Sciences, No. 44 Xiao Hong Shan, Wuhan, Hubei
+            430071, China
+COMMENT     On Oct 13, 2020 this sequence version replaced MN996532.1.
+            
+            ##Assembly-Data-START##
+            Assembly Method       :: CLC Genomics Workbench v. 12.0
+            Sequencing Technology :: Illumina
+            ##Assembly-Data-END##
+FEATURES             Location/Qualifiers
+     source          1..29855
+                     /organism="Bat coronavirus RaTG13"
+                     /mol_type="genomic RNA"
+                     /isolate="RaTG13"
+                     /isolation_source="fecal swab"
+                     /host="Rhinolophus affinis"
+                     /db_xref="taxon:2709072"
+                     /country="China"
+                     /collection_date="24-Jul-2013"
+                     /note="former lab designation: Bat coronavirus Ra4991"
+     gene            266..21552
+                     /gene="orf1ab"
+     CDS             join(266..13465,13465..21552)
+                     /gene="orf1ab"
+                     /ribosomal_slippage
+                     /codon_start=1
+                     /product="orf1ab polyprotein"
+                     /protein_id="QHR63299.2"
+                     /translation="MESLVPGFNEKTHVQLSLPVLQVRDVLVRGFGDSVEEALSEARQ
+                     HLKDGTCGLVEVEKGVLPQLEQPYVFIKRSDARTAPHGHVMVELVAELNGIQYGRSGE
+                     TLGVLVPYVGETPVVYRKVLLRKNGNKGAGGHSYGADLKSFDLGDELGTDPYEDFQEN
+                     WNTKHSSGVTRDLMRELNGGAYTRYVDNNFCGPDGYPLECIKDLLARAGKASCTLSEQ
+                     LDFIDTKRGVYCCREHEHEIAWYTERSEKSYELQTPFEIKLAKKFDTFNGECPNFVFP
+                     LNSTIKTIQPRVEKKKLDGFMGRIRSVYPVASPNECNQMCLSTLMKCDHCGETSWQTG
+                     DFVKATCEFCGTENLTKEGATTCGYLPQNAVVKIYCPACHNPEVGPEHSLAEYHNESG
+                     LKPILRKGGRTIAFGGCVFSYVGCYNKCAYWIPRASANIGCNHTGVVGEGSEGLNDNL
+                     LEILQKEKVNINIVGDFKLNEEIAIILASFSASTSAFVETVKGLDYKTFKQIVESCGN
+                     FKVTKGKAKKGAWNIGEQKSILSPLYAFASEAARVVRSIFSRTLETAQNSVRALQKAA
+                     ITILDGISQYSLRLIDAMMFTSDLVTNNLVVMAYITGGVVQLTSQWLTNIFGTVYEKL
+                     KPVLDWLEEKFKEGVEFLRDGWEIVKFISTCACEIVGGQIVTCAKEIKESVQTFFKLV
+                     NKFLALCADSIIIGGAKLKALNLGETFVTHSKGLYRKCVKPKEETGLLMPLKAPKEII
+                     FLEGETLPTEVLTEEVVLKTGDLQPLEQPTSEAVEAPLVGTPVCINGLMLLEIKDTEK
+                     YCALAPNMMVTNNTFTLKGGAPTKVTFGDDTVIEVQGYKSVNITFELDERIDKVLNEK
+                     CSTYTVELGTEVNEFACVVADAVIKTLQPVSELLIPLGIDLDEWGMATYYLFDESGEF
+                     KLASHMYCSFYPPDEDEEEGDCEEEDFEPPTQYEYGTEDDYQGKSLEFGATSVTPQPE
+                     EELEEDWLDDDSQQTVVQEDDSEVNQTTITQSIAEVQPQLEMEPTPVVQTEVNSFSGY
+                     LKLTDNVYIKNADIVEEAKKVKPTIVVNAANVYLKHGGGVAGALNKATNNAMQVESDH
+                     YIATNGPLKVGGGCVLSGHNLAKNCLHVVGPNVNRGEDIQLLKSAYENFNQHDVLLAP
+                     LLSAGIFGADPVHSLRVCVDTVRTNVYLAVFDKNLYDKLVSSFLEMKSEKQVEQKTAE
+                     IPKEEVKSSITESKLSVEQRQQVDKKIKACVEEVTTTLEETKFLTENLLLYIDINGNL
+                     HPDSATLVNDIDITFLKKDAPYIVGDVVQEGVLTAVVIPTKKAGGTTEMLTKALRKVP
+                     TDNYITTYPGQGLNGYTVEEARTVLKKCKSAFYILPSIISNEKQEILGTVSWNLREML
+                     AHAEETRKLMPVCMETKAIVSTIQRKYKGIKIQEGVVDYGARFYFYTSKTTVASLINT
+                     LNDLNETLVTMPLGYVTHGLNLEEAARYMRSLKVPATVSVSSPDAVTAYNGYLTSSSK
+                     TPEEHFIETISLAGSYKDWSYSGQSTQLGIEFLKRGDKSVYYTSNPITFHLDGEVITF
+                     DNLKILLSLKEVRTIKVFTTVDNINLHTQVVDMSMTYGQQFGPTYLDGADVTKIKPHN
+                     SHEGKTFYVLPNDDTLRAEAFEYYHTTDPSFLGRYMSALNHTKKWKYPQVNGLTSIKW
+                     ADNNCYLATALLTLQQIELKFNPPALQDAYYRARAGEAANFCALILAYCNKTVGELGD
+                     VRETMNYLFQHANLDSCKRVLNVVCKTCGQQQTTLKGVEAVMYMGTLSYEQLKKGVQI
+                     PCTCGKQATQYLVQQESPFVMMSAPPAQYELKHGTFICASEYTGNYQCGHYKHITSKE
+                     TLYCIDGALLTKSSEYKGPITDIFYKENSYITTIKPVIYKLDGVVCTEIDPKLDNYYK
+                     KDNSYFTEQPIDLVPNQPYPNASFDNFKFVCDNIKLADDLNQLTGYKKPASREFKVTF
+                     FPDLNGDVVAIDYKHYTPSFKKGAKLLHKPIVWHVNNATNKATYKPNTWCIRCLWNTK
+                     PVETSNSFDVLKSEDTQGMDNLACEDLKPVSEEVVENPTIQKDILECNVKTTEVVGDI
+                     ILKPANDGLKITEEVGHTDLMAAYVDNSSLTIKKPNELSRVLGLKTLVTHGLAAVNSV
+                     PWDTIANYAKPFLNKVVSTTTNIVTRCLNRVCTNYMPYFFTLLLQLCTFTRSTNSRIK
+                     ASMPTTIAKNTVKSVGKFCLEASFNYLKSPNFFKLINIIIWFLLLSVCLGSLIYSTAA
+                     LGVLMSNLGMPSYCTGYREGYLNSTNVTTAIYCTGSIPCSVCLSGLDSLDTYPSLETI
+                     QITISSFKWDLTAFGLVAEWFLAYILFTRFFYVLGLAAIMQLFFSYFAVHFISNSWLM
+                     WLIINLVQMAPISAMVRMYIFFASFYYVWKSYVHVVDGCTSSTCMMCYKRNRATRVEC
+                     TTIVNGVRRSFYVYANGGKGFCKLHNWNCVNCDTFCAGSTFISDEVARDLSLQFKRPI
+                     NPTDQSSYIVDSVTVKNGSIHLYFDKAGQKTYERHSLSHFVNLDNLRASNTKGSLPIN
+                     VIVFDGKSKCEESSAKSASVYYSQLMCQPILLLDQALVSDVGDSTEVAVKMFDAYVNT
+                     FSSTFNVPMEKLKTLVATAEAELAKNVSLDNVLSTFISAARQGFVDSDVETKDVVECL
+                     KLSHQSDIEVTGDSCNNYMLTYNKVENMTPRDLGACIDCSARHINAQVAKSHNIALIW
+                     NVKDFMSLSEQLRKQIRSAAKKNNLPFKLTCATTRQVVNVVTTKIALKGGKIVNNWLK
+                     QLIKVTLVFLFVAAIFYLITPVHVMSKHTDFSSEIIGYKAIDGGVTRDIASTDTCFAN
+                     KHADFDTWFSQRGGSYTNDKACPLIAAVITREVGFVVPGLPGTILRTTNGDFLHFLPR
+                     VFSAVGNICYTPSKLIEYTDFATSACVLAAECTIFKDASGKPVPYCYDTNVLEGSVAY
+                     ESLRPDTRYVLMDGSIIQFPNTYLEGSVRVVTTFDSEYCRHGTCERSEAGVCVSTSGR
+                     WVLNNDYYRSLPGVFCGVDAVNLLTNMFTPLIQPIGALDISASIVAGGIVAIVVTCLA
+                     YYFMRFRRAFGEYSHVVAFNTLLFLMSFTVLCLTPVYSFLPGVYSVIYLYLTFYLTND
+                     VSFLAHIQWMVMFTPLVPFWITIVYVICISTKHFYWFFSNYLKRRVVFNGVSFSTFEE
+                     AALCTFLLNKEMYLKLRSDVLLPLTQYNRYLALYNKYKYFSGAMDTTSYREAACCHLA
+                     KALNDFSNSGSDVLYQPPQTSITSAVLQSGFRKMAFPSGKVEGCMVQVTCGTTTLNGL
+                     WLDDVVYCPRHVICTSEDMLNPNYEDLLIRKSNHNFLVQAGNVQLRVIGHSMQNCVLK
+                     LKVDTANTKTPKYKFVRIQPGQTFSVLACYNGSPSGVYQCAMRPNFTIKGSFLNGSCG
+                     SVGFNIDYDCVSFCYMHHMELPTGVHAGTDLEGTFYGPFVDRQTAQAAGTDTTITVNV
+                     LAWLYAAVINGDRWFLNRFTTTLNDFNLVAMKYNYEPLTQDHVDILGPLSAQTGIAVL
+                     DMCASLKELLQNGMNGRTILGSALLEDEFTPFDVVRQCSGVTFQSAVKRTIKGTHHWL
+                     LLTILTSLLVLVQSTQWSLFFFVYENAFLPFAMGIIAMSAFAMMFVKHKHAFLCLFLL
+                     PSLATVAYFNMVYMPASWVMRIMTWLDMVDTSLSGFKLKDCVMYASAVVLLILMTART
+                     VYDDGARRVWTLMNVLTLVYKVYYGNALDQAISMWALIISVTSNYSGVVTTVMFLARG
+                     IVFMCVEYCPIFFITGNTLQCIMLVYCFLGYFCTCYFGLFCLLNRYFRLTLGVYDYLV
+                     STQEFRYMNSQGLLPPKNSIDAFKLNIKLLGVGGKPCIKVATVQSKMSDVKCTSVVLL
+                     SVLQQLRVESSSKLWAQCVQLHNDILLAKDTTEAFEKMVSLLSVLLSMQGAVDINKLC
+                     EEMLDNRATLQAIASEFSSLPSYAAFATAQEAYEQAVANGDSEVVLKKLKKSLNVAKS
+                     EFDRDAAMQRKLEKMADQAMTQMYKQARSEDKRAKVTSAMQTMLFTMLRKLDNDALNN
+                     IINNARDGCVPLNIIPLTTAAKLMVVIPDYNTYKNTCDGTTFTYASALWEIQQVVDAD
+                     SKIVQLSEISMDNSPNLAWPLIVTALRANSAVKLQNNELSPVALRQMSCAAGTTQTAC
+                     TDDNALAYYNTTKGGRFVLALLSDLQDLKWARFPKSDGTGTIYTELEPPCRFVTDTPK
+                     GPKVKYLYFIKGLNNLNRGMVLGSLAATVRLQAGNATEVPANSTVLSFCAFAVDAAKA
+                     YKDYLASGGQPITNCVKMLCTHTGTGQAITVTPEANMDQESFGGASCCLYCRCHIDHP
+                     NPKGFCDLKGKYVQIPTTCANDPVGFTLKNTVCTVCGMWKGYGCSCDQLREPMLQSAD
+                     AQSFLNRVCGVSAARLTPCGTGTSTDVVYRAFDIYNDKVAGFAKFLKTNCCRFQEKDE
+                     DDNLIDSYFVVKRHTFSNYQHEETIYNLLKDCPAVAKHDFFKFRIDGDMVPHISRQRL
+                     TKYTMADLVYALRHFDEGNCDTLREILVTYNCCDDDYFNKKDWYDFVENPDILRVYAN
+                     LGERVRQALLKTVQFCDAMRDAGIVGVLTLDNQDLNGNWYDFGDFIQTTPGSGVPIVD
+                     SYYSLLMPILTLTRALTAESHVDTDLTKPYIKWDLLKYDFTEERLKLFDRYFKYWDQT
+                     YHPNCVNCLDDRCILHCANFNVLFSTVFPPTSFGPLVRKIFVDGVPFVVSTGYHFREL
+                     GVVHNQDVNLHSSRLSFKELLVYAADPAMHAASGNLLLDKRTTCFSVAALTNNVAFQT
+                     VKPGNFNKDFYDFAVSKGFFKEGSSVELKHFFFAQDGNAAISDYDYYRYNLPTMCDIR
+                     QLLFVVEVVDKYFDCYDGGCINANQVIVNNLDKSAGFPFNKWGKARLYYDSMSYEDQD
+                     ALFAYTKRNVIPTITQMNLKYAISAKNRARTVAGVSICSTMTNRQFHQKLLKSIAATR
+                     GATVVIGTSKFYGGWHNMLKTVYSDVENPHLMGWDYPKCDRAMPNMLRIMASLVLARK
+                     HTTCCSLSHRFYRLANECAQVLSEMVMCGGSLYVKPGGTSSGDATTAYANSVFNICQA
+                     VTANVNALLSTDGNKIADKHVRNLQHRLYECLYRNRDVDTDFVNEFYAYLRKHFSMMI
+                     LSDDAVVCFNSTYASQGLVASIKNFKSVLYYQNNVFMSEAKCWTETDLTKGPHEFCSQ
+                     HTMLVKQGDDYVYLPYPDPSRILGAGCFVDDIVKTDGTLMIERFVSLAIDAYPLTKHP
+                     NQEYADVFHLYLQYIRKLHDELTGHMLDMYSVMLTNDNTSRYWEPEFYEAMYTPHTVL
+                     QAVGACVLCNSQTSLRCGACIRRPFLCCKCCYDHVISTSHKLVLSVNPYVCNAPGCDV
+                     TDVTQLYLGGMSYYCKSHKPPISFPLCANGQVFGLYKNTCVGSDNVTDFNAIATCDWT
+                     NAGDYILANTCTERLKLFAAETLKATEETFKLSYGIATVREVLSDRELHLSWEVGKPR
+                     PPLNRNYVFTGYRVTKNSKVQIGEYTFEKGDYGDAVVYRGTTTYKLNVGDYFVLTSHT
+                     VMPLSAPTLVPQEHYVRITGLYPTLNISDEFSSNVANYQKVGMQKYSTLQGPPGTGKS
+                     HFAIGLALYYPSARIVYTACSHAAVDALCEKALKYLPIDKCSRIIPARARVECFDKFK
+                     VNSTLEQYVFCTVNALPETTADIVVFDEISMATNYDLSVVNARLRAKHYVYIGDPAQL
+                     PAPRTLLTKGTLEPEYFNSVCRLMKTIGPDMFLGTCRRCPAEIVDTVSALVYDNKLKA
+                     HKDKSAQCFKMFYKGVITHDVSSAINRPQIGVVREFLTRNPTWRKAVFISPYNSQNAV
+                     ASKILGLPTQTVDSSQGSEYDYVIFTQTTETAHSCNVNRFNVAITRAKVGILCIMSDR
+                     DLYDKLQFTSLEIPRRNVATLQAENVTGLFKDCSKVITGLHPTQAPTHLSVDTKFKTE
+                     GLCVDIPGIPKDMTYRRLISMMGFKMNYQVNGYPNMFITREEAVRHVRAWIGFDVEGC
+                     HATREAIGTNLPLQLGFSTGVNLVAVPTGYVDTPNNTDFSRVSAKPPPGDQFKHLIPL
+                     MYKGLPWNVVRIKIVQMLSDTLKNLSDRVVFVLWAHGFELTSMKYFVKIGPERTCCLC
+                     DKRATCFSTASDTYACWHHSIGFDYVYNPFMIDVQQWGFTGNLQSNHDLYCQVHGNAH
+                     VASCDAIMTRCLAVHECFVKRVDWTIEYPIIGDELKINAACRKVQHMVVKAALLADKF
+                     PVLHDIGNPKAIKCVPQADVEWKFYDAQPCSDKAYKIEELFYSYATHSDKFTDGVCLF
+                     WNCNVDRYPANSIVCRFDTRVLSNLNLPGCDGGSLYVNKHAFHTPAFDKSAFVNLKQL
+                     PFFYYSDSPCESHGKQVVSDIDYVPLKSATCITRCNLGGAVCRHHANEYRLYLDAYNM
+                     MISAGFSLWVYKQFDTYNLWNTFTRLQSLENVAFNVVNKGHFDGQQGEVPVSIINNTV
+                     YTKVDGVDVELFENKTTLPVNVAFELWAKRNIKPVPEVKILNNLGVDIAANTVIWDYK
+                     RDAPAHISTIGVCSMTDIAKKPTENICAPLTVFFDGRVNGQVDLFRNARNGVLITEGS
+                     VKGLQPSVGPKQASLNGVTLIGEALKTQFNYYKKVNGVVQQLPETYFTQSRNLKEFKP
+                     RSQMEIDFLELAMDEFIERYKLEGYAFEHIVYGDFSHRQLGGLHLLIGLAKRSKESPL
+                     ELEDFIPMDSTVKNYFITDAQTGSSKCVCSVIDLLLDDFVEIIKSQDLSVVSKVVKVT
+                     IDYTEISFMLWCKDGHVETFYPKLQSSQAWQPGVAMPNLYKMQRMLLEKCDLQNYGDS
+                     ATLPKGIMMNVAKYTQLCQYLNTLTLAVPYNMRVIHFGAGSDKGVAPGTAVLRQWLPT
+                     GTLLVDSDLNDFVSDADSTLIGDCATVHTANKWDLIISDMYDPKTKNVTKENDSKEGF
+                     FTYICGFIQQKLALGGSVAIKITEHSWNADLYKLMGHFAWWTAFVTNVNASSSEAFLI
+                     GCNYLGKPREQIDGYVMHANYIFWRNTNPIQLSSYSLFDMSKFPLKLRGTAVMSLKEG
+                     QINDMILSLLSKGRLIIRENNRVVISSDVLVNN"
+     gene            21560..25369
+                     /gene="S"
+     CDS             21560..25369
+                     /gene="S"
+                     /codon_start=1
+                     /product="spike glycoprotein"
+                     /protein_id="QHR63300.2"
+                     /translation="MFVFLVLLPLVSSQCVNLTTRTQLPPAYTNSSTRGVYYPDKVFR
+                     SSVLHLTQDLFLPFFSNVTWFHAIHVSGTNGIKRFDNPVLPFNDGVYFASTEKSNIIR
+                     GWIFGTTLDSKTQSLLIVNNATNVVIKVCEFQFCNDPFLGVYYHKNNKSWMESEFRVY
+                     SSANNCTFEYVSQPFLMDLEGKQGNFKNLREFVFKNIDGYFKIYSKHTPINLVRDLPP
+                     GFSALEPLVDLPIGINITRFQTLLALHRSYLTPGDSSSGWTAGAAAYYVGYLQPRTFL
+                     LKYNENGTITDAVDCALDPLSETKCTLKSFTVEKGIYQTSNFRVQPTDSIVRFPNITN
+                     LCPFGEVFNATTFASVYAWNRKRISNCVADYSVLYNSTSFSTFKCYGVSPTKLNDLCF
+                     TNVYADSFVITGDEVRQIAPGQTGKIADYNYKLPDDFTGCVIAWNSKHIDAKEGGNFN
+                     YLYRLFRKANLKPFERDISTEIYQAGSKPCNGQTGLNCYYPLYRYGFYPTDGVGHQPY
+                     RVVVLSFELLNAPATVCGPKKSTNLVKNKCVNFNFNGLTGTGVLTESNKKFLPFQQFG
+                     RDIADTTDAVRDPQTLEILDITPCSFGGVSVITPGTNASNQVAVLYQDVNCTEVPVAI
+                     HADQLTPTWRVYSTGSNVFQTRAGCLIGAEHVNNSYECDIPIGAGICASYQTQTNSRS
+                     VASQSIIAYTMSLGAENSVAYSNNSIAIPTNFTISVTTEILPVSMTKTSVDCTMYICG
+                     DSTECSNLLLQYGSFCTQLNRALTGIAVEQDKNTQEVFAQVKQIYKTPPIKDFGGFNF
+                     SQILPDPSKPSKRSFIEDLLFNKVTLADAGFIKQYGDCLGDIAARDLICAQKFNGLTV
+                     LPPLLTDEMIAQYTSALLAGTITSGWTFGAGAALQIPFAMQMAYRFNGIGVTQNVLYE
+                     NQKLIANQFNSAIGKIQDSLSSTASALGKLQDVVNQNAQALNTLVKQLSSNFGAISSV
+                     LNDILSRLDKVEAEVQIDRLITGRLQSLQTYVTQQLIRAAEIRASANLAATKMSECVL
+                     GQSKRVDFCGKGYHLMSFPQSAPHGVVFLHVTYVPAQEKNFTTAPAICHDGKAHFPRE
+                     GVFVSNGTHWFVTQRNFYEPQIITTDNTFVSGSCDVVIGIVNNTVYDPLQPELDSFKE
+                     ELDKYFKNHTSPDVDLGDISGINASVVNIQKEIDRLNEVAKNLNESLIDLQELGKYEQ
+                     YIKWPWYIWLGFIAGLIAIIMVTIMLCCMTSCCSCLKGCCSCGSCCKFDEDDSEPVLK
+                     GVKLHYT"
+     gene            25378..26205
+                     /gene="NS3"
+     CDS             25378..26205
+                     /gene="NS3"
+                     /codon_start=1
+                     /product="nonstructural protein NS3"
+                     /protein_id="QHR63301.1"
+                     /translation="MDLFMRIFTLGTVTLKQGEIKDATPSDSVRATATIPIQASLPFG
+                     WLIVGVAFLAVFQSASKIITLKKRWQLALSKGIHFICNLLLLFVTVYSHLLLVAAGLE
+                     APFLYLYALVYFLQSINFVRIIMRLWLCWKCRSKNPLLYDANYFLCWHTNCYDYCIPY
+                     NSVTSSIVITSGDGTTSPISEHDYQIGGYTEKWESGVKDCVVLHSYFTSDYYQLYSTQ
+                     LSTDTGVEHVTFFIYNKIVDEPEEHVQIHTIDGSSGVVNPAMEPIYDEPTTTTSVPL"
+     gene            26230..26457
+                     /gene="E"
+     CDS             26230..26457
+                     /gene="E"
+                     /codon_start=1
+                     /product="envelope protein"
+                     /protein_id="QHR63302.1"
+                     /translation="MYSFVSEETGTLIVNSVLLFLAFVVFLLVTLAILTALRLCAYCC
+                     NIVNVSLVKPSFYVYSRVKNLNSSRVPDLLV"
+     gene            26508..27173
+                     /gene="M"
+     CDS             26508..27173
+                     /gene="M"
+                     /codon_start=1
+                     /product="membrane protein"
+                     /protein_id="QHR63303.1"
+                     /translation="MADNGTITVEELKKLLEQWNLVIGFLFLTWICLLQFAYANRNRF
+                     LYIIKLIFLWLLWPVTLACFVLAAVYRINWITGGIAIAMACLVGLMWLSYFIASFRLF
+                     ARTRSMWSFNPETNILLNVPLHGTILTRPLLESELVIGAVILRGHLRIAGHHLGRCDI
+                     KDLPKEITVATSRTLSYYKLGASQRVAGDSGFAAYSRYRIGNYKLNTDHSSSSDNIAL
+                     LVQ"
+     gene            27184..27369
+                     /gene="NS6"
+     CDS             27184..27369
+                     /gene="NS6"
+                     /codon_start=1
+                     /product="nonstructural protein NS6"
+                     /protein_id="QHR63304.1"
+                     /translation="MFHLVDFQVTIAEILLIIMRTFKVSIWNLDYIINLIIKNLSKSL
+                     TENKYSQLDEEQPMEID"
+     gene            27375..27740
+                     /gene="NS7a"
+     CDS             27375..27740
+                     /gene="NS7a"
+                     /codon_start=1
+                     /product="nonstructural protein NS7a"
+                     /protein_id="QHR63305.1"
+                     /translation="MKIILFLVLVTLATCELYHYQECVRGTTVLLKEPCSSGTYEGNS
+                     PFHPLADNKFALTCFSTQFAFACPDGVKHVYQLRARSVSPKLFIRQEEVQELYSPIFL
+                     IIAAIVFITLCFTLKRKTE"
+     gene            27737..27868
+                     /gene="NS7b"
+     CDS             27737..27868
+                     /gene="NS7b"
+                     /codon_start=1
+                     /product="nonstructural protein NS7b"
+                     /protein_id="QHR63306.1"
+                     /translation="MSELSLIDFYLCFLAFLLFLVLIMLIIFWFSLELQDHNETCHA"
+     gene            27875..28240
+                     /gene="NS8"
+     CDS             27875..28240
+                     /gene="NS8"
+                     /codon_start=1
+                     /product="nonstructural protein NS8"
+                     /protein_id="QHR63307.1"
+                     /translation="MKLLVFLGILTTVTAFHQECSLQSCAQHQPYVVDDPCPIHFYSK
+                     WYIRVGARKSAPLIELCVDEVGSKSPIQYIDIGNYTVSCSPFTINCQEPKLGSLVVRC
+                     SFYEDFLEYHDVRVVLDFI"
+     gene            28255..29514
+                     /gene="N"
+     CDS             28255..29514
+                     /gene="N"
+                     /codon_start=1
+                     /product="nucleocapsid protein"
+                     /protein_id="QHR63308.1"
+                     /translation="MSDNGPQNQRNAPRITFGGPSDSTGSNQNGERSGARPKQRRPQG
+                     LPNNTASWFTALTQHGKEDLKFPRGQGVPINTNSSPDDQIGYYRRATRRIRGGDGKMK
+                     DLSPRWYFYYLGTGPEAGLPYGANKDGIIWVATEGALNTPKDHIGTRNPANNAAIVLQ
+                     LPQGTTLPKGFYAEGSRGGSQASSRSSSRSRNSSRNSTPGSSRGTSPARMAGNGSDAA
+                     LALLLLDRLNQLESKMSGKGQQQQSQTVTKKSAAEASKKPRQKRTATKQYNVTQAFGR
+                     RGPEQTQGNFGDQELIRQGTDYKHWPQIAQFAPSASAFFGMSRIGMEVTPSGTWLTYT
+                     GAIKLDDKDPNFKDQVILLNKHIDAYKTFPPTEPKKDKKKKADETQALPQRQKKQQTV
+                     TLLPAADLDDFSKQLQQSMSSADSTQA"
+ORIGIN      
+        1 attaaaggtt tatacctttc caggtaacaa accaacgaac tctcgatctc ttgtagatct
+       61 gttctctaaa cgaactttaa aatctgtgtg actgtcactc ggctgcatgc ttagtgcact
+      121 cacgcagtat aattaataac taattactgt cgttgacagg acacgagtaa ctcatctatc
+      181 ttctgcaggt tgcttacggt ttcgtccgtg ttgcagccga tcatcagcac atctaggttt
+      241 cgtccgggtg tgaccgaaag gtaagatgga gagccttgtc cctggtttca acgagaaaac
+      301 acacgtccaa ctcagtttgc ctgtcttaca ggttcgcgac gtgctcgtac gtggctttgg
+      361 agactccgtg gaggaggctt tatcagaggc acgtcaacat cttaaagatg gcacttgtgg
+      421 cttagtagaa gttgaaaaag gtgttttgcc tcaacttgaa cagccctatg tgttcatcaa
+      481 acgttctgat gctcgaactg cacctcatgg ccatgttatg gttgagctgg tagcagaact
+      541 taatggcatt cagtatggtc gtagtggtga gacactcggt gtccttgtcc cttatgtggg
+      601 cgaaacacca gtggtttacc gcaaggttct tcttcgtaag aacggtaata aaggagctgg
+      661 tggccatagt tacggcgctg atctaaagtc gtttgactta ggcgacgagc ttggcactga
+      721 tccttatgaa gattttcaag aaaactggaa cactaaacat agcagtggtg tcacccgtga
+      781 tctcatgcgt gagcttaatg gaggagcata cactcgctat gtcgataaca acttctgtgg
+      841 ccctgatggc taccctcttg agtgcattaa agaccttcta gctcgtgctg gtaaagcttc
+      901 atgcactttg tccgaacaac tggactttat tgacactaaa agaggtgtat actgctgtcg
+      961 tgaacatgag catgagattg cttggtacac ggaacgttct gaaaagagct atgaattgca
+     1021 gacacctttt gaaattaaat tggcaaagaa atttgacaca tttaatgggg aatgtccaaa
+     1081 ttttgtattc cccctaaatt ccacaatcaa gactattcaa ccaagggttg aaaagaaaaa
+     1141 gcttgatggc tttatgggta gaattcgatc tgtctatcca gttgcttcac caaatgaatg
+     1201 caaccaaatg tgcctttcaa ctctcatgaa gtgtgatcat tgtggtgaaa cttcatggca
+     1261 gacaggcgat tttgttaaag ccacttgtga attttgtggc actgaaaatt tgactaaaga
+     1321 gggtgccact acttgtggtt acctacccca aaatgctgtt gtcaaaattt attgtccagc
+     1381 atgtcataat ccagaagtag gacctgagca tagtcttgct gaatatcata atgaatctgg
+     1441 cttgaaaccc attcttcgta agggtggtcg cactattgct tttggaggct gtgtgttctc
+     1501 ctatgttggt tgctacaata agtgtgccta ttggattcca cgtgctagcg ccaacatagg
+     1561 ttgcaatcat acaggtgttg ttggagaagg ttctgaaggt cttaatgata accttcttga
+     1621 aatacttcaa aaagagaaag tcaacatcaa tattgttggt gactttaaac ttaatgaaga
+     1681 gatcgccatt attttggcat ctttttctgc ttctacaagt gcttttgtgg aaactgtgaa
+     1741 aggtttggat tataaaacat tcaaacaaat tgttgaatcc tgcggtaact ttaaagttac
+     1801 aaaggggaag gcaaagaaag gtgcttggaa cattggtgaa caaaaatcaa tattgagtcc
+     1861 tctttatgca tttgcgtcag aggctgctcg tgttgttcga tcaattttct cccgcactct
+     1921 tgaaactgct caaaattccg tgcgtgcctt acagaaggcc gctataacaa tactagatgg
+     1981 aatttcacag tactcactga gactcattga tgctatgatg ttcacatctg atttggttac
+     2041 taacaatctg gttgtaatgg cttacattac aggtggtgtt gttcagttga cttcacagtg
+     2101 gctaacaaat atctttggca ctgtttatga gaaactcaaa cctgttcttg attggctcga
+     2161 agagaaattc aaggaaggtg tagagtttct tagagatggt tgggaaattg ttaaatttat
+     2221 ctcaacttgt gcttgtgaaa ttgtcggtgg acaaattgtc acctgtgcaa aggaaattaa
+     2281 agagagtgtt cagacattct ttaagcttgt aaacaaattt ttggctttat gtgctgactc
+     2341 catcatcatt ggtggagcta aacttaaagc cttgaattta ggtgaaacat ttgtcacaca
+     2401 ctcaaaggga ttgtatagaa agtgtgttaa acccaaagaa gaaactggct tactcatgcc
+     2461 tctgaaagct ccaaaagaaa ttattttctt agagggagaa acacttccta cagaagtgtt
+     2521 aacagaggaa gttgtcttga aaactggtga tttacaacca ttagaacaac ctactagtga
+     2581 agctgttgaa gccccattgg ttggtacacc agtttgcatt aacgggctca tgttgctcga
+     2641 aattaaagac acagaaaagt actgtgccct tgcacctaat atgatggtaa caaacaatac
+     2701 cttcacactt aaaggcggtg caccaacaaa agttactttt ggtgatgaca ctgtgattga
+     2761 agtgcaaggt tataagagtg tgaatatcac ttttgaactt gacgaaagga ttgataaggt
+     2821 acttaacgag aagtgctcta cctatacagt tgaactcggt acagaagtaa atgagtttgc
+     2881 ttgtgttgta gcagatgctg tcataaaaac tttacaacca gtatctgaat tacttatacc
+     2941 actgggcatt gatttagatg agtggggtat ggctacatac tacttatttg atgagtctgg
+     3001 tgaatttaaa ttggcttcac atatgtactg ttctttttat cctccagatg aggatgagga
+     3061 agaaggtgat tgtgaagaag aagattttga accaccaact caatatgagt atggtactga
+     3121 agatgattac caaggtaaat ctttggaatt tggtgccact tctgtcactc ctcaacctga
+     3181 agaagagcta gaagaagatt ggttagatga tgatagtcaa caaactgtcg ttcaagaaga
+     3241 tgacagtgaa gttaatcaga caactatcac tcaatcaatt gctgaggttc aacctcagtt
+     3301 agagatggaa cctacaccag ttgttcagac tgaagtgaat agctttagtg gttatttaaa
+     3361 acttactgac aatgtataca ttaaaaatgc agacattgtg gaagaagcta aaaaggtaaa
+     3421 accaacaata gttgtcaacg cagccaatgt ttaccttaaa catggaggag gtgttgcggg
+     3481 agctttaaat aaggctacta ataatgccat gcaagttgaa tcagatcatt acatagccac
+     3541 caatggacca cttaaagtgg gtggtggctg tgttttgagt ggacacaatc ttgctaaaaa
+     3601 ctgtcttcat gttgttggtc caaatgttaa cagaggtgaa gatattcaac ttcttaagag
+     3661 tgcttatgaa aattttaatc agcacgatgt tctactcgca ccactattat cagccggtat
+     3721 ttttggtgct gaccctgtac attctttaag agtttgtgta gacactgttc gcacaaatgt
+     3781 ctacctagct gtctttgata aaaatctcta tgacaaactt gtttcaagct ttttagaaat
+     3841 gaagagtgaa aagcaagttg aacaaaagac tgctgaaatt cctaaagagg aagttaagtc
+     3901 atctattact gaaagtaaac tttcagttga gcagagacaa caagttgata agaaaatcaa
+     3961 agcttgtgtt gaagaagtta caacaactct ggaagaaact aagtttctca cagaaaattt
+     4021 gttactctat attgacatta atggcaatct tcatccagat tctgccactc ttgttaatga
+     4081 cattgacatc actttcttaa agaaagatgc tccctatata gtgggtgatg ttgttcaaga
+     4141 gggtgtttta actgctgtag ttatacctac taaaaaggct ggtggtacta ctgaaatgct
+     4201 aacgaaagcc ttgagaaaag tgccaacaga taactatata accacttacc caggccaggg
+     4261 tttaaatggt tatactgtag aagaggcaag gacagtgctt aaaaagtgta aaagtgcctt
+     4321 ttacattcta ccatctatta tctctaatga gaagcaagaa attcttggaa ctgtttcttg
+     4381 gaatttgcga gaaatgcttg cacatgcaga ggaaactcgt aaattaatgc ctgtctgtat
+     4441 ggaaactaaa gctatagttt caactataca gcgtaaatac aagggtatta aaatacaaga
+     4501 gggtgtggtt gattatggtg ccagatttta cttttatacc agtaaaacaa ctgtagcatc
+     4561 acttatcaat acactcaacg atctaaatga gactcttgtt acaatgccac ttggctatgt
+     4621 aacacatggt ttaaatttgg aagaagctgc tcggtatatg agatctctca aagtgccagc
+     4681 tacagtttct gtttcttcac ctgatgctgt tacagcgtat aatggttacc ttacttcttc
+     4741 ttctaaaaca cctgaagaac attttattga aaccatctca cttgctggct cttacaaaga
+     4801 ttggtcctat tctggacagt ctacacaact aggtatagaa tttcttaaga gaggtgataa
+     4861 aagtgtgtat tacactagta accctattac atttcaccta gatggtgaag ttatcacctt
+     4921 tgacaatctt aagatacttc tctctttgaa agaagttagg actattaagg tgtttacaac
+     4981 agtagacaac attaaccttc acacgcaagt tgtggacatg tcaatgacat atggacaaca
+     5041 gtttggccca acttatttgg atggagctga tgttactaaa ataaaacctc ataattcaca
+     5101 tgaaggtaaa acgttttatg ttttgcctaa tgatgacact ttacgtgctg aggcttttga
+     5161 gtactaccac acaactgatc ctagttttct gggtaggtac atgtcagcat taaatcacac
+     5221 taaaaagtgg aaatacccac aagtcaatgg tttaacttct attaaatggg cagataacaa
+     5281 ctgttatctt gccactgcat tattaacact acagcaaata gagttgaaat ttaacccacc
+     5341 tgctttacaa gatgcctact acagggcaag agctggtgaa gctgctaatt tttgtgcact
+     5401 tatcttagcc tactgtaaca agacagtagg tgagttaggt gatgttagag aaacaatgaa
+     5461 ttatttgttt caacatgcca atttagattc ttgcaaaaga gtcttgaatg tggtgtgtaa
+     5521 aacttgtgga caacagcaga ctactcttaa gggtgtagaa gctgttatgt acatgggcac
+     5581 actttcttat gaacaactta agaagggtgt tcagatacct tgtacttgtg gtaaacaagc
+     5641 tacacaatat ctagtacaac aagagtcacc ttttgttatg atgtcggcac cacctgctca
+     5701 gtatgaactt aagcatggta catttatttg tgctagtgag tacactggta attaccagtg
+     5761 tggtcactat aaacatataa cttctaaaga aactttgtat tgcatagacg gtgctttact
+     5821 tacaaagtcc tctgagtaca aaggtcctat tacggatatt ttctacaaag aaaatagcta
+     5881 tataacaacc ataaaaccag ttatttataa attggatggt gttgtttgta cagaaattga
+     5941 tcctaagttg gacaattatt ataagaaaga caattcttat ttcacagagc aaccaattga
+     6001 tcttgtgcca aaccaacctt atccgaatgc aagcttcgat aatttcaagt ttgtatgtga
+     6061 taacatcaaa cttgctgatg atttaaacca gttaactggt tacaagaaac ctgcttcaag
+     6121 agagtttaaa gttacattct tccctgactt aaatggtgat gtggtggcta ttgattataa
+     6181 acactacaca ccttctttta agaaaggagc taaattgtta cataaaccta ttgtctggca
+     6241 tgttaacaat gcaactaaca aagctacgta taaaccaaac acttggtgta tacgctgtct
+     6301 ttggaacaca aaaccagttg aaacatcaaa ctcttttgat gtactgaaat cagaggacac
+     6361 gcagggaatg gataatcttg cctgcgaaga tctaaaacca gtctctgaag aagtagtgga
+     6421 aaatcctacc atacagaaag acattcttga gtgtaatgtg aaaactaccg aagttgtagg
+     6481 agacattata cttaaaccag caaatgatgg tttgaaaatt acagaggagg ttggtcacac
+     6541 agatctaatg gctgcttatg tagacaattc tagtcttact attaagaaac ctaatgaatt
+     6601 atctagagta ctaggtttga aaacccttgt tactcatggt ttagctgctg ttaatagtgt
+     6661 tccgtgggat actatagcta attatgctaa gccttttctt aataaagttg ttagcacaac
+     6721 tactaatata gtcacacggt gtttaaaccg tgtttgtact aattatatgc cttatttctt
+     6781 tactttattg ctacaattgt gtacttttac tagaagtaca aattctagaa ttaaagcatc
+     6841 tatgccgact actatagcaa agaatactgt taagagtgtt ggtaaatttt gcctagaggc
+     6901 ttcatttaat tacctgaagt cacctaattt ttttaaattg attaatatta taatttggtt
+     6961 tttactatta agtgtttgtt taggttcttt aatctactca accgctgctc taggtgtttt
+     7021 aatgtctaat ttaggcatgc cttcttactg tactggctac agagaaggct atttgaactc
+     7081 tactaatgtc actacagcaa tctactgtac tggttctata ccttgtagtg tttgtcttag
+     7141 tggtttagat tctttagata cctatccttc tttagaaact atacaaatta ccatttcatc
+     7201 ttttaaatgg gatttaactg cttttggctt agttgcagag tggtttttgg catatattct
+     7261 ttttactagg ttcttctatg tacttggatt ggctgcaatt atgcaattgt ttttcagcta
+     7321 ttttgcagta cattttatta gtaattcttg gcttatgtgg ttaataatta atcttgtaca
+     7381 aatggcccca atttcagcta tggttaggat gtacattttc tttgcatcat tttattatgt
+     7441 atggaaaagt tatgtgcatg ttgtagatgg ttgtacttca tcaacttgta tgatgtgtta
+     7501 caaacgtaat agagcaacaa gagttgaatg tacaactatt gttaatggtg ttagaaggtc
+     7561 cttttatgtc tatgctaatg gaggtaaagg cttttgcaaa ctacataatt ggaattgtgt
+     7621 taattgtgac acattctgtg ctggtagtac atttattagt gatgaagttg cgagagactt
+     7681 gtcactacag tttaaaagac caataaatcc tactgaccag tcttcctaca ttgttgacag
+     7741 tgttacagtg aagaatggtt ccatccatct ttactttgat aaagctggtc aaaagactta
+     7801 tgaaagacat tctctctctc attttgttaa cttagacaat ttgagagcta gtaacactaa
+     7861 aggttcattg cctattaatg ttatagtttt tgatggtaaa tcaaaatgtg aagaatcatc
+     7921 tgcaaaatca gcgtctgttt attacagtca gcttatgtgt caacctatac tgttactaga
+     7981 tcaggcatta gtgtctgatg ttggtgatag tacagaagtt gcagttaaaa tgtttgatgc
+     8041 ttacgttaat acgttttcat caacttttaa cgttccaatg gaaaaactaa aaacactagt
+     8101 tgcaactgca gaagctgaac ttgcaaagaa tgtgtcctta gacaatgtct tatccacctt
+     8161 tatttcagca gctcggcaag ggtttgttga ttcagatgta gaaactaaag atgttgttga
+     8221 atgtcttaaa ttgtcacatc aatctgacat agaagttact ggtgatagtt gtaataacta
+     8281 tatgctcacc tataacaaag ttgaaaacat gacacctcgt gaccttggtg cttgtattga
+     8341 ctgtagtgcg cgtcatatta atgcgcaggt agcaaaaagt cacaatattg cgttgatatg
+     8401 gaacgttaaa gattttatgt cactgtctga acaactacga aaacaaatac gtagtgctgc
+     8461 caaaaagaac aacttgcctt tcaagttgac atgtgcaact actagacaag ttgttaatgt
+     8521 tgtaacaaca aaaatagcac ttaagggtgg taaaattgtt aataattggt tgaagcagtt
+     8581 aattaaagtt acactcgtgt tcctttttgt tgctgctatc ttctatttaa taacacctgt
+     8641 tcatgtcatg tctaaacata ctgacttttc aagtgaaatt atagggtaca aggctatcga
+     8701 tggtggtgtc actcgtgaca tagcatctac agatacttgt tttgctaaca aacatgctga
+     8761 ttttgacaca tggtttagtc agcgtggtgg tagttatact aatgacaaag cttgtccatt
+     8821 gattgctgca gtcataacaa gagaagtggg ttttgtcgtg cctggtcttc ctggtacgat
+     8881 attacgcaca actaatggtg actttttgca tttcttacct agagttttta gtgcagttgg
+     8941 taacatctgc tatacaccat caaaacttat agagtacact gactttgcaa cttcagcttg
+     9001 tgttttggct gctgaatgta caatttttaa agatgcttct ggtaagccag taccatattg
+     9061 ttatgatact aatgtactag aaggttctgt tgcatatgaa agtctacgtc ctgatacacg
+     9121 ttatgtactc atggatggct ctattattca atttcctaac acctaccttg aaggttctgt
+     9181 tagagtggta acaacttttg attctgagta ttgtagacac ggtacttgtg aaagatcaga
+     9241 agctggtgtt tgtgtatcta ctagtggtag atgggtactt aataatgatt attacagatc
+     9301 tttaccagga gttttttgtg gtgtagatgc tgtaaattta cttactaata tgttcacacc
+     9361 actaattcaa cctatcggtg ctttggacat atcagcatct attgtagccg gcggtattgt
+     9421 tgctatcgta gtaacatgcc ttgcctacta ctttatgagg tttagaagag cttttggtga
+     9481 atacagccat gtagttgcct ttaatacttt actattcctt atgtcattca ctgtactctg
+     9541 tttaacacca gtttactcat ttttacctgg cgtttattct gttatttact tgtacttgac
+     9601 attttatctt actaatgatg tttctttctt agcacatatc cagtggatgg ttatgttcac
+     9661 acctttagta cctttctgga taacaattgt ttatgtcatt tgtatttcca caaagcattt
+     9721 ttactggttc tttagtaact acctaaaaag gcgtgtagtc tttaatggtg tttcctttag
+     9781 tacttttgaa gaagctgcgt tatgcacttt cttattaaat aaggaaatgt atctaaaatt
+     9841 gcgtagtgat gtacttctac ctcttacgca atataataga tatttagccc tttataataa
+     9901 gtacaagtat tttagtggag ccatggatac aactagctac agagaagctg cttgttgtca
+     9961 tcttgcaaaa gctctcaatg atttcagtaa ttcaggttct gatgttcttt atcaaccacc
+    10021 acaaacctct atcacctcgg ctgttttgca gagtggtttt agaaaaatgg cattcccatc
+    10081 aggtaaagtt gagggttgca tggtacaagt tacttgtggt acaaccacac ttaatggtct
+    10141 ttggcttgat gatgtagtct actgtccaag acatgtgatc tgcacctctg aagacatgct
+    10201 taatcctaat tatgaagact tacttatccg caagtctaat cataatttct tggtacaggc
+    10261 tggtaatgtc caacttagag ttattggaca ttctatgcaa aattgtgtgc ttaagcttaa
+    10321 ggtagatact gccaatacta agacgcctaa gtataagttt gttcgcattc aacctggaca
+    10381 gactttttca gtgttagctt gttacaatgg ttcaccatct ggtgtttacc agtgtgctat
+    10441 gagacctaac tttacaatta agggttcatt ccttaatggt tcttgtggta gtgttggttt
+    10501 taacatagat tatgactgtg tctctttttg ttacatgcac catatggaat taccaactgg
+    10561 agttcatgct ggcacagact tagaaggtac cttctatgga ccttttgttg acagacaaac
+    10621 agcacaagca gctggtacgg acacaactat cacagtcaat gttttagctt ggttgtacgc
+    10681 tgctgttata aatggagaca ggtggtttct caatcgattt accacaactc ttaatgattt
+    10741 taacctcgtg gctatgaagt acaattatga acctctaaca caggaccatg ttgacatact
+    10801 aggacctctt tctgctcaaa ccggaattgc cgttttagat atgtgtgctt cactaaaaga
+    10861 attactgcaa aatggtatga atggacgtac catattgggt agtgctttat tagaagatga
+    10921 atttacacct tttgatgttg ttagacaatg ctcaggtgtt actttccaaa gtgcagtaaa
+    10981 aagaacaatc aagggcacac accattggtt gttacttaca attttgactt cacttttagt
+    11041 tttagtccag agtactcaat ggtctttgtt cttttttgtg tatgaaaatg cctttttgcc
+    11101 ttttgctatg ggtattattg ctatgtctgc ttttgcaatg atgtttgtta aacataagca
+    11161 tgcattcctc tgtttgttct tgttaccttc tcttgctact gtagcttact ttaatatggt
+    11221 ctatatgcct gctagttggg tgatgcgcat tatgacatgg ttggatatgg ttgatactag
+    11281 tttgtctggt ttcaagctaa aagactgtgt tatgtatgca tcagccgtag tgttactaat
+    11341 ccttatgaca gcaagaactg tgtatgatga tggtgctagg agggtgtgga cacttatgaa
+    11401 tgtcttgaca ctcgtctata aagtttatta tggtaatgct ttagatcaag ctatttccat
+    11461 gtgggctctt ataatctctg ttacttctaa ctactcgggt gtagttacaa ctgtcatgtt
+    11521 cttggccaga ggtattgttt ttatgtgtgt tgagtattgc cctattttct tcataactgg
+    11581 taatacactt cagtgtataa tgctagttta ttgtttctta ggctatttct gtacttgtta
+    11641 ctttggtctc ttttgtttac tcaaccgtta ctttagactg actcttggtg tttatgatta
+    11701 tttggtttcc acacaagagt ttaggtatat gaattcacag ggattgctcc caccaaagaa
+    11761 tagcatagat gcctttaaac tcaacatcaa attgttgggt gttggaggta aaccttgtat
+    11821 taaagtagcc actgtacagt ctaaaatgtc agatgtaaag tgcacgtcag tagtcttact
+    11881 ctcagttttg caacaactta gagtagaatc atcatctaaa ttgtgggctc aatgtgttca
+    11941 gttacacaat gacatactct tagctaaaga tactactgaa gcctttgaaa aaatggtttc
+    12001 actactttct gtcttgcttt ccatgcaggg tgctgtagac ataaacaagc tttgtgaaga
+    12061 aatgcttgac aacagggcaa ccttacaagc tatagcctca gagtttagtt ctcttccatc
+    12121 atatgcagct tttgctaccg ctcaagaagc ttatgagcag gctgttgcta atggtgactc
+    12181 tgaagttgtc cttaaaaagt tgaagaagtc tttgaatgtg gctaaatctg aatttgaccg
+    12241 tgatgcagcc atgcaacgca agttggaaaa gatggctgat caagctatga cccaaatgta
+    12301 taaacaggct agatctgaag acaagagggc aaaagttact agtgctatgc agacaatgct
+    12361 tttcactatg cttagaaagt tggataatga tgcactcaac aacattatca acaatgcaag
+    12421 agatggttgt gttccattga acataatacc tcttacaaca gcagccaaat taatggttgt
+    12481 cataccagac tataacacat ataaaaatac gtgtgatggt acaacattta cttatgcatc
+    12541 ggcattgtgg gaaatccaac aggttgttga tgcagatagt aaaattgttc aacttagtga
+    12601 aattagcatg gacaattcac ctaatttagc atggcctctt attgtaacag ctttaagggc
+    12661 caattctgct gtcaaattac agaataatga gcttagtcct gttgcactac gacagatgtc
+    12721 ttgtgctgcc ggtactacac aaactgcttg cactgatgac aatgcgttag cttactacaa
+    12781 cacaacaaag ggaggtaggt ttgtacttgc attgttatcc gatttacagg atttgaaatg
+    12841 ggctagattc cctaagagtg atggaactgg tactatctat acagaactgg aaccaccttg
+    12901 taggtttgtt acagacacac ctaaaggtcc taaagtgaag tatttatact ttattaaagg
+    12961 attaaacaat ctaaatagag gtatggtact tggtagttta gctgctacag tacgtttaca
+    13021 agctggtaat gcaacagaag tgcctgccaa ttcaactgta ctatctttct gtgcttttgc
+    13081 tgtagatgcc gctaaagcgt acaaagacta tctagctagt gggggacaac caatcactaa
+    13141 ttgtgttaag atgttgtgta cacacactgg tactggtcag gcaataacag ttacaccaga
+    13201 agccaatatg gatcaagaat cctttggtgg tgcatcgtgt tgtctgtact gtcgttgcca
+    13261 catagatcat ccaaatccta aaggattttg tgacttaaaa ggtaagtatg tacaaatacc
+    13321 tacgacttgt gctaatgacc ctgtgggttt tacacttaaa aacacagtct gtaccgtctg
+    13381 cggtatgtgg aaaggttatg gctgtagttg tgatcaactc cgcgaaccca tgcttcagtc
+    13441 agctgatgca caatcgtttt taaacgggtt tgcggtgtaa gtgcagcccg tcttacaccg
+    13501 tgcggcacag gcactagcac tgatgtcgtg tacagggctt ttgacatcta caatgataaa
+    13561 gtagctggtt ttgctaaatt cttaaaaact aattgttgtc gcttccaaga aaaagacgag
+    13621 gatgacaatt taattgattc ttactttgta gttaagagac acactttctc taactaccaa
+    13681 catgaagaaa caatttataa tttacttaag gattgtccag ctgttgctaa acacgacttc
+    13741 tttaagttta gaatagacgg tgacatggta ccacatatat cacgtcaacg tcttactaaa
+    13801 tacacaatgg cagacctcgt ctatgcttta aggcattttg acgaaggcaa ttgtgataca
+    13861 ttaagagaaa tacttgtcac atacaattgt tgtgacgatg attatttcaa taaaaaagac
+    13921 tggtatgatt ttgtagaaaa cccagatata ttacgcgtat acgccaactt aggtgaacgt
+    13981 gtacgccaag ctttgttaaa aacagtacaa ttctgtgatg ccatgcgaga tgctggtatt
+    14041 gtaggtgtac taacattaga taatcaagat ctcaatggta actggtatga tttcggtgac
+    14101 ttcatacaaa ccactccagg tagtggagtt cctattgtag attcttatta ttcattgtta
+    14161 atgcctatac taactttaac tagggcatta actgcagagt cacatgttga cactgactta
+    14221 acaaagccct acattaagtg ggatttgtta aaatatgact ttacggaaga gaggttaaaa
+    14281 ctctttgacc gttattttaa atattgggat cagacatacc acccaaattg tgttaactgt
+    14341 ttggatgaca gatgcattct gcattgtgca aactttaacg ttttattctc tacagtgttc
+    14401 ccacctacaa gttttggacc tctagtgaga aaaatatttg ttgatggtgt tccatttgta
+    14461 gtttcaactg gataccactt cagggagcta ggtgttgtac ataatcagga tgtaaactta
+    14521 catagctcta gacttagttt taaggaatta cttgtgtatg ctgctgaccc tgctatgcac
+    14581 gctgcttctg gtaatttatt actagataaa cgcactacgt gcttctcagt agctgcactt
+    14641 actaacaatg ttgcttttca aactgtcaaa cccggtaatt ttaacaaaga cttctatgac
+    14701 tttgctgtgt ctaagggttt ctttaaggaa ggaagttctg ttgaattaaa acacttcttc
+    14761 tttgctcagg atggtaatgc tgccatcagc gattatgact actatcgtta taatctacca
+    14821 acaatgtgtg atatcagaca actcctattt gtagttgaag ttgttgataa gtactttgat
+    14881 tgttacgatg gtggctgtat taatgctaac caagtcatcg tcaacaacct agacaaatca
+    14941 gctggttttc catttaataa atggggtaag gctagactct attacgattc aatgagttac
+    15001 gaggatcaag atgcactttt cgcatataca aaacgtaatg tcatccctac tataactcaa
+    15061 atgaatctta agtatgccat tagtgcaaag aatagagctc gcaccgtagc tggtgtctct
+    15121 atctgtagta ctatgaccaa tagacagttt catcaaaaat tattgaaatc aatagccgcc
+    15181 actagaggag ctactgtagt aatcggaaca agcaaatttt atggtggttg gcataacatg
+    15241 ttaaaaactg tttacagtga tgtagaaaac cctcatctta tgggttggga ttaccctaaa
+    15301 tgtgatagag ccatgcctaa catgcttaga attatggcct cacttgttct tgctcgcaaa
+    15361 catacaacgt gctgtagctt gtcacaccgt ttctatagat tagctaatga gtgtgctcaa
+    15421 gtattgagtg aaatggtcat gtgtggcggt tcactatatg ttaaaccagg tggaacctca
+    15481 tcaggagatg ccacaactgc ttatgctaat agtgtcttta acatttgtca agctgttacg
+    15541 gccaatgtta atgcactttt atctactgat ggtaacaaaa ttgccgataa gcacgtccgc
+    15601 aatttacaac acagacttta tgagtgtctc tatagaaata gagatgttga cacagacttt
+    15661 gtgaatgagt tttacgcata tttgcgtaaa catttctcaa tgatgatact ttctgatgat
+    15721 gctgttgtgt gtttcaatag cacttatgca tctcaaggtc tagtggctag cataaagaac
+    15781 tttaaatcag ttctttacta tcaaaacaac gtttttatgt ctgaagcaaa atgttggact
+    15841 gagactgacc ttactaaagg acctcatgaa ttttgctctc aacatacaat gctagttaaa
+    15901 cagggtgatg attatgtgta cctcccttac ccggatccat cacgaatctt aggggctggc
+    15961 tgttttgtag atgatatcgt aaaaacagat ggtacactga tgattgaacg gtttgtgtct
+    16021 ttagctatag atgcttaccc acttactaaa catcctaatc aggagtatgc tgatgtcttt
+    16081 cacttgtact tacaatacat aagaaagtta catgatgagt taacaggaca tatgttagac
+    16141 atgtattctg ttatgcttac taatgataac acttcaaggt attgggaacc tgagttttat
+    16201 gaggctatgt acacaccgca tacagtctta caggctgttg gggcttgtgt tctttgcaat
+    16261 tcacagactt cattaagatg tggtgcttgc atacgtagac cattcttatg ctgtaaatgc
+    16321 tgttacgacc acgtcatatc tacatcacat aaattagtct tgtctgttaa tccgtatgtt
+    16381 tgcaatgctc caggttgtga tgtcacagat gtgactcaac tttacttagg aggtatgagc
+    16441 tattattgta aatcacataa accacccatt agttttccgt tgtgtgctaa tggacaagtt
+    16501 tttggtttat ataagaatac atgtgttggt agcgataatg ttactgactt taacgcaatt
+    16561 gcaacatgtg attggacaaa tgctggtgat tacattttag ctaacacctg tactgaaaga
+    16621 ctcaagcttt tcgcagcaga aacgctcaaa gctactgagg agacatttaa actgtcttat
+    16681 ggtattgcca ctgtacgtga agtgctgtct gacagagaat tgcatctttc atgggaagtt
+    16741 ggtaaaccta gaccaccact taaccgaaat tatgtcttta ctggttatcg tgtaactaaa
+    16801 aacagtaaag tacaaatagg agagtacacc tttgaaaaag gtgactatgg tgatgctgtt
+    16861 gtctaccgag gtacaacaac ttacaaacta aatgttggtg actattttgt gctgacatca
+    16921 catacagtaa tgccattaag tgcacctaca ctagtgccac aagagcacta tgttagaatt
+    16981 actggcttat acccaacact caatatttca gatgagtttt ctagcaatgt tgcaaattat
+    17041 caaaaggttg gtatgcaaaa gtattctaca ctccaaggac cacctggtac tggtaagagt
+    17101 cattttgcta ttggcttagc tctctactac ccttctgctc gcatagtgta cacagcttgc
+    17161 tctcatgccg ctgttgatgc actatgtgag aaggcattaa aatatttgcc tatagataaa
+    17221 tgtagtagaa ttatacctgc acgtgctcgt gtagagtgtt ttgataaatt caaagtgaat
+    17281 tcaacattag aacagtacgt cttttgtact gtaaatgcat tgcctgagac gactgcagat
+    17341 atagttgtct ttgatgaaat ttcaatggct acaaattatg atttgagtgt tgtcaatgct
+    17401 agattacgtg ctaagcacta tgtgtacatt ggcgaccctg ctcaattacc agcaccacgc
+    17461 acattgctaa ctaagggcac actagaacca gaatatttca attcagtgtg tagactcatg
+    17521 aaaactatag gtccagacat gttccttgga acttgtcggc gttgtcctgc tgaaattgtt
+    17581 gacactgtga gtgctttggt ttatgataat aagctgaaag cacataaaga caaatcagct
+    17641 caatgcttta aaatgtttta taagggtgtt attactcatg atgtttcatc tgcaattaac
+    17701 aggccacaaa taggcgtggt aagagaattt cttacacgta atcctacttg gagaaaagct
+    17761 gtcttcattt caccttataa ttcacagaat gctgtagcct caaagatttt gggactacca
+    17821 actcaaactg ttgattcatc acagggttca gaatatgact atgtcatatt cactcaaacc
+    17881 actgagacag ctcactcttg taatgtaaac agatttaatg ttgctattac tagagcaaaa
+    17941 gtaggcatac tttgcataat gtctgataga gacctttatg acaagttgca atttacaagt
+    18001 cttgagattc cacgtaggaa tgtggcaact ttacaagctg aaaatgtaac aggacttttt
+    18061 aaggattgta gtaaggtaat cactgggtta cacccaacac aggcacctac acacctcagt
+    18121 gttgacacta aattcaaaac tgaaggttta tgtgttgaca tacctggtat acctaaggac
+    18181 atgacctata gaagactcat ctctatgatg ggtttcaaaa tgaattacca agttaatggt
+    18241 taccctaata tgtttatcac ccgtgaggaa gccgtaagac atgtacgtgc atggattggc
+    18301 tttgatgtcg aggggtgtca tgctactaga gaagctattg gtactaattt acctttacag
+    18361 ctaggctttt ctacaggtgt taacctagtt gctgtaccta caggctatgt tgatacacct
+    18421 aataatacag atttttccag agttagtgct aaaccaccac ctggagatca gtttaaacat
+    18481 cttataccac ttatgtataa aggacttcct tggaatgtag tgcgtataaa gattgtacaa
+    18541 atgttaagtg atacacttaa aaatctctct gacagagtcg tgtttgtctt atgggcacat
+    18601 ggctttgaat taacatctat gaagtatttt gtgaaaatag gacctgagcg cacttgttgt
+    18661 ctatgtgata aacgtgccac atgcttttcc actgcttcag acacttatgc ctgttggcat
+    18721 cattctattg gatttgatta tgtctataat ccgtttatga ttgatgttca acaatggggt
+    18781 tttacaggta acctacaaag caaccatgat ctgtattgtc aggttcatgg taatgcacat
+    18841 gtagctagtt gtgatgcaat catgactaga tgtctagctg tccacgagtg ctttgttaag
+    18901 cgtgttgact ggactattga ataccctata attggtgatg aactgaagat taatgcggct
+    18961 tgtagaaagg ttcaacacat ggttgttaaa gctgcattat tagcagacaa atttccagtt
+    19021 cttcatgaca ttggtaaccc taaagctatt aagtgtgtac ctcaagctga tgtagaatgg
+    19081 aagttctatg acgcacagcc ttgtagtgac aaagcttata aaatagaaga attattctat
+    19141 tcttatgcca cacattctga caaattcaca gatggtgtat gcctattttg gaattgcaat
+    19201 gtcgatagat atcctgctaa ttccattgtt tgtagatttg acactagagt gctatctaac
+    19261 cttaacttgc ctggttgtga tggtggcagt ttgtatgtaa ataaacatgc attccacaca
+    19321 ccagcttttg ataaaagtgc ttttgttaat ttaaaacaat taccattttt ctattactct
+    19381 gacagtccat gtgagtctca tggaaaacaa gtagtgtcag atatagacta tgtaccacta
+    19441 aagtctgcta cgtgcataac acgttgcaat ttaggtggtg ctgtctgtag acatcatgct
+    19501 aatgagtaca gattgtatct tgatgcttac aacatgatga tctcagctgg ctttagcttg
+    19561 tgggtttaca aacaatttga tacttacaac ctctggaata cttttacaag acttcagagt
+    19621 ttagaaaatg tggcttttaa tgttgtaaat aaaggacact ttgatggaca acagggtgaa
+    19681 gtaccagttt ccatcattaa taacactgtt tacacaaaag ttgatggtgt tgatgtagaa
+    19741 ctatttgaaa ataaaacaac attacctgtt aatgtagcat ttgagctctg ggctaagcgc
+    19801 aatattaaac cagtaccaga ggtgaaaata ctcaataatt tgggtgtgga cattgctgct
+    19861 aatactgtga tttgggacta caaaagagat gctccagcac atatatctac tattggtgtt
+    19921 tgttctatga ctgacatagc caagaaacca actgaaaata tttgtgcacc actcactgtc
+    19981 tttttcgatg gtagagtcaa tggtcaagta gacttgttta gaaatgcccg taatggtgtt
+    20041 cttattacag aaggtagtgt taaaggttta caaccatctg taggtcctaa acaagccagt
+    20101 cttaatggag tcacattgat tggagaagcc ttaaaaacac agttcaatta ttacaagaaa
+    20161 gttaatggtg ttgttcaaca actacctgaa acttacttta cccaaagtag aaatttaaaa
+    20221 gaattcaaac ccaggagtca aatggaaatt gatttcttag aattagctat ggatgaattc
+    20281 attgaacggt ataaactaga aggttatgcc ttcgaacata tcgtctatgg agattttagt
+    20341 cataggcagt taggtggttt acatctactg attggactag ctaaacgttc taaggaatca
+    20401 cctcttgaat tagaagattt tattcctatg gacagtacag ttaaaaatta cttcataaca
+    20461 gatgcgcaaa caggttcatc taagtgtgtg tgttctgtta ttgatttatt acttgatgat
+    20521 tttgttgaaa taataaaatc gcaggattta tctgtagttt ctaaggtggt caaagtgacc
+    20581 attgactata cagaaatttc atttatgctt tggtgtaaag atggacatgt tgaaacattt
+    20641 tacccaaaat tacaatctag tcaagcgtgg caaccgggtg ttgctatgcc taatctctac
+    20701 aaaatgcaaa gaatgttact agaaaagtgt gaccttcaaa attatggtga tagtgcaaca
+    20761 ttacctaaag gcataatgat gaatgtcgca aaatatactc aactgtgtca gtatttaaat
+    20821 acacttactt tagctgtacc ctataatatg agggttatac attttggtgc tggttctgat
+    20881 aaaggagttg cacctggtac agctgtttta agacagtggt tgcctacggg tacactactt
+    20941 gtcgattcag atcttaatga ctttgtctct gatgcagatt caactttgat tggtgattgt
+    21001 gcaactgtac atacagctaa taaatgggat ctcattatta gtgatatgta cgatcctaag
+    21061 actaaaaatg ttacaaaaga aaatgattcc aaagagggat ttttcactta catttgtgga
+    21121 tttatacaac aaaagctagc ccttggaggt tctgtagcta taaagataac agagcattct
+    21181 tggaatgccg atctttataa gcttatggga catttcgcat ggtggactgc ttttgttact
+    21241 aatgtaaatg catcttcatc tgaagcattt ttaattgggt gtaattacct tggcaaaccg
+    21301 cgtgaacaga tagatggtta tgtcatgcat gcaaattaca tattttggag gaatacaaac
+    21361 ccaattcagt tgtcttccta ttctttattt gacatgagta aattccccct taaattaagg
+    21421 ggtactgcag ttatgtcttt gaaagaaggt caaatcaatg atatgatttt atctcttctt
+    21481 agtaaaggta gacttataat tagagaaaac aatagagttg ttatttctag tgatgttctt
+    21541 gttaacaact aaacgaacca tgtttgtttt tcttgtttta ttgccactag tttctagtca
+    21601 gtgtgttaat ctaacaacta gaactcagtt acctcctgca tacaccaact catccacccg
+    21661 tggtgtctat taccctgaca aagttttcag atcttcagtt ttacatttaa ctcaggattt
+    21721 gtttttacct ttcttctcca atgtgacctg gttccatgct atacatgttt cagggaccaa
+    21781 tggtattaaa aggtttgata acccagttct gccattcaac gatggcgtct attttgcttc
+    21841 cactgagaag tctaatataa taagaggatg gatttttggt actaccttag attcgaagac
+    21901 ccagtctcta cttattgtta ataacgctac taatgttgtt attaaagtct gtgaatttca
+    21961 attttgtaat gatccatttt tgggtgttta ttaccacaaa aacaacaaaa gttggatgga
+    22021 aagtgagttc agagtttact ctagtgcgaa taattgcact tttgagtatg tctctcagcc
+    22081 ttttcttatg gaccttgaag gaaaacaggg taatttcaaa aatcttaggg aattcgtgtt
+    22141 taagaatatt gatggttatt tcaaaatata ttctaaacat acgcctatta atttagtgcg
+    22201 tgatcttccc cctggttttt cagctttaga accattggta gatctgccaa taggtattaa
+    22261 catcactagg tttcaaactt tacttgcttt acatagaagc tatttgactc ctggtgattc
+    22321 ttcttcaggt tggacagctg gtgctgcagc ttattatgtg ggttatcttc aaccaaggac
+    22381 ttttctacta aaatataatg agaatggaac cattacagat gctgtagact gtgcacttga
+    22441 ccctctttca gaaacaaagt gtacgttaaa atccttcact gttgaaaaag gaatttatca
+    22501 aacctctaac tttagagtcc aaccaacaga ttctattgtt agattcccaa atattacaaa
+    22561 cttatgtcct tttggtgaag tttttaacgc caccacattc gcatcagttt atgcttggaa
+    22621 cagaaagaga attagcaact gtgttgctga ttactctgtc ctatataatt ccacttcatt
+    22681 ttctaccttt aaatgttatg gagtgtctcc tactaaatta aatgatctct gctttactaa
+    22741 tgtttatgca gactcatttg tgattacagg tgatgaagtc agacaaattg cgccaggaca
+    22801 aactggaaag attgctgact acaattataa actaccagat gattttactg gttgtgttat
+    22861 agcttggaat tctaagcata ttgatgcaaa agagggcggt aattttaact atctttaccg
+    22921 tctctttaga aaagctaatc ttaaaccctt tgagagggat atctcaactg aaatttacca
+    22981 agcaggcagc aaaccttgta atggtcaaac tggtctaaat tgctactacc cactttatag
+    23041 atatggattt taccctactg atggtgttgg tcaccaacct tatagggtag tagtactttc
+    23101 ttttgaactt ctaaatgcac cagcaactgt ttgtggacct aagaagtcta ctaacttggt
+    23161 taaaaataaa tgtgtcaatt tcaactttaa tggtttaact ggcacaggtg tcctcacaga
+    23221 gtctaataaa aagtttctac ctttccaaca atttggtaga gacattgcag acactactga
+    23281 tgccgtccgt gatccacaga cacttgagat tcttgacatt acaccatgtt cttttggtgg
+    23341 tgtcagtgtt ataacacctg gaacaaatgc ctctaaccag gttgctgttc tttatcagga
+    23401 tgttaactgc acagaagtcc ctgttgctat ccatgcagac caacttactc ccacttggcg
+    23461 tgtttactcc acaggttcta atgtttttca aacacgtgca ggttgtttaa taggggctga
+    23521 acatgtcaat aactcgtatg agtgtgacat acctattggt gcaggaatat gcgccagtta
+    23581 tcagactcaa actaattcac gtagtgtggc cagtcaatct attattgcct acactatgtc
+    23641 acttggtgca gaaaattcag ttgcttattc taataactct attgccatac ctacaaattt
+    23701 tactattagt gtgaccactg aaattctacc tgtgtctatg acaaagacat cggtagactg
+    23761 tacaatgtat atttgtggtg attcaactga gtgcagcaac cttttgttgc aatatggtag
+    23821 tttttgcaca caattaaatc gtgctttaac tggaatagct gttgaacagg acaaaaatac
+    23881 tcaagaagtt tttgctcaag ttaaacaaat ttataagaca ccaccaatta aagattttgg
+    23941 tggtttcaat ttttcacaaa tattaccaga tccatcaaaa ccaagcaaga ggtcatttat
+    24001 tgaggattta cttttcaata aagtgacact tgctgatgct ggcttcatca aacaatatgg
+    24061 tgattgcctt ggtgatattg ctgctaggga tcttatttgt gctcaaaagt tcaatggcct
+    24121 tactgttctg ccacctttgc tcacagatga aatgatcgct caatacactt ctgcactatt
+    24181 agcaggtaca atcacttctg gttggacttt tggtgcaggt gctgctttac aaataccatt
+    24241 tgccatgcaa atggcttata ggtttaatgg tattggagtt acacagaatg ttctctatga
+    24301 gaaccaaaaa ttgattgcca accagtttaa tagtgctatt ggcaaaattc aagactcact
+    24361 ttcttctaca gcaagtgcac ttggaaaact tcaagatgtt gtcaaccaaa atgcacaagc
+    24421 tttaaacacg cttgttaaac aacttagctc caattttgga gctatttcta gcgtgttaaa
+    24481 tgatatcctt tcacgtctcg acaaagttga ggctgaagtg cagattgaca ggttgatcac
+    24541 aggcagactt caaagcttgc agacatatgt gactcaacaa ttaattagag ctgcagaaat
+    24601 cagagcttct gccaatcttg ctgctactaa aatgtcagag tgtgtactcg gacaatcaaa
+    24661 aagagttgat ttttgtggaa aaggctatca tcttatgtct ttccctcagt cagcacctca
+    24721 tggtgtagtc ttcttgcatg tgacatatgt ccctgcacaa gaaaagaact tcacaactgc
+    24781 tcctgccatt tgtcatgatg gaaaagcaca ctttccacgt gaaggtgttt tcgtttcaaa
+    24841 tggcacacac tggtttgtta cacaaaggaa tttttatgaa ccacaaatta ttacaacaga
+    24901 caacacattt gtctctggta gctgtgatgt tgtaatagga attgtcaaca acacagttta
+    24961 tgatcctttg caaccagaac ttgattcatt caaggaggag ttggataaat actttaaaaa
+    25021 tcatacatca cctgatgtag atttaggtga catttctggc attaatgctt cagttgtcaa
+    25081 tattcaaaag gaaattgacc gcctcaatga ggttgccaaa aatctaaatg aatctctcat
+    25141 cgatctccaa gaacttggaa agtatgaaca gtatataaaa tggccatggt acatttggct
+    25201 aggttttata gctggcttga ttgccataat aatggtcacg attatgcttt gctgtatgac
+    25261 cagttgctgc agttgtctca agggctgttg ttcttgcgga tcttgctgca aatttgatga
+    25321 agacgactct gagccagtgc tcaaaggagt caaattacat tacacataaa cgaacttatg
+    25381 gatttgttta tgagaatttt cacacttgga actgtaactt tgaaacaagg tgaaattaag
+    25441 gatgctactc cttcagattc tgttcgcgct actgcaacga taccgataca agcctcactc
+    25501 cctttcggat ggcttattgt tggcgttgca tttcttgctg tttttcaaag cgcttccaag
+    25561 atcataaccc ttaaaaagag atggcaacta gcactctcta agggtattca ctttatttgc
+    25621 aacttgctgc tgctgtttgt aacagtttac tcacatcttt tgctcgttgc tgctggtctt
+    25681 gaagccccat tcctctacct ctacgcttta gtctacttct tgcagagtat aaactttgta
+    25741 agaataataa tgaggctttg gctttgctgg aaatgccgtt ccaaaaaccc attactctat
+    25801 gatgctaact acttcctttg ttggcatact aattgttatg actattgtat accttacaat
+    25861 agtgtaactt cttcaattgt cattacttca ggtgatggca caacaagtcc tatttctgaa
+    25921 catgactacc agattggtgg ttatactgaa aaatgggagt ctggagtaaa agactgtgtt
+    25981 gtattacaca gttacttcac ttcagattat taccagctgt actcaactca attgagcaca
+    26041 gacactggtg ttgaacatgt taccttcttc atctacaata aaattgttga tgagcctgaa
+    26101 gaacatgtcc aaattcacac aatcgacggt tcatccggag ttgttaatcc agcaatggaa
+    26161 ccaatttatg atgaaccgac gacgactact agcgtgcctt tgtaagcaca agctgatgag
+    26221 tacgaactta tgtactcatt cgtttcggaa gagacaggta cgttaatagt taatagcgta
+    26281 cttctttttc ttgctttcgt ggtattcttg ctagtcacac tagccatcct tactgcgctt
+    26341 cgattgtgtg cgtactgctg caatattgtt aacgtgagtc ttgtaaaacc ttctttttac
+    26401 gtttactctc gtgttaaaaa tctgaattct tctagagttc ctgatcttct ggtctaaacg
+    26461 aactaaatat tatattagtt tttctgtttg gaactttaat tttagccatg gcagataacg
+    26521 gtactattac cgttgaagag ctgaaaaagc tccttgaaca gtggaatcta gtaataggat
+    26581 tcctatttct tacatggatt tgtcttctac aatttgccta tgccaacagg aataggtttt
+    26641 tgtatataat taagttaatt ttcctctggc tgctttggcc agtaacttta gcctgctttg
+    26701 tgcttgctgc tgtttacaga ataaattgga tcactggagg aatcgctatc gcaatggctt
+    26761 gtcttgtagg cttgatgtgg ctgagctact tcattgcttc tttcaggcta tttgcacgta
+    26821 cgcgttccat gtggtcattc aatccagaaa ctaacatttt gctcaacgtg ccactccatg
+    26881 gcactatttt gaccagaccg cttctagaga gtgaacttgt aatcggagct gtcatccttc
+    26941 gtggacatct tcgtattgct ggacaccatc taggacgctg tgacatcaag gacctgccca
+    27001 aagaaatcac tgttgctaca tcacgaacgc tttcttatta caaattggga gcttcacagc
+    27061 gtgtagcagg tgattcaggt tttgctgcat acagtcgcta caggattgga aactacaaat
+    27121 taaacacaga ccattccagt agcagtgaca atattgcttt gcttgtacag taagtgacaa
+    27181 cagatgtttc atctcgttga ctttcaggtt actatagcag agatattact aattattatg
+    27241 aggactttca aagtttccat ttggaacctt gattacatca taaaccttat aattaaaaat
+    27301 ttatctaagt cactaactga gaataaatat tctcaattag atgaagagca accaatggag
+    27361 attgattaac gaacatgaaa attattcttt tcttggtact ggtaacactt gctacttgtg
+    27421 agctttatca ctaccaagag tgtgttagag gtacaacagt acttctaaaa gaaccttgct
+    27481 cttctggaac gtatgaaggc aattcaccat tccatcctct agctgataat aaatttgcac
+    27541 tgacttgctt tagcactcaa tttgcttttg cttgtcctga cggcgtgaaa cacgtctatc
+    27601 agttacgtgc cagatcagtt tcacccaaac tgttcatcag acaagaggaa gttcaagaac
+    27661 tttactcacc aatttttctt atcattgcag caatagtgtt tataacactt tgcttcacac
+    27721 tcaaaagaaa aacagaatga gtgaactttc attaattgac ttctatttgt gctttttagc
+    27781 ctttctgcta ttccttgttt taattatgct tattatcttt tggttctcac ttgaactgca
+    27841 agatcataat gaaacttgtc acgcctaaac gaacatgaaa cttcttgttt tcttaggaat
+    27901 cctcacaaca gtaactgcat ttcaccaaga atgtagttta cagtcatgtg ctcaacacca
+    27961 accatatgta gttgatgacc cgtgtcctat tcacttctat tctaaatggt acattagagt
+    28021 aggagctaga aaatcagcac ctttaattga attgtgcgtg gatgaggttg gttctaaatc
+    28081 acccattcag tacatcgata tcggcaatta tacagtttcc tgttcacctt ttacaattaa
+    28141 ttgccaggag cctaaattgg gtagtcttgt agtgcgttgt tcgttctatg aagacttttt
+    28201 agagtatcat gacgttcgtg ttgttttaga tttcatctaa acgaacaaac taaaatgtct
+    28261 gataatggac cccaaaacca acgaaatgca ccccgcatta cgtttggtgg accctcagat
+    28321 tcaactggca gtaaccagaa tggagaacgc agtggagcac gaccaaaaca acgtcggcct
+    28381 caaggtttac ccaataatac tgcgtcttgg ttcaccgctc tcactcaaca tggcaaggaa
+    28441 gaccttaaat tccctcgagg acaaggcgtt ccgattaata ccaatagcag tccagatgac
+    28501 caaattggct actaccgaag agctaccaga cgaattcgtg gtggtgacgg taaaatgaaa
+    28561 gatctcagtc caagatggta cttttactac ctaggaactg ggccagaagc tggacttccc
+    28621 tatggtgcta acaaagacgg catcatatgg gttgcaactg agggagcctt gaatacacca
+    28681 aaagatcaca ttggcacccg caatcctgct aacaatgctg caatcgtgct acaacttcct
+    28741 caaggaacaa cattgccaaa aggcttctac gcagaaggga gcagaggtgg cagtcaagct
+    28801 tcttctcgct cttcatcacg tagtcgcaac agttcaagaa actcaactcc aggcagcagt
+    28861 aggggaactt cccctgctag gatggctggc aatggcagtg atgctgctct tgctttgctg
+    28921 ctgcttgaca gattgaacca gcttgagagc aaaatgtctg gtaaaggcca acaacaacag
+    28981 agccaaactg tcactaagaa atctgctgca gaggcttcta agaaacctcg gcaaaaacgt
+    29041 actgccacca aacaatacaa tgtaacacaa gcttttggca gacgtggtcc agaacaaacc
+    29101 caaggaaact ttggggatca agaactaatc aggcaaggaa ctgattacaa acattggccg
+    29161 caaattgcac aattcgctcc cagcgcttca gcattcttcg gaatgtcgcg cattggcatg
+    29221 gaagtcacac cttcgggaac gtggttgacc tatacaggtg ccattaaatt ggatgacaaa
+    29281 gatccaaatt tcaaagatca agtcattttg ctgaataagc acattgacgc atacaaaaca
+    29341 ttcccaccaa cagagcctaa aaaggacaaa aagaaaaagg ctgatgaaac tcaagcctta
+    29401 ccgcagagac agaagaaaca gcaaactgtg actcttcttc ctgctgcaga tttggatgac
+    29461 ttctccaaac aattgcaaca atccatgagc agtgctgatt caactcaggc ctaaactcat
+    29521 gcagaccaca caaggcagat gggctatata aacgttttcg cttttccgtt tacgatatat
+    29581 agtctactct tgtgcagaat gaattctcgt aactacatag cacaagtaga tgtagttaac
+    29641 cttaatctca catagcaatc tttaatcagt gtgtaacatt agggaggact tgaaagagcc
+    29701 accacatttt caccgaggcc acgcggagta cgatcgaggg tacagtgaat aatgctaggg
+    29761 agagctgcct atatggaaga gccctaatgt gtaaaattaa ttttagtagt gctatcccat
+    29821 gtgattttaa tagcttctta ggagaatgac aaaaa
+//
+
```

### Comparing `bio-1.7.0/src/biorun/__init__.py` & `bio-1.7.1/biorun/__init__.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/align.py` & `bio-1.7.1/biorun/align.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/code.py` & `bio-1.7.1/biorun/code.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/combine.py` & `bio-1.7.1/biorun/combine.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/comm.py` & `bio-1.7.1/biorun/comm.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/convert.py` & `bio-1.7.1/biorun/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -314,15 +314,15 @@
 
 
 def feature2gff(source, ftype, start, end, strand, uid, name, pid=None):
     """
     Returns a Record as an 11 element  GFF3 list .
     """
     # Reformat the strand
-    strand = "+" if strand > 0 else "-"
+    strand = "+" if strand else "-"
 
     # TODO: is this the phase?
     # phase = feat.get("codon_start", [1])[0] - 1
     phase = "."
 
     # The color for the feature.
     color = COLOR_FOR_TYPE.get(ftype)
```

### Comparing `bio-1.7.0/src/biorun/enrichr.py` & `bio-1.7.1/biorun/enrichr.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/fasta.py` & `bio-1.7.1/biorun/fasta.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/fetch.py` & `bio-1.7.1/biorun/fetch.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/format.py` & `bio-1.7.1/biorun/format.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/gff.py` & `bio-1.7.1/biorun/gff.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/gprof.py` & `bio-1.7.1/biorun/gprof.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/gtf.py` & `bio-1.7.1/biorun/gtf.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/jsonrec.py` & `bio-1.7.1/biorun/jsonrec.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/main.py` & `bio-1.7.1/biorun/main.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/mart.py` & `bio-1.7.1/biorun/mart.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/meta.py` & `bio-1.7.1/biorun/meta.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/models.py` & `bio-1.7.1/biorun/models.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/mygene.py` & `bio-1.7.1/biorun/mygene.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 @plac.opt('fields', "fields", abbrev='f')
 @plac.opt('species', "species", abbrev='s')
 @plac.opt('scopes', "scopes", abbrev='S')
 @plac.pos('query', "download limit")
 def run(limit=5, species='', fields='', scopes='symbol', *query):
     limit = int(limit) if limit else None
 
-    fields = ",".join(['symbol', 'name', 'taxid', fields])
+    fields = ",".join(['symbol', 'name', 'taxid', "refseq", fields])
 
     query = ' '.join(query)
 
     execute(query, fields=fields, species=species, scopes=scopes, size=limit)
 
 
 if __name__ == '__main__':
```

### Comparing `bio-1.7.0/src/biorun/ontology.py` & `bio-1.7.1/biorun/ontology.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/parser.py` & `bio-1.7.1/biorun/parser.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/search.py` & `bio-1.7.1/biorun/search.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 GBK = re.compile(r'(?P<letters>[a-zA-Z]+)(?P<under>_?)(?P<digits>\d+)(\.(?P<version>\d+))?')
 
 # ENA API points
 ENA_API = "https://www.ebi.ac.uk/ena/portal/api"
 ENA_FIELDS = f"{ENA_API}/returnFields"
 ENA_REPORT = f"{ENA_API}/filereport"
 
-
 # The assembly summary file
 ASSEMBLY_SUMMARY_URL = 'https://ftp.ncbi.nlm.nih.gov/genomes/ASSEMBLY_REPORTS/assembly_summary_genbank.txt'
 ASSEMBLY_SUMMARY_PATH = "assembly_summary_genbank.txt"
 ASSEMBLY_SUMMARY_PATH = utils.cache_path(ASSEMBLY_SUMMARY_PATH)
 
 
 def match_srr(text):
```

### Comparing `bio-1.7.0/src/biorun/table.py` & `bio-1.7.1/biorun/table.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/taxon.py` & `bio-1.7.1/biorun/taxon.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/test.py` & `bio-1.7.1/biorun/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,14 +84,15 @@
 
     os.chdir(RUN_DIR)
 
     print(f"# Running {len(cmds)} tests:")
 
     cmds = tqdm(cmds)
 
+    # Run the commands.
     for cmd in cmds:
         fname = cmd.split(">")[1].strip()
         try:
             shell(cmd)
             result = open(join(RUN_DIR, fname)).read()
             expect = open(join(DATA_DIR, fname)).read()
         except Exception as exc:
```

### Comparing `bio-1.7.0/src/biorun/uniq.py` & `bio-1.7.1/biorun/uniq.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/utils.py` & `bio-1.7.1/biorun/utils.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/vcf2fasta.py` & `bio-1.7.1/biorun/vcf2fasta.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/api/ena_fastq.py` & `bio-1.7.1/biorun/api/ena_fastq.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/align_input.vcf` & `bio-1.7.1/biorun/data/align_input.vcf`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/align_s.txt` & `bio-1.7.1/biorun/data/align_s.txt`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/align_s.vcf` & `bio-1.7.1/biorun/data/align_s.vcf`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/explain_neutral.txt` & `bio-1.7.1/biorun/data/explain_neutral.txt`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/fasta_all1.fa` & `bio-1.7.1/biorun/data/fasta_all1.fa`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/fasta_all2.fa` & `bio-1.7.1/biorun/data/fasta_all2.fa`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/fasta_all3.fa` & `bio-1.7.1/biorun/data/fasta_all3.fa`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/fasta_cds.fa` & `bio-1.7.1/biorun/data/fasta_cds.fa`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/fasta_protein.fa` & `bio-1.7.1/biorun/data/fasta_protein.fa`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/fasta_s.fa` & `bio-1.7.1/biorun/data/fasta_s.fa`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/fasta_start.fa` & `bio-1.7.1/biorun/data/fasta_start.fa`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/fasta_stop.fa` & `bio-1.7.1/biorun/data/fasta_stop.fa`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/fasta_translate.fa` & `bio-1.7.1/biorun/data/fasta_translate.fa`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/fetch_enst.txt` & `bio-1.7.1/biorun/data/fetch_enst.txt`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/fetch_gff.gff` & `bio-1.7.1/biorun/data/fetch_gff.gff`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/fetch_prot.fa` & `bio-1.7.1/biorun/data/fetch_prot.fa`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/format_mafft1.txt` & `bio-1.7.1/biorun/data/format_mafft1.txt`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/format_mafft1.vcf` & `bio-1.7.1/biorun/data/format_mafft1.vcf`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/genomes.json` & `bio-1.7.1/biorun/data/genomes.json`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/gff_CDS.gff` & `bio-1.7.1/biorun/data/gff_CDS.gff`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/gff_all.gff` & `bio-1.7.1/biorun/data/gff_all.gff`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/gff_slice.gff` & `bio-1.7.1/biorun/data/gff_slice.gff`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/lineage.txt` & `bio-1.7.1/biorun/data/lineage.txt`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/meta.txt` & `bio-1.7.1/biorun/data/meta.txt`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/search_assembly.json` & `bio-1.7.1/biorun/data/search_assembly.json`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/search_prjn.json` & `bio-1.7.1/biorun/data/search_prjn.json`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/search_prjn.txt` & `bio-1.7.1/biorun/data/search_prjn.txt`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/search_srr.json` & `bio-1.7.1/biorun/data/search_srr.json`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/table_2.txt` & `bio-1.7.1/biorun/data/table_2.txt`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/taxon1.txt` & `bio-1.7.1/biorun/data/taxon1.txt`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/data/usage.sh` & `bio-1.7.1/biorun/data/usage.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #
 # This script is used to generate Python tests.
 #
 # The output generated by each test can be seen at:
 #
-# https://github.com/ialbert/bio/tree/master/test/data
+# https://github.com/ialbert/bio/blob/master/src/biorun/data
 #
 
 # Stop on errors.
 set -uex
 
 # Get a protein.
 bio fetch YP_009724390 > fetch_prot.fa
@@ -23,15 +23,15 @@
 
 # Last ten sequences of all entries.
 bio fasta genomes.gb -end 10 --features > fasta_all1.fa
 
 # Should produce the same output as above
 cat genomes.gb | bio fasta --end  10 --features > fasta_all2.fa
 
-# No muterence between outputs.
+# No difference between outputs.
 diff fasta_all1.fa fasta_all2.fa > nodiff.txt
 
 # Generate a JSON out[put
 cat genomes.gb | bio json > genomes.json
 
 # Last ten sequences of all entries.
 cat genomes.json | bio fasta -end 10  --features > fasta_all3.fa
@@ -129,15 +129,15 @@
 # Slice the GFF file.
 bio gff -s 300 -e 10k genomes.gb > gff_slice.gff
 
 # Taxonomy listing.
 bio taxon 117565 -d 5 > taxon1.txt
 
 # Taxonomy lineage. from file TODO
-# bio taxon genomes.gb --lineage > lineage.txt
+#bio taxon genomes.gb --lineage > lineage.txt
 
 # Getting some metadata for taxon 11138 (Murine hepatitis virus)
 bio meta 11138 -H > meta.txt
 
 # Define exact SO term
 bio explain exon > explain_exon.txt
 
@@ -156,19 +156,19 @@
 cat file1.txt file2.txt | bio  uniq > uniq0.txt
 cat file1.txt file2.txt | bio  uniq -f 2 > uniq1.txt
 cat file1.txt file2.txt | bio  uniq -c -f 2  > uniq3.txt
 
 # Get data from SRA (can be spotty)
 bio search SRR1972976 > search_srr.json
 
-# Get bioproject information
-#bio search PRJNA661333 | wc -l > search_prjn.json
+# Get bioproject information (the order is not stable)
+#bio search PRJNA661333 > search_prjn.json
 
 # Get assembly information
-# bio search GCF_000003085 > search_assembly.json
+bio search GCF_000003085 > search_assembly.json
 
 # Search mygene info
 bio search symbol:HAD --species 1316788 > search_mygene.json
 
 # Access a transcript from ensembl.
 bio fetch ENST00000288602  > fetch_enst.txt
```

### Comparing `bio-1.7.0/src/biorun/libs/placlib.py` & `bio-1.7.1/biorun/libs/placlib.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/libs/sqlitedict.py` & `bio-1.7.1/biorun/libs/sqlitedict.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/libs/xmltodict.py` & `bio-1.7.1/biorun/libs/xmltodict.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/src/biorun/scripts/fasta_filter.py` & `bio-1.7.1/biorun/scripts/fasta_filter.py`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/.gitignore` & `bio-1.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/LICENSE` & `bio-1.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bio-1.7.0/README.md` & `bio-1.7.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -102,33 +102,36 @@
 The ideas and motivations fueling `bio` have been developed while educating the many cohorts of students who used the handbook in the classroom. `bio` is an opinionated take on how bioinformatics, particularly data representation and access, should be simplified and streamlined.
 
 [handbook]: https://www.biostarhandbook.com/
 [docs]: https://www.bioinfo.help/
 
 ## Development
 
-If you clone the repository, we recommend that you install it as a development package with:
+We use the `hatch` build system to manage the software:
 
-    python setup.py develop
+https://github.com/pypa/hatch
+
+You can either use `hatch` or `pip` to install the software in editable mode:
+
+    pip install --editable .
     
 ## Testing
 
 `bio` can test itself, to run all tests execute:
 
     bio test
 
 Tests are automatically built from a shell script that mimics real-life usage scenarios.
 
-* https://github.com/ialbert/bio/blob/master/test/usage.sh
+* https://github.com/ialbert/bio/blob/master/src/biorun/data/usage.sh
 
 ## Generating documentation
 
 To generate the docs, you will need the `bookdown` package:
 
     conda install r-bookdown r-servr
     
 To run the docs in a browse:
     
     make 
     
 then visit http://localhost:8000
-
```

### Comparing `bio-1.7.0/pyproject.toml` & `bio-1.7.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -36,14 +36,20 @@
   'src/biorun/*',
 ]
 
 [project.scripts]
 "bio" = "biorun.__main__:run"
 "fasta_filter.py" = "biorun.scripts.fasta_filter:run"
 
+[tool.hatch.build.targets.sdist]
+include = ["src/biorun/data/*"]
+packages = [
+  "src/biorun",
+]
+
 [tool.hatch.build.targets.wheel]
 include = ["src/biorun/data/*"]
 packages = [
   "src/biorun",
 ]
 
 [tool.hatch.build.targets.scripts]
```

### Comparing `bio-1.7.0/PKG-INFO` & `bio-1.7.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bio
-Version: 1.7.0
+Version: 1.7.1
 Project-URL: Documentation, https://github.com/ialbert/bio#readme
 Project-URL: Issues, https://github.com/ialbert/bio/issues
 Project-URL: Source, https://github.com/ialbert/bio/
 Author-email: Istvan Albert <istvan.albert@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
@@ -126,33 +126,36 @@
 The ideas and motivations fueling `bio` have been developed while educating the many cohorts of students who used the handbook in the classroom. `bio` is an opinionated take on how bioinformatics, particularly data representation and access, should be simplified and streamlined.
 
 [handbook]: https://www.biostarhandbook.com/
 [docs]: https://www.bioinfo.help/
 
 ## Development
 
-If you clone the repository, we recommend that you install it as a development package with:
+We use the `hatch` build system to manage the software:
 
-    python setup.py develop
+https://github.com/pypa/hatch
+
+You can either use `hatch` or `pip` to install the software in editable mode:
+
+    pip install --editable .
     
 ## Testing
 
 `bio` can test itself, to run all tests execute:
 
     bio test
 
 Tests are automatically built from a shell script that mimics real-life usage scenarios.
 
-* https://github.com/ialbert/bio/blob/master/test/usage.sh
+* https://github.com/ialbert/bio/blob/master/src/biorun/data/usage.sh
 
 ## Generating documentation
 
 To generate the docs, you will need the `bookdown` package:
 
     conda install r-bookdown r-servr
     
 To run the docs in a browse:
     
     make 
     
 then visit http://localhost:8000
-
```

