# Comparing `tmp/craftax-1.4.1.tar.gz` & `tmp/craftax-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "craftax-1.4.1.tar", last modified: Tue Apr 30 15:35:29 2024, max compression
+gzip compressed data, was "craftax-1.4.2.tar", last modified: Wed May 29 14:38:20 2024, max compression
```

## Comparing `craftax-1.4.1.tar` & `craftax-1.4.2.tar`

### file list

```diff
@@ -1,263 +1,264 @@
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:35:29.080845 craftax-1.4.1/
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1059 2024-04-03 13:05:48.000000 craftax-1.4.1/LICENSE
--rw-rw-r--   0 mikey     (1000) mikey     (1000)       73 2024-04-30 15:29:51.000000 craftax-1.4.1/MANIFEST.in
--rw-r--r--   0 mikey     (1000) mikey     (1000)    10707 2024-04-30 15:35:29.080845 craftax-1.4.1/PKG-INFO
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     9822 2024-04-30 15:33:21.000000 craftax-1.4.1/README.md
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:35:29.068845 craftax-1.4.1/craftax/
--rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/__init__.py
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:35:29.068845 craftax-1.4.1/craftax/craftax/
--rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/__init__.py
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:35:29.076845 craftax-1.4.1/craftax/craftax/assets/
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      607 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/0.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1827 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/1.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1501 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/2.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1559 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/3.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1533 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/4.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1518 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/5.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1567 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/6.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1538 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/7.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1506 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/8.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1535 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/9.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1825 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/arrow-down.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1731 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/arrow-left.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1752 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/arrow-right.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1833 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/arrow-up.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      603 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/arrow_fire_enchantment.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      602 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/arrow_ice_enchantment.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      652 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/bat.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      719 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/book.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      654 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/boots_fire_enchantment.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      652 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/boots_ice_enchantment.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      693 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/bow.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      953 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/chest.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      670 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/chestplate_fire_enchantment.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      670 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/chestplate_ice_enchantment.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      866 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/coal.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1983 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/cow.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      621 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/dagger.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     5735 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/debug-2.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     5762 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/debug-3.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     5761 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/debug.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)       84 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/debug_tile.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      996 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/deep_thing.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      790 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/dexterity.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      839 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/diamond.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      605 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/diamond_boots.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      685 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/diamond_chestplate.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      642 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/diamond_helmet.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      609 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/diamond_pants.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      733 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/diamond_pickaxe.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      714 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/diamond_sword.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2492 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/drink.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1087 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/enchantment_table_fire.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1092 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/enchantment_table_ice.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2213 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/energy.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2449 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/fence.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      674 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/fire_elemental.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      710 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/fire_grass.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      959 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/fire_stone.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1140 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/fire_tree.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      670 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/fireball.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2292 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/food.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1141 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/fountain.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      723 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/frost_troll.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      910 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/furnace.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      860 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/gnome_archer.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      847 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/gnome_warrior.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      691 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/grass.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1099 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/grave.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1210 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/grave2.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1161 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/grave3.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      741 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/gravel.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2721 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/health.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      666 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/helmet_fire_enchantment.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      666 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/helmet_ice_enchantment.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      689 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/ice_elemental.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      719 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/ice_grass.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      994 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/ice_shrub.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      668 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/iceball.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      933 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/intelligence.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1048 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/iron.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      613 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/iron_boots.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      681 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/iron_chestplate.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      642 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/iron_helmet.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      608 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/iron_pants.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2354 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/iron_pickaxe.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2390 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/iron_sword.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      839 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/knight.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      889 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/knight_archer.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      737 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/kobold.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      729 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/ladder_down.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      855 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/ladder_down_blocked.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      612 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/ladder_up.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2130 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/lava.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      755 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/leaves.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      758 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/lizard.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      745 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/log.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      695 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/mana.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1150 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/necromancer.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1128 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/necromancer_vulnerable.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      769 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/orc_mage.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      777 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/orc_soldier.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      709 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/pants_fire_enchantment.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      702 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/pants_ice_enchantment.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     7488 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/path.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      325 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/path_moss.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      809 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/pigman.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2154 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/plant-ripe.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2511 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/plant-young.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2080 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/plant.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      219 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/plant_on_grass.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     6186 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/player-down.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     6195 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/player-left.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     6212 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/player-right.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     6590 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/player-sleep.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     6144 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/player-up.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      813 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/player.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      715 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/potion_blue.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      723 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/potion_cyan.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      705 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/potion_green.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      715 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/potion_pink.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      708 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/potion_red.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      707 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/potion_yellow.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      245 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/ripe_plant_on_grass.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1110 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/ruby.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      729 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/sand.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1817 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/sapling.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      957 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/sapphire.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     5993 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/skeleton.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      673 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/slimeball.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      729 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/snail.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      668 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/spider.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1219 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/stalagmite.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     7242 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/stone.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2345 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/stone_pickaxe.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2429 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/stone_sword.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      670 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/strength.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      613 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/sword_fire_enchantment.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      620 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/sword_ice_enchantment.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      885 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/table.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)  1769538 2024-03-26 15:46:49.000000 craftax-1.4.1/craftax/craftax/assets/texture_cache.pbz2
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      615 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/torch_in_inventory.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1197 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/torch_on_path.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     7782 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/tree.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      698 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/troll.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2127 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/unknown.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      126 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/wall.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      163 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/wall2.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      198 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/wall_moss.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2198 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/water.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1577 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/wood.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2045 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/wood_pickaxe.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2453 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/wood_sword.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      718 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/xp.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2089 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/assets/zombie.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)    34413 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/constants.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2741 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/craftax_state.py
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:35:29.076845 craftax-1.4.1/craftax/craftax/envs/
--rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/envs/__init__.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     4853 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/envs/craftax_pixels_env.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     5388 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/envs/craftax_symbolic_env.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)   106195 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/game_logic.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     7007 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/play_craftax.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)    41178 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/renderer.py
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:35:29.076845 craftax-1.4.1/craftax/craftax/util/
--rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/util/__init__.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)    11631 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/util/game_logic_utils.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      594 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/util/maths_utils.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2534 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/util/noise.py
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:35:29.076845 craftax-1.4.1/craftax/craftax/world_gen/
--rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/world_gen/__init__.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)    24840 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/world_gen/world_gen.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     9213 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax/world_gen/world_gen_configs.py
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:35:29.076845 craftax-1.4.1/craftax/craftax_classic/
--rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/__init__.py
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:35:29.076845 craftax-1.4.1/craftax/craftax_classic/assets/
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1827 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/1.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1501 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/2.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1559 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/3.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1533 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/4.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1518 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/5.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1567 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/6.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1538 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/7.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1506 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/8.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1535 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/9.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1825 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/arrow-down.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1731 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/arrow-left.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1752 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/arrow-right.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1833 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/arrow-up.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      866 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/coal.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1983 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/cow.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     5735 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/debug-2.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     5762 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/debug-3.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     5761 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/debug.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)       84 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/debug_tile.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      839 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/diamond.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2492 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/drink.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2213 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/energy.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2449 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/fence.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2292 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/food.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      910 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/furnace.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      691 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/grass.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2721 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/health.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1048 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/iron.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2354 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/iron_pickaxe.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2390 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/iron_sword.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2130 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/lava.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      755 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/leaves.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      745 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/log.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     7488 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/path.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2154 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/plant-ripe.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2511 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/plant-young.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2080 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/plant.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      219 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/plant_on_grass.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     6186 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/player-down.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     6195 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/player-left.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     6212 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/player-right.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     6590 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/player-sleep.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     6144 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/player-up.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      813 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/player.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      245 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/ripe_plant_on_grass.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      729 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/sand.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1817 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/sapling.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     5993 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/skeleton.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     7242 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/stone.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2345 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/stone_pickaxe.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2429 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/stone_sword.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      885 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/table.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)  1262198 2024-03-26 15:51:57.000000 craftax-1.4.1/craftax/craftax_classic/assets/texture_cache_classic.pbz2
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     7782 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/tree.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2127 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/unknown.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2198 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/water.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1577 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/wood.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2045 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/wood_pickaxe.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2453 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/wood_sword.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2089 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/assets/zombie.png
--rw-rw-r--   0 mikey     (1000) mikey     (1000)    13946 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/constants.py
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:35:29.076845 craftax-1.4.1/craftax/craftax_classic/envs/
--rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/envs/__init__.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      505 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/envs/common.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     4973 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/envs/craftax_pixels_env.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2086 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/envs/craftax_state.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     5443 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/envs/craftax_symbolic_env.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)    58460 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/game_logic.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     4970 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/play_craftax_classic.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)    24401 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/renderer.py
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:35:29.080845 craftax-1.4.1/craftax/craftax_classic/util/
--rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/util/__init__.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2535 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/util/noise.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)    11690 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_classic/world_gen.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2441 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/craftax_env.py
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:35:29.080845 craftax-1.4.1/craftax/environment_base/
--rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/environment_base/__init__.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     2622 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/environment_base/environment_bases.py
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      290 2024-04-30 15:29:51.000000 craftax-1.4.1/craftax/environment_base/util.py
-drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:35:29.080845 craftax-1.4.1/craftax.egg-info/
--rw-r--r--   0 mikey     (1000) mikey     (1000)    10707 2024-04-30 15:35:29.000000 craftax-1.4.1/craftax.egg-info/PKG-INFO
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     9480 2024-04-30 15:35:29.000000 craftax-1.4.1/craftax.egg-info/SOURCES.txt
--rw-rw-r--   0 mikey     (1000) mikey     (1000)        1 2024-04-30 15:35:29.000000 craftax-1.4.1/craftax.egg-info/dependency_links.txt
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      154 2024-04-30 15:35:29.000000 craftax-1.4.1/craftax.egg-info/entry_points.txt
--rw-rw-r--   0 mikey     (1000) mikey     (1000)      116 2024-04-30 15:35:29.000000 craftax-1.4.1/craftax.egg-info/requires.txt
--rw-rw-r--   0 mikey     (1000) mikey     (1000)        8 2024-04-30 15:35:29.000000 craftax-1.4.1/craftax.egg-info/top_level.txt
--rw-rw-r--   0 mikey     (1000) mikey     (1000)     1065 2024-04-30 15:33:21.000000 craftax-1.4.1/pyproject.toml
--rw-rw-r--   0 mikey     (1000) mikey     (1000)       38 2024-04-30 15:35:29.080845 craftax-1.4.1/setup.cfg
+drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-05-29 14:38:20.515734 craftax-1.4.2/
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1059 2024-04-03 13:05:48.000000 craftax-1.4.2/LICENSE
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)       73 2024-04-30 15:29:51.000000 craftax-1.4.2/MANIFEST.in
+-rw-r--r--   0 mikey     (1000) mikey     (1000)    10939 2024-05-29 14:38:20.515734 craftax-1.4.2/PKG-INFO
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)    10055 2024-05-29 14:37:00.000000 craftax-1.4.2/README.md
+drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-05-29 14:38:20.495734 craftax-1.4.2/craftax/
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/__init__.py
+drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-05-29 14:38:20.495734 craftax-1.4.2/craftax/craftax/
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/__init__.py
+drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-05-29 14:38:20.507734 craftax-1.4.2/craftax/craftax/assets/
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      607 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/0.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1827 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/1.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1501 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/2.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1559 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/3.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1533 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/4.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1518 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/5.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1567 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/6.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1538 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/7.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1506 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/8.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1535 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/9.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1825 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/arrow-down.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1731 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/arrow-left.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1752 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/arrow-right.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1833 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/arrow-up.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      603 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/arrow_fire_enchantment.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      602 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/arrow_ice_enchantment.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      652 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/bat.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      719 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/book.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      654 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/boots_fire_enchantment.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      652 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/boots_ice_enchantment.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      693 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/bow.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      953 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/chest.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      670 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/chestplate_fire_enchantment.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      670 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/chestplate_ice_enchantment.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      866 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/coal.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1983 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/cow.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      621 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/dagger.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     5735 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/debug-2.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     5762 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/debug-3.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     5761 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/debug.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)       84 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/debug_tile.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      996 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/deep_thing.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      790 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/dexterity.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      839 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/diamond.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      605 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/diamond_boots.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      685 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/diamond_chestplate.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      642 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/diamond_helmet.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      609 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/diamond_pants.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      733 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/diamond_pickaxe.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      714 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/diamond_sword.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2492 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/drink.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1087 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/enchantment_table_fire.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1092 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/enchantment_table_ice.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2213 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/energy.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2449 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/fence.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      674 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/fire_elemental.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      710 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/fire_grass.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      959 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/fire_stone.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1140 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/fire_tree.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      670 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/fireball.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2292 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/food.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1141 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/fountain.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      723 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/frost_troll.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      910 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/furnace.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      860 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/gnome_archer.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      847 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/gnome_warrior.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      691 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/grass.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1099 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/grave.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1210 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/grave2.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1161 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/grave3.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      741 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/gravel.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2721 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/health.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      666 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/helmet_fire_enchantment.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      666 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/helmet_ice_enchantment.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      689 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/ice_elemental.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      719 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/ice_grass.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      994 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/ice_shrub.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      668 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/iceball.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      933 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/intelligence.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1048 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/iron.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      613 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/iron_boots.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      681 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/iron_chestplate.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      642 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/iron_helmet.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      608 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/iron_pants.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2354 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/iron_pickaxe.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2390 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/iron_sword.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      839 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/knight.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      889 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/knight_archer.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      737 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/kobold.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      729 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/ladder_down.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      855 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/ladder_down_blocked.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      612 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/ladder_up.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2130 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/lava.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      755 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/leaves.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      758 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/lizard.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      745 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/log.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      695 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/mana.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1150 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/necromancer.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1128 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/necromancer_vulnerable.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      769 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/orc_mage.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      777 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/orc_soldier.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      709 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/pants_fire_enchantment.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      702 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/pants_ice_enchantment.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     7488 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/path.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      325 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/path_moss.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      809 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/pigman.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2154 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/plant-ripe.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2511 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/plant-young.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2080 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/plant.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      219 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/plant_on_grass.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     6186 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/player-down.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     6195 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/player-left.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     6212 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/player-right.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     6590 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/player-sleep.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     6144 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/player-up.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      813 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/player.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      715 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/potion_blue.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      723 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/potion_cyan.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      705 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/potion_green.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      715 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/potion_pink.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      708 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/potion_red.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      707 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/potion_yellow.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      245 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/ripe_plant_on_grass.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1110 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/ruby.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      729 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/sand.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1817 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/sapling.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      957 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/sapphire.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     5993 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/skeleton.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      673 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/slimeball.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      729 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/snail.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      668 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/spider.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1219 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/stalagmite.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     7242 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/stone.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2345 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/stone_pickaxe.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2429 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/stone_sword.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      670 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/strength.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      613 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/sword_fire_enchantment.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      620 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/sword_ice_enchantment.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      885 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/table.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)  3457542 2024-05-02 13:49:20.000000 craftax-1.4.2/craftax/craftax/assets/texture_cache.pbz2
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      615 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/torch_in_inventory.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1197 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/torch_on_path.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     7782 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/tree.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      698 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/troll.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2127 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/unknown.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      126 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/wall.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      163 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/wall2.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      198 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/wall_moss.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2198 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/water.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1577 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/wood.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2045 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/wood_pickaxe.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2453 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/wood_sword.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      718 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/xp.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2089 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/assets/zombie.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)    34413 2024-05-29 14:33:46.000000 craftax-1.4.2/craftax/craftax/constants.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2741 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/craftax_state.py
+drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-05-29 14:38:20.507734 craftax-1.4.2/craftax/craftax/envs/
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/envs/__init__.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      382 2024-05-29 14:36:10.000000 craftax-1.4.2/craftax/craftax/envs/common.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     5020 2024-05-29 14:35:34.000000 craftax-1.4.2/craftax/craftax/envs/craftax_pixels_env.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     5555 2024-05-29 14:35:34.000000 craftax-1.4.2/craftax/craftax/envs/craftax_symbolic_env.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)   106195 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/game_logic.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     7007 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/play_craftax.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)    41178 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/renderer.py
+drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-05-29 14:38:20.507734 craftax-1.4.2/craftax/craftax/util/
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/util/__init__.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)    11631 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/util/game_logic_utils.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      594 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/util/maths_utils.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2534 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/util/noise.py
+drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-05-29 14:38:20.511734 craftax-1.4.2/craftax/craftax/world_gen/
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/world_gen/__init__.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)    24840 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/world_gen/world_gen.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     9213 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax/world_gen/world_gen_configs.py
+drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-05-29 14:38:20.511734 craftax-1.4.2/craftax/craftax_classic/
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/__init__.py
+drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-05-29 14:38:20.515734 craftax-1.4.2/craftax/craftax_classic/assets/
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1827 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/1.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1501 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/2.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1559 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/3.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1533 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/4.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1518 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/5.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1567 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/6.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1538 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/7.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1506 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/8.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1535 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/9.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1825 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/arrow-down.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1731 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/arrow-left.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1752 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/arrow-right.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1833 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/arrow-up.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      866 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/coal.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1983 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/cow.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     5735 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/debug-2.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     5762 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/debug-3.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     5761 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/debug.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)       84 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/debug_tile.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      839 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/diamond.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2492 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/drink.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2213 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/energy.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2449 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/fence.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2292 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/food.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      910 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/furnace.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      691 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/grass.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2721 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/health.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1048 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/iron.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2354 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/iron_pickaxe.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2390 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/iron_sword.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2130 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/lava.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      755 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/leaves.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      745 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/log.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     7488 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/path.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2154 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/plant-ripe.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2511 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/plant-young.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2080 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/plant.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      219 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/plant_on_grass.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     6186 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/player-down.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     6195 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/player-left.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     6212 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/player-right.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     6590 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/player-sleep.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     6144 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/player-up.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      813 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/player.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      245 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/ripe_plant_on_grass.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      729 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/sand.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1817 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/sapling.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     5993 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/skeleton.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     7242 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/stone.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2345 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/stone_pickaxe.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2429 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/stone_sword.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      885 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/table.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)  1262548 2024-05-02 13:49:30.000000 craftax-1.4.2/craftax/craftax_classic/assets/texture_cache_classic.pbz2
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     7782 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/tree.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2127 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/unknown.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2198 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/water.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1577 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/wood.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2045 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/wood_pickaxe.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2453 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/wood_sword.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2089 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/assets/zombie.png
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)    13946 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/constants.py
+drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-05-29 14:38:20.515734 craftax-1.4.2/craftax/craftax_classic/envs/
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/envs/__init__.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      505 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/envs/common.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     4973 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/envs/craftax_pixels_env.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2086 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/envs/craftax_state.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     5443 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/envs/craftax_symbolic_env.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)    58460 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/game_logic.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     4970 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/play_craftax_classic.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)    24401 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/renderer.py
+drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-05-29 14:38:20.515734 craftax-1.4.2/craftax/craftax_classic/util/
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/util/__init__.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2535 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/util/noise.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)    11690 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_classic/world_gen.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2441 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/craftax_env.py
+drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-05-29 14:38:20.515734 craftax-1.4.2/craftax/environment_base/
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)        0 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/environment_base/__init__.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     2622 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/environment_base/environment_bases.py
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      290 2024-04-30 15:29:51.000000 craftax-1.4.2/craftax/environment_base/util.py
+drwxrwxr-x   0 mikey     (1000) mikey     (1000)        0 2024-05-29 14:38:20.515734 craftax-1.4.2/craftax.egg-info/
+-rw-r--r--   0 mikey     (1000) mikey     (1000)    10939 2024-05-29 14:38:20.000000 craftax-1.4.2/craftax.egg-info/PKG-INFO
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     9511 2024-05-29 14:38:20.000000 craftax-1.4.2/craftax.egg-info/SOURCES.txt
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)        1 2024-05-29 14:38:20.000000 craftax-1.4.2/craftax.egg-info/dependency_links.txt
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      154 2024-05-29 14:38:20.000000 craftax-1.4.2/craftax.egg-info/entry_points.txt
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)      116 2024-05-29 14:38:20.000000 craftax-1.4.2/craftax.egg-info/requires.txt
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)        8 2024-05-29 14:38:20.000000 craftax-1.4.2/craftax.egg-info/top_level.txt
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)     1065 2024-05-29 14:37:00.000000 craftax-1.4.2/pyproject.toml
+-rw-rw-r--   0 mikey     (1000) mikey     (1000)       38 2024-05-29 14:38:20.515734 craftax-1.4.2/setup.cfg
```

### Comparing `craftax-1.4.1/LICENSE` & `craftax-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/PKG-INFO` & `craftax-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craftax
-Version: 1.4.1
+Version: 1.4.2
 Summary: An open-world environment for training RL agents
 Author-email: Michael Matthews <michael.matthews@eng.ox.ac.uk>
 Project-URL: Homepage, https://github.com/MichaelTMatthews/Craftax
 Project-URL: Issues, https://github.com/MichaelTMatthews/Craftax/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,15 +31,15 @@
  <img width="80%" src="https://raw.githubusercontent.com/MichaelTMatthews/Craftax/main/images/logo.png" />
 </p>
 
 <p align="center">
         <a href= "https://pypi.org/project/craftax/">
         <img src="https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue" /></a>
         <a href= "https://pypi.org/project/craftax/">
-        <img src="https://img.shields.io/badge/pypi-1.4.1-green" /></a>
+        <img src="https://img.shields.io/badge/pypi-1.4.2-green" /></a>
        <a href= "https://github.com/MichaelTMatthews/Craftax/blob/main/LICENSE">
         <img src="https://img.shields.io/badge/License-MIT-yellow" /></a>
        <a href= "https://craftaxenv.github.io/">
         <img src="https://img.shields.io/badge/blog-link-purple" /></a>
        <a href= "https://arxiv.org/pdf/2402.16801.pdf">
         <img src="https://img.shields.io/badge/arxiv-2402.16801-b31b1b" /></a>
        <a href= "https://github.com/psf/black">
@@ -140,14 +140,15 @@
 # 📋 Scoreboard
 If you would like to add an algorithm please open a PR and provide a reference to the source of the results.
 We report reward as a % of the maximum (226).
 
 ## Craftax-1B
 | Algorithm | Reward (% max) |                                              Code                                               |                  Paper                  |
 |:----------|---------------:|:-----------------------------------------------------------------------------------------------:|:---------------------------------------:|
+| PPO-GTrXL |           18.3 | [TransformerXL_PPO_JAX](https://github.com/Reytuag/transformerXL_PPO_JAX)                       | [PPO](https://arxiv.org/abs/1707.06347), [GTrXL](https://arxiv.org/abs/1910.06764)| 
 | PPO-RNN   |           15.3 | [Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo_rnn.py) | [PPO](https://arxiv.org/abs/1707.06347) |
 | RND       |           12.0 | [Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo_rnd.py) | [RND](https://arxiv.org/abs/1810.12894) |
 | PPO       |           11.9 |   [Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py)   | [PPO](https://arxiv.org/abs/1707.06347) |
 | ICM       |           11.9 |   [Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py)   | [ICM](https://arxiv.org/pdf/1705.05363) |
 | E3B       |           11.0 |   [Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py)   | [E3B](https://arxiv.org/abs/2210.05805) |
 
 
@@ -159,15 +160,15 @@
 | PPO       |            2.2 |   [Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py)   | [PPO](https://arxiv.org/abs/1707.06347) |
 | ICM       |            2.2 |   [Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py)   | [ICM](https://arxiv.org/pdf/1705.05363) |
 | E3B       |            2.2 |   [Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py)   | [E3B](https://arxiv.org/abs/2210.05805) |
 
 
 # 💾 Offline Dataset
 
-A small dataset of trajectories is available [here](https://drive.google.com/file/d/1wCMdUIsGOWYkNW55Rs0rHkYKUZhaQdtq/view?usp=sharing).
+A small dataset of mixed-skill human trajectories is available [here](https://drive.google.com/file/d/1wCMdUIsGOWYkNW55Rs0rHkYKUZhaQdtq/view?usp=sharing).
 Once the zip file has been extracted, the trajectories can be loaded with the `load_compressed_pickle` function.  These were gathered on an earlier version of Craftax and it is recommended you use [v1.1.0](https://github.com/MichaelTMatthews/Craftax/releases/tag/v1.1.0) or earlier to investigate them.
 `run1` is the only trajectory to complete the game.
 
 # 🔎 See Also
 - ⛏️ [Crafter](https://github.com/danijar/crafter) The original Crafter benchmark.
 - ⚔️ [NLE](https://github.com/facebookresearch/nle) NetHack as an RL environment.
 - ⚡ [PureJaxRL](https://github.com/luchris429/purejaxrl) End-to-end RL implementations in Jax.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: craftax Version: 1.4.1 Summary: An open-world
+Metadata-Version: 2.1 Name: craftax Version: 1.4.2 Summary: An open-world
 environment for training RL agents Author-email: Michael Matthews
 eng.ox.ac.uk> Project-URL: Homepage, https://github.com/MichaelTMatthews/
 Craftax Project-URL: Issues, https://github.com/MichaelTMatthews/Craftax/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: jax Requires-Dist: distrax Requires-Dist: optax
@@ -10,15 +10,15 @@
 pre-commit Requires-Dist: argparse Requires-Dist: wandb Requires-Dist: orbax-
 checkpoint Requires-Dist: pygame Requires-Dist: gymnax Requires-Dist: chex
 Requires-Dist: matplotlib Requires-Dist: imageio
    [https://raw.githubusercontent.com/MichaelTMatthews/Craftax/main/images/
                                    logo.png]
                      _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-
 _3_._9_%_2_0_%_7_C_%_2_0_3_._1_0_%_2_0_%_7_C_%_2_0_3_._1_1_%_2_0_%_7_C_%_2_0_3_._1_2_-_b_l_u_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
-  _p_y_p_i_-_1_._4_._1_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_y_e_l_l_o_w_]_[_h_t_t_p_s_:_/_/
+  _p_y_p_i_-_1_._4_._2_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_y_e_l_l_o_w_]_[_h_t_t_p_s_:_/_/
   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_b_l_o_g_-_l_i_n_k_-_p_u_r_p_l_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_a_r_x_i_v_-
 _2_4_0_2_._1_6_8_0_1_-_b_3_1_b_1_b_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_._s_v_g_]
 # âï¸ Craftax Craftax is an RL environment written entirely in _J_A_X. Craftax
 reimplements and significantly extends the game mechanics of _C_r_a_f_t_e_r, taking
 inspiration from roguelike games such as _N_e_t_H_a_c_k. Craftax conforms to the
 _g_y_m_n_a_x interface, allowing easy integration with existing JAX-based frameworks
 like _P_u_r_e_J_a_x_R_L and [JaxUED](https://github.com/DramaCow/jaxued).
@@ -72,52 +72,55 @@
 etc.) then a stale cache could cause errors. You can export the following
 environment variable to force textures to be created from scratch every run.
 ``` export CRAFTAX_RELOAD_TEXTURES=true ``` # ð Scoreboard If you would like
 to add an algorithm please open a PR and provide a reference to the source of
 the results. We report reward as a % of the maximum (226). ## Craftax-1B |
 Algorithm | Reward (% max) | Code | Paper | |:----------|---------------:|:----
 -------------------------------------------------------------------------------
-------------:|:---------------------------------------:| | PPO-RNN | 15.3 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo_rnn.py) | [PPO](https://arxiv.org/abs/1707.06347) | | RND | 12.0 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo_rnd.py) | [RND](https://arxiv.org/abs/1810.12894) | | PPO | 11.9 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo.py) | [PPO](https://arxiv.org/abs/1707.06347) | | ICM | 11.9 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo.py) | [ICM](https://arxiv.org/pdf/1705.05363) | | E3B | 11.0 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo.py) | [E3B](https://arxiv.org/abs/2210.05805) | ## Craftax-1M |
-Algorithm | Reward (% max) | Code | Paper | |:----------|---------------:|:----
--------------------------------------------------------------------------------
-------------:|:---------------------------------------:| | PPO-RNN | 2.3 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo_rnn.py) | [PPO](https://arxiv.org/abs/1707.06347) | | RND | 2.2 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo_rnd.py) | [RND](https://arxiv.org/abs/1810.12894) | | PPO | 2.2 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo.py) | [PPO](https://arxiv.org/abs/1707.06347) | | ICM | 2.2 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo.py) | [ICM](https://arxiv.org/pdf/1705.05363) | | E3B | 2.2 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo.py) | [E3B](https://arxiv.org/abs/2210.05805) | # ð¾ Offline Dataset
-A small dataset of trajectories is available [here](https://drive.google.com/
-file/d/1wCMdUIsGOWYkNW55Rs0rHkYKUZhaQdtq/view?usp=sharing). Once the zip file
-has been extracted, the trajectories can be loaded with the
-`load_compressed_pickle` function. These were gathered on an earlier version of
-Craftax and it is recommended you use [v1.1.0](https://github.com/
-MichaelTMatthews/Craftax/releases/tag/v1.1.0) or earlier to investigate them.
-`run1` is the only trajectory to complete the game. # ð See Also - âï¸
-[Crafter](https://github.com/danijar/crafter) The original Crafter benchmark. -
-âï¸ [NLE](https://github.com/facebookresearch/nle) NetHack as an RL
-environment. - â¡ [PureJaxRL](https://github.com/luchris429/purejaxrl) End-to-
-end RL implementations in Jax. - ð [JaxUED](https://github.com/DramaCow/
-jaxued): CleanRL style UED implementations in Jax. - ð [Minimax](https://
-github.com/facebookresearch/minimax): Modular UED implementations in Jax. -
-ðï¸ [Gymnax](https://github.com/RobertTLange/gymnax): Standard Jax RL
-interface with classic environments. - ð§âð¤âð§ [JaxMARL](https://
-github.com/FLAIROx/JaxMARL): Multi-agent RL in Jax. # ð Citation If you use
-Craftax in your work please cite it as follows: ``` @article
-{matthews2024craftax, title={Craftax: A Lightning-Fast Benchmark for Open-Ended
-Reinforcement Learning}, author={Michael Matthews and Michael Beukman and
-Benjamin Ellis and Mikayel Samvelyan and Matthew Jackson and Samuel Coward and
-Jakob Foerster}, journal={arXiv preprint}, year={2024}, } ```
+------------:|:---------------------------------------:| | PPO-GTrXL | 18.3 |
+[TransformerXL_PPO_JAX](https://github.com/Reytuag/transformerXL_PPO_JAX) |
+[PPO](https://arxiv.org/abs/1707.06347), [GTrXL](https://arxiv.org/abs/
+1910.06764)| | PPO-RNN | 15.3 | [Craftax_Baselines](https://github.com/
+MichaelTMatthews/Craftax_Baselines/blob/main/ppo_rnn.py) | [PPO](https://
+arxiv.org/abs/1707.06347) | | RND | 12.0 | [Craftax_Baselines](https://
+github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo_rnd.py) | [RND]
+(https://arxiv.org/abs/1810.12894) | | PPO | 11.9 | [Craftax_Baselines](https:/
+/github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py) | [PPO](https:
+//arxiv.org/abs/1707.06347) | | ICM | 11.9 | [Craftax_Baselines](https://
+github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py) | [ICM](https:/
+/arxiv.org/pdf/1705.05363) | | E3B | 11.0 | [Craftax_Baselines](https://
+github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py) | [E3B](https:/
+/arxiv.org/abs/2210.05805) | ## Craftax-1M | Algorithm | Reward (% max) | Code
+| Paper | |:----------|---------------:|:--------------------------------------
+---------------------------------------------------------:|:-------------------
+--------------------:| | PPO-RNN | 2.3 | [Craftax_Baselines](https://
+github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo_rnn.py) | [PPO]
+(https://arxiv.org/abs/1707.06347) | | RND | 2.2 | [Craftax_Baselines](https://
+github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo_rnd.py) | [RND]
+(https://arxiv.org/abs/1810.12894) | | PPO | 2.2 | [Craftax_Baselines](https://
+github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py) | [PPO](https:/
+/arxiv.org/abs/1707.06347) | | ICM | 2.2 | [Craftax_Baselines](https://
+github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py) | [ICM](https:/
+/arxiv.org/pdf/1705.05363) | | E3B | 2.2 | [Craftax_Baselines](https://
+github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py) | [E3B](https:/
+/arxiv.org/abs/2210.05805) | # ð¾ Offline Dataset A small dataset of mixed-
+skill human trajectories is available [here](https://drive.google.com/file/d/
+1wCMdUIsGOWYkNW55Rs0rHkYKUZhaQdtq/view?usp=sharing). Once the zip file has been
+extracted, the trajectories can be loaded with the `load_compressed_pickle`
+function. These were gathered on an earlier version of Craftax and it is
+recommended you use [v1.1.0](https://github.com/MichaelTMatthews/Craftax/
+releases/tag/v1.1.0) or earlier to investigate them. `run1` is the only
+trajectory to complete the game. # ð See Also - âï¸ [Crafter](https://
+github.com/danijar/crafter) The original Crafter benchmark. - âï¸ [NLE]
+(https://github.com/facebookresearch/nle) NetHack as an RL environment. - â¡
+[PureJaxRL](https://github.com/luchris429/purejaxrl) End-to-end RL
+implementations in Jax. - ð [JaxUED](https://github.com/DramaCow/jaxued):
+CleanRL style UED implementations in Jax. - ð [Minimax](https://github.com/
+facebookresearch/minimax): Modular UED implementations in Jax. - ðï¸
+[Gymnax](https://github.com/RobertTLange/gymnax): Standard Jax RL interface
+with classic environments. - ð§âð¤âð§ [JaxMARL](https://github.com/
+FLAIROx/JaxMARL): Multi-agent RL in Jax. # ð Citation If you use Craftax in
+your work please cite it as follows: ``` @article{matthews2024craftax, title=
+{Craftax: A Lightning-Fast Benchmark for Open-Ended Reinforcement Learning},
+author={Michael Matthews and Michael Beukman and Benjamin Ellis and Mikayel
+Samvelyan and Matthew Jackson and Samuel Coward and Jakob Foerster}, journal=
+{arXiv preprint}, year={2024}, } ```
```

### Comparing `craftax-1.4.1/README.md` & `craftax-1.4.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
  <img width="80%" src="https://raw.githubusercontent.com/MichaelTMatthews/Craftax/main/images/logo.png" />
 </p>
 
 <p align="center">
         <a href= "https://pypi.org/project/craftax/">
         <img src="https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue" /></a>
         <a href= "https://pypi.org/project/craftax/">
-        <img src="https://img.shields.io/badge/pypi-1.4.1-green" /></a>
+        <img src="https://img.shields.io/badge/pypi-1.4.2-green" /></a>
        <a href= "https://github.com/MichaelTMatthews/Craftax/blob/main/LICENSE">
         <img src="https://img.shields.io/badge/License-MIT-yellow" /></a>
        <a href= "https://craftaxenv.github.io/">
         <img src="https://img.shields.io/badge/blog-link-purple" /></a>
        <a href= "https://arxiv.org/pdf/2402.16801.pdf">
         <img src="https://img.shields.io/badge/arxiv-2402.16801-b31b1b" /></a>
        <a href= "https://github.com/psf/black">
@@ -111,14 +111,15 @@
 # 📋 Scoreboard
 If you would like to add an algorithm please open a PR and provide a reference to the source of the results.
 We report reward as a % of the maximum (226).
 
 ## Craftax-1B
 | Algorithm | Reward (% max) |                                              Code                                               |                  Paper                  |
 |:----------|---------------:|:-----------------------------------------------------------------------------------------------:|:---------------------------------------:|
+| PPO-GTrXL |           18.3 | [TransformerXL_PPO_JAX](https://github.com/Reytuag/transformerXL_PPO_JAX)                       | [PPO](https://arxiv.org/abs/1707.06347), [GTrXL](https://arxiv.org/abs/1910.06764)| 
 | PPO-RNN   |           15.3 | [Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo_rnn.py) | [PPO](https://arxiv.org/abs/1707.06347) |
 | RND       |           12.0 | [Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo_rnd.py) | [RND](https://arxiv.org/abs/1810.12894) |
 | PPO       |           11.9 |   [Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py)   | [PPO](https://arxiv.org/abs/1707.06347) |
 | ICM       |           11.9 |   [Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py)   | [ICM](https://arxiv.org/pdf/1705.05363) |
 | E3B       |           11.0 |   [Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py)   | [E3B](https://arxiv.org/abs/2210.05805) |
 
 
@@ -130,15 +131,15 @@
 | PPO       |            2.2 |   [Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py)   | [PPO](https://arxiv.org/abs/1707.06347) |
 | ICM       |            2.2 |   [Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py)   | [ICM](https://arxiv.org/pdf/1705.05363) |
 | E3B       |            2.2 |   [Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py)   | [E3B](https://arxiv.org/abs/2210.05805) |
 
 
 # 💾 Offline Dataset
 
-A small dataset of trajectories is available [here](https://drive.google.com/file/d/1wCMdUIsGOWYkNW55Rs0rHkYKUZhaQdtq/view?usp=sharing).
+A small dataset of mixed-skill human trajectories is available [here](https://drive.google.com/file/d/1wCMdUIsGOWYkNW55Rs0rHkYKUZhaQdtq/view?usp=sharing).
 Once the zip file has been extracted, the trajectories can be loaded with the `load_compressed_pickle` function.  These were gathered on an earlier version of Craftax and it is recommended you use [v1.1.0](https://github.com/MichaelTMatthews/Craftax/releases/tag/v1.1.0) or earlier to investigate them.
 `run1` is the only trajectory to complete the game.
 
 # 🔎 See Also
 - ⛏️ [Crafter](https://github.com/danijar/crafter) The original Crafter benchmark.
 - ⚔️ [NLE](https://github.com/facebookresearch/nle) NetHack as an RL environment.
 - ⚡ [PureJaxRL](https://github.com/luchris429/purejaxrl) End-to-end RL implementations in Jax.
@@ -152,8 +153,8 @@
 ```
 @article{matthews2024craftax,
   title={Craftax: A Lightning-Fast Benchmark for Open-Ended Reinforcement Learning},
   author={Michael Matthews and Michael Beukman and Benjamin Ellis and Mikayel Samvelyan and Matthew Jackson and Samuel Coward and Jakob Foerster},
   journal={arXiv preprint},
   year={2024},
 }
-```
+```
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
    [https://raw.githubusercontent.com/MichaelTMatthews/Craftax/main/images/
                                    logo.png]
                      _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-
 _3_._9_%_2_0_%_7_C_%_2_0_3_._1_0_%_2_0_%_7_C_%_2_0_3_._1_1_%_2_0_%_7_C_%_2_0_3_._1_2_-_b_l_u_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
-  _p_y_p_i_-_1_._4_._1_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_y_e_l_l_o_w_]_[_h_t_t_p_s_:_/_/
+  _p_y_p_i_-_1_._4_._2_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_y_e_l_l_o_w_]_[_h_t_t_p_s_:_/_/
   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_b_l_o_g_-_l_i_n_k_-_p_u_r_p_l_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_a_r_x_i_v_-
 _2_4_0_2_._1_6_8_0_1_-_b_3_1_b_1_b_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_._s_v_g_]
 # âï¸ Craftax Craftax is an RL environment written entirely in _J_A_X. Craftax
 reimplements and significantly extends the game mechanics of _C_r_a_f_t_e_r, taking
 inspiration from roguelike games such as _N_e_t_H_a_c_k. Craftax conforms to the
 _g_y_m_n_a_x interface, allowing easy integration with existing JAX-based frameworks
 like _P_u_r_e_J_a_x_R_L and [JaxUED](https://github.com/DramaCow/jaxued).
@@ -60,52 +60,55 @@
 etc.) then a stale cache could cause errors. You can export the following
 environment variable to force textures to be created from scratch every run.
 ``` export CRAFTAX_RELOAD_TEXTURES=true ``` # ð Scoreboard If you would like
 to add an algorithm please open a PR and provide a reference to the source of
 the results. We report reward as a % of the maximum (226). ## Craftax-1B |
 Algorithm | Reward (% max) | Code | Paper | |:----------|---------------:|:----
 -------------------------------------------------------------------------------
-------------:|:---------------------------------------:| | PPO-RNN | 15.3 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo_rnn.py) | [PPO](https://arxiv.org/abs/1707.06347) | | RND | 12.0 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo_rnd.py) | [RND](https://arxiv.org/abs/1810.12894) | | PPO | 11.9 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo.py) | [PPO](https://arxiv.org/abs/1707.06347) | | ICM | 11.9 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo.py) | [ICM](https://arxiv.org/pdf/1705.05363) | | E3B | 11.0 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo.py) | [E3B](https://arxiv.org/abs/2210.05805) | ## Craftax-1M |
-Algorithm | Reward (% max) | Code | Paper | |:----------|---------------:|:----
--------------------------------------------------------------------------------
-------------:|:---------------------------------------:| | PPO-RNN | 2.3 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo_rnn.py) | [PPO](https://arxiv.org/abs/1707.06347) | | RND | 2.2 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo_rnd.py) | [RND](https://arxiv.org/abs/1810.12894) | | PPO | 2.2 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo.py) | [PPO](https://arxiv.org/abs/1707.06347) | | ICM | 2.2 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo.py) | [ICM](https://arxiv.org/pdf/1705.05363) | | E3B | 2.2 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo.py) | [E3B](https://arxiv.org/abs/2210.05805) | # ð¾ Offline Dataset
-A small dataset of trajectories is available [here](https://drive.google.com/
-file/d/1wCMdUIsGOWYkNW55Rs0rHkYKUZhaQdtq/view?usp=sharing). Once the zip file
-has been extracted, the trajectories can be loaded with the
-`load_compressed_pickle` function. These were gathered on an earlier version of
-Craftax and it is recommended you use [v1.1.0](https://github.com/
-MichaelTMatthews/Craftax/releases/tag/v1.1.0) or earlier to investigate them.
-`run1` is the only trajectory to complete the game. # ð See Also - âï¸
-[Crafter](https://github.com/danijar/crafter) The original Crafter benchmark. -
-âï¸ [NLE](https://github.com/facebookresearch/nle) NetHack as an RL
-environment. - â¡ [PureJaxRL](https://github.com/luchris429/purejaxrl) End-to-
-end RL implementations in Jax. - ð [JaxUED](https://github.com/DramaCow/
-jaxued): CleanRL style UED implementations in Jax. - ð [Minimax](https://
-github.com/facebookresearch/minimax): Modular UED implementations in Jax. -
-ðï¸ [Gymnax](https://github.com/RobertTLange/gymnax): Standard Jax RL
-interface with classic environments. - ð§âð¤âð§ [JaxMARL](https://
-github.com/FLAIROx/JaxMARL): Multi-agent RL in Jax. # ð Citation If you use
-Craftax in your work please cite it as follows: ``` @article
-{matthews2024craftax, title={Craftax: A Lightning-Fast Benchmark for Open-Ended
-Reinforcement Learning}, author={Michael Matthews and Michael Beukman and
-Benjamin Ellis and Mikayel Samvelyan and Matthew Jackson and Samuel Coward and
-Jakob Foerster}, journal={arXiv preprint}, year={2024}, } ```
+------------:|:---------------------------------------:| | PPO-GTrXL | 18.3 |
+[TransformerXL_PPO_JAX](https://github.com/Reytuag/transformerXL_PPO_JAX) |
+[PPO](https://arxiv.org/abs/1707.06347), [GTrXL](https://arxiv.org/abs/
+1910.06764)| | PPO-RNN | 15.3 | [Craftax_Baselines](https://github.com/
+MichaelTMatthews/Craftax_Baselines/blob/main/ppo_rnn.py) | [PPO](https://
+arxiv.org/abs/1707.06347) | | RND | 12.0 | [Craftax_Baselines](https://
+github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo_rnd.py) | [RND]
+(https://arxiv.org/abs/1810.12894) | | PPO | 11.9 | [Craftax_Baselines](https:/
+/github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py) | [PPO](https:
+//arxiv.org/abs/1707.06347) | | ICM | 11.9 | [Craftax_Baselines](https://
+github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py) | [ICM](https:/
+/arxiv.org/pdf/1705.05363) | | E3B | 11.0 | [Craftax_Baselines](https://
+github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py) | [E3B](https:/
+/arxiv.org/abs/2210.05805) | ## Craftax-1M | Algorithm | Reward (% max) | Code
+| Paper | |:----------|---------------:|:--------------------------------------
+---------------------------------------------------------:|:-------------------
+--------------------:| | PPO-RNN | 2.3 | [Craftax_Baselines](https://
+github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo_rnn.py) | [PPO]
+(https://arxiv.org/abs/1707.06347) | | RND | 2.2 | [Craftax_Baselines](https://
+github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo_rnd.py) | [RND]
+(https://arxiv.org/abs/1810.12894) | | PPO | 2.2 | [Craftax_Baselines](https://
+github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py) | [PPO](https:/
+/arxiv.org/abs/1707.06347) | | ICM | 2.2 | [Craftax_Baselines](https://
+github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py) | [ICM](https:/
+/arxiv.org/pdf/1705.05363) | | E3B | 2.2 | [Craftax_Baselines](https://
+github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py) | [E3B](https:/
+/arxiv.org/abs/2210.05805) | # ð¾ Offline Dataset A small dataset of mixed-
+skill human trajectories is available [here](https://drive.google.com/file/d/
+1wCMdUIsGOWYkNW55Rs0rHkYKUZhaQdtq/view?usp=sharing). Once the zip file has been
+extracted, the trajectories can be loaded with the `load_compressed_pickle`
+function. These were gathered on an earlier version of Craftax and it is
+recommended you use [v1.1.0](https://github.com/MichaelTMatthews/Craftax/
+releases/tag/v1.1.0) or earlier to investigate them. `run1` is the only
+trajectory to complete the game. # ð See Also - âï¸ [Crafter](https://
+github.com/danijar/crafter) The original Crafter benchmark. - âï¸ [NLE]
+(https://github.com/facebookresearch/nle) NetHack as an RL environment. - â¡
+[PureJaxRL](https://github.com/luchris429/purejaxrl) End-to-end RL
+implementations in Jax. - ð [JaxUED](https://github.com/DramaCow/jaxued):
+CleanRL style UED implementations in Jax. - ð [Minimax](https://github.com/
+facebookresearch/minimax): Modular UED implementations in Jax. - ðï¸
+[Gymnax](https://github.com/RobertTLange/gymnax): Standard Jax RL interface
+with classic environments. - ð§âð¤âð§ [JaxMARL](https://github.com/
+FLAIROx/JaxMARL): Multi-agent RL in Jax. # ð Citation If you use Craftax in
+your work please cite it as follows: ``` @article{matthews2024craftax, title=
+{Craftax: A Lightning-Fast Benchmark for Open-Ended Reinforcement Learning},
+author={Michael Matthews and Michael Beukman and Benjamin Ellis and Mikayel
+Samvelyan and Matthew Jackson and Samuel Coward and Jakob Foerster}, journal=
+{arXiv preprint}, year={2024}, } ```
```

### Comparing `craftax-1.4.1/craftax/craftax/assets/0.png` & `craftax-1.4.2/craftax/craftax/assets/0.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/1.png` & `craftax-1.4.2/craftax/craftax/assets/1.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/2.png` & `craftax-1.4.2/craftax/craftax/assets/2.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/3.png` & `craftax-1.4.2/craftax/craftax/assets/3.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/4.png` & `craftax-1.4.2/craftax/craftax/assets/4.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/5.png` & `craftax-1.4.2/craftax/craftax/assets/5.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/6.png` & `craftax-1.4.2/craftax/craftax/assets/6.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/7.png` & `craftax-1.4.2/craftax/craftax/assets/7.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/8.png` & `craftax-1.4.2/craftax/craftax/assets/8.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/9.png` & `craftax-1.4.2/craftax/craftax/assets/9.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/arrow-down.png` & `craftax-1.4.2/craftax/craftax/assets/arrow-down.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/arrow-left.png` & `craftax-1.4.2/craftax/craftax/assets/arrow-left.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/arrow-right.png` & `craftax-1.4.2/craftax/craftax/assets/arrow-right.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/arrow-up.png` & `craftax-1.4.2/craftax/craftax/assets/arrow-up.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/arrow_fire_enchantment.png` & `craftax-1.4.2/craftax/craftax/assets/arrow_fire_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/arrow_ice_enchantment.png` & `craftax-1.4.2/craftax/craftax/assets/arrow_ice_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/bat.png` & `craftax-1.4.2/craftax/craftax/assets/bat.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/book.png` & `craftax-1.4.2/craftax/craftax/assets/book.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/boots_fire_enchantment.png` & `craftax-1.4.2/craftax/craftax/assets/boots_fire_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/boots_ice_enchantment.png` & `craftax-1.4.2/craftax/craftax/assets/boots_ice_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/bow.png` & `craftax-1.4.2/craftax/craftax/assets/bow.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/chest.png` & `craftax-1.4.2/craftax/craftax/assets/chest.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/chestplate_fire_enchantment.png` & `craftax-1.4.2/craftax/craftax/assets/chestplate_fire_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/chestplate_ice_enchantment.png` & `craftax-1.4.2/craftax/craftax/assets/chestplate_ice_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/coal.png` & `craftax-1.4.2/craftax/craftax/assets/coal.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/cow.png` & `craftax-1.4.2/craftax/craftax/assets/cow.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/dagger.png` & `craftax-1.4.2/craftax/craftax/assets/dagger.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/debug-2.png` & `craftax-1.4.2/craftax/craftax/assets/debug-2.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/debug-3.png` & `craftax-1.4.2/craftax/craftax/assets/debug-3.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/debug.png` & `craftax-1.4.2/craftax/craftax/assets/debug.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/deep_thing.png` & `craftax-1.4.2/craftax/craftax/assets/deep_thing.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/dexterity.png` & `craftax-1.4.2/craftax/craftax/assets/dexterity.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/diamond.png` & `craftax-1.4.2/craftax/craftax/assets/diamond.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/diamond_boots.png` & `craftax-1.4.2/craftax/craftax/assets/diamond_boots.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/diamond_chestplate.png` & `craftax-1.4.2/craftax/craftax/assets/diamond_chestplate.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/diamond_helmet.png` & `craftax-1.4.2/craftax/craftax/assets/diamond_helmet.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/diamond_pants.png` & `craftax-1.4.2/craftax/craftax/assets/diamond_pants.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/diamond_pickaxe.png` & `craftax-1.4.2/craftax/craftax/assets/diamond_pickaxe.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/diamond_sword.png` & `craftax-1.4.2/craftax/craftax/assets/diamond_sword.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/drink.png` & `craftax-1.4.2/craftax/craftax/assets/drink.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/enchantment_table_fire.png` & `craftax-1.4.2/craftax/craftax/assets/enchantment_table_fire.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/enchantment_table_ice.png` & `craftax-1.4.2/craftax/craftax/assets/enchantment_table_ice.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/energy.png` & `craftax-1.4.2/craftax/craftax/assets/energy.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/fence.png` & `craftax-1.4.2/craftax/craftax/assets/fence.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/fire_elemental.png` & `craftax-1.4.2/craftax/craftax/assets/fire_elemental.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/fire_grass.png` & `craftax-1.4.2/craftax/craftax/assets/fire_grass.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/fire_stone.png` & `craftax-1.4.2/craftax/craftax/assets/fire_stone.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/fire_tree.png` & `craftax-1.4.2/craftax/craftax/assets/fire_tree.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/fireball.png` & `craftax-1.4.2/craftax/craftax/assets/fireball.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/food.png` & `craftax-1.4.2/craftax/craftax/assets/food.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/fountain.png` & `craftax-1.4.2/craftax/craftax/assets/fountain.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/frost_troll.png` & `craftax-1.4.2/craftax/craftax/assets/frost_troll.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/furnace.png` & `craftax-1.4.2/craftax/craftax/assets/furnace.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/gnome_archer.png` & `craftax-1.4.2/craftax/craftax/assets/gnome_archer.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/gnome_warrior.png` & `craftax-1.4.2/craftax/craftax/assets/gnome_warrior.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/grass.png` & `craftax-1.4.2/craftax/craftax/assets/grass.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/grave.png` & `craftax-1.4.2/craftax/craftax/assets/grave.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/grave2.png` & `craftax-1.4.2/craftax/craftax/assets/grave2.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/grave3.png` & `craftax-1.4.2/craftax/craftax/assets/grave3.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/gravel.png` & `craftax-1.4.2/craftax/craftax/assets/gravel.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/health.png` & `craftax-1.4.2/craftax/craftax/assets/health.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/helmet_fire_enchantment.png` & `craftax-1.4.2/craftax/craftax/assets/helmet_fire_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/helmet_ice_enchantment.png` & `craftax-1.4.2/craftax/craftax/assets/helmet_ice_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/ice_elemental.png` & `craftax-1.4.2/craftax/craftax/assets/ice_elemental.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/ice_grass.png` & `craftax-1.4.2/craftax/craftax/assets/ice_grass.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/ice_shrub.png` & `craftax-1.4.2/craftax/craftax/assets/ice_shrub.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/iceball.png` & `craftax-1.4.2/craftax/craftax/assets/iceball.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/intelligence.png` & `craftax-1.4.2/craftax/craftax/assets/intelligence.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/iron.png` & `craftax-1.4.2/craftax/craftax/assets/iron.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/iron_boots.png` & `craftax-1.4.2/craftax/craftax/assets/iron_boots.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/iron_chestplate.png` & `craftax-1.4.2/craftax/craftax/assets/iron_chestplate.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/iron_helmet.png` & `craftax-1.4.2/craftax/craftax/assets/iron_helmet.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/iron_pants.png` & `craftax-1.4.2/craftax/craftax/assets/iron_pants.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/iron_pickaxe.png` & `craftax-1.4.2/craftax/craftax/assets/iron_pickaxe.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/iron_sword.png` & `craftax-1.4.2/craftax/craftax/assets/iron_sword.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/knight.png` & `craftax-1.4.2/craftax/craftax/assets/knight.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/knight_archer.png` & `craftax-1.4.2/craftax/craftax/assets/knight_archer.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/kobold.png` & `craftax-1.4.2/craftax/craftax/assets/kobold.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/ladder_down.png` & `craftax-1.4.2/craftax/craftax/assets/ladder_down.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/ladder_down_blocked.png` & `craftax-1.4.2/craftax/craftax/assets/ladder_down_blocked.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/ladder_up.png` & `craftax-1.4.2/craftax/craftax/assets/ladder_up.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/lava.png` & `craftax-1.4.2/craftax/craftax/assets/lava.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/leaves.png` & `craftax-1.4.2/craftax/craftax/assets/leaves.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/lizard.png` & `craftax-1.4.2/craftax/craftax/assets/lizard.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/log.png` & `craftax-1.4.2/craftax/craftax/assets/log.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/mana.png` & `craftax-1.4.2/craftax/craftax/assets/mana.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/necromancer.png` & `craftax-1.4.2/craftax/craftax/assets/necromancer.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/necromancer_vulnerable.png` & `craftax-1.4.2/craftax/craftax/assets/necromancer_vulnerable.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/orc_mage.png` & `craftax-1.4.2/craftax/craftax/assets/orc_mage.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/orc_soldier.png` & `craftax-1.4.2/craftax/craftax/assets/orc_soldier.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/pants_fire_enchantment.png` & `craftax-1.4.2/craftax/craftax/assets/pants_fire_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/pants_ice_enchantment.png` & `craftax-1.4.2/craftax/craftax/assets/pants_ice_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/path.png` & `craftax-1.4.2/craftax/craftax/assets/path.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/pigman.png` & `craftax-1.4.2/craftax/craftax/assets/pigman.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/plant-ripe.png` & `craftax-1.4.2/craftax/craftax/assets/plant-ripe.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/plant-young.png` & `craftax-1.4.2/craftax/craftax/assets/plant-young.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/plant.png` & `craftax-1.4.2/craftax/craftax/assets/plant.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/player-down.png` & `craftax-1.4.2/craftax/craftax/assets/player-down.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/player-left.png` & `craftax-1.4.2/craftax/craftax/assets/player-left.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/player-right.png` & `craftax-1.4.2/craftax/craftax/assets/player-right.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/player-sleep.png` & `craftax-1.4.2/craftax/craftax/assets/player-sleep.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/player-up.png` & `craftax-1.4.2/craftax/craftax/assets/player-up.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/player.png` & `craftax-1.4.2/craftax/craftax/assets/player.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/potion_blue.png` & `craftax-1.4.2/craftax/craftax/assets/potion_blue.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/potion_cyan.png` & `craftax-1.4.2/craftax/craftax/assets/potion_cyan.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/potion_green.png` & `craftax-1.4.2/craftax/craftax/assets/potion_green.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/potion_pink.png` & `craftax-1.4.2/craftax/craftax/assets/potion_pink.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/potion_red.png` & `craftax-1.4.2/craftax/craftax/assets/potion_red.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/potion_yellow.png` & `craftax-1.4.2/craftax/craftax/assets/potion_yellow.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/ruby.png` & `craftax-1.4.2/craftax/craftax/assets/ruby.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/sand.png` & `craftax-1.4.2/craftax/craftax/assets/sand.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/sapling.png` & `craftax-1.4.2/craftax/craftax/assets/sapling.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/sapphire.png` & `craftax-1.4.2/craftax/craftax/assets/sapphire.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/skeleton.png` & `craftax-1.4.2/craftax/craftax/assets/skeleton.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/slimeball.png` & `craftax-1.4.2/craftax/craftax/assets/slimeball.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/snail.png` & `craftax-1.4.2/craftax/craftax/assets/snail.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/spider.png` & `craftax-1.4.2/craftax/craftax/assets/spider.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/stalagmite.png` & `craftax-1.4.2/craftax/craftax/assets/stalagmite.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/stone.png` & `craftax-1.4.2/craftax/craftax/assets/stone.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/stone_pickaxe.png` & `craftax-1.4.2/craftax/craftax/assets/stone_pickaxe.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/stone_sword.png` & `craftax-1.4.2/craftax/craftax/assets/stone_sword.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/strength.png` & `craftax-1.4.2/craftax/craftax/assets/strength.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/sword_fire_enchantment.png` & `craftax-1.4.2/craftax/craftax/assets/sword_fire_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/sword_ice_enchantment.png` & `craftax-1.4.2/craftax/craftax/assets/sword_ice_enchantment.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/table.png` & `craftax-1.4.2/craftax/craftax/assets/table.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/torch_in_inventory.png` & `craftax-1.4.2/craftax/craftax/assets/torch_in_inventory.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/torch_on_path.png` & `craftax-1.4.2/craftax/craftax/assets/torch_on_path.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/tree.png` & `craftax-1.4.2/craftax/craftax/assets/tree.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/troll.png` & `craftax-1.4.2/craftax/craftax/assets/troll.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/unknown.png` & `craftax-1.4.2/craftax/craftax/assets/unknown.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/water.png` & `craftax-1.4.2/craftax/craftax/assets/water.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/wood.png` & `craftax-1.4.2/craftax/craftax/assets/wood.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/wood_pickaxe.png` & `craftax-1.4.2/craftax/craftax/assets/wood_pickaxe.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/wood_sword.png` & `craftax-1.4.2/craftax/craftax/assets/wood_sword.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/xp.png` & `craftax-1.4.2/craftax/craftax/assets/xp.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/assets/zombie.png` & `craftax-1.4.2/craftax/craftax/assets/zombie.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/constants.py` & `craftax-1.4.2/craftax/craftax/constants.py`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/craftax_state.py` & `craftax-1.4.2/craftax/craftax/craftax_state.py`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/envs/craftax_pixels_env.py` & `craftax-1.4.2/craftax/craftax/envs/craftax_pixels_env.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from jax import lax
 from gymnax.environments import spaces, environment
 from typing import Tuple, Optional
 import chex
 
 from craftax.craftax.constants import *
+from craftax.craftax.envs.common import log_achievements_to_info
 from craftax.craftax.game_logic import craftax_step, is_game_over
 from craftax.craftax.craftax_state import EnvState, EnvParams, StaticEnvParams
 from craftax.craftax.renderer import render_craftax_pixels
 from craftax.craftax.world_gen.world_gen import generate_world
 from craftax.environment_base.environment_bases import EnvironmentNoAutoReset
 
 
@@ -30,15 +31,16 @@
     def step_env(
         self, key: chex.PRNGKey, state: EnvState, action: int, params: EnvParams
     ) -> Tuple[chex.Array, EnvState, float, bool, dict]:
 
         state, reward = craftax_step(key, state, action, params, self.static_env_params)
 
         done = self.is_terminal(state, params)
-        info = {"discount": self.discount(state, params)}
+        info = log_achievements_to_info(state, done)
+        info["discount"] = self.discount(state, params)
 
         return (
             lax.stop_gradient(self.get_obs(state)),
             lax.stop_gradient(state),
             reward,
             done,
             info,
@@ -101,15 +103,16 @@
     def step_env(
         self, key: chex.PRNGKey, state: EnvState, action: int, params: EnvParams
     ) -> Tuple[chex.Array, EnvState, float, bool, dict]:
 
         state, reward = craftax_step(key, state, action, params, self.static_env_params)
 
         done = self.is_terminal(state, params)
-        info = {"discount": self.discount(state, params)}
+        info = log_achievements_to_info(state, done)
+        info["discount"] = self.discount(state, params)
 
         return (
             lax.stop_gradient(self.get_obs(state)),
             lax.stop_gradient(state),
             reward,
             done,
             info,
```

### Comparing `craftax-1.4.1/craftax/craftax/envs/craftax_symbolic_env.py` & `craftax-1.4.2/craftax/craftax/envs/craftax_symbolic_env.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import jax
 from jax import lax
 from gymnax.environments import spaces, environment
 from typing import Tuple, Optional
 import chex
 
+from craftax.craftax.envs.common import log_achievements_to_info
 from craftax.environment_base.environment_bases import EnvironmentNoAutoReset
 from craftax.craftax.constants import *
 from craftax.craftax.game_logic import craftax_step, is_game_over
 from craftax.craftax.craftax_state import EnvState, EnvParams, StaticEnvParams
 from craftax.craftax.renderer import render_craftax_symbolic
 from craftax.craftax.world_gen.world_gen import generate_world
 
@@ -52,15 +53,16 @@
 
     def step_env(
         self, rng: chex.PRNGKey, state: EnvState, action: int, params: EnvParams
     ) -> Tuple[chex.Array, EnvState, float, bool, dict]:
         state, reward = craftax_step(rng, state, action, params, self.static_env_params)
 
         done = self.is_terminal(state, params)
-        info = {"discount": self.discount(state, params)}
+        info = log_achievements_to_info(state, done)
+        info["discount"] = self.discount(state, params)
 
         return (
             lax.stop_gradient(self.get_obs(state)),
             lax.stop_gradient(state),
             reward,
             done,
             info,
@@ -124,15 +126,16 @@
 
     def step_env(
         self, rng: chex.PRNGKey, state: EnvState, action: int, params: EnvParams
     ) -> Tuple[chex.Array, EnvState, float, bool, dict]:
         state, reward = craftax_step(rng, state, action, params, self.static_env_params)
 
         done = self.is_terminal(state, params)
-        info = {"discount": self.discount(state, params)}
+        info = log_achievements_to_info(state, done)
+        info["discount"] = self.discount(state, params)
 
         return (
             lax.stop_gradient(self.get_obs(state)),
             lax.stop_gradient(state),
             reward,
             done,
             info,
```

### Comparing `craftax-1.4.1/craftax/craftax/game_logic.py` & `craftax-1.4.2/craftax/craftax/game_logic.py`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/play_craftax.py` & `craftax-1.4.2/craftax/craftax/play_craftax.py`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/renderer.py` & `craftax-1.4.2/craftax/craftax/renderer.py`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/util/game_logic_utils.py` & `craftax-1.4.2/craftax/craftax/util/game_logic_utils.py`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/util/maths_utils.py` & `craftax-1.4.2/craftax/craftax/util/maths_utils.py`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/util/noise.py` & `craftax-1.4.2/craftax/craftax/util/noise.py`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/world_gen/world_gen.py` & `craftax-1.4.2/craftax/craftax/world_gen/world_gen.py`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax/world_gen/world_gen_configs.py` & `craftax-1.4.2/craftax/craftax/world_gen/world_gen_configs.py`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/1.png` & `craftax-1.4.2/craftax/craftax_classic/assets/1.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/2.png` & `craftax-1.4.2/craftax/craftax_classic/assets/2.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/3.png` & `craftax-1.4.2/craftax/craftax_classic/assets/3.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/4.png` & `craftax-1.4.2/craftax/craftax_classic/assets/4.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/5.png` & `craftax-1.4.2/craftax/craftax_classic/assets/5.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/6.png` & `craftax-1.4.2/craftax/craftax_classic/assets/6.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/7.png` & `craftax-1.4.2/craftax/craftax_classic/assets/7.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/8.png` & `craftax-1.4.2/craftax/craftax_classic/assets/8.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/9.png` & `craftax-1.4.2/craftax/craftax_classic/assets/9.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/arrow-down.png` & `craftax-1.4.2/craftax/craftax_classic/assets/arrow-down.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/arrow-left.png` & `craftax-1.4.2/craftax/craftax_classic/assets/arrow-left.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/arrow-right.png` & `craftax-1.4.2/craftax/craftax_classic/assets/arrow-right.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/arrow-up.png` & `craftax-1.4.2/craftax/craftax_classic/assets/arrow-up.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/coal.png` & `craftax-1.4.2/craftax/craftax_classic/assets/coal.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/cow.png` & `craftax-1.4.2/craftax/craftax_classic/assets/cow.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/debug-2.png` & `craftax-1.4.2/craftax/craftax_classic/assets/debug-2.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/debug-3.png` & `craftax-1.4.2/craftax/craftax_classic/assets/debug-3.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/debug.png` & `craftax-1.4.2/craftax/craftax_classic/assets/debug.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/diamond.png` & `craftax-1.4.2/craftax/craftax_classic/assets/diamond.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/drink.png` & `craftax-1.4.2/craftax/craftax_classic/assets/drink.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/energy.png` & `craftax-1.4.2/craftax/craftax_classic/assets/energy.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/fence.png` & `craftax-1.4.2/craftax/craftax_classic/assets/fence.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/food.png` & `craftax-1.4.2/craftax/craftax_classic/assets/food.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/furnace.png` & `craftax-1.4.2/craftax/craftax_classic/assets/furnace.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/grass.png` & `craftax-1.4.2/craftax/craftax_classic/assets/grass.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/health.png` & `craftax-1.4.2/craftax/craftax_classic/assets/health.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/iron.png` & `craftax-1.4.2/craftax/craftax_classic/assets/iron.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/iron_pickaxe.png` & `craftax-1.4.2/craftax/craftax_classic/assets/iron_pickaxe.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/iron_sword.png` & `craftax-1.4.2/craftax/craftax_classic/assets/iron_sword.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/lava.png` & `craftax-1.4.2/craftax/craftax_classic/assets/lava.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/leaves.png` & `craftax-1.4.2/craftax/craftax_classic/assets/leaves.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/log.png` & `craftax-1.4.2/craftax/craftax_classic/assets/log.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/path.png` & `craftax-1.4.2/craftax/craftax_classic/assets/path.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/plant-ripe.png` & `craftax-1.4.2/craftax/craftax_classic/assets/plant-ripe.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/plant-young.png` & `craftax-1.4.2/craftax/craftax_classic/assets/plant-young.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/plant.png` & `craftax-1.4.2/craftax/craftax_classic/assets/plant.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/player-down.png` & `craftax-1.4.2/craftax/craftax_classic/assets/player-down.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/player-left.png` & `craftax-1.4.2/craftax/craftax_classic/assets/player-left.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/player-right.png` & `craftax-1.4.2/craftax/craftax_classic/assets/player-right.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/player-sleep.png` & `craftax-1.4.2/craftax/craftax_classic/assets/player-sleep.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/player-up.png` & `craftax-1.4.2/craftax/craftax_classic/assets/player-up.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/player.png` & `craftax-1.4.2/craftax/craftax_classic/assets/player.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/sand.png` & `craftax-1.4.2/craftax/craftax_classic/assets/sand.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/sapling.png` & `craftax-1.4.2/craftax/craftax_classic/assets/sapling.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/skeleton.png` & `craftax-1.4.2/craftax/craftax_classic/assets/skeleton.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/stone.png` & `craftax-1.4.2/craftax/craftax_classic/assets/stone.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/stone_pickaxe.png` & `craftax-1.4.2/craftax/craftax_classic/assets/stone_pickaxe.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/stone_sword.png` & `craftax-1.4.2/craftax/craftax_classic/assets/stone_sword.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/table.png` & `craftax-1.4.2/craftax/craftax_classic/assets/table.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/tree.png` & `craftax-1.4.2/craftax/craftax_classic/assets/tree.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/unknown.png` & `craftax-1.4.2/craftax/craftax_classic/assets/unknown.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/water.png` & `craftax-1.4.2/craftax/craftax_classic/assets/water.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/wood.png` & `craftax-1.4.2/craftax/craftax_classic/assets/wood.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/wood_pickaxe.png` & `craftax-1.4.2/craftax/craftax_classic/assets/wood_pickaxe.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/wood_sword.png` & `craftax-1.4.2/craftax/craftax_classic/assets/wood_sword.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/assets/zombie.png` & `craftax-1.4.2/craftax/craftax_classic/assets/zombie.png`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/constants.py` & `craftax-1.4.2/craftax/craftax_classic/constants.py`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/envs/craftax_pixels_env.py` & `craftax-1.4.2/craftax/craftax_classic/envs/craftax_pixels_env.py`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/envs/craftax_state.py` & `craftax-1.4.2/craftax/craftax_classic/envs/craftax_state.py`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/envs/craftax_symbolic_env.py` & `craftax-1.4.2/craftax/craftax_classic/envs/craftax_symbolic_env.py`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/game_logic.py` & `craftax-1.4.2/craftax/craftax_classic/game_logic.py`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/play_craftax_classic.py` & `craftax-1.4.2/craftax/craftax_classic/play_craftax_classic.py`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/renderer.py` & `craftax-1.4.2/craftax/craftax_classic/renderer.py`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/util/noise.py` & `craftax-1.4.2/craftax/craftax_classic/util/noise.py`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_classic/world_gen.py` & `craftax-1.4.2/craftax/craftax_classic/world_gen.py`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/craftax_env.py` & `craftax-1.4.2/craftax/craftax_env.py`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax/environment_base/environment_bases.py` & `craftax-1.4.2/craftax/environment_base/environment_bases.py`

 * *Files identical despite different names*

### Comparing `craftax-1.4.1/craftax.egg-info/PKG-INFO` & `craftax-1.4.2/craftax.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: craftax
-Version: 1.4.1
+Version: 1.4.2
 Summary: An open-world environment for training RL agents
 Author-email: Michael Matthews <michael.matthews@eng.ox.ac.uk>
 Project-URL: Homepage, https://github.com/MichaelTMatthews/Craftax
 Project-URL: Issues, https://github.com/MichaelTMatthews/Craftax/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -31,15 +31,15 @@
  <img width="80%" src="https://raw.githubusercontent.com/MichaelTMatthews/Craftax/main/images/logo.png" />
 </p>
 
 <p align="center">
         <a href= "https://pypi.org/project/craftax/">
         <img src="https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11%20%7C%203.12-blue" /></a>
         <a href= "https://pypi.org/project/craftax/">
-        <img src="https://img.shields.io/badge/pypi-1.4.1-green" /></a>
+        <img src="https://img.shields.io/badge/pypi-1.4.2-green" /></a>
        <a href= "https://github.com/MichaelTMatthews/Craftax/blob/main/LICENSE">
         <img src="https://img.shields.io/badge/License-MIT-yellow" /></a>
        <a href= "https://craftaxenv.github.io/">
         <img src="https://img.shields.io/badge/blog-link-purple" /></a>
        <a href= "https://arxiv.org/pdf/2402.16801.pdf">
         <img src="https://img.shields.io/badge/arxiv-2402.16801-b31b1b" /></a>
        <a href= "https://github.com/psf/black">
@@ -140,14 +140,15 @@
 # 📋 Scoreboard
 If you would like to add an algorithm please open a PR and provide a reference to the source of the results.
 We report reward as a % of the maximum (226).
 
 ## Craftax-1B
 | Algorithm | Reward (% max) |                                              Code                                               |                  Paper                  |
 |:----------|---------------:|:-----------------------------------------------------------------------------------------------:|:---------------------------------------:|
+| PPO-GTrXL |           18.3 | [TransformerXL_PPO_JAX](https://github.com/Reytuag/transformerXL_PPO_JAX)                       | [PPO](https://arxiv.org/abs/1707.06347), [GTrXL](https://arxiv.org/abs/1910.06764)| 
 | PPO-RNN   |           15.3 | [Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo_rnn.py) | [PPO](https://arxiv.org/abs/1707.06347) |
 | RND       |           12.0 | [Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo_rnd.py) | [RND](https://arxiv.org/abs/1810.12894) |
 | PPO       |           11.9 |   [Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py)   | [PPO](https://arxiv.org/abs/1707.06347) |
 | ICM       |           11.9 |   [Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py)   | [ICM](https://arxiv.org/pdf/1705.05363) |
 | E3B       |           11.0 |   [Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py)   | [E3B](https://arxiv.org/abs/2210.05805) |
 
 
@@ -159,15 +160,15 @@
 | PPO       |            2.2 |   [Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py)   | [PPO](https://arxiv.org/abs/1707.06347) |
 | ICM       |            2.2 |   [Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py)   | [ICM](https://arxiv.org/pdf/1705.05363) |
 | E3B       |            2.2 |   [Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py)   | [E3B](https://arxiv.org/abs/2210.05805) |
 
 
 # 💾 Offline Dataset
 
-A small dataset of trajectories is available [here](https://drive.google.com/file/d/1wCMdUIsGOWYkNW55Rs0rHkYKUZhaQdtq/view?usp=sharing).
+A small dataset of mixed-skill human trajectories is available [here](https://drive.google.com/file/d/1wCMdUIsGOWYkNW55Rs0rHkYKUZhaQdtq/view?usp=sharing).
 Once the zip file has been extracted, the trajectories can be loaded with the `load_compressed_pickle` function.  These were gathered on an earlier version of Craftax and it is recommended you use [v1.1.0](https://github.com/MichaelTMatthews/Craftax/releases/tag/v1.1.0) or earlier to investigate them.
 `run1` is the only trajectory to complete the game.
 
 # 🔎 See Also
 - ⛏️ [Crafter](https://github.com/danijar/crafter) The original Crafter benchmark.
 - ⚔️ [NLE](https://github.com/facebookresearch/nle) NetHack as an RL environment.
 - ⚡ [PureJaxRL](https://github.com/luchris429/purejaxrl) End-to-end RL implementations in Jax.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: craftax Version: 1.4.1 Summary: An open-world
+Metadata-Version: 2.1 Name: craftax Version: 1.4.2 Summary: An open-world
 environment for training RL agents Author-email: Michael Matthews
 eng.ox.ac.uk> Project-URL: Homepage, https://github.com/MichaelTMatthews/
 Craftax Project-URL: Issues, https://github.com/MichaelTMatthews/Craftax/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: jax Requires-Dist: distrax Requires-Dist: optax
@@ -10,15 +10,15 @@
 pre-commit Requires-Dist: argparse Requires-Dist: wandb Requires-Dist: orbax-
 checkpoint Requires-Dist: pygame Requires-Dist: gymnax Requires-Dist: chex
 Requires-Dist: matplotlib Requires-Dist: imageio
    [https://raw.githubusercontent.com/MichaelTMatthews/Craftax/main/images/
                                    logo.png]
                      _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_p_y_t_h_o_n_-
 _3_._9_%_2_0_%_7_C_%_2_0_3_._1_0_%_2_0_%_7_C_%_2_0_3_._1_1_%_2_0_%_7_C_%_2_0_3_._1_2_-_b_l_u_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/
-  _p_y_p_i_-_1_._4_._1_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_y_e_l_l_o_w_]_[_h_t_t_p_s_:_/_/
+  _p_y_p_i_-_1_._4_._2_-_g_r_e_e_n_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_M_I_T_-_y_e_l_l_o_w_]_[_h_t_t_p_s_:_/_/
   _i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_b_l_o_g_-_l_i_n_k_-_p_u_r_p_l_e_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_a_r_x_i_v_-
 _2_4_0_2_._1_6_8_0_1_-_b_3_1_b_1_b_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_c_o_d_e_%_2_0_s_t_y_l_e_-_b_l_a_c_k_-_0_0_0_0_0_0_._s_v_g_]
 # âï¸ Craftax Craftax is an RL environment written entirely in _J_A_X. Craftax
 reimplements and significantly extends the game mechanics of _C_r_a_f_t_e_r, taking
 inspiration from roguelike games such as _N_e_t_H_a_c_k. Craftax conforms to the
 _g_y_m_n_a_x interface, allowing easy integration with existing JAX-based frameworks
 like _P_u_r_e_J_a_x_R_L and [JaxUED](https://github.com/DramaCow/jaxued).
@@ -72,52 +72,55 @@
 etc.) then a stale cache could cause errors. You can export the following
 environment variable to force textures to be created from scratch every run.
 ``` export CRAFTAX_RELOAD_TEXTURES=true ``` # ð Scoreboard If you would like
 to add an algorithm please open a PR and provide a reference to the source of
 the results. We report reward as a % of the maximum (226). ## Craftax-1B |
 Algorithm | Reward (% max) | Code | Paper | |:----------|---------------:|:----
 -------------------------------------------------------------------------------
-------------:|:---------------------------------------:| | PPO-RNN | 15.3 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo_rnn.py) | [PPO](https://arxiv.org/abs/1707.06347) | | RND | 12.0 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo_rnd.py) | [RND](https://arxiv.org/abs/1810.12894) | | PPO | 11.9 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo.py) | [PPO](https://arxiv.org/abs/1707.06347) | | ICM | 11.9 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo.py) | [ICM](https://arxiv.org/pdf/1705.05363) | | E3B | 11.0 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo.py) | [E3B](https://arxiv.org/abs/2210.05805) | ## Craftax-1M |
-Algorithm | Reward (% max) | Code | Paper | |:----------|---------------:|:----
--------------------------------------------------------------------------------
-------------:|:---------------------------------------:| | PPO-RNN | 2.3 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo_rnn.py) | [PPO](https://arxiv.org/abs/1707.06347) | | RND | 2.2 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo_rnd.py) | [RND](https://arxiv.org/abs/1810.12894) | | PPO | 2.2 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo.py) | [PPO](https://arxiv.org/abs/1707.06347) | | ICM | 2.2 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo.py) | [ICM](https://arxiv.org/pdf/1705.05363) | | E3B | 2.2 |
-[Craftax_Baselines](https://github.com/MichaelTMatthews/Craftax_Baselines/blob/
-main/ppo.py) | [E3B](https://arxiv.org/abs/2210.05805) | # ð¾ Offline Dataset
-A small dataset of trajectories is available [here](https://drive.google.com/
-file/d/1wCMdUIsGOWYkNW55Rs0rHkYKUZhaQdtq/view?usp=sharing). Once the zip file
-has been extracted, the trajectories can be loaded with the
-`load_compressed_pickle` function. These were gathered on an earlier version of
-Craftax and it is recommended you use [v1.1.0](https://github.com/
-MichaelTMatthews/Craftax/releases/tag/v1.1.0) or earlier to investigate them.
-`run1` is the only trajectory to complete the game. # ð See Also - âï¸
-[Crafter](https://github.com/danijar/crafter) The original Crafter benchmark. -
-âï¸ [NLE](https://github.com/facebookresearch/nle) NetHack as an RL
-environment. - â¡ [PureJaxRL](https://github.com/luchris429/purejaxrl) End-to-
-end RL implementations in Jax. - ð [JaxUED](https://github.com/DramaCow/
-jaxued): CleanRL style UED implementations in Jax. - ð [Minimax](https://
-github.com/facebookresearch/minimax): Modular UED implementations in Jax. -
-ðï¸ [Gymnax](https://github.com/RobertTLange/gymnax): Standard Jax RL
-interface with classic environments. - ð§âð¤âð§ [JaxMARL](https://
-github.com/FLAIROx/JaxMARL): Multi-agent RL in Jax. # ð Citation If you use
-Craftax in your work please cite it as follows: ``` @article
-{matthews2024craftax, title={Craftax: A Lightning-Fast Benchmark for Open-Ended
-Reinforcement Learning}, author={Michael Matthews and Michael Beukman and
-Benjamin Ellis and Mikayel Samvelyan and Matthew Jackson and Samuel Coward and
-Jakob Foerster}, journal={arXiv preprint}, year={2024}, } ```
+------------:|:---------------------------------------:| | PPO-GTrXL | 18.3 |
+[TransformerXL_PPO_JAX](https://github.com/Reytuag/transformerXL_PPO_JAX) |
+[PPO](https://arxiv.org/abs/1707.06347), [GTrXL](https://arxiv.org/abs/
+1910.06764)| | PPO-RNN | 15.3 | [Craftax_Baselines](https://github.com/
+MichaelTMatthews/Craftax_Baselines/blob/main/ppo_rnn.py) | [PPO](https://
+arxiv.org/abs/1707.06347) | | RND | 12.0 | [Craftax_Baselines](https://
+github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo_rnd.py) | [RND]
+(https://arxiv.org/abs/1810.12894) | | PPO | 11.9 | [Craftax_Baselines](https:/
+/github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py) | [PPO](https:
+//arxiv.org/abs/1707.06347) | | ICM | 11.9 | [Craftax_Baselines](https://
+github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py) | [ICM](https:/
+/arxiv.org/pdf/1705.05363) | | E3B | 11.0 | [Craftax_Baselines](https://
+github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py) | [E3B](https:/
+/arxiv.org/abs/2210.05805) | ## Craftax-1M | Algorithm | Reward (% max) | Code
+| Paper | |:----------|---------------:|:--------------------------------------
+---------------------------------------------------------:|:-------------------
+--------------------:| | PPO-RNN | 2.3 | [Craftax_Baselines](https://
+github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo_rnn.py) | [PPO]
+(https://arxiv.org/abs/1707.06347) | | RND | 2.2 | [Craftax_Baselines](https://
+github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo_rnd.py) | [RND]
+(https://arxiv.org/abs/1810.12894) | | PPO | 2.2 | [Craftax_Baselines](https://
+github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py) | [PPO](https:/
+/arxiv.org/abs/1707.06347) | | ICM | 2.2 | [Craftax_Baselines](https://
+github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py) | [ICM](https:/
+/arxiv.org/pdf/1705.05363) | | E3B | 2.2 | [Craftax_Baselines](https://
+github.com/MichaelTMatthews/Craftax_Baselines/blob/main/ppo.py) | [E3B](https:/
+/arxiv.org/abs/2210.05805) | # ð¾ Offline Dataset A small dataset of mixed-
+skill human trajectories is available [here](https://drive.google.com/file/d/
+1wCMdUIsGOWYkNW55Rs0rHkYKUZhaQdtq/view?usp=sharing). Once the zip file has been
+extracted, the trajectories can be loaded with the `load_compressed_pickle`
+function. These were gathered on an earlier version of Craftax and it is
+recommended you use [v1.1.0](https://github.com/MichaelTMatthews/Craftax/
+releases/tag/v1.1.0) or earlier to investigate them. `run1` is the only
+trajectory to complete the game. # ð See Also - âï¸ [Crafter](https://
+github.com/danijar/crafter) The original Crafter benchmark. - âï¸ [NLE]
+(https://github.com/facebookresearch/nle) NetHack as an RL environment. - â¡
+[PureJaxRL](https://github.com/luchris429/purejaxrl) End-to-end RL
+implementations in Jax. - ð [JaxUED](https://github.com/DramaCow/jaxued):
+CleanRL style UED implementations in Jax. - ð [Minimax](https://github.com/
+facebookresearch/minimax): Modular UED implementations in Jax. - ðï¸
+[Gymnax](https://github.com/RobertTLange/gymnax): Standard Jax RL interface
+with classic environments. - ð§âð¤âð§ [JaxMARL](https://github.com/
+FLAIROx/JaxMARL): Multi-agent RL in Jax. # ð Citation If you use Craftax in
+your work please cite it as follows: ``` @article{matthews2024craftax, title=
+{Craftax: A Lightning-Fast Benchmark for Open-Ended Reinforcement Learning},
+author={Michael Matthews and Michael Beukman and Benjamin Ellis and Mikayel
+Samvelyan and Matthew Jackson and Samuel Coward and Jakob Foerster}, journal=
+{arXiv preprint}, year={2024}, } ```
```

### Comparing `craftax-1.4.1/craftax.egg-info/SOURCES.txt` & `craftax-1.4.2/craftax.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -157,14 +157,15 @@
 craftax/craftax/assets/water.png
 craftax/craftax/assets/wood.png
 craftax/craftax/assets/wood_pickaxe.png
 craftax/craftax/assets/wood_sword.png
 craftax/craftax/assets/xp.png
 craftax/craftax/assets/zombie.png
 craftax/craftax/envs/__init__.py
+craftax/craftax/envs/common.py
 craftax/craftax/envs/craftax_pixels_env.py
 craftax/craftax/envs/craftax_symbolic_env.py
 craftax/craftax/util/__init__.py
 craftax/craftax/util/game_logic_utils.py
 craftax/craftax/util/maths_utils.py
 craftax/craftax/util/noise.py
 craftax/craftax/world_gen/__init__.py
```

### Comparing `craftax-1.4.1/pyproject.toml` & `craftax-1.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "craftax"
-version = "1.4.1"
+version = "1.4.2"
 authors = [
   { name="Michael Matthews", email="michael.matthews@eng.ox.ac.uk" },
 ]
 description = "An open-world environment for training RL agents"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

