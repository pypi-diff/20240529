# Comparing `tmp/youqu-2.6.1.tar.gz` & `tmp/youqu-2.6.2.tar.gz`

## Comparing `youqu-2.6.1.tar` & `youqu-2.6.2.tar`

### file list

```diff
@@ -1,228 +1,223 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/CURRENT
--rw-r--r--   0        0        0    41974 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/conftest.py
--rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/env.sh
--rw-r--r--   0        0        0     3703 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/manage.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/pytest.ini
--rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/ruff.toml
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/startproject.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/apps/__init__.py
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/__init__.py
--rw-r--r--   0        0        0    11047 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/globalconfig.ini
--rw-r--r--   0        0        0    11354 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/globalconfig.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/playbook.toml
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/pmsmark.ini
--rw-r--r--   0        0        0    20451 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/pylintrc.cfg
--rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/skipif.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/sleepx.ini
--rw-r--r--   0        0        0      226 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/subcmd.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/ci.json
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/language.ini
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/${app_name}_assert.py-tpl
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/.gitignore-tpl
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/__init__.py-tpl
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/config.ini-tpl
--rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/config.py-tpl
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/conftest.py-tpl
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/control-tpl
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/mycase.csv-tpl
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/case/__init__.py-tpl
--rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/case/base_case.py-tpl
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/case/test_mycase_001.py-tpl
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/case/test_mycase_002.py-tpl
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/case/assert_res/readme
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/widget/${app_name}_widget.py-tpl
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/widget/__init__.py-tpl
--rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/widget/base_widget.py-tpl
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/widget/other.ini-tpl
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/widget/other_widget.py-tpl
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/widget/ui.ini-tpl
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/widget/case_res/readme
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/setting/template/app_template/widget/pic_res/readme
--rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/__init__.py
--rw-r--r--   0        0        0    18200 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/assert_common.py
--rw-r--r--   0        0        0    26404 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/button_center.py
--rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/calculate.py
--rw-r--r--   0        0        0     8407 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/cmdctl.py
--rw-r--r--   0        0        0     6975 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/csvctl.py
--rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/custom_exception.py
--rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/dbus_utils.py
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/desktop.py
--rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/dogtail_utils.py
--rw-r--r--   0        0        0    10856 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/filectl.py
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/filter_image.py
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/image_utils.py
--rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/mouse_key.py
--rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/ocr_utils.py
--rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/pinyin.py
--rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/read_csv.py
--rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/read_toml.py
--rw-r--r--   0        0        0     3672 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/recording_screen.py
--rw-r--r--   0        0        0     2185 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/requestx.py
--rw-r--r--   0        0        0    15610 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/shortcut.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/singleton.py
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/sleepx.py
--rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/startapp.py
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/startproject.py
--rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/video_utils.py
--rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/wayland_wininfo.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/webui.py
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/ydotool.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/__init__.py
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/__init__.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/__version__.py
--rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/cli.py
--rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/colors.py
--rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/consts.py
--rw-r--r--   0        0        0    12752 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/core.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/py.typed
--rw-r--r--   0        0        0    29547 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/fonts/3d.json
--rw-r--r--   0        0        0    16516 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/fonts/block.json
--rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/fonts/chrome.json
--rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/fonts/grid.json
--rw-r--r--   0        0        0    37089 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/fonts/huge.json
--rw-r--r--   0        0        0    13028 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/fonts/pallet.json
--rw-r--r--   0        0        0    15470 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/fonts/shade.json
--rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/fonts/simple.json
--rw-r--r--   0        0        0     8083 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/fonts/simple3d.json
--rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/fonts/simpleBlock.json
--rw-r--r--   0        0        0    13027 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/fonts/slick.json
--rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/cfonts/fonts/tiny.json
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/colorama/__init__.py
--rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/colorama/ansi.py
--rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/colorama/ansitowin32.py
--rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/colorama/initialise.py
--rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/colorama/win32.py
--rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/colorama/winterm.py
--rw-r--r--   0        0        0    18011 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/COPYING
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/__init__.py
--rw-r--r--   0        0        0     8012 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/config.py
--rw-r--r--   0        0        0    12153 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/distro.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/dump.py
--rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/errors.py
--rw-r--r--   0        0        0     9448 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/i18n.py
--rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/logging.py
--rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/path.py
--rw-r--r--   0        0        0    15256 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/predicate.py
--rw-r--r--   0        0        0    13055 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/procedural.py
--rw-r--r--   0        0        0     9565 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/rawinput.py
--rw-r--r--   0        0        0    17581 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/rawinput_wayland.py
--rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/sessions.py
--rw-r--r--   0        0        0     7988 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/tc.py
--rw-r--r--   0        0        0    48139 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/tree.py
--rw-r--r--   0        0        0    16049 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/utils.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/version.py
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/wrapped.py
--rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/icons/dogtail-head-48.png
--rw-r--r--   0        0        0    55404 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/icons/dogtail-head.svg
--rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/icons/dogtail-tail-48.png
--rw-r--r--   0        0        0    29904 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/dogtail/icons/dogtail-tail.svg
--rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/pyautogui/LICENSE.txt
--rw-r--r--   0        0        0    78875 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/pyautogui/__init__.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/pyautogui/__main__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/pyautogui/_pyautogui_java.py
--rw-r--r--   0        0        0    14827 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/pyautogui/_pyautogui_osx.py
--rw-r--r--   0        0        0    17011 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/pyautogui/_pyautogui_wayland.py
--rw-r--r--   0        0        0    20065 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/pyautogui/_pyautogui_win.py
--rw-r--r--   0        0        0    15261 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/pyautogui/_pyautogui_x11.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/pygtkcompat/__init__.py
--rw-r--r--   0        0        0    14200 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/pygtkcompat/generictreemodel.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/pygtkcompat/meson.build
--rw-r--r--   0        0        0    20672 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/pygtkcompat/pygtkcompat.py
--rwxr-xr-x   0        0        0    30155 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/sniff
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/sniff.desktop
--rw-r--r--   0        0        0    20943 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/sniff.ui
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/button.xpm
--rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/checkbutton.xpm
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/checkmenuitem.xpm
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/colorselection.xpm
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/combo.xpm
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/dialog.xpm
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/image.xpm
--rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/label.xpm
--rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/menubar.xpm
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/menuitem.xpm
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/notebook.xpm
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/scrolledwindow.xpm
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/spinbutton.xpm
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/statusbar.xpm
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/table.xpm
--rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/text.xpm
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/toolbar.xpm
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/tree.xpm
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/treeitem.xpm
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/unknown.xpm
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/viewport.xpm
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/vscrollbar.xpm
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/vseparator.xpm
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/sniff/icons/window.xpm
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/wayland_autotool/CMakeLists.txt
--rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/wayland_autotool/README.md
--rw-r--r--   0        0        0     9324 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/wayland_autotool/autotool.cpp
--rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/wayland_autotool/autotool.h
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/wayland_autotool/install.sh
--rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/wayland_autotool/main.cpp
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/.editorconfig
--rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/CMakeLists.txt
--rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/LICENSE
--rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/Client/tool_click.c
--rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/Client/tool_key.c
--rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/Client/tool_mousemove.c
--rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/Client/tool_type.c
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/Client/ydotool.c
--rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/Client/ydotool.h
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/Daemon/CMakeLists.txt
--rwxr-xr-x   0        0        0      223 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/Daemon/ydotool.service-openrc.in
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/Daemon/ydotool.service.in
--rw-r--r--   0        0        0    16544 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/Daemon/ydotoold.c
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/manpage/CMakeLists.txt
--rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/manpage/ydotool.1.scd
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/depends/ydotool/manpage/ydotoold.8.scd
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/git/__init__.py
--rw-r--r--   0        0        0     2230 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/git/_cargo.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/git/check.py
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/git/clone.py
--rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/git/code_statistics.py
--rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/git/commit.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/plugins/__init__.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/plugins/allure_report_extend.py
--rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/plugins/emoji_hooks.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/plugins/mng.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/pms/__init__.py
--rw-r--r--   0        0        0     4725 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/pms/_base.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/pms/_cargo.py
--rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/pms/csv2pms.py
--rw-r--r--   0        0        0    11725 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/pms/pms2csv.py
--rw-r--r--   0        0        0     5574 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/pms/send2pms.py
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/pms/suite.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/pms/task.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/remotectl/__init__.py
--rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/remotectl/_base.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/remotectl/_remote_dogtail_ctl.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/remotectl/_remote_other_ctl.py
--rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/remotectl/remote.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/rtk/__init__.py
--rw-r--r--   0        0        0     3839 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/rtk/_base.py
--rw-r--r--   0        0        0    11436 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/rtk/_cargo.py
--rw-r--r--   0        0        0    16780 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/rtk/local_runner.py
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/rtk/playbook.py
--rw-r--r--   0        0        0    21570 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/rtk/remote_runner.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/__init__.py
--rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/_env_base.sh
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/check_python_source.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/command_complete.sh
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/docs_env.sh
--rwxr-xr-x   0        0        0     3274 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/env_dev.sh
--rw-r--r--   0        0        0     5836 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/env_vir.sh
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/opencv_rpc_server.py
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/pylint.sh
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/sslclone.sh
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/sub_deb.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/sub_depends.py
--rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/sub_env_cut.py
--rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/sub_remote.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/sub_sources.py
--rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/sub_webui.py
--rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/src/utils/vnc.sh
--rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 youqu-2.6.1/pyproject.toml
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 youqu-2.6.1/youqu/README.md
--rw-r--r--   0        0        0     5645 2020-02-02 00:00:00.000000 youqu-2.6.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/CURRENT
+-rw-r--r--   0        0        0    42855 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/conftest.py
+-rw-r--r--   0        0        0     1715 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/env.sh
+-rw-r--r--   0        0        0     3458 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/manage.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/pytest.ini
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/startproject.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/apps/__init__.py
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/__init__.py
+-rw-r--r--   0        0        0    11027 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/globalconfig.ini
+-rw-r--r--   0        0        0    11354 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/globalconfig.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/pmsmark.ini
+-rw-r--r--   0        0        0    20451 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/pylintrc.cfg
+-rw-r--r--   0        0        0     2953 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/skipif.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/sleepx.ini
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/template/ci.json
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/template/language.ini
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/template/app_template/${app_name}_assert.py-tpl
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/template/app_template/.gitignore-tpl
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/template/app_template/__init__.py-tpl
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/template/app_template/config.ini-tpl
+-rw-r--r--   0        0        0     2619 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/template/app_template/config.py-tpl
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/template/app_template/conftest.py-tpl
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/template/app_template/control-tpl
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/template/app_template/mycase.csv-tpl
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/template/app_template/case/__init__.py-tpl
+-rw-r--r--   0        0        0      255 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/template/app_template/case/base_case.py-tpl
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/template/app_template/case/test_mycase_001.py-tpl
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/template/app_template/case/test_mycase_002.py-tpl
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/template/app_template/case/assert_res/readme
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/template/app_template/widget/${app_name}_widget.py-tpl
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/template/app_template/widget/__init__.py-tpl
+-rw-r--r--   0        0        0     2324 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/template/app_template/widget/base_widget.py-tpl
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/template/app_template/widget/other.ini-tpl
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/template/app_template/widget/other_widget.py-tpl
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/template/app_template/widget/ui.ini-tpl
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/template/app_template/widget/case_res/readme
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/setting/template/app_template/widget/pic_res/readme
+-rw-r--r--   0        0        0     2109 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/__init__.py
+-rw-r--r--   0        0        0    18200 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/assert_common.py
+-rw-r--r--   0        0        0    26404 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/button_center.py
+-rw-r--r--   0        0        0     1700 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/calculate.py
+-rw-r--r--   0        0        0     8572 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/cmdctl.py
+-rw-r--r--   0        0        0     6975 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/csvctl.py
+-rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/custom_exception.py
+-rw-r--r--   0        0        0     2921 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/dbus_utils.py
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/desktop.py
+-rw-r--r--   0        0        0     7644 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/dogtail_utils.py
+-rw-r--r--   0        0        0    10856 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/filectl.py
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/filter_image.py
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/image_utils.py
+-rw-r--r--   0        0        0    14377 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/mouse_key.py
+-rw-r--r--   0        0        0     3785 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/ocr_utils.py
+-rw-r--r--   0        0        0      798 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/pinyin.py
+-rw-r--r--   0        0        0     1330 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/read_csv.py
+-rw-r--r--   0        0        0      417 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/read_toml.py
+-rw-r--r--   0        0        0     3672 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/recording_screen.py
+-rw-r--r--   0        0        0     2654 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/requestx.py
+-rw-r--r--   0        0        0    15927 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/shortcut.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/singleton.py
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/sleepx.py
+-rw-r--r--   0        0        0     4348 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/startapp.py
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/startproject.py
+-rw-r--r--   0        0        0     1167 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/video_utils.py
+-rw-r--r--   0        0        0     5039 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/wayland_wininfo.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/webui.py
+-rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/ydotool.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/__init__.py
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/cfonts/__init__.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/cfonts/__version__.py
+-rw-r--r--   0        0        0     4783 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/cfonts/cli.py
+-rw-r--r--   0        0        0     6451 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/cfonts/colors.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/cfonts/consts.py
+-rw-r--r--   0        0        0    12752 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/cfonts/core.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/cfonts/py.typed
+-rw-r--r--   0        0        0    29547 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/cfonts/fonts/3d.json
+-rw-r--r--   0        0        0    16516 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/cfonts/fonts/block.json
+-rw-r--r--   0        0        0     4771 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/cfonts/fonts/chrome.json
+-rw-r--r--   0        0        0    11811 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/cfonts/fonts/grid.json
+-rw-r--r--   0        0        0    37089 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/cfonts/fonts/huge.json
+-rw-r--r--   0        0        0    13028 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/cfonts/fonts/pallet.json
+-rw-r--r--   0        0        0    15470 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/cfonts/fonts/shade.json
+-rw-r--r--   0        0        0     3896 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/cfonts/fonts/simple.json
+-rw-r--r--   0        0        0     8083 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/cfonts/fonts/simple3d.json
+-rw-r--r--   0        0        0     7299 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/cfonts/fonts/simpleBlock.json
+-rw-r--r--   0        0        0    13027 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/cfonts/fonts/slick.json
+-rw-r--r--   0        0        0     2568 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/cfonts/fonts/tiny.json
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/colorama/__init__.py
+-rw-r--r--   0        0        0     2522 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/colorama/ansi.py
+-rw-r--r--   0        0        0    11128 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/colorama/ansitowin32.py
+-rw-r--r--   0        0        0     3325 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/colorama/initialise.py
+-rw-r--r--   0        0        0     6181 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/colorama/win32.py
+-rw-r--r--   0        0        0     7134 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/colorama/winterm.py
+-rw-r--r--   0        0        0    18011 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/dogtail/COPYING
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/dogtail/__init__.py
+-rw-r--r--   0        0        0     8012 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/dogtail/config.py
+-rw-r--r--   0        0        0    12153 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/dogtail/distro.py
+-rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/dogtail/dump.py
+-rw-r--r--   0        0        0      751 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/dogtail/errors.py
+-rw-r--r--   0        0        0     9448 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/dogtail/i18n.py
+-rw-r--r--   0        0        0     7191 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/dogtail/logging.py
+-rw-r--r--   0        0        0     3333 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/dogtail/path.py
+-rw-r--r--   0        0        0    15256 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/dogtail/predicate.py
+-rw-r--r--   0        0        0    13055 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/dogtail/procedural.py
+-rw-r--r--   0        0        0     9565 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/dogtail/rawinput.py
+-rw-r--r--   0        0        0    17581 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/dogtail/rawinput_wayland.py
+-rw-r--r--   0        0        0     7063 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/dogtail/sessions.py
+-rw-r--r--   0        0        0     7988 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/dogtail/tc.py
+-rw-r--r--   0        0        0    48139 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/dogtail/tree.py
+-rw-r--r--   0        0        0    16049 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/dogtail/utils.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/dogtail/version.py
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/dogtail/wrapped.py
+-rw-r--r--   0        0        0     2759 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/dogtail/icons/dogtail-head-48.png
+-rw-r--r--   0        0        0    55404 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/dogtail/icons/dogtail-head.svg
+-rw-r--r--   0        0        0     2462 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/dogtail/icons/dogtail-tail-48.png
+-rw-r--r--   0        0        0    29904 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/dogtail/icons/dogtail-tail.svg
+-rw-r--r--   0        0        0     1481 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/pyautogui/LICENSE.txt
+-rw-r--r--   0        0        0    78875 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/pyautogui/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/pyautogui/__main__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/pyautogui/_pyautogui_java.py
+-rw-r--r--   0        0        0    14827 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/pyautogui/_pyautogui_osx.py
+-rw-r--r--   0        0        0    17011 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/pyautogui/_pyautogui_wayland.py
+-rw-r--r--   0        0        0    20065 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/pyautogui/_pyautogui_win.py
+-rw-r--r--   0        0        0    15261 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/pyautogui/_pyautogui_x11.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/pygtkcompat/__init__.py
+-rw-r--r--   0        0        0    14200 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/pygtkcompat/generictreemodel.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/pygtkcompat/meson.build
+-rw-r--r--   0        0        0    20672 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/pygtkcompat/pygtkcompat.py
+-rwxr-xr-x   0        0        0    30155 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/sniff/sniff
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/sniff/sniff.desktop
+-rw-r--r--   0        0        0    20943 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/sniff/sniff.ui
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/sniff/icons/button.xpm
+-rw-r--r--   0        0        0      725 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/sniff/icons/checkbutton.xpm
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/sniff/icons/checkmenuitem.xpm
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/sniff/icons/colorselection.xpm
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/sniff/icons/combo.xpm
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/sniff/icons/dialog.xpm
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/sniff/icons/image.xpm
+-rw-r--r--   0        0        0      674 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/sniff/icons/label.xpm
+-rw-r--r--   0        0        0      735 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/sniff/icons/menubar.xpm
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/sniff/icons/menuitem.xpm
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/sniff/icons/notebook.xpm
+-rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/sniff/icons/scrolledwindow.xpm
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/sniff/icons/spinbutton.xpm
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/sniff/icons/statusbar.xpm
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/sniff/icons/table.xpm
+-rw-r--r--   0        0        0      705 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/sniff/icons/text.xpm
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/sniff/icons/toolbar.xpm
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/sniff/icons/tree.xpm
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/sniff/icons/treeitem.xpm
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/sniff/icons/unknown.xpm
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/sniff/icons/viewport.xpm
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/sniff/icons/vscrollbar.xpm
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/sniff/icons/vseparator.xpm
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/sniff/icons/window.xpm
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/wayland_autotool/CMakeLists.txt
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/wayland_autotool/README.md
+-rw-r--r--   0        0        0     9324 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/wayland_autotool/autotool.cpp
+-rw-r--r--   0        0        0     2929 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/wayland_autotool/autotool.h
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/wayland_autotool/install.sh
+-rw-r--r--   0        0        0      844 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/wayland_autotool/main.cpp
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/ydotool/.editorconfig
+-rw-r--r--   0        0        0     1277 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/ydotool/CMakeLists.txt
+-rw-r--r--   0        0        0    34523 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/ydotool/LICENSE
+-rw-r--r--   0        0        0     4536 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/ydotool/Client/tool_click.c
+-rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/ydotool/Client/tool_key.c
+-rw-r--r--   0        0        0     4174 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/ydotool/Client/tool_mousemove.c
+-rw-r--r--   0        0        0     8344 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/ydotool/Client/tool_type.c
+-rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/ydotool/Client/ydotool.c
+-rw-r--r--   0        0        0     2363 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/ydotool/Client/ydotool.h
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/ydotool/Daemon/CMakeLists.txt
+-rwxr-xr-x   0        0        0      223 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/ydotool/Daemon/ydotool.service-openrc.in
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/ydotool/Daemon/ydotool.service.in
+-rw-r--r--   0        0        0    16544 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/ydotool/Daemon/ydotoold.c
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/ydotool/manpage/CMakeLists.txt
+-rw-r--r--   0        0        0     3262 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/ydotool/manpage/ydotool.1.scd
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/depends/ydotool/manpage/ydotoold.8.scd
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/git/__init__.py
+-rw-r--r--   0        0        0     2278 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/git/_cargo.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/git/check.py
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/git/clone.py
+-rw-r--r--   0        0        0     8733 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/git/code_statistics.py
+-rw-r--r--   0        0        0     2496 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/git/commit.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/plugins/__init__.py
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/plugins/allure_report_extend.py
+-rw-r--r--   0        0        0      967 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/plugins/emoji_hooks.py
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/plugins/mng.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/pms/__init__.py
+-rw-r--r--   0        0        0     3826 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/pms/_base.py
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/pms/_cargo.py
+-rw-r--r--   0        0        0     4403 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/pms/csv2pms.py
+-rw-r--r--   0        0        0    11725 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/pms/pms2csv.py
+-rw-r--r--   0        0        0     5574 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/pms/send2pms.py
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/pms/suite.py
+-rw-r--r--   0        0        0     1514 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/pms/task.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/remotectl/__init__.py
+-rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/remotectl/_base.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/remotectl/_remote_dogtail_ctl.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/remotectl/_remote_other_ctl.py
+-rw-r--r--   0        0        0     2836 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/remotectl/remote.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/rtk/__init__.py
+-rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/rtk/_base.py
+-rw-r--r--   0        0        0    11384 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/rtk/_cargo.py
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/rtk/api_client.py
+-rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/rtk/json_backfill.py
+-rw-r--r--   0        0        0    17068 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/rtk/local_runner.py
+-rw-r--r--   0        0        0    25258 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/rtk/remote_runner.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/utils/__init__.py
+-rw-r--r--   0        0        0     4341 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/utils/_env_base.sh
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/utils/check_python_source.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/utils/command_complete.sh
+-rwxr-xr-x   0        0        0     3274 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/utils/env_dev.sh
+-rw-r--r--   0        0        0     5617 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/utils/env_vir.sh
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/utils/pylint.sh
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/utils/sslclone.sh
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/utils/sub_deb.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/utils/sub_depends.py
+-rw-r--r--   0        0        0      448 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/utils/sub_env_cut.py
+-rw-r--r--   0        0        0      390 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/utils/sub_remote.py
+-rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/utils/sub_sources.py
+-rw-r--r--   0        0        0      389 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/src/utils/sub_webui.py
+-rw-r--r--   0        0        0     1292 2020-02-02 00:00:00.000000 youqu-2.6.2/pyproject.toml
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 youqu-2.6.2/youqu/README.md
+-rw-r--r--   0        0        0     5645 2020-02-02 00:00:00.000000 youqu-2.6.2/PKG-INFO
```

### Comparing `youqu-2.6.1/youqu/conftest.py` & `youqu-2.6.2/youqu/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,37 +21,43 @@
         sys.path.append(i.value)
 
 from os import system
 from os import remove
 from os import makedirs
 from os import walk
 from os.path import exists
+from os.path import join
 from os.path import splitext
 from enum import Enum
 from time import sleep
-from collections import deque
+from collections import deque, Counter
 from datetime import datetime
 from json import dumps
 from re import findall
 from shutil import copyfile
 from multiprocessing import Process
 from concurrent.futures import wait
 from concurrent.futures import ThreadPoolExecutor
 from concurrent.futures import ALL_COMPLETED
 
-import letmego
 import allure
 import pytest
 from _pytest.mark import Mark
 from _pytest.terminal import TerminalReporter
 from funnylog.conf import setting as log_setting
 
-letmego.conf.setting.PASSWORD = GlobalConfig.PASSWORD
-letmego.conf.setting.RUNNING_MAN_FILE = f"{GlobalConfig.REPORT_PATH}/_running_man.log"
-letmego.conf.setting.DEBUG = GlobalConfig.LETMEGO_DEBUG
+try:
+    import letmego
+
+    HAS_LETMEGO = True
+    letmego.conf.setting.PASSWORD = GlobalConfig.PASSWORD
+    letmego.conf.setting.RUNNING_MAN_FILE = f"{GlobalConfig.REPORT_PATH}/_running_man.log"
+    letmego.conf.setting.DEBUG = GlobalConfig.LETMEGO_DEBUG
+except ModuleNotFoundError:
+    HAS_LETMEGO = False
 
 log_setting.LOG_FILE_PATH = GlobalConfig.REPORT_PATH
 log_setting.CLASS_NAME_STARTSWITH = GlobalConfig.CLASS_NAME_STARTSWITH
 log_setting.CLASS_NAME_ENDSWITH = GlobalConfig.CLASS_NAME_ENDSWITH
 log_setting.CLASS_NAME_CONTAIN = GlobalConfig.CLASS_NAME_CONTAIN
 
 from setting import skipif
@@ -141,15 +147,15 @@
     parser.addoption("--slaves", action="store", default="", help="远程测试机")
     parser.addoption(
         "--autostart", action="store", default="", help="重启类场景开启letmego执行方案"
     )
 
 
 def pytest_cmdline_main(config):
-    # 初始化log配置，以解决allure报告日志格式问题
+    # 初始化log配置，以解决html报告日志格式问题
     log_info = logger(config.option.log_level)
     config.option.log_level = config.option.log_level
     config.option.log_format = log_info.log_format
     config.option.log_date_format = log_info.date_format
 
 
 def pytest_addhooks(pluginmanager):
@@ -309,15 +315,15 @@
                 for index, title in enumerate(txt_list[0].strip().split(",")):
                     if title.strip() == FixedCsvTitle.skip_reason.value:
                         skip_index = index - 1
                     elif title.strip() == FixedCsvTitle.fixed.value:
                         fixed_index = index - 1
                     elif title.strip() == FixedCsvTitle.removed.value:
                         removed_index = index - 1
-                    elif title.strip() == FixedCsvTitle.pms_case_id.value:
+                    elif title.strip() == FixedCsvTitle.pms_case_id.value.strip("*"):
                         pms_id_index = index - 1
 
                 taglines = [txt.strip().split(",") for txt in txt_list[1:]]
                 id_tags_dict = {f"{int(i[0]):0>3}": i[1:] for i in taglines if i[0]}
                 # 每个csv文件单独管理一套index
                 containers[csv_path] = id_tags_dict
                 containers[csv_path][ConfStr.SKIP_INDEX.value] = skip_index
@@ -430,16 +436,17 @@
                     session.items.remove(item)
 
     if session.config.option.autostart:
         for item in session.items[::-1]:
             _reruns = None
             if hasattr(session.config.option, "reruns"):
                 _reruns = session.config.option.reruns
-            if letmego.read_testcase_running_status(item, reruns=_reruns):
-                session.items.remove(item)
+            if HAS_LETMEGO:
+                if letmego.read_testcase_running_status(item, reruns=_reruns):
+                    session.items.remove(item)
 
     if (suite_id or task_id) and session.items:
         print("\n即将执行的用例:")
         for item in session.items:
             for mark in item.own_markers:
                 if mark.args == (FixedCsvTitle.pms_case_id.value,):
                     print(f"case_id: {mark.name}, case_name: {item.name}")
@@ -534,15 +541,15 @@
                 "w+",
                 encoding="utf-8",
         ) as _f:
             _f.writelines(execute2)
 
 
 def pytest_runtest_setup(item):
-    if hasattr(item, "execution_count"):
+    if HAS_LETMEGO and hasattr(item, "execution_count"):
         letmego.conf.setting.EXECUTION_COUNT = item.execution_count
 
     print()  # 处理首行日志换行的问题
     current_item_count = f"[{item.session.items.index(item) + 1}/{item.session.item_count}] "
     try:
         current_item_percent = "{:.0f}%".format(
             int(item.session.items.index(item) + 1) / int(item.session.item_count) * 100
@@ -592,17 +599,17 @@
 
 def pytest_runtest_teardown(item):
     logger.info(f"{FLAG_FEEL} teardown {FLAG_FEEL}")
     sessiontimeout = item.session.sessiontimeout
     if sessiontimeout:
         duration = datetime.now() - item.session.config.option.start_time
         if duration.seconds > int(sessiontimeout):
-            # 处理时间秒为 XX分XX秒
+            # 处理时间秒为 xx分xx秒
             _min, sec = divmod(duration.seconds, 60)
-            # 处理时间分为 XX小时xx分xx秒
+            # 处理时间分为 xx小时xx分xx秒
             hour, _min = divmod(_min, 60)
             raise item.session.Interrupted(f"会话超时（{hour}小时{_min}分{sec}秒）,用例强制终止!")
 
 
 @pytest.hookimpl(hookwrapper=True, tryfirst=True)
 def pytest_runtest_makereport(item, call):
     out = yield
@@ -626,15 +633,15 @@
                     allure.dynamic.tag(mark.name)
     if report.when == "call":
         logger.info(f"运行结果: {str(report.outcome).upper()}")
         if write_json(item.session):
             # 只要是需要数据回填（无论是自动还是手动）,都需要写json结果.
             write_case_result(item, report)
 
-        if item.config.option.autostart:
+        if HAS_LETMEGO and item.config.option.autostart:
             letmego.write_testcase_running_status(item, report)
     try:
         if item.execution_count >= (int(item.config.option.record_failed_case) + 1):
             if report.when == "call":  # 存放录屏当次测试结果
                 item.record["result"] = report.outcome
                 try:
                     # 记录断言的模板图片
@@ -734,37 +741,59 @@
                 config=config, head_line=report.head_line
             )
         return report.outcome, short, verbose
     return None
 
 
 def pytest_sessionfinish(session):
+    tr = session.config.pluginmanager.get_plugin("terminalreporter")
+    execute = {}
+    for _, items in tr.stats.items():
+        for item in items:
+            if hasattr(item, "outcome"):
+                default_result = {"result": "blocked", "longrepr": "None"}
+                if item.outcome == ConfStr.PASSED.value:
+                    default_result["result"] = "pass"
+                elif item.outcome == ConfStr.SKIPPED.value:
+                    default_result["result"] = "skip"
+                elif item.outcome == ConfStr.RERUN.value:
+                    continue
+                else:
+                    default_result["result"] = "fail"
+                default_result["longrepr"] = item.longreprtext
+                item_name = item.fspath
+                if not execute.get(item_name) or (
+                        item.outcome != ConfStr.PASSED.value
+                        and execute.get(item_name).get("result") == "pass"
+                ):
+                    execute[item_name] = default_result
+
+    json_report_path = join(GlobalConfig.JSON_REPORT_PATH, "json")
+    if not exists(json_report_path):
+        makedirs(json_report_path)
+    with open(f"{json_report_path}/detail_report.json", "w", encoding="utf-8") as _f:
+        _f.write(dumps(execute, indent=2, ensure_ascii=False))
+
+    res = Counter([execute.get(i).get("result") for i in execute])
+    with open(f"{json_report_path}/summarize.json", "w", encoding="utf-8") as _f:
+        _f.write(dumps(
+            {
+                "total": sum(res.values()),
+                "pass": res.get("pass", 0),
+                "fail": res.get("fail", 0),
+                "skip": res.get("skip", 0),
+            },
+            indent=2,
+            ensure_ascii=False
+        ))
+
     if session.config.option.allure_report_dir:
-        tr = session.config.pluginmanager.get_plugin("terminalreporter")
-        execute = {}
-        for _, items in tr.stats.items():
-            for item in items:
-                if hasattr(item, "outcome"):
-                    default_result = {"result": "blocked", "longrepr": "None"}
-                    if item.outcome == ConfStr.PASSED.value:
-                        default_result["result"] = "pass"
-                    elif item.outcome == ConfStr.SKIPPED.value:
-                        default_result["result"] = "skip"
-                    elif item.outcome == ConfStr.RERUN.value:
-                        continue
-                    else:
-                        default_result["result"] = "fail"
-                    default_result["longrepr"] = item.longreprtext
-                    item_name = item.fspath
-                    if not execute.get(item_name) or (
-                            item.outcome != ConfStr.PASSED.value
-                            and execute.get(item_name).get("result") == "pass"
-                    ):
-                        execute[item_name] = default_result
+
         AllureReportExtend.environment_info(session, execute)
+        # 后续移除
         if execute:
             with open(f"{GlobalConfig.ROOT_DIR}/ci_result.json", "w", encoding="utf-8") as _f:
                 _f.write(dumps(execute, indent=2, ensure_ascii=False))
 
     if session.config.option.pms_user and session.config.option.pms_password:
 
         def send2pms(case_res_path, data_send_result_csv):
```

### Comparing `youqu-2.6.1/youqu/env.sh` & `youqu-2.6.2/youqu/env.sh`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/manage.py` & `youqu-2.6.2/youqu/manage.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,29 +31,28 @@
 
 class Manage:
     __author__ = "mikigo<huangmingqiang@uniontech.com>"
 
     def __init__(self):
         from src.plugins.mng import trim
         from src.plugins.mng import help_tip
+        from src.plugins.mng import SubCmd
 
         trim()
         logger(GlobalConfig.LOG_LEVEL)
 
         self.cmd_args = sys.argv[1:]
         if not self.cmd_args:
             print(help_tip())
             sys.exit(1)
         parser = ArgumentParser(epilog=self.__author__)
         subparsers = parser.add_subparsers(help="子命令")
-        from setting.subcmd import SubCmd
 
         sub_parser_remote = subparsers.add_parser(SubCmd.remote.value)
         sub_parser_run = subparsers.add_parser(SubCmd.run.value)
-        sub_parser_playbook = subparsers.add_parser(SubCmd.playbook.value)
         sub_parser_pms = subparsers.add_parser(SubCmd.pmsctl.value)
         sub_parser_csv = subparsers.add_parser(SubCmd.csvctl.value)
         sub_parser_git = subparsers.add_parser(SubCmd.git.value)
 
         if self.cmd_args[0] == SubCmd.remote.value:
             from src.rtk._cargo import remote_runner
             from src.rtk.remote_runner import RemoteRunner
@@ -63,18 +62,14 @@
 
         elif self.cmd_args[0] == SubCmd.run.value:
             from src.rtk._cargo import local_runner
             from src.rtk.local_runner import LocalRunner
 
             _local_kwargs, _ = local_runner(parser, sub_parser_run, self.cmd_args)
             LocalRunner(**_local_kwargs).local_run()
-        elif self.cmd_args[0] == SubCmd.playbook.value:
-            from src.rtk._cargo import playbook_control
-
-            playbook_control(parser, sub_parser_playbook)
 
         elif self.cmd_args[0] == SubCmd.pmsctl.value:
             from src.pms._cargo import pms_control
 
             pms_control(parser, sub_parser_pms)
 
         elif self.cmd_args[0] == SubCmd.csvctl.value:
```

### Comparing `youqu-2.6.1/youqu/startproject.py` & `youqu-2.6.2/youqu/startproject.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/setting/globalconfig.ini` & `youqu-2.6.2/youqu/setting/globalconfig.ini`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
 OCR_TIMEOUT = 5
 
 ;OCR识别的最大次数
 OCR_MAX_MATCH_NUMBER = 100
 
 ;=============================== IMAGE CONFIG ===================================
 ;OpenCV服务端地址
-OPENCV_SERVER_HOST = youqu.uniontech.com
+OPENCV_SERVER_HOST =
 
 ;图像识别端口
 OPENCV_PORT = 8889
 
 ;网络重试次数
 OPENCV_NETWORK_RETRY = 1
```

### Comparing `youqu-2.6.1/youqu/setting/globalconfig.py` & `youqu-2.6.2/youqu/setting/globalconfig.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/setting/pylintrc.cfg` & `youqu-2.6.2/youqu/setting/pylintrc.cfg`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/setting/skipif.py` & `youqu-2.6.2/youqu/setting/skipif.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/setting/template/app_template/config.py-tpl` & `youqu-2.6.2/youqu/setting/template/app_template/config.py-tpl`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/setting/template/app_template/case/test_mycase_002.py-tpl` & `youqu-2.6.2/youqu/setting/template/app_template/case/test_mycase_002.py-tpl`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/setting/template/app_template/widget/base_widget.py-tpl` & `youqu-2.6.2/youqu/setting/template/app_template/widget/base_widget.py-tpl`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/setting/template/app_template/widget/ui.ini-tpl` & `youqu-2.6.2/youqu/setting/template/app_template/widget/ui.ini-tpl`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/__init__.py` & `youqu-2.6.2/youqu/src/__init__.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/assert_common.py` & `youqu-2.6.2/youqu/src/assert_common.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/button_center.py` & `youqu-2.6.2/youqu/src/button_center.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/calculate.py` & `youqu-2.6.2/youqu/src/calculate.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/cmdctl.py` & `youqu-2.6.2/youqu/src/cmdctl.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
 
 import os
 # SPDX-License-Identifier: GPL-2.0-only
 # pylint: disable=C0114
 import subprocess
+import sys
 
 from setting import conf
 from src import logger
 from src.custom_exception import ShellExecutionFailed
 
 
 class CmdCtl:
@@ -43,24 +44,28 @@
                     retcode, process.args, output=stdout, stderr=stderr
                 )
         return subprocess.CompletedProcess(process.args, retcode, stdout, stderr)
 
     @classmethod
     def _getstatusoutput(cls, command, timeout):
         """getstatusoutput"""
+        kwargs = {
+            "shell": True,
+            "stderr": subprocess.STDOUT,
+            "stdout": subprocess.PIPE,
+            "timeout": timeout,
+        }
         try:
-            result = cls._run(
-                command,
-                shell=True,
-                text=True,
-                stderr=subprocess.STDOUT,
-                stdout=subprocess.PIPE,
-                timeout=timeout,
+            if sys.version_info >= (3, 7):
+                kwargs["text"] = True
+            result = cls._run(command,**kwargs
             )
             data = result.stdout
+            if isinstance(data, bytes):
+                data = data.decode("utf-8")
             exitcode = result.returncode
         except subprocess.CalledProcessError as ex:
             data = ex.output
             exitcode = ex.returncode
         except subprocess.TimeoutExpired as ex:
             # pylint: disable=unnecessary-dunder-call
             data = ex.__str__()
```

### Comparing `youqu-2.6.1/youqu/src/csvctl.py` & `youqu-2.6.2/youqu/src/csvctl.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/custom_exception.py` & `youqu-2.6.2/youqu/src/custom_exception.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/dbus_utils.py` & `youqu-2.6.2/youqu/src/dbus_utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/desktop.py` & `youqu-2.6.2/youqu/src/desktop.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/dogtail_utils.py` & `youqu-2.6.2/youqu/src/dogtail_utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/filectl.py` & `youqu-2.6.2/youqu/src/filectl.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/filter_image.py` & `youqu-2.6.2/youqu/src/filter_image.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/image_utils.py` & `youqu-2.6.2/youqu/src/image_utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/mouse_key.py` & `youqu-2.6.2/youqu/src/mouse_key.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/ocr_utils.py` & `youqu-2.6.2/youqu/src/ocr_utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/pinyin.py` & `youqu-2.6.2/youqu/src/pinyin.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/read_csv.py` & `youqu-2.6.2/youqu/src/read_csv.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/recording_screen.py` & `youqu-2.6.2/youqu/src/recording_screen.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/requestx.py` & `youqu-2.6.2/youqu/src/requestx.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 #!/usr/bin/env python3
 # _*_ coding:utf-8 _*_
-
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
-
 # SPDX-License-Identifier: GPL-2.0-only
-# pylint: disable=C0114,C0115,W0621,C0103
-from urllib import request
+from http import cookiejar
 from urllib import parse
+from urllib import request
 from urllib.request import build_opener
-from http import cookiejar
+import json as _json
 
 
 class RequestX:
     def __init__(
-        self,
-        login_url=None,
-        headers=None,
-        data=None,
+            self,
+            login_url=None,
+            headers=None,
+            data=None,
     ):
         self.login_url = login_url
         self.headers = headers
         self.data = parse.urlencode(data).encode("utf-8") if data else None
         self.kwargs = {}
         if self.login_url:
             self.kwargs["url"] = self.login_url
@@ -50,14 +48,27 @@
         :return:
         """
         if timeout is None:
             timeout = object()
         response = self.session.open(url, data=data, timeout=timeout).read().decode()
         return response
 
+    @classmethod
+    def post(cls, url: str, headers: dict, data: dict = None, json: dict=None):
+        if data:
+            params = parse.urlencode(data).encode("utf-8")
+        elif json:
+            params = _json.dumps(json)
+            params = bytes(params, "utf-8")
+        else:
+            raise ValueError
+        r = request.Request(url=url, data=params, headers=headers, method="POST")
+        req = request.urlopen(r).read().decode("utf-8")
+        return req
+
 
 if __name__ == "__main__":
     user = ""  # 工号
     password = ""  # 密码
     login_url = "https://pms.uniontech.com/user-login-Lw==.html"
     headers = {"content-type": "application/x-www-form-urlencoded; charset=UTF-8"}
     data = {
```

### Comparing `youqu-2.6.1/youqu/src/shortcut.py` & `youqu-2.6.2/youqu/src/shortcut.py`

 * *Files 2% similar despite different names*

```diff
@@ -699,14 +699,23 @@
          快捷键打开剪切板
         :return:
         """
         sleep(1)
         cls.hot_key("ctrl", "alt", "v")
 
     @classmethod
+    def ctrl_alt_delete(cls):
+        """
+         快捷键打开剪切板
+        :return:
+        """
+        sleep(1)
+        cls.hot_key("ctrl", "alt", "delete")
+
+    @classmethod
     def ctrl_printscreen(cls):
         """
          快捷键启动延时截图
         :return:
         """
         sleep(1)
         cls.hot_key("ctrl", "printscreen")
@@ -839,14 +848,21 @@
     def super_d(cls):
         """快捷键 super + d
         :return:
         """
         cls.hot_key("win", "d")
 
     @classmethod
+    def super_l(cls):
+        """快捷键 super + l
+        :return:
+        """
+        cls.hot_key("win", "l")
+
+    @classmethod
     def super(cls):
         """快捷键 super
         :return:
         """
         cls.hot_key("win")
 
     @classmethod
```

### Comparing `youqu-2.6.1/youqu/src/singleton.py` & `youqu-2.6.2/youqu/src/singleton.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/sleepx.py` & `youqu-2.6.2/youqu/src/sleepx.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/startapp.py` & `youqu-2.6.2/youqu/src/startapp.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/startproject.py` & `youqu-2.6.2/youqu/src/startproject.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/video_utils.py` & `youqu-2.6.2/youqu/src/video_utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/wayland_wininfo.py` & `youqu-2.6.2/youqu/src/wayland_wininfo.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/webui.py` & `youqu-2.6.2/youqu/src/webui.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/ydotool.py` & `youqu-2.6.2/youqu/src/ydotool.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/cfonts/cli.py` & `youqu-2.6.2/youqu/src/depends/cfonts/cli.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/cfonts/colors.py` & `youqu-2.6.2/youqu/src/depends/cfonts/colors.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/cfonts/consts.py` & `youqu-2.6.2/youqu/src/depends/cfonts/consts.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/cfonts/core.py` & `youqu-2.6.2/youqu/src/depends/cfonts/core.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/cfonts/fonts/3d.json` & `youqu-2.6.2/youqu/src/depends/cfonts/fonts/3d.json`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/cfonts/fonts/block.json` & `youqu-2.6.2/youqu/src/depends/cfonts/fonts/block.json`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/cfonts/fonts/chrome.json` & `youqu-2.6.2/youqu/src/depends/cfonts/fonts/chrome.json`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/cfonts/fonts/grid.json` & `youqu-2.6.2/youqu/src/depends/cfonts/fonts/grid.json`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/cfonts/fonts/huge.json` & `youqu-2.6.2/youqu/src/depends/cfonts/fonts/huge.json`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/cfonts/fonts/pallet.json` & `youqu-2.6.2/youqu/src/depends/cfonts/fonts/pallet.json`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/cfonts/fonts/shade.json` & `youqu-2.6.2/youqu/src/depends/cfonts/fonts/shade.json`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/cfonts/fonts/simple.json` & `youqu-2.6.2/youqu/src/depends/cfonts/fonts/simple.json`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/cfonts/fonts/simple3d.json` & `youqu-2.6.2/youqu/src/depends/cfonts/fonts/simple3d.json`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/cfonts/fonts/simpleBlock.json` & `youqu-2.6.2/youqu/src/depends/cfonts/fonts/simpleBlock.json`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/cfonts/fonts/slick.json` & `youqu-2.6.2/youqu/src/depends/cfonts/fonts/slick.json`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/cfonts/fonts/tiny.json` & `youqu-2.6.2/youqu/src/depends/cfonts/fonts/tiny.json`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/colorama/ansi.py` & `youqu-2.6.2/youqu/src/depends/colorama/ansi.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/colorama/ansitowin32.py` & `youqu-2.6.2/youqu/src/depends/colorama/ansitowin32.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/colorama/initialise.py` & `youqu-2.6.2/youqu/src/depends/colorama/initialise.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/colorama/win32.py` & `youqu-2.6.2/youqu/src/depends/colorama/win32.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/colorama/winterm.py` & `youqu-2.6.2/youqu/src/depends/colorama/winterm.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/dogtail/COPYING` & `youqu-2.6.2/youqu/src/depends/dogtail/COPYING`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/dogtail/__init__.py` & `youqu-2.6.2/youqu/src/depends/dogtail/__init__.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/dogtail/config.py` & `youqu-2.6.2/youqu/src/depends/dogtail/config.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/dogtail/distro.py` & `youqu-2.6.2/youqu/src/depends/dogtail/distro.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/dogtail/dump.py` & `youqu-2.6.2/youqu/src/depends/dogtail/dump.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/dogtail/errors.py` & `youqu-2.6.2/youqu/src/depends/dogtail/errors.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/dogtail/i18n.py` & `youqu-2.6.2/youqu/src/depends/dogtail/i18n.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/dogtail/logging.py` & `youqu-2.6.2/youqu/src/depends/dogtail/logging.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/dogtail/path.py` & `youqu-2.6.2/youqu/src/depends/dogtail/path.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/dogtail/predicate.py` & `youqu-2.6.2/youqu/src/depends/dogtail/predicate.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/dogtail/procedural.py` & `youqu-2.6.2/youqu/src/depends/dogtail/procedural.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/dogtail/rawinput.py` & `youqu-2.6.2/youqu/src/depends/dogtail/rawinput.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/dogtail/rawinput_wayland.py` & `youqu-2.6.2/youqu/src/depends/dogtail/rawinput_wayland.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/dogtail/sessions.py` & `youqu-2.6.2/youqu/src/depends/dogtail/sessions.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/dogtail/tc.py` & `youqu-2.6.2/youqu/src/depends/dogtail/tc.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/dogtail/tree.py` & `youqu-2.6.2/youqu/src/depends/dogtail/tree.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/dogtail/utils.py` & `youqu-2.6.2/youqu/src/depends/dogtail/utils.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/dogtail/version.py` & `youqu-2.6.2/youqu/src/depends/dogtail/version.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/dogtail/wrapped.py` & `youqu-2.6.2/youqu/src/depends/dogtail/wrapped.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/dogtail/icons/dogtail-head-48.png` & `youqu-2.6.2/youqu/src/depends/dogtail/icons/dogtail-head-48.png`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/dogtail/icons/dogtail-head.svg` & `youqu-2.6.2/youqu/src/depends/dogtail/icons/dogtail-head.svg`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/dogtail/icons/dogtail-tail-48.png` & `youqu-2.6.2/youqu/src/depends/dogtail/icons/dogtail-tail-48.png`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/dogtail/icons/dogtail-tail.svg` & `youqu-2.6.2/youqu/src/depends/dogtail/icons/dogtail-tail.svg`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/pyautogui/LICENSE.txt` & `youqu-2.6.2/youqu/src/depends/pyautogui/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/pyautogui/__init__.py` & `youqu-2.6.2/youqu/src/depends/pyautogui/__init__.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/pyautogui/_pyautogui_osx.py` & `youqu-2.6.2/youqu/src/depends/pyautogui/_pyautogui_osx.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/pyautogui/_pyautogui_wayland.py` & `youqu-2.6.2/youqu/src/depends/pyautogui/_pyautogui_wayland.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/pyautogui/_pyautogui_win.py` & `youqu-2.6.2/youqu/src/depends/pyautogui/_pyautogui_win.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/pyautogui/_pyautogui_x11.py` & `youqu-2.6.2/youqu/src/depends/pyautogui/_pyautogui_x11.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/pygtkcompat/__init__.py` & `youqu-2.6.2/youqu/src/depends/pygtkcompat/__init__.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/pygtkcompat/generictreemodel.py` & `youqu-2.6.2/youqu/src/depends/pygtkcompat/generictreemodel.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/pygtkcompat/pygtkcompat.py` & `youqu-2.6.2/youqu/src/depends/pygtkcompat/pygtkcompat.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/sniff/sniff` & `youqu-2.6.2/youqu/src/depends/sniff/sniff`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/sniff/sniff.ui` & `youqu-2.6.2/youqu/src/depends/sniff/sniff.ui`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/sniff/icons/button.xpm` & `youqu-2.6.2/youqu/src/depends/sniff/icons/button.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/sniff/icons/checkbutton.xpm` & `youqu-2.6.2/youqu/src/depends/sniff/icons/checkbutton.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/sniff/icons/checkmenuitem.xpm` & `youqu-2.6.2/youqu/src/depends/sniff/icons/checkmenuitem.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/sniff/icons/colorselection.xpm` & `youqu-2.6.2/youqu/src/depends/sniff/icons/colorselection.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/sniff/icons/combo.xpm` & `youqu-2.6.2/youqu/src/depends/sniff/icons/combo.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/sniff/icons/dialog.xpm` & `youqu-2.6.2/youqu/src/depends/sniff/icons/dialog.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/sniff/icons/image.xpm` & `youqu-2.6.2/youqu/src/depends/sniff/icons/image.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/sniff/icons/label.xpm` & `youqu-2.6.2/youqu/src/depends/sniff/icons/label.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/sniff/icons/menubar.xpm` & `youqu-2.6.2/youqu/src/depends/sniff/icons/menubar.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/sniff/icons/menuitem.xpm` & `youqu-2.6.2/youqu/src/depends/sniff/icons/menuitem.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/sniff/icons/notebook.xpm` & `youqu-2.6.2/youqu/src/depends/sniff/icons/notebook.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/sniff/icons/scrolledwindow.xpm` & `youqu-2.6.2/youqu/src/depends/sniff/icons/scrolledwindow.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/sniff/icons/spinbutton.xpm` & `youqu-2.6.2/youqu/src/depends/sniff/icons/spinbutton.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/sniff/icons/statusbar.xpm` & `youqu-2.6.2/youqu/src/depends/sniff/icons/statusbar.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/sniff/icons/table.xpm` & `youqu-2.6.2/youqu/src/depends/sniff/icons/table.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/sniff/icons/text.xpm` & `youqu-2.6.2/youqu/src/depends/sniff/icons/text.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/sniff/icons/toolbar.xpm` & `youqu-2.6.2/youqu/src/depends/sniff/icons/toolbar.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/sniff/icons/tree.xpm` & `youqu-2.6.2/youqu/src/depends/sniff/icons/tree.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/sniff/icons/treeitem.xpm` & `youqu-2.6.2/youqu/src/depends/sniff/icons/treeitem.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/sniff/icons/unknown.xpm` & `youqu-2.6.2/youqu/src/depends/sniff/icons/unknown.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/sniff/icons/viewport.xpm` & `youqu-2.6.2/youqu/src/depends/sniff/icons/viewport.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/sniff/icons/vscrollbar.xpm` & `youqu-2.6.2/youqu/src/depends/sniff/icons/vscrollbar.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/sniff/icons/vseparator.xpm` & `youqu-2.6.2/youqu/src/depends/sniff/icons/vseparator.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/sniff/icons/window.xpm` & `youqu-2.6.2/youqu/src/depends/sniff/icons/window.xpm`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/wayland_autotool/CMakeLists.txt` & `youqu-2.6.2/youqu/src/depends/wayland_autotool/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/wayland_autotool/autotool.cpp` & `youqu-2.6.2/youqu/src/depends/wayland_autotool/autotool.cpp`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/wayland_autotool/autotool.h` & `youqu-2.6.2/youqu/src/depends/wayland_autotool/autotool.h`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/wayland_autotool/main.cpp` & `youqu-2.6.2/youqu/src/depends/wayland_autotool/main.cpp`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/ydotool/CMakeLists.txt` & `youqu-2.6.2/youqu/src/depends/ydotool/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/ydotool/LICENSE` & `youqu-2.6.2/youqu/src/depends/ydotool/LICENSE`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/ydotool/Client/tool_click.c` & `youqu-2.6.2/youqu/src/depends/ydotool/Client/tool_click.c`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/ydotool/Client/tool_key.c` & `youqu-2.6.2/youqu/src/depends/ydotool/Client/tool_key.c`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/ydotool/Client/tool_mousemove.c` & `youqu-2.6.2/youqu/src/depends/ydotool/Client/tool_mousemove.c`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/ydotool/Client/tool_type.c` & `youqu-2.6.2/youqu/src/depends/ydotool/Client/tool_type.c`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/ydotool/Client/ydotool.c` & `youqu-2.6.2/youqu/src/depends/ydotool/Client/ydotool.c`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/ydotool/Client/ydotool.h` & `youqu-2.6.2/youqu/src/depends/ydotool/Client/ydotool.h`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/ydotool/Daemon/ydotoold.c` & `youqu-2.6.2/youqu/src/depends/ydotool/Daemon/ydotoold.c`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/ydotool/manpage/ydotool.1.scd` & `youqu-2.6.2/youqu/src/depends/ydotool/manpage/ydotool.1.scd`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/depends/ydotool/manpage/ydotoold.8.scd` & `youqu-2.6.2/youqu/src/depends/ydotool/manpage/ydotoold.8.scd`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/git/_cargo.py` & `youqu-2.6.2/youqu/src/git/_cargo.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 def git_control(parser=None, sub_parser_git=None):
     sub_parser_git.add_argument(
         "-a",
         "--app",
         default="",
         help="应用名称：apps/autotest_deepin_music 或 autotest_deepin_music",
     )
-    sub_parser_git.add_argument("-u", "--user", default="", help="git仓库用户名")
-    sub_parser_git.add_argument("-p", "--password", default="", help="git仓库地密码")
-    sub_parser_git.add_argument("-l", "--url", default="", help="git仓库地址")
+    sub_parser_git.add_argument("-u", "--git_user", default="", help="git仓库用户名")
+    sub_parser_git.add_argument("-p", "--git_password", default="", help="git仓库地密码")
+    sub_parser_git.add_argument("-l", "--git_url", default="", help="git仓库地址")
     sub_parser_git.add_argument("-b", "--branch_or_tag", default="", help="分支或Tag")
     sub_parser_git.add_argument("-d", "--depth", default="", help="git仓库克隆深度")
     sub_parser_git.add_argument("-s", "--startdate", default="", help="统计开始时间")
     sub_parser_git.add_argument("-e", "--enddate", default="", help="统计结束时间")
     args = parser.parse_args()
     from src.rtk._base import Args
     from setting import conf
 
     git_kwargs = {
         Args.app_name.value: args.app or conf.APP_NAME,
-        Args.url.value: args.url or conf.GIT_URL,
-        Args.user.value: args.user or conf.GIT_USER,
-        Args.password.value: args.password or conf.GIT_PASSWORD,
+        Args.git_url.value: args.git_url or conf.GIT_URL,
+        Args.git_user.value: args.git_user or conf.GIT_USER,
+        Args.git_password.value: args.git_password or conf.GIT_PASSWORD,
         Args.branch.value: args.branch_or_tag or conf.BRANCH,
         Args.depth.value: args.depth or conf.DEPTH,
         Args.startdate.value: args.startdate or conf.START_DATE,
         Args.enddate.value: args.enddate or conf.END_DATE,
     }
     from src.git.check import check_git_installed
 
-    if git_kwargs.get(Args.url.value):
+    if git_kwargs.get(Args.git_url.value):
         if all(
             [
-                git_kwargs.get(Args.user.value),
-                git_kwargs.get(Args.password.value),
+                git_kwargs.get(Args.git_user.value),
+                git_kwargs.get(Args.git_password.value),
             ]
         ):
             from src.git.clone import sslclone as git_clone
         else:
             from src.git.clone import clone as git_clone
         check_git_installed()
         git_clone(**git_kwargs)
```

### Comparing `youqu-2.6.1/youqu/src/git/clone.py` & `youqu-2.6.2/youqu/src/git/clone.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,48 +9,54 @@
 
 def git_config():
     os.system("git config --global http.lowSpeedLimit 0")
     os.system("git config --global http.lowSpeedTime 999999")
 
 
 def sslclone(
-    url: str = None,
-    user: str = None,
-    password: str = None,
+    git_url: str = None,
+    git_user: str = None,
+    git_password: str = None,
     branch: str = None,
     path_to: str = None,
     depth: [str, int] = None,
     **kwargs,
 ):
     branch = branch or conf.BRANCH
     depth = depth or conf.DEPTH
     if path_to is None:
         path_to = "apps"
     git_config()
     clone_cmd = (
         f"cd {conf.ROOT_DIR}/src/utils && "
         f"bash sslclone.sh {conf.ROOT_DIR}/{path_to} "
-        f"{url or conf.GIT_URL} "
-        f"{user or conf.GTI_USER} {password or conf.GIT_PASSWORD} "
+        f"{git_url or conf.GIT_URL} "
+        f"{git_user or conf.GTI_USER} {git_password or conf.GIT_PASSWORD} "
         f"{branch or ''} {depth or ''}"
     )
     print(clone_cmd)
     os.system(clone_cmd)
     # relax
     sleep(2)
 
 
-def clone(url: str = None, branch: str = "", path_to: str = None, depth: [str, int] = "", **kwargs):
+def clone(
+        git_url: str = None,
+        branch: str = "",
+        path_to: str = None,
+        depth: [str, int] = "",
+        **kwargs
+):
     branch = branch or conf.BRANCH
     depth = depth or conf.DEPTH
     if path_to is None:
         path_to = "apps"
     git_config()
     clone_cmd = (
         f"cd {conf.ROOT_DIR}/{path_to} && git clone "
-        f"{url or conf.GIT_URL} "
+        f"{git_url or conf.GIT_URL} "
         f"{f'-b {branch}' if branch else ''} {f'--depth {depth}' if depth else ''}"
     )
     print(clone_cmd)
     os.system(clone_cmd)
     # relax
     sleep(2)
```

### Comparing `youqu-2.6.1/youqu/src/git/code_statistics.py` & `youqu-2.6.2/youqu/src/git/code_statistics.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/git/commit.py` & `youqu-2.6.2/youqu/src/git/commit.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/plugins/allure_report_extend.py` & `youqu-2.6.2/youqu/src/plugins/allure_report_extend.py`

 * *Files 18% similar despite different names*

```diff
@@ -32,38 +32,28 @@
             w = partial(wf, _f)
 
             py_case_info = ""
             if execute:
                 total, failed, passed, skiped, _ = collect_result(execute)
                 py_case_info = f"{total}/{passed}/{failed}/{skiped}"
 
-            w(f"PMS用例维度(总数/通过/失败/跳过)={py_case_info}")
+            w(f"Py用例维度(总数/通过/失败/跳过)={py_case_info}")
             w(f"网络地址={GlobalConfig.USERNAME}@{GlobalConfig.HOST_IP}")
             w(f"工作目录={GlobalConfig.ROOT_DIR}")
             w(f"镜像版本={GlobalConfig.VERSION}")
 
             screen = Tk()
             w(f"分辨率={screen.winfo_screenwidth()}x{screen.winfo_screenheight()}")
             w(f"显示协议={GlobalConfig.DISPLAY_SERVER.title()}")
 
             try:
-                cpu_info = (
-                    os.popen(
-                        f"echo '{GlobalConfig.PASSWORD}' | sudo -S dmidecode -s  processor-version"
-                    )
-                    .readlines()[0]
-                    .strip("\n")
-                )
-                w(f"CPU信息={cpu_info}")
-
-
-                mem_info = os.popen(
-                    f'''echo '{GlobalConfig.PASSWORD}' | sudo -S dmidecode|grep -A16 'Memory Device' | '''
-                    'grep -v "Memory Device Mapped Address" | grep "Range Size"'
-                ).readlines()
-                MEM_TOTAL = sum([int(i.split(":")[1].rstrip(" GB\n").strip()) for i in mem_info])
-                w(f"内存信息={MEM_TOTAL}G")
+                cpu_info = os.popen('cat /proc/cpuinfo | grep "model name"').readlines()
+                if cpu_info:
+                    w(f"CPU信息={cpu_info[0]}")
+                mem_info = os.popen('cat /proc/meminfo | grep MemTotal').readlines()
+                if mem_info:
+                    w(f"内存信息={mem_info[0]}")
             except IndexError:
                 ...
 
             os_info = os.popen("uname -a").read()
             w(f"内核信息={os_info}")
```

### Comparing `youqu-2.6.1/youqu/src/plugins/emoji_hooks.py` & `youqu-2.6.2/youqu/src/plugins/emoji_hooks.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/plugins/mng.py` & `youqu-2.6.2/youqu/src/plugins/mng.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,17 +1,19 @@
-from setting.subcmd import SubCmd
+from enum import Enum
+from enum import unique
 from setting.globalconfig import GlobalConfig
 
 
 def help_tip():
-    color = "34"
+    color = "32"
     return (
-        f"\033[1;{color}mmanage.py\033[0m 支持 \033[1;{color}m{[i.value for i in SubCmd]}\033[0m 命令, "
-        f"\n您需要传入一个命令,可以使用 \033[1;{color}m-h\033[0m 或 \033[1;{color}m--help\033[0m 查看每个命令参数的详细使用说明,"
-        f"\n比如: \033[1;{color}myouqu manage.py run -h\033[0m \n"
+        f'''\033[1;{color}mYouQu\033[0m 支持的子命令:\n    '''
+        f'''\033[1;{color}m{str([i.value for i in SubCmd]).replace("'", "").strip("[").strip("]")}\033[0m'''
+        f"\n您需要传入其中一个子命令,可以使用 \033[1;{color}m-h\033[0m 或 \033[1;{color}m--help\033[0m 查看每个命令参数的详细使用说明."
+        f"\n如: \033[1;{color}myouqu manage.py run -h\033[0m \n"
     )
 
 
 def start_app(startapp=None):
     if startapp:
         from src.startapp import StartApp
 
@@ -21,12 +23,23 @@
 
 
 def trim():
     from src.depends.cfonts import say
 
     say(GlobalConfig.PROJECT_NAME)
     version_font = "slick"
+    color = "32"
     say(GlobalConfig.current_tag, font=version_font, space=False)
-    say(f"Code: \033[0;32m{GlobalConfig.GITHUB_URL}\033[0m", font="console", space=False)
-    say(f"Docs: \033[0;32m{GlobalConfig.DOCS_URL}\033[0m", font="console", space=False)
-    say(f"PyPI: \033[0;32m{GlobalConfig.PyPI_URL}\033[0m", font="console", space=False)
-    say("=" * 60, font="console", space=False)
+    say(f"Code: \033[1;{color}m{GlobalConfig.GITHUB_URL}\033[0m", font="console", space=False)
+    say(f"Docs: \033[1;{color}m{GlobalConfig.DOCS_URL}\033[0m", font="console", space=False)
+    say(f"PyPI: \033[1;{color}m{GlobalConfig.PyPI_URL}\033[0m", font="console", space=False)
+    say(f'\033[1;{color}m{"=" * 60}\033[0m', font="console", space=False)
+
+
+@unique
+class SubCmd(Enum):
+    run = "run"
+    remote = "remote"
+    pmsctl = "pmsctl"
+    csvctl = "csvctl"
+    startapp = "startapp"
+    git = "git"
```

### Comparing `youqu-2.6.1/youqu/src/pms/_base.py` & `youqu-2.6.2/youqu/src/pms/_base.py`

 * *Files 23% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from re import findall, sub
 
 from setting.globalconfig import GlobalConfig
 from src import logger
 from src.requestx import RequestX
 
 MAX_CASE_NUMBER = 10000
-# pylint: disable=unnecessary-lambda-assignment,R0903
 runs_id_cmd_log = lambda x: sub(r"'run_case_id': '\d+', ", "", str(x))
 
 
 class _Base:
     __author__ = "huangmingqiang@uniontech.com"
 
     def __init__(self, user=None, password=None):
@@ -34,41 +33,14 @@
             "verifyRand": "370729017",
             "keepLogin": "0",
         }
         # pylint: disable=invalid-name
         self.rx = RequestX(login_url=login_url, headers=headers, data=data)
 
 
-def _unicode_to_cn(in_str):
-    """
-    修改数据并进行编码解码操作，以完成u码转中文
-    :param in_str: 字符串
-    :return:/
-    """
-    local_in_str_replace = (
-        in_str.replace(r"\"", '"')
-        .replace(r"\/", "/")
-        .replace(r"\\u", r"\u")
-        .replace(r"\\n", "")
-        .replace(r"\\r", "")
-    )
-    if isinstance(local_in_str_replace, bytes):
-        local_temp = str(local_in_str_replace, encoding="utf-8")
-        local_out = local_temp.encode("utf-8").decode("unicode_escape")
-    else:
-        local_out = local_in_str_replace.encode("utf-8").decode("unicode_escape")
-    return (
-        local_out.replace('"data":"{', '"data":{')
-        .replace('","md5"', ',"md5"')
-        .replace(":null", ':"null"')
-        .replace(":true", ':"true"')
-        .replace(":false", ':"false"')
-    )
-
-
 def write_case_result(item, report):
     """写用例执行的结果"""
     case_result_tpl = {
         "at_case_id": None,
         "case_id": None,
         "from_case_id": None,
         "task_id": None,
```

### Comparing `youqu-2.6.1/youqu/src/pms/_cargo.py` & `youqu-2.6.2/youqu/src/pms/_cargo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setting.globalconfig import GlobalConfig
 
 
-def pms_control(self, parser=None, sub_parser_pms=None):
+def pms_control(parser=None, sub_parser_pms=None):
     """pms相关功能命令行参数"""
     sub_parser_pms.add_argument(
         "-a",
         "--app",
         default="",
         help="应用名称：apps/autotest_deepin_music 或 autotest_deepin_music",
     )
@@ -32,20 +32,20 @@
     sub_parser_pms.add_argument(
         "--trigger", choices=["auto", "hand", ""], default="", help="触发者"
     )
     args = parser.parse_args()
     from src.rtk._base import Args
 
     pms_kwargs = {
-        Args.app_name.value: args.app or self.default_app,
-        Args.pms_user.value: args.pms_user or self.default_pms_user,
-        Args.pms_password.value: args.pms_password or self.default_pms_password,
-        Args.pms2csv.value: args.pms2csv or self.default_pms2csv,
-        Args.pms_link_csv.value: args.pms_link_csv or self.default_pms_link_csv,
-        Args.send2task.value: args.send2task or self.default_send2task,
+        Args.app_name.value: args.app,
+        Args.pms_user.value: args.pms_user,
+        Args.pms_password.value: args.pms_password,
+        Args.pms2csv.value: args.pms2csv,
+        Args.pms_link_csv.value: args.pms_link_csv,
+        Args.send2task.value: args.send2task,
         Args.task_id.value: args.task_id or GlobalConfig.TASK_ID,
         Args.trigger.value: args.trigger or GlobalConfig.TRIGGER,
     }
     if pms_kwargs.get(Args.pms2csv.value):
         from src.pms.pms2csv import Pms2Csv
 
         Pms2Csv(
```

### Comparing `youqu-2.6.1/youqu/src/pms/csv2pms.py` & `youqu-2.6.2/youqu/src/pms/csv2pms.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/pms/pms2csv.py` & `youqu-2.6.2/youqu/src/pms/pms2csv.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/pms/send2pms.py` & `youqu-2.6.2/youqu/src/pms/send2pms.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/pms/suite.py` & `youqu-2.6.2/youqu/src/pms/suite.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,59 +1,42 @@
 #!/usr/bin/env python3
 # _*_ coding:utf-8 _*_
-
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
-
 # SPDX-License-Identifier: GPL-2.0-only
-# pylint: disable=C0114
-# pylint: disable=C0301,C0116,R1710,W0201,R0903
 import json
 import re
 from collections import deque
 
 from src import logger
-from src.pms._base import _Base
-from src.pms._base import _unicode_to_cn
 from src.pms._base import MAX_CASE_NUMBER
+from src.pms._base import _Base
 
 
 class Suite(_Base):
     """获取测试套件关联的用例"""
 
     __author__ = "huangmingqiang@uniontech.com"
 
     def get_suite_data(self, suite_id):
         url = f"https://pms.uniontech.com/testsuite-view-{suite_id}-id_desc-1-{MAX_CASE_NUMBER}-1.json"
-        self.res = self.rx.open_url(url, timeout=10)
-        res_str = _unicode_to_cn(self.res)
+        res = self.rx.open_url(url, timeout=10)
         try:
-            res_dict = json.loads(res_str)
+            res_dict = json.loads(res)
         except json.decoder.JSONDecodeError:
             logger.error(f"爬取pms数据失败, 请检查模块 id 是否为: {suite_id}")
             return
 
-        cases = res_dict.get("data").get("cases")
+        cases = json.loads(res_dict.get("data")).get("cases")
         res_data = deque()
         for run_case_id in cases:
-            # 产品库ID
             case_id = cases.get(run_case_id).get("id")
-            # 用例库ID
             from_case_id = cases.get(run_case_id).get("fromCaseID")
             case_title = cases.get(run_case_id).get("title")
-            # 从用例标题中取出自动化用例id [001]
-            at_case_id = re.findall(r"\[(\d{3})\]", case_title)
-            # 如果id存在，并且之前没有出现过
-            try:
-                at_case_id = at_case_id[0]
-            except IndexError:
-                at_case_id = "   "
             res_data.append(
                 {
-                    "at_case_id": at_case_id,
                     "case_id": case_id,
                     "from_case_id": from_case_id,
                     "run_case_id": run_case_id,
                     "case_title": case_title,
                 }
             )
-
         return res_data
```

### Comparing `youqu-2.6.1/youqu/src/pms/task.py` & `youqu-2.6.2/youqu/src/pms/task.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,54 +1,43 @@
 #!/usr/bin/env python3
 # _*_ coding:utf-8 _*_
-
 # SPDX-FileCopyrightText: 2023 UnionTech Software Technology Co., Ltd.
-
 # SPDX-License-Identifier: GPL-2.0-only
-# pylint: disable=C0114,C0301,C0116,W0707,R0903
 import json
 import re
 from collections import deque
 
-from src.pms._base import _Base
-from src.pms._base import _unicode_to_cn
 from src.pms._base import MAX_CASE_NUMBER
+from src.pms._base import _Base
 
 
 class Task(_Base):
     """获取测试套件关联的用例"""
 
     __author__ = "huangmingqiang@uniontech.com"
 
     def get_task_data(self, task_id):
         task_json_url = f"https://pms.uniontech.com/testtask-cases-{task_id}-all-0-id_desc-4-{MAX_CASE_NUMBER}-1.json"
         res = self.rx.open_url(task_json_url, timeout=10)
-        res_str = _unicode_to_cn(res)
         try:
-            res_dict = json.loads(res_str)
+            res_dict = json.loads(res)
         except json.decoder.JSONDecodeError:
             raise EnvironmentError(
                 f"{task_json_url} 未获取到有效数据！\n 请检查你的PMS账号密码是否正确。"
             )
-        runs = res_dict.get("data").get("runs")
+        runs = json.loads(res_dict.get("data")).get("runs")
         runs_ids = deque()
         for run_case_id in runs:
             # 产品库ID
             case_id = runs.get(run_case_id).get("case")
             # 用例库ID
             from_case_id = runs.get(run_case_id).get("fromCaseID")
             case_title = runs.get(run_case_id).get("title")
-            at_case_id = re.findall(r"\[(\d{3})\]", case_title)
-            try:
-                at_case_id = at_case_id[0]
-            except IndexError:
-                at_case_id = "   "
             runs_ids.append(
                 {
-                    "at_case_id": at_case_id,
                     "case_id": case_id,
                     "from_case_id": from_case_id,
                     "run_case_id": run_case_id,
                     "case_title": case_title,
                 }
             )
         return runs_ids
```

### Comparing `youqu-2.6.1/youqu/src/remotectl/_base.py` & `youqu-2.6.2/youqu/src/remotectl/_base.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/remotectl/_remote_dogtail_ctl.py` & `youqu-2.6.2/youqu/src/remotectl/_remote_dogtail_ctl.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/remotectl/_remote_other_ctl.py` & `youqu-2.6.2/youqu/src/remotectl/_remote_other_ctl.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/remotectl/remote.py` & `youqu-2.6.2/youqu/src/remotectl/remote.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/rtk/_base.py` & `youqu-2.6.2/youqu/src/rtk/_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -54,24 +54,28 @@
     parallel = "parallel"
     autostart = "autostart"
     pyid2csv = "pyid2csv"
     export_csv_file = "export_csv_file"
     pms2csv = "pms2csv"
     pms_link_csv = "pms_link_csv"
     send2task = "send2task"
-    url = "url"
     startdate = "startdate"
     enddate = "enddate"
-    user = "user"
-    password = "password"
+    git_url = "git_url"
+    git_user = "git_user"
+    git_password = "git_password"
     depth = "depth"
     path_to = "path_to"
     execution_mode = "execution_mode"
     slaves = "slaves"
     pms_case_file_path = "pms_case_file_path"
+    json_backfill_base_url = "json_backfill_base_url"
+    json_backfill_task_id = "json_backfill_task_id"
+    json_backfill_user = "json_backfill_user"
+    json_backfill_password = "json_backfill_password"
 
 
 def transform_app_name(app_name):
     if not app_name:
         return None
     if "-" in app_name:
         raise ValueError(f"{app_name} 中存在 ['-'] 符号")
```

### Comparing `youqu-2.6.1/youqu/src/rtk/_cargo.py` & `youqu-2.6.2/youqu/src/rtk/_cargo.py`

 * *Files 10% similar despite different names*

```diff
@@ -105,22 +105,25 @@
         Args.project_name.value: args.project_name,
         Args.build_location.value: args.build_location,
         Args.line.value: args.line,
         Args.autostart.value: args.autostart,
         Args.slaves.value: args.slaves,
     }
     if local_kwargs.get(Args.autostart.value) or GlobalConfig.AUTOSTART:
-        import letmego
+        try:
+            import letmego
 
-        letmego.conf.setting.PASSWORD = GlobalConfig.PASSWORD
-        letmego.register_autostart_service(
-            user=GlobalConfig.USERNAME,
-            working_directory=GlobalConfig.ROOT_DIR,
-            cmd=f"pipenv run python manage.py {' '.join(cmd_args)}",
-        )
+            letmego.conf.setting.PASSWORD = GlobalConfig.PASSWORD
+            letmego.register_autostart_service(
+                user=GlobalConfig.USERNAME,
+                working_directory=GlobalConfig.ROOT_DIR,
+                cmd=f"pipenv run python manage.py {' '.join(cmd_args)}",
+            )
+        except ModuleNotFoundError:
+            ...
     return local_kwargs, args
 
 
 def remote_runner(parser, sub_parser_remote):
     sub_parser_remote.add_argument(
         "-c",
         "--clients",
@@ -147,37 +150,87 @@
         default=False,
         help="搭建测试环境,如果为yes，不管send_code是否为yes都会发送代码到测试机.",
     )
     sub_parser_remote.add_argument(
         "-cp", "--client_password", default="", help="测试机密码（全局）"
     )
     sub_parser_remote.add_argument(
+        "--git_url", default="", help="git仓库地址"
+    )
+    sub_parser_remote.add_argument(
+        "--git_user", default="", help="git仓库用户名"
+    )
+    sub_parser_remote.add_argument(
+        "--git_password", default="", help="git仓库密码"
+    )
+    sub_parser_remote.add_argument(
+        "-b", "--branch_or_tag", default="", help="分支或Tag"
+    )
+    sub_parser_remote.add_argument(
+        "-d", "--depth", default="", help="git仓库克隆深度"
+    )
+    sub_parser_remote.add_argument(
         "-y",
         "--parallel",
         default="",
         help=(
             "yes:表示所有测试机并行跑，执行相同的测试用例;"
             "no:表示测试机分布式执行，服务端会根据收集到的测试用例自动分配给各个测试机执行。"
         ),
     )
+    sub_parser_remote.add_argument(
+        "--json_backfill_base_url", default="", help="json报告回填的接口地址"
+    )
+    sub_parser_remote.add_argument(
+        "--json_backfill_task_id", default="", help="json报告回填所属任务id"
+    )
+    sub_parser_remote.add_argument(
+        "--json_backfill_user", default="", help="json报告回填的用户名"
+    )
+    sub_parser_remote.add_argument(
+        "--json_backfill_password", default="", help="json报告回填的密码"
+    )
 
     local_kwargs, args = local_runner(parser, sub_parser_remote)
     from src.rtk._base import Args
 
     remote_kwargs = {
         Args.clients.value: args.clients,
         Args.send_code.value: args.send_code,
         Args.build_env.value: args.build_env,
         Args.client_password.value: args.client_password,
+        Args.git_url.value: args.git_url or GlobalConfig.GIT_URL,
+        Args.git_user.value: args.git_user or GlobalConfig.GIT_USER,
+        Args.git_password.value: args.git_password or GlobalConfig.GIT_PASSWORD,
+        Args.branch.value: args.branch_or_tag or GlobalConfig.BRANCH,
+        Args.depth.value: args.depth or GlobalConfig.DEPTH,
         Args.parallel.value: args.parallel,
+        Args.json_backfill_base_url.value: args.json_backfill_base_url,
+        Args.json_backfill_task_id.value: args.json_backfill_task_id,
+        Args.json_backfill_user.value: args.json_backfill_user,
+        Args.json_backfill_password.value: args.json_backfill_password,
     }
     _remote_kwargs = {
         "remote_kwargs": remote_kwargs,
         "local_kwargs": local_kwargs,
     }
+
+    if remote_kwargs.get(Args.git_url.value):
+        if all(
+                [
+                    remote_kwargs.get(Args.git_user.value),
+                    remote_kwargs.get(Args.git_password.value),
+                ]
+        ):
+            from src.git.clone import sslclone as git_clone
+        else:
+            from src.git.clone import clone as git_clone
+        from src.git.check import check_git_installed
+        check_git_installed()
+        git_clone(**remote_kwargs)
     return _remote_kwargs
 
 
 def csv_control(parser=None, sub_parser_csv=None):
     sub_parser_csv.add_argument(
         "-a",
         "--app",
@@ -219,57 +272,7 @@
 
         LocalRunner(**csv_kwargs).local_run()
     else:
         logger.error(
             f"需要传递一些有用参数或配置项：{Args.pyid2csv.value} 或 {Args.export_csv_file.value}"
             "，您可以使用 -h 或 --help 查看支持的参数"
         )
-
-
-def playbook_control(parser, sub_parser_playbook):
-    sub_parser_playbook.add_argument("-l", "--url", default="", help="git仓库地址")
-    sub_parser_playbook.add_argument("-u", "--user", default="", help="git仓库用户名")
-    sub_parser_playbook.add_argument("-p", "--password", default="", help="git仓库地密码")
-    sub_parser_playbook.add_argument("-b", "--branch_or_tag", default="", help="分支或Tag")
-    sub_parser_playbook.add_argument("-d", "--depth", default="", help="git仓库克隆深度")
-    sub_parser_playbook.add_argument("-o", "--path_to", default="", help="仓库克隆到路径")
-    sub_parser_playbook.add_argument(
-        "-e", "--execution_mode", default="", choices=["", "run", "remote"], help="执行的模式：run、remote"
-    )
-    sub_parser_playbook.add_argument(
-        "-c",
-        "--clients",
-        default="",
-        help="远程执行, 输入远程机器的机器信息：user@ip:password, 多个机器用'/'连接",
-    )
-    sub_parser_playbook.add_argument(
-        "-s",
-        "--slaves",
-        default="",
-        help="多端交互式控制, 输入远程机器的机器信息：user@ip:password, 多个机器用'/'连接",
-    )
-    sub_parser_playbook.add_argument(
-        "-k", "--keywords", default="", help="需要执行用例的关键词表达式"
-    )
-    sub_parser_playbook.add_argument("-t", "--tags", default="", help="需要执行用例的标签表达式")
-    sub_parser_playbook.add_argument(
-        "-pf", "--pms_case_file_path", default="", help="PMS用例导出文件路径"
-    )
-    args = parser.parse_args()
-    from src.rtk._base import Args
-    from src.rtk.playbook import PlayBook
-
-    playbook_cli_kwargs = {
-        Args.url.value: args.url,
-        Args.user.value: args.user,
-        Args.password.value: args.password,
-        Args.branch.value: args.branch_or_tag,
-        Args.depth.value: args.depth,
-        Args.path_to.value: args.path_to,
-        Args.execution_mode.value: args.execution_mode,
-        Args.clients.value: args.clients,
-        Args.slaves.value: args.slaves,
-        Args.keywords.value: args.keywords,
-        Args.tags.value: args.tags,
-        Args.pms_case_file_path.value: args.pms_case_file_path,
-    }
-    PlayBook(playbook_cli_kwargs)
```

### Comparing `youqu-2.6.1/youqu/src/rtk/local_runner.py` & `youqu-2.6.2/youqu/src/rtk/local_runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 # SPDX-License-Identifier: GPL-2.0-only
 # pylint: disable=C0114
 # pylint: disable=C0301,R0913,R0914,W0613,R0912,R0915,E0401,C0413,C0103,C0116
 import json
 import re
 import sys
+from collections import Counter
 from os import chdir
 from os import environ
 from os import listdir
 from os import makedirs
 from os import system
 from os.path import exists
 from os.path import expanduser
@@ -27,16 +28,14 @@
 from setting.globalconfig import GetCfg
 from setting.globalconfig import GlobalConfig
 
 al_setting.html_title = GlobalConfig.REPORT_TITLE
 al_setting.report_name = GlobalConfig.REPORT_NAME
 al_setting.report_language = GlobalConfig.REPORT_LANGUAGE
 
-import letmego
-
 from src import logger
 from src.rtk._base import Args, write_json
 from src.requestx import RequestX
 from src.rtk._base import transform_app_name
 
 environ["DISPLAY"] = ":0"
 
@@ -45,50 +44,50 @@
     """
     本地执行器
     """
 
     __author__ = "Mikigo <huangmingqiang@uniontech.com>"
 
     def __init__(
-        self,
-        app_name=None,
-        keywords=None,
-        tags=None,
-        report_formats=None,
-        max_fail=None,
-        reruns=None,
-        record_failed_case=None,
-        clean=None,
-        log_level=None,
-        timeout=None,
-        debug=False,
-        noskip=None,
-        ifixed=None,
-        send_pms=None,
-        task_id=None,
-        suite_id=None,
-        trigger=None,
-        resolution=None,
-        case_file=None,
-        deb_path=None,
-        pms_user=None,
-        pms_password=None,
-        pms_info_file=None,
-        top=None,
-        lastfailed=None,
-        duringfail=None,
-        repeat=None,
-        project_name=None,
-        build_location=None,
-        line=None,
-        collection_only=None,
-        autostart=None,
-        export_csv_file=None,
-        slaves=None,
-        **kwargs,
+            self,
+            app_name=None,
+            keywords=None,
+            tags=None,
+            report_formats=None,
+            max_fail=None,
+            reruns=None,
+            record_failed_case=None,
+            clean=None,
+            log_level=None,
+            timeout=None,
+            debug=False,
+            noskip=None,
+            ifixed=None,
+            send_pms=None,
+            task_id=None,
+            suite_id=None,
+            trigger=None,
+            resolution=None,
+            case_file=None,
+            deb_path=None,
+            pms_user=None,
+            pms_password=None,
+            pms_info_file=None,
+            top=None,
+            lastfailed=None,
+            duringfail=None,
+            repeat=None,
+            project_name=None,
+            build_location=None,
+            line=None,
+            collection_only=None,
+            autostart=None,
+            export_csv_file=None,
+            slaves=None,
+            **kwargs,
     ):
         logger("INFO")
         try:
             github_tags = RequestX().open_url(
                 f"https://api.github.com/repos/linuxdeepin/youqu/tags", timeout=1
             )
             latest_tag = json.loads(github_tags)[0].get("name")
@@ -278,35 +277,35 @@
             cmd.extend(["--slaves", self.slaves])
 
         report_formats = default.get(Args.report_formats.value)
         if report_formats:
             report_formats = [i.strip() for i in report_formats.split(",")]
             # allure
             if (GlobalConfig.ReportFormat.ALLURE in report_formats) and (
-                GlobalConfig.ReportFormat.JSON not in report_formats
+                    GlobalConfig.ReportFormat.JSON not in report_formats
             ):
                 self.make_allure_report(cmd, GlobalConfig.ReportFormat.ALLURE, proj_path)
             # xml
             if GlobalConfig.ReportFormat.XML in report_formats:
                 self.make_xml_report(
                     app_dir,
                     default.get(Args.case_file.value),
                     cmd,
                     GlobalConfig.ReportFormat.XML,
                     proj_path,
                 )
             # json
             if (GlobalConfig.ReportFormat.ALLURE not in report_formats) and (
-                GlobalConfig.ReportFormat.JSON in report_formats
+                    GlobalConfig.ReportFormat.JSON in report_formats
             ):
                 self.make_allure_report(cmd, GlobalConfig.ReportFormat.ALLURE, proj_path)
                 self.make_dir(join(GlobalConfig.REPORT_PATH, GlobalConfig.ReportFormat.JSON))
             # allure json
             if (GlobalConfig.ReportFormat.ALLURE in report_formats) and (
-                GlobalConfig.ReportFormat.JSON in report_formats
+                    GlobalConfig.ReportFormat.JSON in report_formats
             ):
                 self.make_allure_report(cmd, GlobalConfig.ReportFormat.ALLURE, proj_path)
                 self.make_dir(join(GlobalConfig.REPORT_PATH, GlobalConfig.ReportFormat.JSON))
         return cmd
 
     @staticmethod
     def set_recursion_limit(strings):
@@ -354,44 +353,48 @@
 
         if self.project_name and self.build_location and self.line:
             write_json(
                 project_name=self.project_name,
                 build_location=self.build_location,
                 line=self.line,
             )
+
         allure_report_path = join(GlobalConfig.ALLURE_REPORT_PATH, GlobalConfig.ReportFormat.ALLURE)
         allure_html_report_path = join(GlobalConfig.ALLURE_REPORT_PATH, "allure_html")
 
         json_report_path = join(GlobalConfig.ALLURE_REPORT_PATH, GlobalConfig.ReportFormat.JSON)
 
         if self.default.get(Args.report_formats.value):
             report_formats = [
                 i.strip() for i in self.default.get(Args.report_formats.value).split(",")
             ]
             if (GlobalConfig.ReportFormat.ALLURE in report_formats) or (
-                GlobalConfig.ReportFormat.JSON in report_formats
+                    GlobalConfig.ReportFormat.JSON in report_formats
             ):
                 if exists(allure_html_report_path):
                     system(f"rm -rf {allure_html_report_path}")
                 makedirs(allure_html_report_path)
 
                 AllureCustom.gen(allure_report_path, allure_html_report_path)
 
                 if GlobalConfig.ReportFormat.JSON in report_formats:
                     system(
                         f"cp {allure_html_report_path}/widgets/suites.json "
                         f"{json_report_path}/"
                         f"result_{self.default.get(Args.app_name.value)}_{GlobalConfig.TIME_STRING}_{GlobalConfig.HOST_IP.replace('.', '')}.json"
                     )
-
-        if exists(letmego.conf.setting.RUNNING_MAN_FILE):
-            letmego.unregister_autostart_service()
-            letmego.clean_running_man(
-                copy_to=f"{GlobalConfig.REPORT_PATH}/_running_man_{GlobalConfig.TIME_STRING}.log"
-            )
+        try:
+            import letmego
+            if exists(letmego.conf.setting.RUNNING_MAN_FILE):
+                letmego.unregister_autostart_service()
+                letmego.clean_running_man(
+                    copy_to=f"{GlobalConfig.REPORT_PATH}/_running_man_{GlobalConfig.TIME_STRING}.log"
+                )
+        except ModuleNotFoundError:
+            ...
 
     def install_deb(self):
         logger.info("安装deb包")
         system(
             f"cd {self.default.get(Args.deb_path.value)}/ && echo {GlobalConfig.PASSWORD} | sudo -S dpkg -i *.deb"
         )
         logger.info("deb包安装完成")
```

### Comparing `youqu-2.6.1/youqu/src/rtk/remote_runner.py` & `youqu-2.6.2/youqu/src/rtk/remote_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,25 +6,24 @@
 # SPDX-License-Identifier: GPL-2.0-only
 # pylint: disable=C0114
 # pylint: disable=E0401,C0413,R0902,R0913,R0914,W0613,C0301,C0415,C0103
 import json
 import os
 import re
 import sys
-from configparser import ConfigParser
+from concurrent.futures import ALL_COMPLETED
+from concurrent.futures import ThreadPoolExecutor
+from concurrent.futures import wait
 from itertools import cycle
 from os import listdir
 from os import makedirs
 from os import popen
 from os import system
 from os.path import exists
 from os.path import splitext
-from concurrent.futures import ThreadPoolExecutor
-from concurrent.futures import wait
-from concurrent.futures import ALL_COMPLETED
 from time import sleep
 from time import strftime
 
 from allure_custom import AllureCustom
 from allure_custom.conf import setting
 
 from setting.globalconfig import GlobalConfig
@@ -46,32 +45,32 @@
     远程执行器：控制多台测试机远程执行用例。
     在 setting/remote.ini 里面配置要执行的测试机信息。
     """
 
     __author__ = "Mikigo <huangmingqiang@uniontech.com>"
 
     def __init__(
-        self,
-        remote_kwargs: dict = None,
-        local_kwargs: dict = None,
+            self,
+            remote_kwargs: dict = None,
+            local_kwargs: dict = None,
     ):
         self.remote_kwargs = remote_kwargs
         self.local_kwargs = local_kwargs
         logger("INFO")
         self.parallel = conf.PARALLEL
         self.clean_server_report_dir = conf.CLEAN_SERVER_REPORT_DIR
         self.clean_client_report_dir = conf.CLEAN_CLIENT_REPORT_DIR
         self.send_code = conf.SEND_CODE
         self.scan = int(conf.SCAN)
         self.client_env = conf.BUILD_ENV
         self.client_password = conf.CLIENT_PASSWORD
 
         self._default = {
             Args.client_password.value: remote_kwargs.get("client_password")
-            or self.client_password,
+                                        or self.client_password,
         }
 
         client_dict = {}
         _client = remote_kwargs.get("clients") or conf.CLIENTS
         if _client:
             clients = _client.split("/")
             for index, client in enumerate(clients):
@@ -92,43 +91,52 @@
             Args.app_name.value: transform_app_name(
                 local_kwargs.get("app_name") or GlobalConfig.APP_NAME
             ),
             Args.clients.value: client_dict,
             Args.send_code.value: remote_kwargs.get("send_code") or self.send_code,
             Args.build_env.value: remote_kwargs.get("build_env") or self.client_env,
             Args.parallel.value: remote_kwargs.get("parallel") or self.parallel,
+            Args.json_backfill_base_url.value: remote_kwargs.get("json_backfill_base_url"),
+            Args.json_backfill_task_id.value: remote_kwargs.get("json_backfill_task_id"),
+            Args.json_backfill_user.value: remote_kwargs.get("json_backfill_user"),
+            Args.json_backfill_password.value: remote_kwargs.get("json_backfill_password"),
         }
         # 客户端地址
         if "/home/" not in GlobalConfig.ROOT_DIR:
             raise EnvironmentError
         self.server_project_path = "/".join(GlobalConfig.ROOT_DIR.split("/")[3:])
         self.client_report_path = lambda x: f"/home/{x}/{self.server_project_path}/report"
         self.client_allure_report_path = (
-            lambda x: f"/home/{x}/{self.server_project_path}/{GlobalConfig.report_cfg.get('ALLURE_REPORT_PATH', default='report')}/allure".replace(
+            lambda
+                x: f"/home/{x}/{self.server_project_path}/{GlobalConfig.report_cfg.get('ALLURE_REPORT_PATH', default='report')}/allure".replace(
                 "//", "/"
             )
         )
         self.client_pms_json_report_path = (
             lambda x, y: f"/home/{x}/{self.server_project_path}/report/pms_{y}"
         )
-
+        self.client_json_report_path = (
+            lambda x: f"/home/{x}/{self.server_project_path}/report/json"
+        )
+        self.strf_time = strftime("%m%d%p%I%M%S")
+        self.server_detail_json_path = f"{GlobalConfig.REPORT_PATH}/json/{self.strf_time}_remote"
         self.client_xml_report_path = (
-            lambda x: f"/home/{x}/{self.server_project_path}/{GlobalConfig.report_cfg.get('XML_REPORT_PATH', default='report')}/xml".replace(
+            lambda
+                x: f"/home/{x}/{self.server_project_path}/{GlobalConfig.report_cfg.get('XML_REPORT_PATH', default='report')}/xml".replace(
                 "//", "/"
             )
         )
         self.client_list = list(self.default.get(Args.clients.value).keys())
         _pty = "t"
         if len(self.client_list) >= 2:
             _pty = "T"
         self.ssh = f"sshpass -p '%s' ssh -{_pty}"
         self.scp = "sshpass -p '%s' scp -r"
         self.rsync = "sshpass -p '%s' rsync -av -e ssh"
         self.empty = "> /dev/null 2>&1"
-        self.strf_time = strftime("%m%d%p%I%M%S")
 
         self.collection_json = False
         self.server_json_dir_id = None
         self.pms_user = None
         self.pms_password = None
 
     def send_code_to_client(self, user, _ip, password):
@@ -147,25 +155,36 @@
         system(
             f'{self.ssh % password} {user}@{_ip} "mkdir -p ~/{self.server_project_path}" {self.empty}'
         )
         # 过滤目录
         app_name: str = self.default.get(Args.app_name.value)
         exclude = ""
         for i in [
-            "report",
             "__pycache__",
             ".pytest_cache",
             ".vscode",
             ".idea",
             ".git",
+            ".github",
+            ".reuse",
             "docs",
-            "site",
+            "node_modules",
+            "report",
+            ".gitignore",
+            "CONTRIBUTING.md",
+            "LICENSE",
+            "package.json",
+            "Pipfile",
+            "Pipfile.lock",
+            "pnpm-lock.yaml",
+            "publish.sh",
+            "pyproject.toml",
             "README.md",
-            "README.zh_CN.md",
             "RELEASE.md",
+            "ruff.toml",
         ]:
             exclude += f"--exclude='{i}' "
         if app_name:
             for i in listdir(GlobalConfig.APPS_PATH):
                 if i == "__init__.py":
                     continue
                 if app_name.replace("-", "_") != i:
@@ -290,14 +309,16 @@
             if i[1] is None:
                 continue
             i = list(i)
             i[0] = f"--{i[0]}"
             i[1] = f"'{i[1]}'"
             if i[0] == "--app_name":
                 real_app_name = f"apps/{self.default.get(Args.app_name.value)}"
+                if self.default.get(Args.app_name.value) is None:
+                    real_app_name = ""
                 continue
 
             _tmp_args.extend(i)
         cmd.extend(
             [
                 f"~/{self.server_project_path}/{real_app_name}",
                 "&&",
@@ -308,20 +329,20 @@
         from src.rtk.local_runner import LocalRunner
 
         lr = LocalRunner(debug=True)
         lr_args = {k: v for k, v in lr.export_default.items() if v}
         rr_args = {k: v for k, v in self.local_kwargs.items() if v}
         lr_args.update(rr_args)
         if all(
-            [
-                lr_args.get(Args.task_id.value),
-                lr_args.get(Args.pms_user.value),
-                lr_args.get(Args.pms_password.value),
-                lr_args.get(Args.send_pms.value) == "finish",
-            ]
+                [
+                    lr_args.get(Args.task_id.value),
+                    lr_args.get(Args.pms_user.value),
+                    lr_args.get(Args.pms_password.value),
+                    lr_args.get(Args.send_pms.value) == "finish",
+                ]
         ):
             lr_args[Args.trigger.value] = "hand"
             self.collection_json = True
             self.pms_user = lr_args.get(Args.pms_user.value)
             self.pms_password = lr_args.get(Args.pms_password.value)
             self.server_json_dir_id = lr_args.get(Args.task_id.value)
         pytest_cmd = lr.create_pytest_cmd(
@@ -329,16 +350,16 @@
             default=lr_args,
             proj_path=f"/home/{user}/{self.server_project_path}",
         )
 
         cmd.extend(pytest_cmd)
         cmd.append('"')
         cmd_str = " ".join(cmd)
+        logger.info(f"\n{cmd_str}\n")
         if self.default.get(Args.debug.value):
-            logger.info(f"\n{cmd_str}\n")
             logger.info("DEBUG 模式不执行用例!")
         else:
             system(cmd_str)
 
     def pytest_co_cmd(self):
         """
          创建收集用例的命令行参数
@@ -408,28 +429,43 @@
         """
          远程复制报告
         :param user:
         :param _ip:
         :param password:
         :return:
         """
-        server_allure_path = f"{GlobalConfig.REPORT_PATH}/allure/{self.strf_time}_ip{_ip}_{self.default.get(Args.app_name.value)}"
-        self.make_dir(server_allure_path)
-        system(
-            f"{self.scp % password} {user}@{_ip}:{self.client_allure_report_path(user)}/* {server_allure_path}/ {self.empty}"
-        )
-        generate_allure_html = f"{server_allure_path}/html"
+        html_dir_endswith = f"_{self.default.get(Args.app_name.value)}" if self.default.get(Args.app_name.value) else ""
+        if not self.default.get(Args.parallel.value):
+            self.nginx_server_allure_path = f"{GlobalConfig.REPORT_PATH}/allure/{self.strf_time}{html_dir_endswith}"
+            self.make_dir(self.nginx_server_allure_path)
+            system(
+                f"{self.scp % password} {user}@{_ip}:{self.client_allure_report_path(user)}/* {self.nginx_server_allure_path}/ {self.empty}"
+            )
+        else:
+            server_allure_path = f"{GlobalConfig.REPORT_PATH}/allure/{self.strf_time}_ip{_ip}{html_dir_endswith}"
+            self.make_dir(server_allure_path)
+            system(
+                f"{self.scp % password} {user}@{_ip}:{self.client_allure_report_path(user)}/* {server_allure_path}/ {self.empty}"
+            )
+            generate_allure_html = f"{server_allure_path}/html"
+            AllureCustom.gen(server_allure_path, generate_allure_html)
 
-        AllureCustom.gen(server_allure_path, generate_allure_html)
         if self.collection_json:
             server_json_path = f"{GlobalConfig.REPORT_PATH}/pms_{self.server_json_dir_id}/{self.strf_time}_ip{_ip}_{self.default.get(Args.app_name.value)}"
             self.make_dir(server_json_path)
             system(
                 f"{self.scp % password} {user}@{_ip}:{self.client_pms_json_report_path(user, self.server_json_dir_id)}/* {server_json_path}/ {self.empty}"
             )
+        self.make_dir(self.server_detail_json_path)
+        system(
+            f"{self.scp % password} {user}@{_ip}:{self.client_json_report_path(user)}/detail_report.json {self.server_detail_json_path}/detail_report_{_ip}.json"
+        )
+        system(
+            f"{self.scp % password} {user}@{_ip}:{self.client_json_report_path(user)}/summarize.json {self.server_detail_json_path}/summarize_{_ip}.json"
+        )
 
     def remote_finish_send_to_pms(self):
         json_path = f"{GlobalConfig.REPORT_PATH}/pms_{self.server_json_dir_id}"
         self.make_dir(json_path)
         res = {}
         for root, dirs, files in os.walk(json_path):
             for file in files:
@@ -471,14 +507,45 @@
             wait(_ps, return_when=ALL_COMPLETED)
         else:
             user, _ip, password = self.default.get(Args.clients.value).get(client_list[0])
             self.scp_report(user, _ip, password)
 
         if self.collection_json:
             self.remote_finish_send_to_pms()
+        if all([
+            self.default.get(Args.json_backfill_base_url.value),
+            self.default.get(Args.json_backfill_task_id.value),
+            self.default.get(Args.json_backfill_user.value),
+            self.default.get(Args.json_backfill_password.value)
+        ]):
+            from src.rtk.json_backfill import JsonBackfill
+            JsonBackfill(
+                base_url=self.default.get(Args.json_backfill_base_url.value),
+                username=self.default.get(Args.json_backfill_user.value),
+                password=self.default.get(Args.json_backfill_password.value),
+            ).remote_backfill(self.server_detail_json_path, self.default.get(Args.json_backfill_task_id.value))
+        # 分布式执行的情况下需要汇总结果
+        if not self.default.get(Args.parallel.value):
+            summarize = {
+                "total": 0,
+                "pass": 0,
+                "fail": 0,
+                "skip": 0,
+            }
+            for file in os.listdir(self.server_detail_json_path):
+                if file.startswith("summarize_") and file.endswith(".json"):
+                    with open(f"{self.server_detail_json_path}/{file}", "r", encoding="utf-8") as f:
+                        res = json.load(f)
+                    for i in summarize.keys():
+                        summarize[i] += res.get(i)
+            with open(f"{self.server_detail_json_path}/summarize.json", "w", encoding="utf-8") as _f:
+                _f.write(json.dumps(summarize, indent=2, ensure_ascii=False))
+
+            generate_allure_html = f"{self.nginx_server_allure_path}/html"
+            AllureCustom.gen(self.nginx_server_allure_path, generate_allure_html)
 
     def parallel_run(self, client_list):
         """
          并行跑
         :param client_list:
         :return:
         """
```

### Comparing `youqu-2.6.1/youqu/src/utils/_env_base.sh` & `youqu-2.6.2/youqu/src/utils/_env_base.sh`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/utils/check_python_source.py` & `youqu-2.6.2/youqu/src/utils/check_python_source.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/utils/env_dev.sh` & `youqu-2.6.2/youqu/src/utils/env_dev.sh`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 
     if [ "${debian_platform}" = "true" ]; then
         sudo apt update
     fi
 
     deb_array=(
         python3-pip
-        sshpass
         scrot
         python3-tk
         python3-pyatspi
         openjdk-11-jdk-headless
         python3-opencv
     )
 
@@ -68,32 +67,30 @@
     pytest-rerunfailures==10.2
     pytest-timeout==2.1.0
     allure-pytest==2.9.45
     pdocr-rpc
     allure-custom
     funnylog
     image-center
-    letmego
-    tomli
 )
 # 裁剪基础环境
 if [ "${ENV_CUT_FLAG}" = "cut" ]; then
     pip_array=(
         pytest==6.2.5
         pytest-rerunfailures==10.2
         pytest-timeout==2.1.0
         allure-pytest==2.9.45
         allure-custom
         funnylog
-        tomli
     )
 fi
 
 if [ ${debian_platform} == false ]; then
         pip_array[${#pip_array[@]}]=numpy
+        pip_array[${#pip_array[@]}]="pillow==8.4.0"
     fi
 
 for p in ${pip_array[*]}
 do
     sudo pip3 install ${p} > /tmp/env.log 2>&1
     check_status ${p}
     pip3 list | grep -v grep | grep ${p}
```

### Comparing `youqu-2.6.1/youqu/src/utils/env_vir.sh` & `youqu-2.6.2/youqu/src/utils/env_vir.sh`

 * *Files 2% similar despite different names*

```diff
@@ -18,29 +18,27 @@
     if [ "${debian_platform}" = "true" ]; then
         sudo apt update
     fi
 
     deb_array=(
         python3-pip
         python3-tk
-        sshpass
         scrot
         openjdk-11-jdk-headless
         gir1.2-atspi-2.0
         libatk-adaptor
         at-spi2-core
         python3-opencv
     )
     cd ${ROOT_DIR}/src/utils
     BASICENV=$(python3 sub_env_cut.py)
     if [ "${BASICENV}" = "BASICENV" ]; then
         ENV_CUT_FLAG="cut"
         deb_array=(
             python3-pip
-            sshpass
             openjdk-11-jdk-headless
         )
     fi
 
     if [ "${debian_platform}" = "false" ]; then
         deb_array[${#deb_array[@]}]=java-11-openjdk-headless
         deb_array[${#deb_array[@]}]=python3-tkinter
@@ -122,27 +120,24 @@
     pytest-rerunfailures==10.2
     pytest-timeout==2.1.0
     allure-pytest==2.9.45
     funnylog
     pdocr-rpc
     image-center
     allure-custom
-    letmego
-    tomli
 )
 
 if [ "${ENV_CUT_FLAG}" = "cut" ]; then
     pip_array=(
         pytest==6.2.5
         pytest-rerunfailures==10.2
         pytest-timeout==2.1.0
         allure-pytest==2.9.45
         allure-custom
         funnylog
-        tomli
     )
 fi
 
 for p in ${pip_array[*]}
 do
     pipenv run pip install ${p} -i ${pypi_mirror} > /tmp/env.log 2>&1
     check_status ${p}
@@ -178,24 +173,21 @@
 check_status auto_uos
 pip_show=$(pipenv run pip show auto_uos | grep Location)
 public_location=$(echo "${pip_show}" | cut -d ":" -f2 | python3 -c "s=input();print(s.strip())")
 sudo rm -rf ${ROOT_DIR}/public
 sudo cp -r ${public_location}/auto_uos ${ROOT_DIR}/public
 sudo chmod -R 777 ${ROOT_DIR}/public
 
+cd ${ROOT_DIR}
 rm -rf Pipfile
 echo "${python_virtualenv_path}"
 pipenv run pip list
 system_env
 
 echo 'pipenv run python "$@"' | sudo tee /usr/bin/youqu > /dev/null 2>&1
 echo "pipenv shell" | sudo tee /usr/bin/youqu-shell > /dev/null 2>&1
 echo "pipenv --rm" | sudo tee /usr/bin/youqu-rm > /dev/null 2>&1
 sudo chmod +x /usr/bin/youqu
 sudo chmod +x /usr/bin/youqu-shell
 sudo chmod +x /usr/bin/youqu-rm
 
-#cp --force ${ROOT_DIR}/src/utils/command_complete.sh ${HOME}/.config/
-#echo "source ${HOME}/.config/command_complete.sh" >> $HOME/.bashrc
-#source $HOME/.bashrc
-
 cd ${ROOT_DIR};youqu manage.py -h
```

### Comparing `youqu-2.6.1/youqu/src/utils/pylint.sh` & `youqu-2.6.2/youqu/src/utils/pylint.sh`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/utils/sslclone.sh` & `youqu-2.6.2/youqu/src/utils/sslclone.sh`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/src/utils/sub_deb.py` & `youqu-2.6.2/youqu/src/utils/sub_deb.py`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/youqu/README.md` & `youqu-2.6.2/youqu/README.md`

 * *Files identical despite different names*

### Comparing `youqu-2.6.1/PKG-INFO` & `youqu-2.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: youqu
-Version: 2.6.1
+Version: 2.6.2
 Summary: youqu
 Project-URL: Source, https://github.com/linuxdeepin/youqu
 Project-URL: Documentation, https://linuxdeepin.github.io/youqu
 Author-email: mikigo <huangmingqiang@uniontech.com>
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3.7
+Classifier: Programming Language :: Python :: 3.6
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 <p align="center">
   <a href="https://linuxdeepin.github.io/youqu">
     <img src="./docs/assets/logo.png" width="520" alt="YouQu">
   </a>
 </p>
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
-Metadata-Version: 2.1 Name: youqu Version: 2.6.1 Summary: youqu Project-URL:
+Metadata-Version: 2.1 Name: youqu Version: 2.6.2 Summary: youqu Project-URL:
 Source, https://github.com/linuxdeepin/youqu Project-URL: Documentation, https:
 //linuxdeepin.github.io/youqu Author-email: mikigo
 uniontech.com> Classifier: License :: OSI Approved :: GNU General Public
 License v2 (GPLv2) Classifier: Operating System :: OS Independent Classifier:
-Programming Language :: Python :: 3.7 Requires-Python: >=3.7 Description-
+Programming Language :: Python :: 3.6 Requires-Python: >=3.6 Description-
 Content-Type: text/markdown
                                     _[_Y_o_u_Q_u_]
 YYoouuQQuu?ï?¼??æ???è?¶?£?ï?¼??ï?¼??ä?¸??ä?¸?ª?ä?½?¿?ç??¨?ç?®??å???ä?¸??å???è??½?å?¼?º?å?¤?§?ç???è??ª?å??¨?å???æ?µ??è?¯??å??º?ç?¡??æ?¡??æ??¶?ã??
 [![GitHub issues](https://img.shields.io/github/issues/linuxdeepin/
 youqu?color=%23F79431)](https://github.com/linuxdeepin/youqu/issues) [![PyPI]
 (https://img.shields.io/pypi/v/
 youqu?style=flat&logo=github&link=https%3A%2F%2Fpypi.org%2Fproject%2Fyouqu%2F&color=%23F79431)]
```

