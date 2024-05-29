# Comparing `tmp/libdaw-0.8.0.tar.gz` & `tmp/libdaw-0.9.1.tar.gz`

## Comparing `libdaw-0.8.0.tar` & `libdaw-0.9.1.tar`

### file list

```diff
@@ -1,157 +1,158 @@
--rw-r--r--   0     1001      127      427 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/Cargo.toml
--rw-r--r--   0     1001      127     1879 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/lib.rs
--rw-r--r--   0     1001      127      281 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/metronome/parse.rs
--rw-r--r--   0     1001      127    10846 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/metronome.rs
--rw-r--r--   0     1001      127      531 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/nodes/add.rs
--rw-r--r--   0     1001      127      870 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/nodes/constant_value.rs
--rw-r--r--   0     1001      127     1987 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/nodes/delay.rs
--rw-r--r--   0     1001      127     2253 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/nodes/detune.rs
--rw-r--r--   0     1001      127     5813 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/nodes/envelope.rs
--rw-r--r--   0     1001      127      806 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/nodes/gain.rs
--rw-r--r--   0     1001      127     1045 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/nodes/graph/error.rs
--rw-r--r--   0     1001      127    17261 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/nodes/graph.rs
--rw-r--r--   0     1001      127     6778 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/nodes/instrument.rs
--rw-r--r--   0     1001      127     1195 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/nodes/multi_frequency.rs
--rw-r--r--   0     1001      127      564 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/nodes/multiply.rs
--rw-r--r--   0     1001      127      462 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/nodes/passthrough.rs
--rw-r--r--   0     1001      127     1783 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/nodes/sawtooth_oscillator.rs
--rw-r--r--   0     1001      127     1688 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/nodes/sine_oscillator.rs
--rw-r--r--   0     1001      127     2172 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/nodes/square_oscillator.rs
--rw-r--r--   0     1001      127     1806 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/nodes/triangle_oscillator.rs
--rw-r--r--   0     1001      127      802 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/nodes.rs
--rw-r--r--   0     1001      127     1121 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/chord/parse.rs
--rw-r--r--   0     1001      127     3687 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/chord.rs
--rw-r--r--   0     1001      127      950 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/duration/parse.rs
--rw-r--r--   0     1001      127     1160 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/duration.rs
--rw-r--r--   0     1001      127      429 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/inversion/parse.rs
--rw-r--r--   0     1001      127      780 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/inversion.rs
--rw-r--r--   0     1001      127     1320 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/item/parse.rs
--rw-r--r--   0     1001      127     6282 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/item.rs
--rw-r--r--   0     1001      127      545 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/note/parse.rs
--rw-r--r--   0     1001      127     2930 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/note.rs
--rw-r--r--   0     1001      127      432 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/note_pitch/parse.rs
--rw-r--r--   0     1001      127     1677 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/note_pitch.rs
--rw-r--r--   0     1001      127      885 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/overlapped/parse.rs
--rw-r--r--   0     1001      127     2854 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/overlapped.rs
--rw-r--r--   0     1001      127      798 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/pitch/parse.rs
--rw-r--r--   0     1001      127     1894 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/pitch.rs
--rw-r--r--   0     1001      127      336 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/rest/parse.rs
--rw-r--r--   0     1001      127     1133 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/rest.rs
--rw-r--r--   0     1001      127      687 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/scale/parse.rs
--rw-r--r--   0     1001      127     2406 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/scale.rs
--rw-r--r--   0     1001      127      875 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/sequence/parse.rs
--rw-r--r--   0     1001      127     3306 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/sequence.rs
--rw-r--r--   0     1001      127     2007 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/set/parse.rs
--rw-r--r--   0     1001      127     1530 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/set.rs
--rw-r--r--   0     1001      127      408 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/state_member/parse.rs
--rw-r--r--   0     1001      127      677 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/state_member.rs
--rw-r--r--   0     1001      127      553 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/step/parse.rs
--rw-r--r--   0     1001      127     2194 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/step.rs
--rw-r--r--   0     1001      127     1712 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation/tone_generation_state.rs
--rw-r--r--   0     1001      127      551 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/notation.rs
--rw-r--r--   0     1001      127     1553 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/parse.rs
--rw-r--r--   0     1001      127     2192 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/pitch/parse.rs
--rw-r--r--   0     1001      127     6401 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/pitch.rs
--rw-r--r--   0     1001      127     1726 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/stream/iter.rs
--rw-r--r--   0     1001      127     5784 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/stream.rs
--rw-r--r--   0     1001      127     1622 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/sync.rs
--rw-r--r--   0     1001      127     2361 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/time/duration.rs
--rw-r--r--   0     1001      127     2115 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/time/time.rs
--rw-r--r--   0     1001      127     3185 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/time/timestamp.rs
--rw-r--r--   0     1001      127      172 2024-05-27 05:53:35.000000 libdaw-0.8.0/libdaw/src/time.rs
--rw-r--r--   0     1001      127      101 2024-05-27 05:53:35.000000 libdaw-0.8.0/README.md
--rw-r--r--   0        0        0      390 1970-01-01 00:00:00.000000 libdaw-0.8.0/python-libdaw/Cargo.toml
--rw-r--r--   0     1001      127     3526 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/.gitignore
--rw-r--r--   0     1001      127      131 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/README.md
--rw-r--r--   0     1001      127        6 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/docs/.gitignore
--rw-r--r--   0     1001      127      638 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/docs/Makefile
--rw-r--r--   0     1001      127      804 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/docs/make.bat
--rw-r--r--   0     1001      127        5 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/docs/requirements.txt
--rw-r--r--   0     1001      127      962 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/docs/source/conf.py
--rw-r--r--   0     1001      127      445 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/docs/source/index.rst
--rw-r--r--   0     1001      127      147 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/docs/source/libdaw/metronome.rst
--rw-r--r--   0     1001      127      161 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/docs/source/libdaw/nodes/envelope.rst
--rw-r--r--   0     1001      127      154 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/docs/source/libdaw/nodes/graph.rst
--rw-r--r--   0     1001      127      168 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/docs/source/libdaw/nodes/instrument.rst
--rw-r--r--   0     1001      127      181 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/docs/source/libdaw/nodes.rst
--rw-r--r--   0     1001      127       93 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/docs/source/libdaw/notation.rst
--rw-r--r--   0     1001      127      134 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/docs/source/libdaw/pitch.rst
--rw-r--r--   0     1001      127      133 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/docs/source/libdaw/time.rst
--rw-r--r--   0     1001      127      192 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/docs/source/libdaw.rst
--rw-r--r--   0     1001      127     1780 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/examples/1564.py
--rw-r--r--   0     1001      127     1662 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/examples/blues.py
--rwxr-xr-x   0     1001      127     1689 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/examples/instrument-test.py
--rw-r--r--   0     1001      127     1425 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/examples/pachelbel-canon-progression.py
--rw-r--r--   0     1001      127     1634 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/examples/round.py
--rw-r--r--   0     1001      127     1526 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/examples/scale-inversion-notation.py
--rw-r--r--   0     1001      127     1482 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/examples/simple-notation.py
--rw-r--r--   0     1001      127     1389 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/examples/simple-scale-notation.py
--rw-r--r--   0     1001      127      169 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/python/libdaw/__init__.py
--rw-r--r--   0     1001      127      933 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/python/libdaw/__init__.pyi
--rw-r--r--   0     1001      127     1588 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/python/libdaw/metronome.pyi
--rw-r--r--   0     1001      127     2528 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/python/libdaw/nodes/__init__.pyi
--rw-r--r--   0     1001      127      173 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/python/libdaw/nodes/envelope.pyi
--rw-r--r--   0     1001      127       23 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/python/libdaw/nodes/graph.pyi
--rw-r--r--   0     1001      127      151 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/python/libdaw/nodes/instrument.pyi
--rw-r--r--   0     1001      127     7533 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/python/libdaw/notation.pyi
--rw-r--r--   0     1001      127     1061 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/python/libdaw/pitch.pyi
--rw-r--r--   0     1001      127        0 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/python/libdaw/py.typed
--rw-r--r--   0     1001      127     1497 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/python/libdaw/time.pyi
--rw-r--r--   0     1001      127      491 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/frequency_node.rs
--rw-r--r--   0     1001      127     3052 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/lib.rs
--rw-r--r--   0     1001      127     4697 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/metronome.rs
--rw-r--r--   0     1001      127      976 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/node.rs
--rw-r--r--   0     1001      127      514 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/nodes/add.rs
--rw-r--r--   0     1001      127      580 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/nodes/constant_value.rs
--rw-r--r--   0     1001      127      586 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/nodes/delay.rs
--rw-r--r--   0     1001      127      845 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/nodes/detune.rs
--rw-r--r--   0     1001      127     1868 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/nodes/envelope.rs
--rw-r--r--   0     1001      127      644 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/nodes/gain.rs
--rw-r--r--   0     1001      127     4581 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/nodes/graph.rs
--rw-r--r--   0     1001      127     2715 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/nodes/instrument.rs
--rw-r--r--   0     1001      127      672 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/nodes/multi_frequency.rs
--rw-r--r--   0     1001      127      534 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/nodes/multiply.rs
--rw-r--r--   0     1001      127      489 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/nodes/passthrough.rs
--rw-r--r--   0     1001      127      756 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/nodes/sawtooth_oscillator.rs
--rw-r--r--   0     1001      127      705 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/nodes/sine_oscillator.rs
--rw-r--r--   0     1001      127      748 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/nodes/square_oscillator.rs
--rw-r--r--   0     1001      127      756 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/nodes/triangle_oscillator.rs
--rw-r--r--   0     1001      127     1787 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/nodes.rs
--rw-r--r--   0     1001      127     7021 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/notation/chord.rs
--rw-r--r--   0     1001      127     4134 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/notation/duration.rs
--rw-r--r--   0     1001      127     1472 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/notation/inversion.rs
--rw-r--r--   0     1001      127     4835 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/notation/item.rs
--rw-r--r--   0     1001      127     1982 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/notation/note/note_pitch.rs
--rw-r--r--   0     1001      127     4043 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/notation/note.rs
--rw-r--r--   0     1001      127     6110 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/notation/overlapped.rs
--rw-r--r--   0     1001      127     2936 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/notation/pitch.rs
--rw-r--r--   0     1001      127     1561 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/notation/rest.rs
--rw-r--r--   0     1001      127     4478 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/notation/scale.rs
--rw-r--r--   0     1001      127     5945 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/notation/sequence.rs
--rw-r--r--   0     1001      127     3323 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/notation/set.rs
--rw-r--r--   0     1001      127     1218 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/notation/state_member.rs
--rw-r--r--   0     1001      127     1983 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/notation/step.rs
--rw-r--r--   0     1001      127     1195 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/notation.rs
--rw-r--r--   0     1001      127     5729 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/pitch/pitch.rs
--rw-r--r--   0     1001      127     2648 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/pitch.rs
--rw-r--r--   0     1001      127     2178 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/play.rs
--rw-r--r--   0     1001      127     2638 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/stream.rs
--rw-r--r--   0     1001      127     5721 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/src/time.rs
--rw-r--r--   0     1001      127        0 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/test/__init__.py
--rw-r--r--   0     1001      127      471 2024-05-27 05:53:35.000000 libdaw-0.8.0/python-libdaw/test/test_pitch.py
--rw-r--r--   0     1001      127    30727 2024-05-27 05:53:43.000000 libdaw-0.8.0/Cargo.lock
--rw-r--r--   0        0        0      241 1970-01-01 00:00:00.000000 libdaw-0.8.0/Cargo.toml
--rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 libdaw-0.8.0/pyproject.toml
--rw-r--r--   0     1001      127     7533 2024-05-27 05:53:35.000000 libdaw-0.8.0/python/libdaw/notation.pyi
--rw-r--r--   0     1001      127      169 2024-05-27 05:53:35.000000 libdaw-0.8.0/python/libdaw/__init__.py
--rw-r--r--   0     1001      127        0 2024-05-27 05:53:35.000000 libdaw-0.8.0/python/libdaw/py.typed
--rw-r--r--   0     1001      127     1061 2024-05-27 05:53:35.000000 libdaw-0.8.0/python/libdaw/pitch.pyi
--rw-r--r--   0     1001      127     1497 2024-05-27 05:53:35.000000 libdaw-0.8.0/python/libdaw/time.pyi
--rw-r--r--   0     1001      127      933 2024-05-27 05:53:35.000000 libdaw-0.8.0/python/libdaw/__init__.pyi
--rw-r--r--   0     1001      127     1588 2024-05-27 05:53:35.000000 libdaw-0.8.0/python/libdaw/metronome.pyi
--rw-r--r--   0     1001      127      151 2024-05-27 05:53:35.000000 libdaw-0.8.0/python/libdaw/nodes/instrument.pyi
--rw-r--r--   0     1001      127       23 2024-05-27 05:53:35.000000 libdaw-0.8.0/python/libdaw/nodes/graph.pyi
--rw-r--r--   0     1001      127      173 2024-05-27 05:53:35.000000 libdaw-0.8.0/python/libdaw/nodes/envelope.pyi
--rw-r--r--   0     1001      127     2528 2024-05-27 05:53:35.000000 libdaw-0.8.0/python/libdaw/nodes/__init__.pyi
--rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 libdaw-0.8.0/PKG-INFO
+-rw-r--r--   0     1001      127      427 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/Cargo.toml
+-rw-r--r--   0     1001      127     1879 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/lib.rs
+-rw-r--r--   0     1001      127      281 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/metronome/parse.rs
+-rw-r--r--   0     1001      127    10846 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/metronome.rs
+-rw-r--r--   0     1001      127      540 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/nodes/add.rs
+-rw-r--r--   0     1001      127      873 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/nodes/constant_value.rs
+-rw-r--r--   0     1001      127     2002 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/nodes/delay.rs
+-rw-r--r--   0     1001      127     2253 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/nodes/detune.rs
+-rw-r--r--   0     1001      127     5813 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/nodes/envelope.rs
+-rw-r--r--   0     1001      127      806 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/nodes/gain.rs
+-rw-r--r--   0     1001      127     1045 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/nodes/graph/error.rs
+-rw-r--r--   0     1001      127    17261 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/nodes/graph.rs
+-rw-r--r--   0     1001      127     6778 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/nodes/instrument.rs
+-rw-r--r--   0     1001      127     1195 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/nodes/multi_frequency.rs
+-rw-r--r--   0     1001      127      573 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/nodes/multiply.rs
+-rw-r--r--   0     1001      127      462 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/nodes/passthrough.rs
+-rw-r--r--   0     1001      127     1786 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/nodes/sawtooth_oscillator.rs
+-rw-r--r--   0     1001      127     1691 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/nodes/sine_oscillator.rs
+-rw-r--r--   0     1001      127     2175 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/nodes/square_oscillator.rs
+-rw-r--r--   0     1001      127     1809 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/nodes/triangle_oscillator.rs
+-rw-r--r--   0     1001      127      802 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/nodes.rs
+-rw-r--r--   0     1001      127     1121 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/chord/parse.rs
+-rw-r--r--   0     1001      127     3687 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/chord.rs
+-rw-r--r--   0     1001      127      950 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/duration/parse.rs
+-rw-r--r--   0     1001      127     1160 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/duration.rs
+-rw-r--r--   0     1001      127      429 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/inversion/parse.rs
+-rw-r--r--   0     1001      127      780 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/inversion.rs
+-rw-r--r--   0     1001      127     1320 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/item/parse.rs
+-rw-r--r--   0     1001      127     6282 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/item.rs
+-rw-r--r--   0     1001      127      545 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/note/parse.rs
+-rw-r--r--   0     1001      127     2930 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/note.rs
+-rw-r--r--   0     1001      127      432 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/note_pitch/parse.rs
+-rw-r--r--   0     1001      127     1677 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/note_pitch.rs
+-rw-r--r--   0     1001      127      885 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/overlapped/parse.rs
+-rw-r--r--   0     1001      127     2854 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/overlapped.rs
+-rw-r--r--   0     1001      127      798 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/pitch/parse.rs
+-rw-r--r--   0     1001      127     1894 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/pitch.rs
+-rw-r--r--   0     1001      127      336 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/rest/parse.rs
+-rw-r--r--   0     1001      127     1133 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/rest.rs
+-rw-r--r--   0     1001      127      687 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/scale/parse.rs
+-rw-r--r--   0     1001      127     2757 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/scale.rs
+-rw-r--r--   0     1001      127      875 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/sequence/parse.rs
+-rw-r--r--   0     1001      127     3306 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/sequence.rs
+-rw-r--r--   0     1001      127     2007 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/set/parse.rs
+-rw-r--r--   0     1001      127     1530 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/set.rs
+-rw-r--r--   0     1001      127      408 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/state_member/parse.rs
+-rw-r--r--   0     1001      127      677 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/state_member.rs
+-rw-r--r--   0     1001      127      553 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/step/parse.rs
+-rw-r--r--   0     1001      127     2194 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/step.rs
+-rw-r--r--   0     1001      127     1712 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation/tone_generation_state.rs
+-rw-r--r--   0     1001      127      551 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/notation.rs
+-rw-r--r--   0     1001      127     1553 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/parse.rs
+-rw-r--r--   0     1001      127     2192 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/pitch/parse.rs
+-rw-r--r--   0     1001      127     6401 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/pitch.rs
+-rw-r--r--   0     1001      127     1726 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/sample/iter.rs
+-rw-r--r--   0     1001      127     5518 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/sample.rs
+-rw-r--r--   0     1001      127     1622 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/sync.rs
+-rw-r--r--   0     1001      127     2361 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/time/duration.rs
+-rw-r--r--   0     1001      127     2115 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/time/time.rs
+-rw-r--r--   0     1001      127     3185 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/time/timestamp.rs
+-rw-r--r--   0     1001      127      172 2024-05-29 20:19:09.000000 libdaw-0.9.1/libdaw/src/time.rs
+-rw-r--r--   0     1001      127      101 2024-05-29 20:19:09.000000 libdaw-0.9.1/README.md
+-rw-r--r--   0        0        0      390 1970-01-01 00:00:00.000000 libdaw-0.9.1/python-libdaw/Cargo.toml
+-rw-r--r--   0     1001      127     3526 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/.gitignore
+-rw-r--r--   0     1001      127      131 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/README.md
+-rw-r--r--   0     1001      127        6 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/docs/.gitignore
+-rw-r--r--   0     1001      127      638 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/docs/Makefile
+-rw-r--r--   0     1001      127      804 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/docs/make.bat
+-rw-r--r--   0     1001      127        5 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/docs/requirements.txt
+-rw-r--r--   0     1001      127      962 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/docs/source/conf.py
+-rw-r--r--   0     1001      127      445 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/docs/source/index.rst
+-rw-r--r--   0     1001      127      147 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/docs/source/libdaw/metronome.rst
+-rw-r--r--   0     1001      127      161 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/docs/source/libdaw/nodes/envelope.rst
+-rw-r--r--   0     1001      127      154 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/docs/source/libdaw/nodes/graph.rst
+-rw-r--r--   0     1001      127      168 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/docs/source/libdaw/nodes/instrument.rst
+-rw-r--r--   0     1001      127      181 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/docs/source/libdaw/nodes.rst
+-rw-r--r--   0     1001      127       93 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/docs/source/libdaw/notation.rst
+-rw-r--r--   0     1001      127      134 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/docs/source/libdaw/pitch.rst
+-rw-r--r--   0     1001      127      133 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/docs/source/libdaw/time.rst
+-rw-r--r--   0     1001      127      192 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/docs/source/libdaw.rst
+-rw-r--r--   0     1001      127     1780 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/examples/1564.py
+-rw-r--r--   0     1001      127     1662 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/examples/blues.py
+-rwxr-xr-x   0     1001      127     1689 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/examples/instrument-test.py
+-rw-r--r--   0     1001      127     1425 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/examples/pachelbel-canon-progression.py
+-rw-r--r--   0     1001      127     1634 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/examples/round.py
+-rw-r--r--   0     1001      127     1526 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/examples/scale-inversion-notation.py
+-rw-r--r--   0     1001      127     1482 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/examples/simple-notation.py
+-rw-r--r--   0     1001      127     1389 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/examples/simple-scale-notation.py
+-rw-r--r--   0     1001      127      169 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/python/libdaw/__init__.py
+-rw-r--r--   0     1001      127      897 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/python/libdaw/__init__.pyi
+-rw-r--r--   0     1001      127     1588 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/python/libdaw/metronome.pyi
+-rw-r--r--   0     1001      127     2528 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/python/libdaw/nodes/__init__.pyi
+-rw-r--r--   0     1001      127      173 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/python/libdaw/nodes/envelope.pyi
+-rw-r--r--   0     1001      127       23 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/python/libdaw/nodes/graph.pyi
+-rw-r--r--   0     1001      127      151 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/python/libdaw/nodes/instrument.pyi
+-rw-r--r--   0     1001      127     7533 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/python/libdaw/notation.pyi
+-rw-r--r--   0     1001      127     1061 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/python/libdaw/pitch.pyi
+-rw-r--r--   0     1001      127        0 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/python/libdaw/py.typed
+-rw-r--r--   0     1001      127     1497 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/python/libdaw/time.pyi
+-rw-r--r--   0     1001      127      491 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/frequency_node.rs
+-rw-r--r--   0     1001      127    11336 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/indexing.rs
+-rw-r--r--   0     1001      127     2036 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/lib.rs
+-rw-r--r--   0     1001      127     4697 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/metronome.rs
+-rw-r--r--   0     1001      127      976 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/node.rs
+-rw-r--r--   0     1001      127      514 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/nodes/add.rs
+-rw-r--r--   0     1001      127      580 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/nodes/constant_value.rs
+-rw-r--r--   0     1001      127      586 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/nodes/delay.rs
+-rw-r--r--   0     1001      127      845 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/nodes/detune.rs
+-rw-r--r--   0     1001      127     1868 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/nodes/envelope.rs
+-rw-r--r--   0     1001      127      644 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/nodes/gain.rs
+-rw-r--r--   0     1001      127     4581 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/nodes/graph.rs
+-rw-r--r--   0     1001      127     2715 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/nodes/instrument.rs
+-rw-r--r--   0     1001      127      672 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/nodes/multi_frequency.rs
+-rw-r--r--   0     1001      127      534 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/nodes/multiply.rs
+-rw-r--r--   0     1001      127      489 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/nodes/passthrough.rs
+-rw-r--r--   0     1001      127      756 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/nodes/sawtooth_oscillator.rs
+-rw-r--r--   0     1001      127      705 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/nodes/sine_oscillator.rs
+-rw-r--r--   0     1001      127      748 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/nodes/square_oscillator.rs
+-rw-r--r--   0     1001      127      756 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/nodes/triangle_oscillator.rs
+-rw-r--r--   0     1001      127     1787 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/nodes.rs
+-rw-r--r--   0     1001      127     8309 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/notation/chord.rs
+-rw-r--r--   0     1001      127     4134 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/notation/duration.rs
+-rw-r--r--   0     1001      127     1472 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/notation/inversion.rs
+-rw-r--r--   0     1001      127     5002 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/notation/item.rs
+-rw-r--r--   0     1001      127     1982 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/notation/note/note_pitch.rs
+-rw-r--r--   0     1001      127     4043 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/notation/note.rs
+-rw-r--r--   0     1001      127     7222 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/notation/overlapped.rs
+-rw-r--r--   0     1001      127     2936 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/notation/pitch.rs
+-rw-r--r--   0     1001      127     1561 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/notation/rest.rs
+-rw-r--r--   0     1001      127     5718 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/notation/scale.rs
+-rw-r--r--   0     1001      127     7047 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/notation/sequence.rs
+-rw-r--r--   0     1001      127     3323 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/notation/set.rs
+-rw-r--r--   0     1001      127     1218 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/notation/state_member.rs
+-rw-r--r--   0     1001      127     1983 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/notation/step.rs
+-rw-r--r--   0     1001      127     1195 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/notation.rs
+-rw-r--r--   0     1001      127     5729 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/pitch/pitch.rs
+-rw-r--r--   0     1001      127     2648 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/pitch.rs
+-rw-r--r--   0     1001      127     2181 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/play.rs
+-rw-r--r--   0     1001      127     3973 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/sample.rs
+-rw-r--r--   0     1001      127     5721 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/src/time.rs
+-rw-r--r--   0     1001      127        0 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/test/__init__.py
+-rw-r--r--   0     1001      127      471 2024-05-29 20:19:09.000000 libdaw-0.9.1/python-libdaw/test/test_pitch.py
+-rw-r--r--   0     1001      127    30727 2024-05-29 20:19:13.000000 libdaw-0.9.1/Cargo.lock
+-rw-r--r--   0        0        0      241 1970-01-01 00:00:00.000000 libdaw-0.9.1/Cargo.toml
+-rw-r--r--   0        0        0      606 1970-01-01 00:00:00.000000 libdaw-0.9.1/pyproject.toml
+-rw-r--r--   0     1001      127     7533 2024-05-29 20:19:09.000000 libdaw-0.9.1/python/libdaw/notation.pyi
+-rw-r--r--   0     1001      127      169 2024-05-29 20:19:09.000000 libdaw-0.9.1/python/libdaw/__init__.py
+-rw-r--r--   0     1001      127        0 2024-05-29 20:19:09.000000 libdaw-0.9.1/python/libdaw/py.typed
+-rw-r--r--   0     1001      127     1061 2024-05-29 20:19:09.000000 libdaw-0.9.1/python/libdaw/pitch.pyi
+-rw-r--r--   0     1001      127     1497 2024-05-29 20:19:09.000000 libdaw-0.9.1/python/libdaw/time.pyi
+-rw-r--r--   0     1001      127      897 2024-05-29 20:19:09.000000 libdaw-0.9.1/python/libdaw/__init__.pyi
+-rw-r--r--   0     1001      127     1588 2024-05-29 20:19:09.000000 libdaw-0.9.1/python/libdaw/metronome.pyi
+-rw-r--r--   0     1001      127      151 2024-05-29 20:19:09.000000 libdaw-0.9.1/python/libdaw/nodes/instrument.pyi
+-rw-r--r--   0     1001      127       23 2024-05-29 20:19:09.000000 libdaw-0.9.1/python/libdaw/nodes/graph.pyi
+-rw-r--r--   0     1001      127      173 2024-05-29 20:19:09.000000 libdaw-0.9.1/python/libdaw/nodes/envelope.pyi
+-rw-r--r--   0     1001      127     2528 2024-05-29 20:19:09.000000 libdaw-0.9.1/python/libdaw/nodes/__init__.pyi
+-rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 libdaw-0.9.1/PKG-INFO
```

### Comparing `libdaw-0.8.0/libdaw/src/lib.rs` & `libdaw-0.9.1/libdaw/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 pub mod metronome;
 pub mod nodes;
 pub mod notation;
 mod parse;
 pub mod pitch;
-pub mod stream;
+pub mod sample;
 mod sync;
 pub mod time;
 
+pub use sample::Sample;
 use std::fmt::Debug;
 use std::sync::Arc;
-pub use stream::Stream;
 
 pub type Error = Box<dyn std::error::Error + Send + Sync>;
 pub type Result<T> = std::result::Result<T, Error>;
 
 /// An audio node trait, allowing a sample_rate to be set and processing to
 /// be performed. Some things like setters are self, not mut self, because we
 /// need to support Arc<dyn Node> so upcasting works.  This will be fixed when
 /// https://github.com/rust-lang/rust/issues/65991 is fully finished and in
 /// stable rust.  When that happens, the interface will change to &mut self
 /// methods.
 pub trait Node: Debug + Send + Sync {
     fn process<'a, 'b, 'c>(
         &'a self,
-        inputs: &'b [Stream],
-        outputs: &'c mut Vec<Stream>,
+        inputs: &'b [Sample],
+        outputs: &'c mut Vec<Sample>,
     ) -> Result<()>;
 }
 
 impl Iterator for &dyn Node {
-    type Item = Result<Vec<Stream>>;
+    type Item = Result<Vec<Sample>>;
 
     fn next(&mut self) -> Option<Self::Item> {
         let mut outputs = Vec::new();
         Some(match self.process(&[], &mut outputs) {
             Err(e) => Err(e),
             Ok(()) => Ok(outputs),
         })
```

### Comparing `libdaw-0.8.0/libdaw/src/metronome.rs` & `libdaw-0.9.1/libdaw/src/metronome.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/nodes/add.rs` & `libdaw-0.9.1/libdaw/src/nodes/add.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use crate::{stream::Stream, Node, Result};
+use crate::{sample::Sample, Node, Result};
 
 #[derive(Debug)]
 pub struct Add {
     channels: usize,
 }
 
 impl Add {
@@ -12,16 +12,16 @@
         }
     }
 }
 
 impl Node for Add {
     fn process<'a, 'b, 'c>(
         &'a self,
-        inputs: &'b [Stream],
-        outputs: &'c mut Vec<Stream>,
+        inputs: &'b [Sample],
+        outputs: &'c mut Vec<Sample>,
     ) -> Result<()> {
-        let mut output: Stream = inputs.iter().sum();
-        output.resize(self.channels, 0.0);
+        let mut output: Sample = inputs.iter().sum();
+        output.channels.resize(self.channels, 0.0);
         outputs.push(output);
         Ok(())
     }
 }
```

### Comparing `libdaw-0.8.0/libdaw/src/nodes/constant_value.rs` & `libdaw-0.9.1/libdaw/src/nodes/constant_value.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use crate::stream::Stream;
+use crate::sample::Sample;
 use crate::sync::AtomicF64;
 use crate::{Node, Result};
 
 use std::sync::atomic::Ordering;
 
 #[derive(Debug, Default)]
 pub struct ConstantValue {
@@ -22,14 +22,14 @@
     }
     pub fn set_value(&self, value: f64) {
         self.value.store(value, Ordering::Relaxed);
     }
 }
 
 impl Node for ConstantValue {
-    fn process<'a, 'b>(&'a self, _: &'b [Stream], outputs: &'a mut Vec<Stream>) -> Result<()> {
-        let mut stream = Stream::new(self.channels);
+    fn process<'a, 'b>(&'a self, _: &'b [Sample], outputs: &'a mut Vec<Sample>) -> Result<()> {
+        let mut stream = Sample::zeroed(self.channels);
         stream.fill(self.value.load(Ordering::Relaxed));
         outputs.push(stream);
         Ok(())
     }
 }
```

### Comparing `libdaw-0.8.0/libdaw/src/nodes/delay.rs` & `libdaw-0.9.1/libdaw/src/nodes/delay.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-use crate::{stream::Stream, time::Duration, Node, Result};
+use crate::{sample::Sample, time::Duration, Node, Result};
 use std::{
     collections::VecDeque,
     sync::{
         atomic::{AtomicU64, Ordering},
         Mutex,
     },
 };
 
 #[derive(Debug)]
-struct Sample {
+struct DelaySample {
     play_sample: u64,
-    stream: Stream,
+    stream: Sample,
 }
 
-type Buffer = VecDeque<Sample>;
+type Buffer = VecDeque<DelaySample>;
 
 #[derive(Debug)]
 pub struct Delay {
     buffers: Mutex<Vec<Buffer>>,
     sample: AtomicU64,
     delay: u64,
 }
@@ -32,16 +32,16 @@
         }
     }
 }
 
 impl Node for Delay {
     fn process<'a, 'b, 'c>(
         &'a self,
-        inputs: &'b [Stream],
-        outputs: &'c mut Vec<Stream>,
+        inputs: &'b [Sample],
+        outputs: &'c mut Vec<Sample>,
     ) -> Result<()> {
         if self.delay == 0 {
             outputs.extend_from_slice(inputs);
             return Ok(());
         }
         let sample = self
             .sample
@@ -60,15 +60,15 @@
                 .front()
                 .map(|buffer_sample| sample >= buffer_sample.play_sample)
                 .unwrap_or(false);
             if play {
                 outputs.push(buffer.pop_front().expect("buffer will not be empty").stream);
             }
             if let Some(stream) = inputs.get(i).cloned() {
-                buffer.push_back(Sample {
+                buffer.push_back(DelaySample {
                     play_sample,
                     stream,
                 });
             }
         }
         Ok(())
     }
```

### Comparing `libdaw-0.8.0/libdaw/src/nodes/detune.rs` & `libdaw-0.9.1/libdaw/src/nodes/detune.rs`

 * *Files 4% similar despite different names*

```diff
@@ -42,16 +42,16 @@
         self.detune.load(Ordering::Relaxed)
     }
 }
 
 impl Node for Detune {
     fn process<'a, 'b, 'c>(
         &'a self,
-        inputs: &'b [crate::stream::Stream],
-        outputs: &'c mut Vec<crate::stream::Stream>,
+        inputs: &'b [crate::sample::Sample],
+        outputs: &'c mut Vec<crate::sample::Sample>,
     ) -> Result<()> {
         self.node.process(inputs, outputs)
     }
 }
 
 impl FrequencyNode for Detune {
     fn get_frequency(&self) -> Result<f64> {
```

### Comparing `libdaw-0.8.0/libdaw/src/nodes/envelope.rs` & `libdaw-0.9.1/libdaw/src/nodes/envelope.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 use crate::{
-    stream::Stream,
+    sample::Sample,
     time::{Duration, Time},
     Node, Result,
 };
 use std::sync::atomic::{AtomicU64, Ordering};
 
 #[derive(Debug, Clone, Copy)]
 pub enum Offset {
@@ -129,16 +129,16 @@
         }
     }
 }
 
 impl Node for Envelope {
     fn process<'a, 'b, 'c>(
         &'a self,
-        inputs: &'b [Stream],
-        outputs: &'c mut Vec<Stream>,
+        inputs: &'b [Sample],
+        outputs: &'c mut Vec<Sample>,
     ) -> Result<()> {
         outputs.extend_from_slice(inputs);
 
         let envelope_len = self.envelope.len();
         let volume = match envelope_len {
             0 => return Ok(()),
             1 => self.envelope[0].volume,
```

### Comparing `libdaw-0.8.0/libdaw/src/nodes/gain.rs` & `libdaw-0.9.1/libdaw/src/nodes/gain.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use crate::{stream::Stream, sync::AtomicF64, Node, Result};
+use crate::{sample::Sample, sync::AtomicF64, Node, Result};
 use std::sync::atomic::Ordering;
 
 #[derive(Debug)]
 pub struct Gain {
     gain: AtomicF64,
 }
 
@@ -21,16 +21,16 @@
         self.gain.load(Ordering::Relaxed)
     }
 }
 
 impl Node for Gain {
     fn process<'a, 'b, 'c>(
         &'a self,
-        inputs: &'b [Stream],
-        outputs: &'c mut Vec<Stream>,
+        inputs: &'b [Sample],
+        outputs: &'c mut Vec<Sample>,
     ) -> Result<()> {
         outputs.extend_from_slice(inputs);
         let gain = self.gain.load(Ordering::Relaxed);
 
         for output in outputs {
             *output *= gain;
         }
```

### Comparing `libdaw-0.8.0/libdaw/src/nodes/graph/error.rs` & `libdaw-0.9.1/libdaw/src/nodes/graph/error.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/nodes/graph.rs` & `libdaw-0.9.1/libdaw/src/nodes/graph.rs`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 mod error;
 
 pub use error::Error;
 
 type Result<T> = std::result::Result<T, Error>;
 
 use crate::nodes::Passthrough;
-use crate::stream::Stream;
+use crate::sample::Sample;
 use crate::Node;
 use nohash_hasher::{IntSet, IsEnabled};
 
 use std::hash::Hash;
 use std::sync::{Arc, Mutex};
 use Error::IllegalIndex;
 use Error::NoSuchConnection;
@@ -28,16 +28,16 @@
     source: Index,
     stream: Option<usize>,
 }
 
 #[derive(Debug)]
 struct Slot {
     node: Strong,
-    output: Mutex<Vec<Stream>>,
-    input_buffer: Mutex<Vec<Stream>>,
+    output: Mutex<Vec<Sample>>,
+    input_buffer: Mutex<Vec<Sample>>,
     inputs: Vec<Input>,
 }
 
 /// The processing order list, keeping the list in memory so that we only have
 /// to rebuild it if the graph has changed.
 #[derive(Debug, Default)]
 struct ProcessList {
@@ -379,16 +379,16 @@
         }
     }
 
     /// Process all inputs from roots down to the sink.
     /// All sinks are added together to turn this into a single output.
     fn process<'a, 'b, 'c>(
         &'a mut self,
-        inputs: &'b [Stream],
-        outputs: &'c mut Vec<Stream>,
+        inputs: &'b [Sample],
+        outputs: &'c mut Vec<Sample>,
     ) -> crate::Result<()> {
         self.build_process_list();
         // First process all process-needing nodes in reverse order.
         for node in self
             .process_list
             .lock()
             .expect("mutex poisoned")
@@ -515,16 +515,16 @@
             .remove_output(source, stream)
     }
 }
 
 impl Node for Graph {
     fn process<'a, 'b, 'c>(
         &'a self,
-        inputs: &'b [Stream],
-        outputs: &'c mut Vec<Stream>,
+        inputs: &'b [Sample],
+        outputs: &'c mut Vec<Sample>,
     ) -> crate::Result<()> {
         self.inner
             .lock()
             .expect("mutex poisoned")
             .process(inputs, outputs)
     }
 }
```

### Comparing `libdaw-0.8.0/libdaw/src/nodes/instrument.rs` & `libdaw-0.9.1/libdaw/src/nodes/instrument.rs`

 * *Files 2% similar despite different names*

```diff
@@ -147,16 +147,16 @@
         Ok(())
     }
 }
 
 impl Node for Instrument {
     fn process<'a, 'b, 'c>(
         &'a self,
-        inputs: &'b [crate::stream::Stream],
-        outputs: &'c mut Vec<crate::stream::Stream>,
+        inputs: &'b [crate::sample::Sample],
+        outputs: &'c mut Vec<crate::sample::Sample>,
     ) -> Result<()> {
         let sample = self
             .sample
             .swap(self.sample.load(Ordering::Relaxed) + 1, Ordering::Relaxed);
         let detune = self.detune.load(Ordering::Relaxed);
 
         let mut queue = self.queue.lock().expect("mutex poisoned");
```

### Comparing `libdaw-0.8.0/libdaw/src/nodes/multi_frequency.rs` & `libdaw-0.9.1/libdaw/src/nodes/multi_frequency.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use crate::{stream::Stream, sync::AtomicF64, FrequencyNode, Node, Result};
+use crate::{sample::Sample, sync::AtomicF64, FrequencyNode, Node, Result};
 use std::sync::{atomic::Ordering, Arc};
 
 /// A FrequencyNode that wraps any number of other frequency nodes
 #[derive(Debug)]
 pub struct MultiFrequency {
     nodes: Box<[Arc<dyn FrequencyNode>]>,
     frequency: AtomicF64,
@@ -29,16 +29,16 @@
         Ok(self.frequency.load(Ordering::Relaxed))
     }
 }
 
 impl Node for MultiFrequency {
     fn process<'a, 'b, 'c>(
         &'a self,
-        inputs: &'b [Stream],
-        outputs: &'c mut Vec<Stream>,
+        inputs: &'b [Sample],
+        outputs: &'c mut Vec<Sample>,
     ) -> Result<()> {
         for node in self.nodes.iter() {
             node.process(inputs, outputs)?;
         }
         Ok(())
     }
 }
```

### Comparing `libdaw-0.8.0/libdaw/src/nodes/multiply.rs` & `libdaw-0.9.1/libdaw/src/nodes/multiply.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use crate::{stream::Stream, Node, Result};
+use crate::{sample::Sample, Node, Result};
 
 #[derive(Debug, Default)]
 pub struct Multiply {
     channels: usize,
 }
 
 impl Multiply {
@@ -12,16 +12,16 @@
         }
     }
 }
 
 impl Node for Multiply {
     fn process<'a, 'b, 'c>(
         &'a self,
-        inputs: &'b [Stream],
-        outputs: &'c mut Vec<Stream>,
+        inputs: &'b [Sample],
+        outputs: &'c mut Vec<Sample>,
     ) -> Result<()> {
-        let mut output: Stream = inputs.iter().product();
-        output.resize(self.channels, 0.0);
+        let mut output: Sample = inputs.iter().product();
+        output.channels.resize(self.channels, 0.0);
         outputs.push(output);
         Ok(())
     }
 }
```

### Comparing `libdaw-0.8.0/libdaw/src/nodes/sawtooth_oscillator.rs` & `libdaw-0.9.1/libdaw/src/nodes/sawtooth_oscillator.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use crate::{stream::Stream, sync::AtomicF64, FrequencyNode, Node, Result};
+use crate::{sample::Sample, sync::AtomicF64, FrequencyNode, Node, Result};
 use std::sync::atomic::Ordering;
 
 #[derive(Debug)]
 pub struct SawtoothOscillator {
     frequency: AtomicF64,
     sample_rate: f64,
     sample: AtomicF64,
@@ -41,21 +41,21 @@
     }
     fn get_frequency(&self) -> Result<f64> {
         Ok(self.frequency.load(Ordering::Relaxed))
     }
 }
 
 impl Node for SawtoothOscillator {
-    fn process<'a, 'b, 'c>(&'a self, _: &'b [Stream], outputs: &'c mut Vec<Stream>) -> Result<()> {
+    fn process<'a, 'b, 'c>(&'a self, _: &'b [Sample], outputs: &'c mut Vec<Sample>) -> Result<()> {
         let sample = self.sample.swap(
             (self.sample.load(Ordering::Relaxed) + self.delta.load(Ordering::Relaxed) + 1.0f64)
                 % 2.0f64
                 - 1.0f64,
             Ordering::Relaxed,
         );
 
-        let mut output = Stream::new(self.channels);
+        let mut output = Sample::zeroed(self.channels);
         output.fill(sample);
         outputs.push(output);
         Ok(())
     }
 }
```

### Comparing `libdaw-0.8.0/libdaw/src/nodes/sine_oscillator.rs` & `libdaw-0.9.1/libdaw/src/nodes/sine_oscillator.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use crate::{stream::Stream, sync::AtomicF64, FrequencyNode, Node, Result};
+use crate::{sample::Sample, sync::AtomicF64, FrequencyNode, Node, Result};
 use std::{f64, sync::atomic::Ordering};
 
 #[derive(Debug)]
 pub struct SineOscillator {
     frequency: AtomicF64,
     sample_rate: f64,
     /// Ramps from 0 to TAU per period
@@ -40,19 +40,19 @@
     }
     fn get_frequency(&self) -> Result<f64> {
         Ok(self.frequency.load(Ordering::Relaxed))
     }
 }
 
 impl Node for SineOscillator {
-    fn process<'a, 'b, 'c>(&'a self, _: &'b [Stream], outputs: &'c mut Vec<Stream>) -> Result<()> {
+    fn process<'a, 'b, 'c>(&'a self, _: &'b [Sample], outputs: &'c mut Vec<Sample>) -> Result<()> {
         let ramp = self.ramp.swap(
             (self.ramp.load(Ordering::Relaxed) + self.delta.load(Ordering::Relaxed))
                 % f64::consts::TAU,
             Ordering::Relaxed,
         );
-        let mut output = Stream::new(self.channels);
+        let mut output = Sample::zeroed(self.channels);
         output.fill(ramp.sin());
         outputs.push(output);
         Ok(())
     }
 }
```

### Comparing `libdaw-0.8.0/libdaw/src/nodes/square_oscillator.rs` & `libdaw-0.9.1/libdaw/src/nodes/square_oscillator.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use crate::stream::Stream;
+use crate::sample::Sample;
 use crate::sync::AtomicF64;
 use crate::{FrequencyNode, Node, Result};
 
 use std::sync::atomic::Ordering;
 
 #[derive(Debug)]
 pub struct SquareOscillator {
@@ -43,16 +43,16 @@
     }
     fn get_frequency(&self) -> Result<f64> {
         Ok(self.frequency.load(Ordering::Relaxed))
     }
 }
 
 impl Node for SquareOscillator {
-    fn process<'a, 'b, 'c>(&'a self, _: &'b [Stream], outputs: &'c mut Vec<Stream>) -> Result<()> {
-        let mut output = Stream::new(self.channels);
+    fn process<'a, 'b, 'c>(&'a self, _: &'b [Sample], outputs: &'c mut Vec<Sample>) -> Result<()> {
+        let mut output = Sample::zeroed(self.channels);
         let sample = self.sample.load(Ordering::Relaxed);
         output.fill(sample);
         outputs.push(output);
 
         let mut samples_since_switch = self.samples_since_switch.load(Ordering::Relaxed);
         let samples_per_switch = self.samples_per_switch.load(Ordering::Relaxed);
         if samples_since_switch >= samples_per_switch {
```

### Comparing `libdaw-0.8.0/libdaw/src/nodes/triangle_oscillator.rs` & `libdaw-0.9.1/libdaw/src/nodes/triangle_oscillator.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use crate::stream::Stream;
+use crate::sample::Sample;
 use crate::sync::AtomicF64;
 use crate::{FrequencyNode, Node, Result};
 
 use std::sync::atomic::Ordering;
 
 #[derive(Debug)]
 pub struct TriangleOscillator {
@@ -43,22 +43,22 @@
     }
     fn get_frequency(&self) -> Result<f64> {
         Ok(self.frequency.load(Ordering::Relaxed))
     }
 }
 
 impl Node for TriangleOscillator {
-    fn process<'a, 'b, 'c>(&'a self, _: &'b [Stream], outputs: &'c mut Vec<Stream>) -> Result<()> {
+    fn process<'a, 'b, 'c>(&'a self, _: &'b [Sample], outputs: &'c mut Vec<Sample>) -> Result<()> {
         let ramp = self.ramp.swap(
             (self.ramp.load(Ordering::Relaxed) + self.delta.load(Ordering::Relaxed)) % 1.0f64,
             Ordering::Relaxed,
         );
         // Builds this pattern:
         // /\
         //   \/
         let sample = (((ramp - 0.25).abs() - 0.5).abs() - 0.25) * 4.0;
-        let mut output = Stream::new(self.channels);
+        let mut output = Sample::zeroed(self.channels);
         output.fill(sample);
         outputs.push(output);
         Ok(())
     }
 }
```

### Comparing `libdaw-0.8.0/libdaw/src/nodes.rs` & `libdaw-0.9.1/libdaw/src/nodes.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/notation/chord/parse.rs` & `libdaw-0.9.1/libdaw/src/notation/chord/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/notation/chord.rs` & `libdaw-0.9.1/libdaw/src/notation/chord.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/notation/duration/parse.rs` & `libdaw-0.9.1/libdaw/src/notation/duration/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/notation/duration.rs` & `libdaw-0.9.1/libdaw/src/notation/duration.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/notation/inversion.rs` & `libdaw-0.9.1/libdaw/src/notation/inversion.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/notation/item/parse.rs` & `libdaw-0.9.1/libdaw/src/notation/item/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/notation/item.rs` & `libdaw-0.9.1/libdaw/src/notation/item.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/notation/note/parse.rs` & `libdaw-0.9.1/libdaw/src/notation/note/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/notation/note.rs` & `libdaw-0.9.1/libdaw/src/notation/note.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/notation/note_pitch.rs` & `libdaw-0.9.1/libdaw/src/notation/note_pitch.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/notation/overlapped/parse.rs` & `libdaw-0.9.1/libdaw/src/notation/overlapped/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/notation/overlapped.rs` & `libdaw-0.9.1/libdaw/src/notation/overlapped.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/notation/pitch/parse.rs` & `libdaw-0.9.1/libdaw/src/notation/pitch/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/notation/pitch.rs` & `libdaw-0.9.1/libdaw/src/notation/pitch.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/notation/rest.rs` & `libdaw-0.9.1/libdaw/src/notation/rest.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/notation/scale/parse.rs` & `libdaw-0.9.1/libdaw/src/notation/scale/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/notation/scale.rs` & `libdaw-0.9.1/libdaw/src/notation/scale.rs`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 use super::{tone_generation_state::ToneGenerationState, NotePitch, Pitch};
 use crate::{
     parse::IResult,
     pitch::{PitchClass, PitchName},
 };
 use nom::{combinator::all_consuming, error::convert_error, Finish as _};
 use std::{
+    ops::RangeBounds,
     str::FromStr,
     sync::{Arc, Mutex},
+    vec::Drain,
 };
 
 #[derive(Debug, Clone)]
 pub struct Scale {
     pitches: Vec<NotePitch>,
 }
 
@@ -72,14 +74,24 @@
                 adjustment: 0.0,
             })),
             octave: Some(4),
             octave_shift: 0,
         })));
         self.pitches = vec![pitch];
     }
+
+    pub fn drain<R>(&mut self, range: R) -> crate::Result<Drain<'_, NotePitch>>
+    where
+        R: RangeBounds<usize>,
+    {
+        if range.contains(&0) && range.contains(&(self.pitches.len() - 1)) {
+            return Err("Can not empty scale".into());
+        }
+        Ok(self.pitches.drain(range))
+    }
 }
 
 impl FromStr for Scale {
     type Err = String;
 
     fn from_str(s: &str) -> Result<Self, Self::Err> {
         let scale = all_consuming(Self::parse)(s)
```

### Comparing `libdaw-0.8.0/libdaw/src/notation/sequence/parse.rs` & `libdaw-0.9.1/libdaw/src/notation/sequence/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/notation/sequence.rs` & `libdaw-0.9.1/libdaw/src/notation/sequence.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/notation/set/parse.rs` & `libdaw-0.9.1/libdaw/src/notation/set/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/notation/set.rs` & `libdaw-0.9.1/libdaw/src/notation/set.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/notation/state_member.rs` & `libdaw-0.9.1/libdaw/src/notation/state_member.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/notation/step/parse.rs` & `libdaw-0.9.1/libdaw/src/notation/step/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/notation/step.rs` & `libdaw-0.9.1/libdaw/src/notation/step.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/notation/tone_generation_state.rs` & `libdaw-0.9.1/libdaw/src/notation/tone_generation_state.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/notation.rs` & `libdaw-0.9.1/libdaw/src/notation.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/parse.rs` & `libdaw-0.9.1/libdaw/src/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/pitch/parse.rs` & `libdaw-0.9.1/libdaw/src/pitch/parse.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/pitch.rs` & `libdaw-0.9.1/libdaw/src/pitch.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/stream/iter.rs` & `libdaw-0.9.1/libdaw/src/sample/iter.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/stream.rs` & `libdaw-0.9.1/libdaw/src/sample.rs`

 * *Files 22% similar despite different names*

```diff
@@ -4,292 +4,276 @@
 
 use std::{
     iter::{Product, Sum},
     ops::{Add, AddAssign, Deref, DerefMut, Mul, MulAssign},
 };
 
 #[derive(Debug, Clone, Default)]
-pub struct Stream {
-    samples: Vec<f64>,
+pub struct Sample {
+    pub channels: Vec<f64>,
 }
 
-impl Stream {
-    pub fn new(channels: usize) -> Self {
+impl Sample {
+    pub fn zeroed(len: usize) -> Self {
         Self {
-            samples: vec![0.0; channels],
+            channels: vec![0.0; len],
         }
     }
-
-    pub fn channels(&self) -> usize {
-        self.samples.len()
-    }
-
-    pub fn resize(&mut self, new_len: usize, value: f64) {
-        self.samples.resize(new_len, value)
-    }
-
-    pub fn resize_with<F>(&mut self, new_len: usize, f: F)
-    where
-        F: FnMut() -> f64,
-    {
-        self.samples.resize_with(new_len, f)
-    }
-
     pub fn iter(&self) -> iter::Iter<'_> {
-        iter::Iter(self.samples.iter())
+        iter::Iter(self.channels.iter())
     }
 }
 
-impl IntoIterator for Stream {
+impl IntoIterator for Sample {
     type Item = f64;
 
     type IntoIter = iter::IntoIter;
 
     fn into_iter(self) -> Self::IntoIter {
-        iter::IntoIter(self.samples.into_iter())
+        iter::IntoIter(self.channels.into_iter())
     }
 }
-impl<'a> IntoIterator for &'a Stream {
+impl<'a> IntoIterator for &'a Sample {
     type Item = &'a f64;
 
     type IntoIter = iter::Iter<'a>;
 
     fn into_iter(self) -> Self::IntoIter {
         self.iter()
     }
 }
 
-impl From<Vec<f64>> for Stream {
+impl From<Vec<f64>> for Sample {
     fn from(samples: Vec<f64>) -> Self {
-        Self { samples }
+        Self { channels: samples }
     }
 }
-impl From<Stream> for Vec<f64> {
-    fn from(value: Stream) -> Self {
-        value.samples
+impl From<Sample> for Vec<f64> {
+    fn from(value: Sample) -> Self {
+        value.channels
     }
 }
 
-impl Deref for Stream {
+impl Deref for Sample {
     type Target = [f64];
 
     fn deref(&self) -> &Self::Target {
-        &self.samples
+        &self.channels
     }
 }
 
-impl DerefMut for Stream {
+impl DerefMut for Sample {
     fn deref_mut(&mut self) -> &mut Self::Target {
-        &mut self.samples
+        &mut self.channels
     }
 }
 
-impl AddAssign<&Stream> for Stream {
-    fn add_assign(&mut self, rhs: &Stream) {
+impl AddAssign<&Sample> for Sample {
+    fn add_assign(&mut self, rhs: &Sample) {
         if self.len() < rhs.len() {
-            self.resize(rhs.len(), 0.0);
+            self.channels.resize(rhs.len(), 0.0);
         }
-        for (l, &r) in self.samples.iter_mut().zip(&rhs.samples) {
+        for (l, &r) in self.channels.iter_mut().zip(&rhs.channels) {
             *l += r;
         }
     }
 }
 
-impl AddAssign for Stream {
+impl AddAssign for Sample {
     fn add_assign(&mut self, rhs: Self) {
         if self.len() < rhs.len() {
-            self.resize(rhs.len(), 0.0);
+            self.channels.resize(rhs.len(), 0.0);
         }
-        for (l, r) in self.samples.iter_mut().zip(rhs.samples) {
+        for (l, r) in self.channels.iter_mut().zip(rhs.channels) {
             *l += r;
         }
     }
 }
-impl Add for &Stream {
-    type Output = Stream;
+impl Add for &Sample {
+    type Output = Sample;
 
-    fn add(self, rhs: &Stream) -> Self::Output {
+    fn add(self, rhs: &Sample) -> Self::Output {
         let mut output = self.clone();
         output += rhs;
         output
     }
 }
 
-impl Add<Stream> for &Stream {
-    type Output = Stream;
+impl Add<Sample> for &Sample {
+    type Output = Sample;
 
-    fn add(self, rhs: Stream) -> Self::Output {
+    fn add(self, rhs: Sample) -> Self::Output {
         let mut output = self.clone();
         output += rhs;
         output
     }
 }
-impl Add<&Stream> for Stream {
-    type Output = Stream;
+impl Add<&Sample> for Sample {
+    type Output = Sample;
 
-    fn add(mut self, rhs: &Stream) -> Self::Output {
+    fn add(mut self, rhs: &Sample) -> Self::Output {
         self += rhs;
         self
     }
 }
 
-impl Add for Stream {
-    type Output = Stream;
+impl Add for Sample {
+    type Output = Sample;
 
-    fn add(mut self, rhs: Stream) -> Self::Output {
+    fn add(mut self, rhs: Sample) -> Self::Output {
         self += rhs;
         self
     }
 }
 
-impl MulAssign<&Stream> for Stream {
-    fn mul_assign(&mut self, rhs: &Stream) {
+impl MulAssign<&Sample> for Sample {
+    fn mul_assign(&mut self, rhs: &Sample) {
         if self.len() < rhs.len() {
-            self.resize(rhs.len(), 0.0);
+            self.channels.resize(rhs.len(), 0.0);
         }
-        for (l, &r) in self.samples.iter_mut().zip(&rhs.samples) {
+        for (l, &r) in self.channels.iter_mut().zip(&rhs.channels) {
             *l *= r;
         }
     }
 }
 
-impl MulAssign for Stream {
+impl MulAssign for Sample {
     fn mul_assign(&mut self, rhs: Self) {
         if self.len() < rhs.len() {
-            self.resize(rhs.len(), 0.0);
+            self.channels.resize(rhs.len(), 0.0);
         }
-        for (l, r) in self.samples.iter_mut().zip(rhs.samples) {
+        for (l, r) in self.channels.iter_mut().zip(rhs.channels) {
             *l *= r;
         }
     }
 }
-impl Mul<&Stream> for &Stream {
-    type Output = Stream;
+impl Mul<&Sample> for &Sample {
+    type Output = Sample;
 
-    fn mul(self, rhs: &Stream) -> Self::Output {
+    fn mul(self, rhs: &Sample) -> Self::Output {
         let mut output = self.clone();
         output *= rhs;
         output
     }
 }
 
-impl Mul<Stream> for &Stream {
-    type Output = Stream;
+impl Mul<Sample> for &Sample {
+    type Output = Sample;
 
-    fn mul(self, rhs: Stream) -> Self::Output {
+    fn mul(self, rhs: Sample) -> Self::Output {
         let mut output = self.clone();
         output *= rhs;
         output
     }
 }
-impl Mul<&Stream> for Stream {
-    type Output = Stream;
+impl Mul<&Sample> for Sample {
+    type Output = Sample;
 
-    fn mul(mut self, rhs: &Stream) -> Self::Output {
+    fn mul(mut self, rhs: &Sample) -> Self::Output {
         self *= rhs;
         self
     }
 }
 
-impl Mul for Stream {
-    type Output = Stream;
+impl Mul for Sample {
+    type Output = Sample;
 
-    fn mul(mut self, rhs: Stream) -> Self::Output {
+    fn mul(mut self, rhs: Sample) -> Self::Output {
         self *= rhs;
         self
     }
 }
 
-impl MulAssign<f64> for Stream {
+impl MulAssign<f64> for Sample {
     fn mul_assign(&mut self, rhs: f64) {
         let rhs = rhs;
-        for l in self.samples.iter_mut() {
+        for l in self.channels.iter_mut() {
             *l *= rhs;
         }
     }
 }
 
-impl Mul<f64> for &Stream {
-    type Output = Stream;
+impl Mul<f64> for &Sample {
+    type Output = Sample;
 
     fn mul(self, rhs: f64) -> Self::Output {
         let mut output = self.clone();
         output *= rhs;
         output
     }
 }
 
-impl Mul<f64> for Stream {
-    type Output = Stream;
+impl Mul<f64> for Sample {
+    type Output = Sample;
 
     fn mul(mut self, rhs: f64) -> Self::Output {
         self *= rhs;
         self
     }
 }
 
-impl Mul<Stream> for f64 {
-    type Output = Stream;
+impl Mul<Sample> for f64 {
+    type Output = Sample;
 
-    fn mul(self, rhs: Stream) -> Self::Output {
+    fn mul(self, rhs: Sample) -> Self::Output {
         rhs * self
     }
 }
 
-impl Mul<&Stream> for f64 {
-    type Output = Stream;
+impl Mul<&Sample> for f64 {
+    type Output = Sample;
 
-    fn mul(self, rhs: &Stream) -> Self::Output {
+    fn mul(self, rhs: &Sample) -> Self::Output {
         rhs * self
     }
 }
 
-impl Sum for Stream {
+impl Sum for Sample {
     fn sum<I>(iter: I) -> Self
     where
         I: Iterator<Item = Self>,
     {
-        let mut output = Stream::new(0);
+        let mut output = Sample::zeroed(0);
         for item in iter {
             output += item;
         }
         output
     }
 }
 
-impl<'a> Sum<&'a Stream> for Stream {
+impl<'a> Sum<&'a Sample> for Sample {
     fn sum<I>(iter: I) -> Self
     where
-        I: Iterator<Item = &'a Stream>,
+        I: Iterator<Item = &'a Sample>,
     {
-        let mut output = Stream::new(0);
+        let mut output = Sample::zeroed(0);
         for item in iter {
             output += item;
         }
         output
     }
 }
-impl Product for Stream {
+impl Product for Sample {
     fn product<I>(iter: I) -> Self
     where
         I: Iterator<Item = Self>,
     {
-        let mut output = Stream::new(0);
+        let mut output = Sample::zeroed(0);
         for item in iter {
             output *= item;
         }
         output
     }
 }
 
-impl<'a> Product<&'a Stream> for Stream {
+impl<'a> Product<&'a Sample> for Sample {
     fn product<I>(iter: I) -> Self
     where
-        I: Iterator<Item = &'a Stream>,
+        I: Iterator<Item = &'a Sample>,
     {
-        let mut output = Stream::new(0);
+        let mut output = Sample::zeroed(0);
         for item in iter {
             output *= item;
         }
         output
     }
 }
```

### Comparing `libdaw-0.8.0/libdaw/src/sync.rs` & `libdaw-0.9.1/libdaw/src/sync.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/time/duration.rs` & `libdaw-0.9.1/libdaw/src/time/duration.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/time/time.rs` & `libdaw-0.9.1/libdaw/src/time/time.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/libdaw/src/time/timestamp.rs` & `libdaw-0.9.1/libdaw/src/time/timestamp.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/.github/workflows/CI.yml` & `libdaw-0.9.1/python-libdaw/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/.gitignore` & `libdaw-0.9.1/python-libdaw/.gitignore`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/docs/Makefile` & `libdaw-0.9.1/python-libdaw/docs/Makefile`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/docs/make.bat` & `libdaw-0.9.1/python-libdaw/docs/make.bat`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/docs/source/conf.py` & `libdaw-0.9.1/python-libdaw/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/examples/1564.py` & `libdaw-0.9.1/python-libdaw/examples/1564.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/examples/blues.py` & `libdaw-0.9.1/python-libdaw/examples/blues.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/examples/instrument-test.py` & `libdaw-0.9.1/python-libdaw/examples/instrument-test.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/examples/pachelbel-canon-progression.py` & `libdaw-0.9.1/python-libdaw/examples/pachelbel-canon-progression.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/examples/round.py` & `libdaw-0.9.1/python-libdaw/examples/round.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/examples/scale-inversion-notation.py` & `libdaw-0.9.1/python-libdaw/examples/scale-inversion-notation.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/examples/simple-notation.py` & `libdaw-0.9.1/python-libdaw/examples/simple-notation.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/examples/simple-scale-notation.py` & `libdaw-0.9.1/python-libdaw/examples/simple-scale-notation.py`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/python/libdaw/__init__.pyi` & `libdaw-0.9.1/python-libdaw/python/libdaw/__init__.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from collections.abc import Sequence
 
-class Stream:
-    def __new__(cls: type, value: int | Sequence[float]):
-        '''Create a new stream with either the number of channels or the given starting values.
+class Sample:
+    def __new__(cls: type, channels: Sequence[float]):
+        '''Create a new sample with the given starting values.
         '''
     def __getitem__(self, index: int) -> float: ...
     def __setitem__(self, index: int, value: float) -> None: ...
     def __len__(self) -> int: ...
     def __str__(self) -> str: ...
-    def __add__(self, other: Stream) -> Stream: ...
-    def __iadd__(self, other: Stream) -> Stream: ...
-    def __mul__(self, other: Stream) -> Stream: ...
-    def __imul__(self, other: Stream) -> Stream: ...
+    def __add__(self, other: Sample) -> Sample: ...
+    def __iadd__(self, other: Sample) -> Sample: ...
+    def __mul__(self, other: Sample) -> Sample: ...
+    def __imul__(self, other: Sample) -> Sample: ...
 
 class Node:
-    def process(self, inputs: Sequence[Stream]) -> Sequence[Stream]: ...
+    def process(self, inputs: Sequence[Sample]) -> Sequence[Sample]: ...
 
 class FrequencyNode(Node):
     @property
     def frequency(self) -> float: ...
 
     @frequency.setter
     def frequency(self, value: float) -> None: ...
```

### Comparing `libdaw-0.8.0/python-libdaw/python/libdaw/metronome.pyi` & `libdaw-0.9.1/python-libdaw/python/libdaw/metronome.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/python/libdaw/nodes/__init__.pyi` & `libdaw-0.9.1/python-libdaw/python/libdaw/nodes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/python/libdaw/notation.pyi` & `libdaw-0.9.1/python-libdaw/python/libdaw/notation.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/python/libdaw/pitch.pyi` & `libdaw-0.9.1/python-libdaw/python/libdaw/pitch.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/python/libdaw/time.pyi` & `libdaw-0.9.1/python-libdaw/python/libdaw/time.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/metronome.rs` & `libdaw-0.9.1/python-libdaw/src/metronome.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/node.rs` & `libdaw-0.9.1/python-libdaw/src/node.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-use crate::{Result, Stream};
+use crate::{Result, Sample};
 use pyo3::{pyclass, pymethods, Bound};
 use std::sync::Arc;
 
 #[derive(Debug, Clone)]
 #[pyclass(subclass, module = "libdaw")]
 pub struct Node(pub Arc<dyn ::libdaw::Node>);
 
 #[pymethods]
 impl Node {
-    pub fn process(&self, inputs: Vec<Bound<'_, Stream>>) -> Result<Vec<Stream>> {
+    pub fn process(&self, inputs: Vec<Bound<'_, Sample>>) -> Result<Vec<Sample>> {
         let mut outputs = Vec::new();
         let inputs: Vec<_> = inputs.into_iter().map(|i| i.borrow().0.clone()).collect();
         self.0.process(&inputs, &mut outputs)?;
-        let outputs: Vec<_> = outputs.into_iter().map(Stream).collect();
+        let outputs: Vec<_> = outputs.into_iter().map(Sample).collect();
         Ok(outputs)
     }
 
     pub fn __repr__(&self) -> String {
         format!("{:?}", (&*self.0))
     }
 
     pub fn __iter__(self_: Bound<'_, Node>) -> Bound<'_, Node> {
         self_
     }
 
-    pub fn __next__(&self) -> Result<Option<Vec<Stream>>> {
+    pub fn __next__(&self) -> Result<Option<Vec<Sample>>> {
         match (&*self.0).next() {
-            Some(outputs) => Ok(Some(outputs?.into_iter().map(Stream).collect())),
+            Some(outputs) => Ok(Some(outputs?.into_iter().map(Sample).collect())),
             None => Ok(None),
         }
     }
 }
```

### Comparing `libdaw-0.8.0/python-libdaw/src/nodes/add.rs` & `libdaw-0.9.1/python-libdaw/src/nodes/add.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/nodes/constant_value.rs` & `libdaw-0.9.1/python-libdaw/src/nodes/constant_value.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/nodes/delay.rs` & `libdaw-0.9.1/python-libdaw/src/nodes/delay.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/nodes/detune.rs` & `libdaw-0.9.1/python-libdaw/src/nodes/detune.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/nodes/envelope.rs` & `libdaw-0.9.1/python-libdaw/src/nodes/envelope.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/nodes/gain.rs` & `libdaw-0.9.1/python-libdaw/src/nodes/gain.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/nodes/graph.rs` & `libdaw-0.9.1/python-libdaw/src/nodes/graph.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/nodes/instrument.rs` & `libdaw-0.9.1/python-libdaw/src/nodes/instrument.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/nodes/multi_frequency.rs` & `libdaw-0.9.1/python-libdaw/src/nodes/multi_frequency.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/nodes/multiply.rs` & `libdaw-0.9.1/python-libdaw/src/nodes/multiply.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/nodes/sawtooth_oscillator.rs` & `libdaw-0.9.1/python-libdaw/src/nodes/sawtooth_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/nodes/sine_oscillator.rs` & `libdaw-0.9.1/python-libdaw/src/nodes/sine_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/nodes/square_oscillator.rs` & `libdaw-0.9.1/python-libdaw/src/nodes/square_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/nodes/triangle_oscillator.rs` & `libdaw-0.9.1/python-libdaw/src/nodes/triangle_oscillator.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/nodes.rs` & `libdaw-0.9.1/python-libdaw/src/nodes.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/notation/chord.rs` & `libdaw-0.9.1/python-libdaw/src/notation/chord.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 use super::{duration::Duration, NotePitch, StateMember};
 use crate::{
+    indexing::{IndexOrSlice, InsertIndex, ItemOrSequence, PopIndex},
     metronome::{Beat, MaybeMetronome},
     nodes::instrument::Tone,
     pitch::MaybePitchStandard,
-    resolve_index, resolve_index_for_insert,
 };
 use libdaw::{metronome::Beat as DawBeat, notation::Chord as DawChord};
 use pyo3::{
-    exceptions::PyIndexError, pyclass, pymethods, Bound, IntoPy as _, Py, PyResult,
-    PyTraverseError, PyVisit, Python,
+    pyclass, pymethods, Bound, IntoPy as _, Py, PyResult, PyTraverseError, PyVisit, Python,
 };
 use std::{
     ops::Deref as _,
     sync::{Arc, Mutex},
 };
 
-#[pyclass(module = "libdaw.notation")]
+#[pyclass(module = "libdaw.notation", sequence)]
 #[derive(Debug, Clone)]
 pub struct Chord {
     pub inner: Arc<Mutex<DawChord>>,
     pub pitches: Vec<NotePitch>,
 }
 
 impl Chord {
@@ -133,26 +132,71 @@
     pub fn __str__(&self) -> String {
         format!("{:#?}", self.inner.lock().expect("poisoned"))
     }
 
     pub fn __len__(&self) -> usize {
         self.pitches.len()
     }
-    pub fn __getitem__(&self, index: isize) -> PyResult<NotePitch> {
-        let index = resolve_index(self.pitches.len(), index)?;
-        Ok(self.pitches[index].clone())
-    }
-    pub fn __setitem__(&mut self, py: Python<'_>, index: isize, value: NotePitch) -> PyResult<()> {
-        let index = resolve_index(self.pitches.len(), index)?;
-        self.inner.lock().expect("poisoned").pitches[index] = value.as_inner(py);
-        self.pitches[index] = value;
-        Ok(())
+    pub fn __getitem__(
+        &self,
+        py: Python<'_>,
+        index: IndexOrSlice<'_>,
+    ) -> PyResult<ItemOrSequence<NotePitch, Self>> {
+        index.get(&self.pitches)?.map_sequence(move |pitches| {
+            let inner_pitches = pitches
+                .iter()
+                .map(move |pitch| pitch.as_inner(py))
+                .collect();
+            let lock = self.inner.lock().expect("poisoned");
+            let inner = Arc::new(Mutex::new(DawChord {
+                length: lock.length,
+                duration: lock.duration,
+                state_member: lock.state_member,
+                pitches: inner_pitches,
+            }));
+            Ok(Self { inner, pitches })
+        })
+    }
+    pub fn __setitem__(
+        &mut self,
+        py: Python<'_>,
+        index: IndexOrSlice<'_>,
+        value: ItemOrSequence<NotePitch>,
+    ) -> PyResult<()> {
+        let len = self.pitches.len();
+        let mut userdata = (self.inner.lock().expect("poisoned"), &mut self.pitches);
+        index.normalize(len)?.set(
+            value,
+            &mut userdata,
+            move |(lock, pitches), index, value| {
+                lock.pitches[index] = value.as_inner(py);
+                pitches[index] = value;
+                Ok(())
+            },
+            move |(lock, pitches), index, value| {
+                lock.pitches.insert(index, value.as_inner(py));
+                pitches.insert(index, value);
+                Ok(())
+            },
+            move |(lock, pitches), range| {
+                lock.pitches.drain(range.clone());
+                pitches.drain(range);
+                Ok(())
+            },
+        )
     }
-    pub fn __delitem__(&mut self, index: isize) -> PyResult<()> {
-        self.pop(Some(index)).map(|_| ())
+    pub fn __delitem__(&mut self, index: IndexOrSlice<'_>) -> PyResult<()> {
+        let len = self.pitches.len();
+        let mut lock = self.inner.lock().expect("poisoned");
+        let pitches = &mut self.pitches;
+        index.normalize(len)?.delete(move |range| {
+            lock.pitches.drain(range.clone());
+            pitches.drain(range);
+            Ok(())
+        })
     }
 
     pub fn __iter__(&self) -> ChordIterator {
         ChordIterator(self.pitches.clone().into_iter())
     }
 
     pub fn append(&mut self, py: Python<'_>, value: NotePitch) -> PyResult<()> {
@@ -161,34 +205,28 @@
             .expect("poisoned")
             .pitches
             .push(value.as_inner(py));
         self.pitches.push(value);
         Ok(())
     }
 
-    pub fn insert(&mut self, py: Python<'_>, index: isize, value: NotePitch) -> PyResult<()> {
-        let index = resolve_index_for_insert(self.pitches.len(), index)?;
+    pub fn insert(&mut self, py: Python<'_>, index: InsertIndex, value: NotePitch) -> PyResult<()> {
+        let index = index.normalize(self.pitches.len())?;
         self.inner
             .lock()
             .expect("poisoned")
             .pitches
             .insert(index, value.as_inner(py));
         self.pitches.insert(index, value);
         Ok(())
     }
 
-    pub fn pop(&mut self, index: Option<isize>) -> PyResult<NotePitch> {
-        let len = self.pitches.len();
-        if len == 0 {
-            return Err(PyIndexError::new_err("Pop from empty"));
-        }
-        let index = match index {
-            Some(index) => resolve_index(len, index)?,
-            None => len - 1,
-        };
+    #[pyo3(signature = (index = Default::default()))]
+    pub fn pop(&mut self, index: PopIndex) -> PyResult<NotePitch> {
+        let index = index.normalize(self.pitches.len())?;
         self.inner.lock().expect("poisoned").pitches.remove(index);
         Ok(self.pitches.remove(index))
     }
     pub fn __getnewargs__(
         &self,
     ) -> (
         Vec<NotePitch>,
```

### Comparing `libdaw-0.8.0/python-libdaw/src/notation/duration.rs` & `libdaw-0.9.1/python-libdaw/src/notation/duration.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/notation/inversion.rs` & `libdaw-0.9.1/python-libdaw/src/notation/inversion.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/notation/item.rs` & `libdaw-0.9.1/python-libdaw/src/notation/item.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 use super::{Chord, Inversion, Note, Overlapped, Rest, Scale, Sequence, Set};
 use crate::Result;
 use libdaw::notation::Item as DawItem;
 use pyo3::{
-    exceptions::PyTypeError, pyfunction, types::PyAnyMethods as _, AsPyPointer, Bound,
-    FromPyObject, IntoPy, Py, PyAny, PyResult, Python,
+    exceptions::PyTypeError,
+    pyfunction,
+    types::{PyAnyMethods as _, PyTypeMethods as _},
+    AsPyPointer, Bound, FromPyObject, IntoPy, Py, PyAny, PyResult, Python,
 };
 
 /// A wrapper enum for converting between Rust Items and the Python classes.
 #[derive(Debug, Clone)]
 pub enum Item {
     Note(Py<Note>),
     Chord(Py<Chord>),
@@ -69,15 +71,19 @@
         } else if let Ok(scale) = value.downcast::<Scale>() {
             Self::Scale(scale.clone().unbind())
         } else if let Ok(inversion) = value.downcast::<Inversion>() {
             Self::Inversion(inversion.clone().unbind())
         } else if let Ok(set) = value.downcast::<Set>() {
             Self::Set(set.clone().unbind())
         } else {
-            return Err(PyTypeError::new_err("Item was invalid type"));
+            let type_ = value.get_type();
+            let type_name = type_.name()?;
+            return Err(PyTypeError::new_err(format!(
+                "Item was invalid type: {type_name}"
+            )));
         })
     }
 }
 
 impl IntoPy<Py<PyAny>> for Item {
     fn into_py(self, py: Python<'_>) -> Py<PyAny> {
         match self {
```

### Comparing `libdaw-0.8.0/python-libdaw/src/notation/note/note_pitch.rs` & `libdaw-0.9.1/python-libdaw/src/notation/note/note_pitch.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/notation/note.rs` & `libdaw-0.9.1/python-libdaw/src/notation/note.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/notation/overlapped.rs` & `libdaw-0.9.1/python-libdaw/src/notation/overlapped.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 use super::{Item, StateMember};
 use crate::{
+    indexing::{IndexOrSlice, InsertIndex, ItemOrSequence, PopIndex},
     metronome::{Beat, MaybeMetronome},
     nodes::instrument::Tone,
     pitch::MaybePitchStandard,
-    resolve_index, resolve_index_for_insert,
 };
 use libdaw::{metronome::Beat as DawBeat, notation::Overlapped as DawOverlapped};
 use pyo3::{
-    exceptions::PyIndexError, pyclass, pymethods, Bound, IntoPy as _, Py, PyResult,
-    PyTraverseError, PyVisit, Python,
+    pyclass, pymethods, Bound, IntoPy as _, Py, PyResult, PyTraverseError, PyVisit, Python,
 };
 use std::{
     ops::Deref as _,
     sync::{Arc, Mutex},
 };
 
-#[pyclass(module = "libdaw.notation")]
+#[pyclass(module = "libdaw.notation", sequence)]
 #[derive(Debug, Clone)]
 pub struct Overlapped {
     pub inner: Arc<Mutex<DawOverlapped>>,
     pub items: Vec<Item>,
 }
 
 impl Overlapped {
@@ -115,26 +114,66 @@
         format!("{:#?}", self.inner.lock().expect("poisoned"))
     }
 
     pub fn __len__(&self) -> usize {
         self.items.len()
     }
 
-    pub fn __getitem__(&self, index: isize) -> PyResult<Item> {
-        let index = resolve_index(self.items.len(), index)?;
-        Ok(self.items[index].clone())
-    }
-    pub fn __setitem__(&mut self, py: Python<'_>, index: isize, value: Item) -> PyResult<()> {
-        let index = resolve_index(self.items.len(), index)?;
-        self.inner.lock().expect("poisoned").items[index] = value.as_inner(py);
-        self.items[index] = value;
-        Ok(())
+    pub fn __getitem__(
+        &self,
+        py: Python<'_>,
+        index: IndexOrSlice<'_>,
+    ) -> PyResult<ItemOrSequence<Item, Self>> {
+        index.get(&self.items)?.map_sequence(move |items| {
+            let inner_items = items.iter().map(move |item| item.as_inner(py)).collect();
+            let lock = self.inner.lock().expect("poisoned");
+            let inner = Arc::new(Mutex::new(DawOverlapped {
+                state_member: lock.state_member,
+                items: inner_items,
+            }));
+            Ok(Self { inner, items })
+        })
     }
-    pub fn __delitem__(&mut self, index: isize) -> PyResult<()> {
-        self.pop(Some(index)).map(|_| ())
+    pub fn __setitem__(
+        &mut self,
+        py: Python<'_>,
+        index: IndexOrSlice<'_>,
+        value: ItemOrSequence<Item>,
+    ) -> PyResult<()> {
+        let len = self.items.len();
+        let mut userdata = (self.inner.lock().expect("poisoned"), &mut self.items);
+        index.normalize(len)?.set(
+            value,
+            &mut userdata,
+            move |(lock, items), index, value| {
+                lock.items[index] = value.as_inner(py);
+                items[index] = value;
+                Ok(())
+            },
+            move |(lock, items), index, value| {
+                lock.items.insert(index, value.as_inner(py));
+                items.insert(index, value);
+                Ok(())
+            },
+            move |(lock, items), range| {
+                lock.items.drain(range.clone());
+                items.drain(range);
+                Ok(())
+            },
+        )
+    }
+    pub fn __delitem__(&mut self, index: IndexOrSlice<'_>) -> PyResult<()> {
+        let len = self.items.len();
+        let mut lock = self.inner.lock().expect("poisoned");
+        let items = &mut self.items;
+        index.normalize(len)?.delete(move |range| {
+            lock.items.drain(range.clone());
+            items.drain(range);
+            Ok(())
+        })
     }
 
     pub fn __iter__(&self) -> OverlappedIterator {
         OverlappedIterator(self.items.clone().into_iter())
     }
 
     pub fn append(&mut self, py: Python<'_>, value: Item) -> PyResult<()> {
@@ -143,35 +182,28 @@
             .expect("poisoned")
             .items
             .push(value.as_inner(py));
         self.items.push(value);
         Ok(())
     }
 
-    pub fn insert(&mut self, py: Python<'_>, index: isize, value: Item) -> PyResult<()> {
-        let index = resolve_index_for_insert(self.items.len(), index)?;
+    pub fn insert(&mut self, py: Python<'_>, index: InsertIndex, value: Item) -> PyResult<()> {
+        let index = index.normalize(self.items.len())?;
         self.inner
             .lock()
             .expect("poisoned")
             .items
             .insert(index, value.as_inner(py));
         self.items.insert(index, value);
         Ok(())
     }
 
-    pub fn pop(&mut self, index: Option<isize>) -> PyResult<Item> {
-        let len = self.items.len();
-        if len == 0 {
-            return Err(PyIndexError::new_err("Pop from empty"));
-        }
-        let index = match index {
-            Some(index) => resolve_index(self.items.len(), index)?,
-            None => len - 1,
-        };
-
+    #[pyo3(signature = (index = Default::default()))]
+    pub fn pop(&mut self, index: PopIndex) -> PyResult<Item> {
+        let index = index.normalize(self.items.len())?;
         self.inner.lock().expect("poisoned").items.remove(index);
         Ok(self.items.remove(index))
     }
 
     pub fn __getnewargs__(&self) -> (Vec<Item>, Option<StateMember>) {
         (
             self.items.clone(),
```

### Comparing `libdaw-0.8.0/python-libdaw/src/notation/pitch.rs` & `libdaw-0.9.1/python-libdaw/src/notation/pitch.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/notation/rest.rs` & `libdaw-0.9.1/python-libdaw/src/notation/rest.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/notation/sequence.rs` & `libdaw-0.9.1/python-libdaw/src/notation/sequence.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 use super::{Item, StateMember};
 use crate::{
+    indexing::{IndexOrSlice, InsertIndex, ItemOrSequence, PopIndex},
     metronome::{Beat, MaybeMetronome},
     nodes::instrument::Tone,
     pitch::MaybePitchStandard,
-    resolve_index, resolve_index_for_insert,
 };
 use libdaw::{metronome::Beat as DawBeat, notation::Sequence as DawSequence};
-use pyo3::{
-    exceptions::PyIndexError, pyclass, pymethods, Bound, IntoPy, Py, PyResult, PyTraverseError,
-    PyVisit, Python,
-};
+use pyo3::{pyclass, pymethods, Bound, IntoPy, Py, PyResult, PyTraverseError, PyVisit, Python};
 use std::{
     ops::Deref,
     sync::{Arc, Mutex},
 };
 
-#[pyclass(module = "libdaw.notation")]
+#[pyclass(module = "libdaw.notation", sequence)]
 #[derive(Debug, Clone)]
 pub struct Sequence {
     pub inner: Arc<Mutex<DawSequence>>,
     pub items: Vec<Item>,
 }
 
 impl Sequence {
@@ -113,27 +110,66 @@
     pub fn __repr__(&self) -> String {
         format!("{:?}", self.inner.lock().expect("poisoned"))
     }
     pub fn __str__(&self) -> String {
         format!("{:#?}", self.inner.lock().expect("poisoned"))
     }
 
-    pub fn __getitem__(&self, index: isize) -> PyResult<Item> {
-        let index = resolve_index(self.items.len(), index)?;
-        Ok(self.items[index].clone())
+    pub fn __getitem__(
+        &self,
+        py: Python<'_>,
+        index: IndexOrSlice<'_>,
+    ) -> PyResult<ItemOrSequence<Item, Self>> {
+        index.get(&self.items)?.map_sequence(move |items| {
+            let inner_items = items.iter().map(move |item| item.as_inner(py)).collect();
+            let lock = self.inner.lock().expect("poisoned");
+            let inner = Arc::new(Mutex::new(DawSequence {
+                state_member: lock.state_member,
+                items: inner_items,
+            }));
+            Ok(Self { inner, items })
+        })
     }
-
-    pub fn __setitem__(&mut self, py: Python<'_>, index: isize, value: Item) -> PyResult<()> {
-        let index = resolve_index(self.items.len(), index)?;
-        self.inner.lock().expect("poisoned").items[index] = value.as_inner(py);
-        self.items[index] = value;
-        Ok(())
+    pub fn __setitem__(
+        &mut self,
+        py: Python<'_>,
+        index: IndexOrSlice<'_>,
+        value: ItemOrSequence<Item>,
+    ) -> PyResult<()> {
+        let len = self.items.len();
+        let mut userdata = (self.inner.lock().expect("poisoned"), &mut self.items);
+        index.normalize(len)?.set(
+            value,
+            &mut userdata,
+            move |(lock, items), index, value| {
+                lock.items[index] = value.as_inner(py);
+                items[index] = value;
+                Ok(())
+            },
+            move |(lock, items), index, value| {
+                lock.items.insert(index, value.as_inner(py));
+                items.insert(index, value);
+                Ok(())
+            },
+            move |(lock, items), range| {
+                lock.items.drain(range.clone());
+                items.drain(range);
+                Ok(())
+            },
+        )
     }
-    pub fn __delitem__(&mut self, index: isize) -> PyResult<()> {
-        self.pop(Some(index)).map(|_| ())
+    pub fn __delitem__(&mut self, index: IndexOrSlice<'_>) -> PyResult<()> {
+        let len = self.items.len();
+        let mut lock = self.inner.lock().expect("poisoned");
+        let items = &mut self.items;
+        index.normalize(len)?.delete(move |range| {
+            lock.items.drain(range.clone());
+            items.drain(range);
+            Ok(())
+        })
     }
 
     pub fn __iter__(&self) -> SequenceIterator {
         SequenceIterator(self.items.clone().into_iter())
     }
 
     pub fn append(&mut self, py: Python<'_>, value: Item) -> PyResult<()> {
@@ -142,35 +178,28 @@
             .expect("poisoned")
             .items
             .push(value.as_inner(py));
         self.items.push(value);
         Ok(())
     }
 
-    pub fn insert(&mut self, py: Python<'_>, index: isize, value: Item) -> PyResult<()> {
-        let index = resolve_index_for_insert(self.items.len(), index)?;
+    pub fn insert(&mut self, py: Python<'_>, index: InsertIndex, value: Item) -> PyResult<()> {
+        let index = index.normalize(self.items.len())?;
         self.inner
             .lock()
             .expect("poisoned")
             .items
             .insert(index, value.as_inner(py));
         self.items.insert(index, value);
         Ok(())
     }
 
-    pub fn pop(&mut self, index: Option<isize>) -> PyResult<Item> {
-        let len = self.items.len();
-        if len == 0 {
-            return Err(PyIndexError::new_err("Pop from empty"));
-        }
-        let index = match index {
-            Some(index) => resolve_index(self.items.len(), index)?,
-            None => len - 1,
-        };
-
+    #[pyo3(signature = (index = Default::default()))]
+    pub fn pop(&mut self, index: PopIndex) -> PyResult<Item> {
+        let index = index.normalize(self.items.len())?;
         self.inner.lock().expect("poisoned").items.remove(index);
         Ok(self.items.remove(index))
     }
     pub fn __getnewargs__(&self) -> (Vec<Item>, Option<StateMember>) {
         (
             self.items.clone(),
             self.inner
```

### Comparing `libdaw-0.8.0/python-libdaw/src/notation/set.rs` & `libdaw-0.9.1/python-libdaw/src/notation/set.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/notation/state_member.rs` & `libdaw-0.9.1/python-libdaw/src/notation/state_member.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/notation/step.rs` & `libdaw-0.9.1/python-libdaw/src/notation/step.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/notation.rs` & `libdaw-0.9.1/python-libdaw/src/notation.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/pitch/pitch.rs` & `libdaw-0.9.1/python-libdaw/src/pitch/pitch.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/pitch.rs` & `libdaw-0.9.1/python-libdaw/src/pitch.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python-libdaw/src/play.rs` & `libdaw-0.9.1/python-libdaw/src/play.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 use crate::Node;
-use libdaw::Stream;
+use libdaw::Sample;
 use pyo3::{pyfunction, Bound, Python};
 use rodio::{OutputStream, Sink};
 use std::sync::mpsc::{sync_channel, Receiver};
 
 /// Rodio audio source
 #[derive(Debug)]
 pub struct Source {
     sample_rate: u32,
     channels: u16,
-    receiver: Receiver<Stream>,
-    sample: <Stream as IntoIterator>::IntoIter,
+    receiver: Receiver<Sample>,
+    sample: <Sample as IntoIterator>::IntoIter,
 }
 
 impl Source {
     fn refresh(&mut self) {
         if self.sample.len() == 0 {
             if let Ok(sample) = self.receiver.recv() {
                 self.sample = sample.into_iter();
@@ -62,26 +62,26 @@
     let sink = Sink::try_new(&stream_handle)?;
     let (sender, receiver) = sync_channel(sample_rate as usize * 10);
     sink.append(Source {
         sample_rate,
         channels,
         receiver,
         // The initial sample is empty.
-        sample: Stream::default().into_iter(),
+        sample: Sample::default().into_iter(),
     });
     let node = node.borrow().0.clone();
     let mut outputs = Vec::new();
     loop {
         py.check_signals()?;
         outputs.clear();
         node.process(&[], &mut outputs)?;
         let sample = outputs
             .iter()
             .fold(None, move |acc, stream| match acc {
                 Some(acc) => Some(acc + stream),
                 None => Some(stream.clone()),
             })
-            .unwrap_or_else(move || Stream::new(channels as usize));
+            .unwrap_or_else(move || Sample::zeroed(channels as usize));
 
         sender.send(sample)?;
     }
 }
```

### Comparing `libdaw-0.8.0/python-libdaw/src/time.rs` & `libdaw-0.9.1/python-libdaw/src/time.rs`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/Cargo.lock` & `libdaw-0.9.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
 name = "libc"
 version = "0.2.155"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "97b3888a4aecf77e811145cadf6eef5901f4782c53886191b2f693f24761847c"
 
 [[package]]
 name = "libdaw"
-version = "0.8.0"
+version = "0.9.1"
 dependencies = [
  "nohash-hasher",
  "nom",
  "ordered-float",
 ]
 
 [[package]]
@@ -665,15 +665,15 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "python-libdaw"
-version = "0.8.0"
+version = "0.9.1"
 dependencies = [
  "libdaw",
  "nohash-hasher",
  "pyo3",
  "rodio",
 ]
```

### Comparing `libdaw-0.8.0/pyproject.toml` & `libdaw-0.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python/libdaw/notation.pyi` & `libdaw-0.9.1/python/libdaw/notation.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python/libdaw/pitch.pyi` & `libdaw-0.9.1/python/libdaw/pitch.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python/libdaw/time.pyi` & `libdaw-0.9.1/python/libdaw/time.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python/libdaw/__init__.pyi` & `libdaw-0.9.1/python/libdaw/__init__.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from collections.abc import Sequence
 
-class Stream:
-    def __new__(cls: type, value: int | Sequence[float]):
-        '''Create a new stream with either the number of channels or the given starting values.
+class Sample:
+    def __new__(cls: type, channels: Sequence[float]):
+        '''Create a new sample with the given starting values.
         '''
     def __getitem__(self, index: int) -> float: ...
     def __setitem__(self, index: int, value: float) -> None: ...
     def __len__(self) -> int: ...
     def __str__(self) -> str: ...
-    def __add__(self, other: Stream) -> Stream: ...
-    def __iadd__(self, other: Stream) -> Stream: ...
-    def __mul__(self, other: Stream) -> Stream: ...
-    def __imul__(self, other: Stream) -> Stream: ...
+    def __add__(self, other: Sample) -> Sample: ...
+    def __iadd__(self, other: Sample) -> Sample: ...
+    def __mul__(self, other: Sample) -> Sample: ...
+    def __imul__(self, other: Sample) -> Sample: ...
 
 class Node:
-    def process(self, inputs: Sequence[Stream]) -> Sequence[Stream]: ...
+    def process(self, inputs: Sequence[Sample]) -> Sequence[Sample]: ...
 
 class FrequencyNode(Node):
     @property
     def frequency(self) -> float: ...
 
     @frequency.setter
     def frequency(self, value: float) -> None: ...
```

### Comparing `libdaw-0.8.0/python/libdaw/metronome.pyi` & `libdaw-0.9.1/python/libdaw/metronome.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/python/libdaw/nodes/__init__.pyi` & `libdaw-0.9.1/python/libdaw/nodes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `libdaw-0.8.0/PKG-INFO` & `libdaw-0.9.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: libdaw
-Version: 0.8.0
+Version: 0.9.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 License: MPL 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

