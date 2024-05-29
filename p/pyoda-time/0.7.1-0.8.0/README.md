# Comparing `tmp/pyoda_time-0.7.1.tar.gz` & `tmp/pyoda_time-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoda_time-0.7.1.tar", max compression
+gzip compressed data, was "pyoda_time-0.8.0.tar", max compression
```

## Comparing `pyoda_time-0.7.1.tar` & `pyoda_time-0.8.0.tar`

### file list

```diff
@@ -1,151 +1,168 @@
--rw-r--r--   0        0        0    11357 2024-05-17 20:05:11.540821 pyoda_time-0.7.1/LICENSE.txt
--rw-r--r--   0        0        0      595 2024-05-17 20:05:11.540821 pyoda_time-0.7.1/NOTICE.txt
--rw-r--r--   0        0        0     1692 2024-05-17 20:05:11.540821 pyoda_time-0.7.1/README.md
--rw-r--r--   0        0        0     1506 2024-05-17 20:05:11.560821 pyoda_time-0.7.1/pyoda_time/__init__.py
--rw-r--r--   0        0        0     1093 2024-05-17 20:05:11.560821 pyoda_time-0.7.1/pyoda_time/_calendar_ordinal.py
--rw-r--r--   0        0        0    36810 2024-05-17 20:05:11.560821 pyoda_time-0.7.1/pyoda_time/_calendar_system.py
--rw-r--r--   0        0        0      164 2024-05-17 20:05:11.560821 pyoda_time-0.7.1/pyoda_time/_compatibility/__init__.py
--rw-r--r--   0        0        0      770 2024-05-17 20:05:11.560821 pyoda_time-0.7.1/pyoda_time/_compatibility/_argument_exception.py
--rw-r--r--   0        0        0     2039 2024-05-17 20:05:11.560821 pyoda_time-0.7.1/pyoda_time/_compatibility/_calendar.py
--rw-r--r--   0        0        0    26120 2024-05-17 20:05:11.560821 pyoda_time-0.7.1/pyoda_time/_compatibility/_calendar_data.py
--rw-r--r--   0        0        0     4094 2024-05-17 20:05:11.560821 pyoda_time-0.7.1/pyoda_time/_compatibility/_calendar_id.py
--rw-r--r--   0        0        0    57748 2024-05-17 20:05:11.560821 pyoda_time-0.7.1/pyoda_time/_compatibility/_culture_data.py
--rw-r--r--   0        0        0    18099 2024-05-17 20:05:11.560821 pyoda_time-0.7.1/pyoda_time/_compatibility/_culture_info.py
--rw-r--r--   0        0        0     1757 2024-05-17 20:05:11.560821 pyoda_time-0.7.1/pyoda_time/_compatibility/_culture_not_found_exception.py
--rw-r--r--   0        0        0     1652 2024-05-17 20:05:11.560821 pyoda_time-0.7.1/pyoda_time/_compatibility/_culture_types.py
--rw-r--r--   0        0        0    23385 2024-05-17 20:05:11.560821 pyoda_time-0.7.1/pyoda_time/_compatibility/_date_time_format_info.py
--rw-r--r--   0        0        0      372 2024-05-17 20:05:11.560821 pyoda_time-0.7.1/pyoda_time/_compatibility/_day_of_week.py
--rw-r--r--   0        0        0     1148 2024-05-17 20:05:11.560821 pyoda_time-0.7.1/pyoda_time/_compatibility/_globalization_mode.py
--rw-r--r--   0        0        0      789 2024-05-17 20:05:11.560821 pyoda_time-0.7.1/pyoda_time/_compatibility/_gregorian_calendar.py
--rw-r--r--   0        0        0     1090 2024-05-17 20:05:11.560821 pyoda_time-0.7.1/pyoda_time/_compatibility/_gregorian_calendar_helper.py
--rw-r--r--   0        0        0      666 2024-05-17 20:05:11.560821 pyoda_time-0.7.1/pyoda_time/_compatibility/_gregorian_calendar_types.py
--rw-r--r--   0        0        0     2823 2024-05-17 20:05:11.560821 pyoda_time-0.7.1/pyoda_time/_compatibility/_hebrew_calendar.py
--rw-r--r--   0        0        0     2073 2024-05-17 20:05:11.560821 pyoda_time-0.7.1/pyoda_time/_compatibility/_hijri_calendar.py
--rw-r--r--   0        0        0      980 2024-05-17 20:05:11.560821 pyoda_time-0.7.1/pyoda_time/_compatibility/_i_format_provider.py
--rw-r--r--   0        0        0   172662 2024-05-17 20:05:11.560821 pyoda_time-0.7.1/pyoda_time/_compatibility/_icu_locale_data.py
--rw-r--r--   0        0        0    13348 2024-05-17 20:05:11.560821 pyoda_time-0.7.1/pyoda_time/_compatibility/_interop.py
--rw-r--r--   0        0        0     4767 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_compatibility/_japanese_calendar.py
--rw-r--r--   0        0        0     1152 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_compatibility/_korean_calendar.py
--rw-r--r--   0        0        0     2968 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_compatibility/_number_format_info.py
--rw-r--r--   0        0        0     1226 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_compatibility/_persian_calendar.py
--rw-r--r--   0        0        0     1150 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_compatibility/_string_builder.py
--rw-r--r--   0        0        0     1111 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_compatibility/_taiwan_calendar.py
--rw-r--r--   0        0        0      936 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_compatibility/_text_info.py
--rw-r--r--   0        0        0      814 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_compatibility/_thai_buddhist_calendar.py
--rw-r--r--   0        0        0      799 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_compatibility/_um_al_qura_calendar.py
--rw-r--r--   0        0        0      797 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_date_adjusters.py
--rw-r--r--   0        0        0     1934 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_date_interval.py
--rw-r--r--   0        0        0     3481 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_date_time_zone.py
--rw-r--r--   0        0        0    37920 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_duration.py
--rw-r--r--   0        0        0    19497 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_instant.py
--rw-r--r--   0        0        0      464 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_iso_day_of_week.py
--rw-r--r--   0        0        0    17684 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_local_date.py
--rw-r--r--   0        0        0    15920 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_local_date_time.py
--rw-r--r--   0        0        0     4755 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_local_instant.py
--rw-r--r--   0        0        0    25129 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_local_time.py
--rw-r--r--   0        0        0    18405 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_offset.py
--rw-r--r--   0        0        0     4229 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_offset_date_time.py
--rw-r--r--   0        0        0     2697 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_offset_time.py
--rw-r--r--   0        0        0    33887 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_period.py
--rw-r--r--   0        0        0     4545 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_period_builder.py
--rw-r--r--   0        0        0     1390 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_period_units.py
--rw-r--r--   0        0        0     3545 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_pyoda_constants.py
--rw-r--r--   0        0        0     8954 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_year_month.py
--rw-r--r--   0        0        0     4146 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_year_month_day.py
--rw-r--r--   0        0        0     4559 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_year_month_day_calendar.py
--rw-r--r--   0        0        0     3668 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/_zoned_date_time.py
--rw-r--r--   0        0        0      677 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/calendars/__init__.py
--rw-r--r--   0        0        0    11193 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/calendars/_badi_year_month_day_calculator.py
--rw-r--r--   0        0        0      411 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/calendars/_calendar_week_rule.py
--rw-r--r--   0        0        0     1310 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/calendars/_coptic_year_month_day_calculator.py
--rw-r--r--   0        0        0     4366 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/calendars/_era.py
--rw-r--r--   0        0        0     1208 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/calendars/_era_calculator.py
--rw-r--r--   0        0        0     2438 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/calendars/_fixed_month_year_month_day_calculator.py
--rw-r--r--   0        0        0     2048 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/calendars/_g_j_era_calculator.py
--rw-r--r--   0        0        0     3741 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/calendars/_g_j_year_month_day_calculator.py
--rw-r--r--   0        0        0     7126 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/calendars/_gregorian_year_month_day_calculator.py
--rw-r--r--   0        0        0     1781 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/calendars/_hebrew_month_converter.py
--rw-r--r--   0        0        0     1620 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/calendars/_hebrew_month_numbering.py
--rw-r--r--   0        0        0    12707 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/calendars/_hebrew_scriptural_calculator.py
--rw-r--r--   0        0        0    10894 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/calendars/_hebrew_year_month_day_calculator.py
--rw-r--r--   0        0        0      850 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/calendars/_i_week_year_rule.py
--rw-r--r--   0        0        0      866 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/calendars/_islamic_epoch.py
--rw-r--r--   0        0        0     1754 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/calendars/_islamic_leap_year_pattern.py
--rw-r--r--   0        0        0     7858 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/calendars/_islamic_year_month_day_calculator.py
--rw-r--r--   0        0        0     1559 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/calendars/_julian_year_month_day_calculator.py
--rw-r--r--   0        0        0     9097 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/calendars/_persian_year_month_day_calculator.py
--rw-r--r--   0        0        0     4737 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/calendars/_regular_year_month_day_calculator.py
--rw-r--r--   0        0        0    11988 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/calendars/_simple_week_year_rule.py
--rw-r--r--   0        0        0     2070 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/calendars/_single_era_calculator.py
--rw-r--r--   0        0        0     6168 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/calendars/_um_al_qura_year_month_day_calculator.py
--rw-r--r--   0        0        0     2998 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/calendars/_week_year_rules.py
--rw-r--r--   0        0        0    11714 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/calendars/_year_month_day_calculator.py
--rw-r--r--   0        0        0     2404 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/calendars/_year_start_cache_entry.py
--rw-r--r--   0        0        0      188 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/fields/__init__.py
--rw-r--r--   0        0        0      843 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/fields/_date_period_fields.py
--rw-r--r--   0        0        0     3111 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/fields/_fixed_length_date_period_field.py
--rw-r--r--   0        0        0     1552 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/fields/_i_date_period_field.py
--rw-r--r--   0        0        0     1039 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/fields/_months_period_field.py
--rw-r--r--   0        0        0     5401 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/fields/_time_period_field.py
--rw-r--r--   0        0        0     2112 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/fields/_years_period_field.py
--rw-r--r--   0        0        0      188 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/globalization/__init__.py
--rw-r--r--   0        0        0     1287 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/globalization/_pattern_resources.py
--rw-r--r--   0        0        0    24404 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/globalization/_pyoda_format_info.py
--rw-r--r--   0        0        0        0 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/py.typed
--rw-r--r--   0        0        0      803 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/text/__init__.py
--rw-r--r--   0        0        0     4803 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/text/_composite_pattern_builder.py
--rw-r--r--   0        0        0     1289 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/text/_fixed_format_info_pattern_parser.py
--rw-r--r--   0        0        0     7164 2024-05-17 20:05:11.564822 pyoda_time-0.7.1/pyoda_time/text/_format_helper.py
--rw-r--r--   0        0        0      932 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/text/_i_partial_pattern.py
--rw-r--r--   0        0        0     1781 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/text/_i_pattern.py
--rw-r--r--   0        0        0    10384 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/text/_instant_pattern.py
--rw-r--r--   0        0        0     4142 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/text/_instant_pattern_parser.py
--rw-r--r--   0        0        0      834 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/text/_invalid_pattern_exception.py
--rw-r--r--   0        0        0    13443 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/text/_local_date_pattern.py
--rw-r--r--   0        0        0    18274 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/text/_local_date_pattern_parser.py
--rw-r--r--   0        0        0    21615 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/text/_local_date_time_pattern.py
--rw-r--r--   0        0        0    15907 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/text/_local_date_time_pattern_parser.py
--rw-r--r--   0        0        0    16845 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/text/_local_time_pattern.py
--rw-r--r--   0        0        0    12001 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/text/_local_time_pattern_parser.py
--rw-r--r--   0        0        0     7527 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/text/_offset_pattern.py
--rw-r--r--   0        0        0    12491 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/text/_offset_pattern_parser.py
--rw-r--r--   0        0        0     1044 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/text/_parse_bucket.py
--rw-r--r--   0        0        0    18467 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/text/_parse_result.py
--rw-r--r--   0        0        0     3604 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/text/_text_cursor.py
--rw-r--r--   0        0        0     7703 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/text/_text_error_messages.py
--rw-r--r--   0        0        0      403 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/text/_unparsable_value_error.py
--rw-r--r--   0        0        0     9795 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/text/_value_cursor.py
--rw-r--r--   0        0        0      188 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/text/patterns/__init__.py
--rw-r--r--   0        0        0    11760 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/text/patterns/_date_pattern_helper.py
--rw-r--r--   0        0        0      594 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/text/patterns/_i_pattern_parser.py
--rw-r--r--   0        0        0     1545 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/text/patterns/_pattern_bcl_support.py
--rw-r--r--   0        0        0     4895 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/text/patterns/_pattern_cursor.py
--rw-r--r--   0        0        0     2263 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/text/patterns/_pattern_fields.py
--rw-r--r--   0        0        0    31977 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/text/patterns/_stepped_pattern_builder.py
--rw-r--r--   0        0        0    13177 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/text/patterns/_time_pattern_helper.py
--rw-r--r--   0        0        0      423 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/time_zones/__init__.py
--rw-r--r--   0        0        0     2001 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/time_zones/_fixed_date_time_zone.py
--rw-r--r--   0        0        0      777 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/time_zones/_i_zone_interval_map.py
--rw-r--r--   0        0        0     9198 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/time_zones/_tzdb_zone_1970_location.py
--rw-r--r--   0        0        0     5807 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/time_zones/_tzdb_zone_location.py
--rw-r--r--   0        0        0     8399 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/time_zones/_zone_interval.py
--rw-r--r--   0        0        0      297 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/time_zones/cldr/__init__.py
--rw-r--r--   0        0        0     6446 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/time_zones/cldr/_map_zone.py
--rw-r--r--   0        0        0     7056 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/time_zones/cldr/_windows_zones.py
--rw-r--r--   0        0        0      188 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/time_zones/io/__init__.py
--rw-r--r--   0        0        0     9693 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/time_zones/io/_date_time_zone_reader.py
--rw-r--r--   0        0        0    11633 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/time_zones/io/_date_time_zone_writer.py
--rw-r--r--   0        0        0     2906 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/time_zones/io/_i_date_time_zone_reader.py
--rw-r--r--   0        0        0     2832 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/time_zones/io/_i_date_time_zone_writer.py
--rw-r--r--   0        0        0     7959 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/time_zones/io/_tzdb_stream_data.py
--rw-r--r--   0        0        0     2084 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/time_zones/io/_tzdb_stream_field.py
--rw-r--r--   0        0        0     1801 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/time_zones/io/_tzdb_stream_field_id.py
--rw-r--r--   0        0        0      277 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/utility/__init__.py
--rw-r--r--   0        0        0     2620 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/utility/_cache.py
--rw-r--r--   0        0        0     5089 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/utility/_csharp_compatibility.py
--rw-r--r--   0        0        0      521 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/utility/_hash_code_helper.py
--rw-r--r--   0        0        0      488 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/utility/_invalid_pyoda_data_exception.py
--rw-r--r--   0        0        0     1904 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/utility/_preconditions.py
--rw-r--r--   0        0        0     2115 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyoda_time/utility/_tick_arithmetic.py
--rw-r--r--   0        0        0     1665 2024-05-17 20:05:11.568822 pyoda_time-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     2448 1970-01-01 00:00:00.000000 pyoda_time-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-29 09:07:51.312253 pyoda_time-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0      595 2024-05-29 09:07:51.312253 pyoda_time-0.8.0/NOTICE.txt
+-rw-r--r--   0        0        0     1840 2024-05-29 09:07:51.312253 pyoda_time-0.8.0/README.md
+-rw-r--r--   0        0        0     1993 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/__init__.py
+-rw-r--r--   0        0        0     3746 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_ambiguous_time_error.py
+-rw-r--r--   0        0        0     9081 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_annual_date.py
+-rw-r--r--   0        0        0     1093 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_calendar_ordinal.py
+-rw-r--r--   0        0        0    36810 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_calendar_system.py
+-rw-r--r--   0        0        0      164 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/__init__.py
+-rw-r--r--   0        0        0      770 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/_argument_exception.py
+-rw-r--r--   0        0        0     2039 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/_calendar.py
+-rw-r--r--   0        0        0    26120 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/_calendar_data.py
+-rw-r--r--   0        0        0     4094 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/_calendar_id.py
+-rw-r--r--   0        0        0    57748 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/_culture_data.py
+-rw-r--r--   0        0        0    18099 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/_culture_info.py
+-rw-r--r--   0        0        0     1757 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/_culture_not_found_exception.py
+-rw-r--r--   0        0        0     1652 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/_culture_types.py
+-rw-r--r--   0        0        0    23385 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/_date_time_format_info.py
+-rw-r--r--   0        0        0      372 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/_day_of_week.py
+-rw-r--r--   0        0        0     1148 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/_globalization_mode.py
+-rw-r--r--   0        0        0      789 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/_gregorian_calendar.py
+-rw-r--r--   0        0        0     1090 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/_gregorian_calendar_helper.py
+-rw-r--r--   0        0        0      666 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/_gregorian_calendar_types.py
+-rw-r--r--   0        0        0     2823 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/_hebrew_calendar.py
+-rw-r--r--   0        0        0     2073 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/_hijri_calendar.py
+-rw-r--r--   0        0        0      980 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/_i_format_provider.py
+-rw-r--r--   0        0        0   172662 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/_icu_locale_data.py
+-rw-r--r--   0        0        0    13348 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/_interop.py
+-rw-r--r--   0        0        0     4767 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/_japanese_calendar.py
+-rw-r--r--   0        0        0     1152 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/_korean_calendar.py
+-rw-r--r--   0        0        0     2968 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/_number_format_info.py
+-rw-r--r--   0        0        0     1226 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/_persian_calendar.py
+-rw-r--r--   0        0        0     1151 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/_string_builder.py
+-rw-r--r--   0        0        0     1111 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/_taiwan_calendar.py
+-rw-r--r--   0        0        0      936 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/_text_info.py
+-rw-r--r--   0        0        0      814 2024-05-29 09:07:51.332255 pyoda_time-0.8.0/pyoda_time/_compatibility/_thai_buddhist_calendar.py
+-rw-r--r--   0        0        0      799 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/_compatibility/_um_al_qura_calendar.py
+-rw-r--r--   0        0        0     6492 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/_date_adjusters.py
+-rw-r--r--   0        0        0     1934 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/_date_interval.py
+-rw-r--r--   0        0        0    10453 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/_date_time_zone.py
+-rw-r--r--   0        0        0    37920 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/_duration.py
+-rw-r--r--   0        0        0    19227 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/_instant.py
+-rw-r--r--   0        0        0     8159 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/_interval.py
+-rw-r--r--   0        0        0      464 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/_iso_day_of_week.py
+-rw-r--r--   0        0        0    20647 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/_local_date.py
+-rw-r--r--   0        0        0    16549 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/_local_date_time.py
+-rw-r--r--   0        0        0     8015 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/_local_instant.py
+-rw-r--r--   0        0        0    31271 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/_local_time.py
+-rw-r--r--   0        0        0    18405 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/_offset.py
+-rw-r--r--   0        0        0     4809 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/_offset_date_time.py
+-rw-r--r--   0        0        0    11005 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/_offset_time.py
+-rw-r--r--   0        0        0    33887 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/_period.py
+-rw-r--r--   0        0        0     4545 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/_period_builder.py
+-rw-r--r--   0        0        0     1390 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/_period_units.py
+-rw-r--r--   0        0        0     3545 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/_pyoda_constants.py
+-rw-r--r--   0        0        0     2697 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/_skipped_time_error.py
+-rw-r--r--   0        0        0     1665 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/_time_adjusters.py
+-rw-r--r--   0        0        0     8991 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/_year_month.py
+-rw-r--r--   0        0        0     4234 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/_year_month_day.py
+-rw-r--r--   0        0        0     4559 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/_year_month_day_calendar.py
+-rw-r--r--   0        0        0     3896 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/_zoned_date_time.py
+-rw-r--r--   0        0        0      677 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/calendars/__init__.py
+-rw-r--r--   0        0        0    11193 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/calendars/_badi_year_month_day_calculator.py
+-rw-r--r--   0        0        0      411 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/calendars/_calendar_week_rule.py
+-rw-r--r--   0        0        0     1310 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/calendars/_coptic_year_month_day_calculator.py
+-rw-r--r--   0        0        0     4366 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/calendars/_era.py
+-rw-r--r--   0        0        0     1208 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/calendars/_era_calculator.py
+-rw-r--r--   0        0        0     2438 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/calendars/_fixed_month_year_month_day_calculator.py
+-rw-r--r--   0        0        0     2048 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/calendars/_g_j_era_calculator.py
+-rw-r--r--   0        0        0     3741 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/calendars/_g_j_year_month_day_calculator.py
+-rw-r--r--   0        0        0     8399 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/calendars/_gregorian_year_month_day_calculator.py
+-rw-r--r--   0        0        0     1781 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/calendars/_hebrew_month_converter.py
+-rw-r--r--   0        0        0     1620 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/calendars/_hebrew_month_numbering.py
+-rw-r--r--   0        0        0    12707 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/calendars/_hebrew_scriptural_calculator.py
+-rw-r--r--   0        0        0    10894 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/calendars/_hebrew_year_month_day_calculator.py
+-rw-r--r--   0        0        0      850 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/calendars/_i_week_year_rule.py
+-rw-r--r--   0        0        0      866 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/calendars/_islamic_epoch.py
+-rw-r--r--   0        0        0     1754 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/calendars/_islamic_leap_year_pattern.py
+-rw-r--r--   0        0        0     7858 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/calendars/_islamic_year_month_day_calculator.py
+-rw-r--r--   0        0        0     1559 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/calendars/_julian_year_month_day_calculator.py
+-rw-r--r--   0        0        0     9097 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/calendars/_persian_year_month_day_calculator.py
+-rw-r--r--   0        0        0     4737 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/calendars/_regular_year_month_day_calculator.py
+-rw-r--r--   0        0        0    11988 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/calendars/_simple_week_year_rule.py
+-rw-r--r--   0        0        0     2070 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/calendars/_single_era_calculator.py
+-rw-r--r--   0        0        0     6168 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/calendars/_um_al_qura_year_month_day_calculator.py
+-rw-r--r--   0        0        0     2998 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/calendars/_week_year_rules.py
+-rw-r--r--   0        0        0    11714 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/calendars/_year_month_day_calculator.py
+-rw-r--r--   0        0        0     2404 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/calendars/_year_start_cache_entry.py
+-rw-r--r--   0        0        0      188 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/fields/__init__.py
+-rw-r--r--   0        0        0      843 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/fields/_date_period_fields.py
+-rw-r--r--   0        0        0     3111 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/fields/_fixed_length_date_period_field.py
+-rw-r--r--   0        0        0     1552 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/fields/_i_date_period_field.py
+-rw-r--r--   0        0        0     1039 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/fields/_months_period_field.py
+-rw-r--r--   0        0        0     5661 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/fields/_time_period_field.py
+-rw-r--r--   0        0        0     2112 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/fields/_years_period_field.py
+-rw-r--r--   0        0        0      188 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/globalization/__init__.py
+-rw-r--r--   0        0        0     1287 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/globalization/_pattern_resources.py
+-rw-r--r--   0        0        0    25175 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/globalization/_pyoda_format_info.py
+-rw-r--r--   0        0        0        0 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/py.typed
+-rw-r--r--   0        0        0      803 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/text/__init__.py
+-rw-r--r--   0        0        0     4803 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/text/_composite_pattern_builder.py
+-rw-r--r--   0        0        0     1289 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/text/_fixed_format_info_pattern_parser.py
+-rw-r--r--   0        0        0     7612 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/text/_format_helper.py
+-rw-r--r--   0        0        0      932 2024-05-29 09:07:51.336255 pyoda_time-0.8.0/pyoda_time/text/_i_partial_pattern.py
+-rw-r--r--   0        0        0     1781 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/text/_i_pattern.py
+-rw-r--r--   0        0        0    10380 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/text/_instant_pattern.py
+-rw-r--r--   0        0        0     4142 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/text/_instant_pattern_parser.py
+-rw-r--r--   0        0        0      834 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/text/_invalid_pattern_exception.py
+-rw-r--r--   0        0        0    13443 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/text/_local_date_pattern.py
+-rw-r--r--   0        0        0    18274 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/text/_local_date_pattern_parser.py
+-rw-r--r--   0        0        0    21615 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/text/_local_date_time_pattern.py
+-rw-r--r--   0        0        0    15907 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/text/_local_date_time_pattern_parser.py
+-rw-r--r--   0        0        0    16951 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/text/_local_time_pattern.py
+-rw-r--r--   0        0        0    12697 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/text/_local_time_pattern_parser.py
+-rw-r--r--   0        0        0     7527 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/text/_offset_pattern.py
+-rw-r--r--   0        0        0    12491 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/text/_offset_pattern_parser.py
+-rw-r--r--   0        0        0     1044 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/text/_parse_bucket.py
+-rw-r--r--   0        0        0    18467 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/text/_parse_result.py
+-rw-r--r--   0        0        0     3604 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/text/_text_cursor.py
+-rw-r--r--   0        0        0     7703 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/text/_text_error_messages.py
+-rw-r--r--   0        0        0      403 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/text/_unparsable_value_error.py
+-rw-r--r--   0        0        0     9795 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/text/_value_cursor.py
+-rw-r--r--   0        0        0      188 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/text/patterns/__init__.py
+-rw-r--r--   0        0        0    11760 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/text/patterns/_date_pattern_helper.py
+-rw-r--r--   0        0        0      594 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/text/patterns/_i_pattern_parser.py
+-rw-r--r--   0        0        0     1545 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/text/patterns/_pattern_bcl_support.py
+-rw-r--r--   0        0        0     4895 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/text/patterns/_pattern_cursor.py
+-rw-r--r--   0        0        0     2263 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/text/patterns/_pattern_fields.py
+-rw-r--r--   0        0        0    31988 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/text/patterns/_stepped_pattern_builder.py
+-rw-r--r--   0        0        0    14059 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/text/patterns/_time_pattern_helper.py
+-rw-r--r--   0        0        0   132921 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/Tzdb.nzd
+-rw-r--r--   0        0        0      605 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/__init__.py
+-rw-r--r--   0        0        0     2152 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/_cached_date_time_zone.py
+-rw-r--r--   0        0        0     6270 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/_caching_zone_interval_map.py
+-rw-r--r--   0        0        0     4336 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/_fixed_date_time_zone.py
+-rw-r--r--   0        0        0     4426 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/_i_date_time_zone_source.py
+-rw-r--r--   0        0        0      777 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/_i_zone_interval_map.py
+-rw-r--r--   0        0        0     9754 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/_precalculated_date_time_zone.py
+-rw-r--r--   0        0        0     9850 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/_standard_daylight_alternating_map.py
+-rw-r--r--   0        0        0     1817 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/_transition.py
+-rw-r--r--   0        0        0      581 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/_transition_mode.py
+-rw-r--r--   0        0        0    16547 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/_tzdb_date_time_zone_source.py
+-rw-r--r--   0        0        0     9198 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/_tzdb_zone_1970_location.py
+-rw-r--r--   0        0        0     5807 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/_tzdb_zone_location.py
+-rw-r--r--   0        0        0     8568 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/_zone_interval.py
+-rw-r--r--   0        0        0     6751 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/_zone_local_mapping.py
+-rw-r--r--   0        0        0    15669 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/_zone_recurrence.py
+-rw-r--r--   0        0        0    11534 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/_zone_year_offset.py
+-rw-r--r--   0        0        0      297 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/cldr/__init__.py
+-rw-r--r--   0        0        0     6446 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/cldr/_map_zone.py
+-rw-r--r--   0        0        0     7056 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/cldr/_windows_zones.py
+-rw-r--r--   0        0        0      188 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/io/__init__.py
+-rw-r--r--   0        0        0     9795 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/io/_date_time_zone_reader.py
+-rw-r--r--   0        0        0    11633 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/io/_date_time_zone_writer.py
+-rw-r--r--   0        0        0     2906 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/io/_i_date_time_zone_reader.py
+-rw-r--r--   0        0        0     2832 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/io/_i_date_time_zone_writer.py
+-rw-r--r--   0        0        0    10480 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/io/_tzdb_stream_data.py
+-rw-r--r--   0        0        0     2138 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/io/_tzdb_stream_field.py
+-rw-r--r--   0        0        0     1801 2024-05-29 09:07:51.340255 pyoda_time-0.8.0/pyoda_time/time_zones/io/_tzdb_stream_field_id.py
+-rw-r--r--   0        0        0      277 2024-05-29 09:07:51.344256 pyoda_time-0.8.0/pyoda_time/utility/__init__.py
+-rw-r--r--   0        0        0     2620 2024-05-29 09:07:51.344256 pyoda_time-0.8.0/pyoda_time/utility/_cache.py
+-rw-r--r--   0        0        0     5634 2024-05-29 09:07:51.344256 pyoda_time-0.8.0/pyoda_time/utility/_csharp_compatibility.py
+-rw-r--r--   0        0        0      521 2024-05-29 09:07:51.344256 pyoda_time-0.8.0/pyoda_time/utility/_hash_code_helper.py
+-rw-r--r--   0        0        0      488 2024-05-29 09:07:51.344256 pyoda_time-0.8.0/pyoda_time/utility/_invalid_pyoda_data_exception.py
+-rw-r--r--   0        0        0     1904 2024-05-29 09:07:51.344256 pyoda_time-0.8.0/pyoda_time/utility/_preconditions.py
+-rw-r--r--   0        0        0     2115 2024-05-29 09:07:51.344256 pyoda_time-0.8.0/pyoda_time/utility/_tick_arithmetic.py
+-rw-r--r--   0        0        0     1661 2024-05-29 09:07:51.344256 pyoda_time-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     2596 1970-01-01 00:00:00.000000 pyoda_time-0.8.0/PKG-INFO
```

### Comparing `pyoda_time-0.7.1/LICENSE.txt` & `pyoda_time-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/NOTICE.txt` & `pyoda_time-0.8.0/NOTICE.txt`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/README.md` & `pyoda_time-0.8.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 ![PyPI - Status](https://img.shields.io/pypi/status/pyoda-time)
 ![PyPI - Version](https://img.shields.io/pypi/v/pyoda-time)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyoda-time)
 ![GitHub License](https://img.shields.io/github/license/chrisimcevoy/pyoda-time)
 [![Documentation Status](https://readthedocs.org/projects/pyoda-time/badge/?version=latest)](https://pyoda-time.readthedocs.io/en/latest/?badge=latest)
+[![codecov](https://codecov.io/github/chrisimcevoy/pyoda-time/graph/badge.svg?token=I1QQES7AVT)](https://codecov.io/github/chrisimcevoy/pyoda-time)
 
 # Pyoda Time
 
 Pyoda Time is an alternative date and time API for Python. 
 
 It helps you to think about your data more clearly, and express operations on that data more precisely.
```

### Comparing `pyoda_time-0.7.1/pyoda_time/__init__.py` & `pyoda_time-0.8.0/pyoda_time/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,62 +1,75 @@
 # Copyright 2024 The Pyoda Time Authors. All rights reserved.
 # Use of this source code is governed by the Apache License 2.0,
 # as found in the LICENSE.txt file.
 
-__version__ = "0.7.1"
+__version__ = "0.8.0"
 
 __all__: list[str] = [
     "calendars",
     "fields",
     "globalization",
     "text",
     "time_zones",
     "utility",
+    "AmbiguousTimeError",
+    "AnnualDate",
     "CalendarSystem",
     "DateAdjusters",
     "DateInterval",
     "DateTimeZone",
     "Duration",
     "Instant",
+    "Interval",
     "IsoDayOfWeek",
     "LocalDate",
     "LocalTime",
     "LocalDateTime",
     "Offset",
     "OffsetDateTime",
     "OffsetTime",
     "Period",
     "PeriodBuilder",
     "PeriodUnits",
     "PyodaConstants",
+    "SkippedTimeError",
+    "TimeAdjusters",
     "YearMonth",
     "ZonedDateTime",
 ]
 
 
 from . import (
     calendars,
     fields,
     globalization,
     text,
     time_zones,
     utility,
 )
+
+# Need to force PyodaConstants to import first, so that default arguments in other
+# classes which uses PyodaConstants (e.g. Interval) don't blow up.
+from ._pyoda_constants import PyodaConstants  # isort: skip
+from ._ambiguous_time_error import AmbiguousTimeError
+from ._annual_date import AnnualDate
 from ._calendar_system import CalendarSystem
 from ._date_adjusters import DateAdjusters
 from ._date_interval import DateInterval
 from ._date_time_zone import DateTimeZone
 from ._duration import Duration
 from ._instant import Instant
+from ._interval import Interval
 from ._iso_day_of_week import IsoDayOfWeek
 from ._local_date import LocalDate
 from ._local_date_time import LocalDateTime
 from ._local_time import LocalTime
 from ._offset import Offset
 from ._offset_date_time import OffsetDateTime
 from ._offset_time import OffsetTime
 from ._period import Period
 from ._period_builder import PeriodBuilder
 from ._period_units import PeriodUnits
-from ._pyoda_constants import PyodaConstants
+from ._skipped_time_error import SkippedTimeError
+from ._time_adjusters import TimeAdjusters
 from ._year_month import YearMonth
 from ._zoned_date_time import ZonedDateTime
```

### Comparing `pyoda_time-0.7.1/pyoda_time/_calendar_ordinal.py` & `pyoda_time-0.8.0/pyoda_time/_calendar_ordinal.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_calendar_system.py` & `pyoda_time-0.8.0/pyoda_time/_calendar_system.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_compatibility/_argument_exception.py` & `pyoda_time-0.8.0/pyoda_time/_compatibility/_argument_exception.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_compatibility/_calendar.py` & `pyoda_time-0.8.0/pyoda_time/_compatibility/_calendar.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_compatibility/_calendar_data.py` & `pyoda_time-0.8.0/pyoda_time/_compatibility/_calendar_data.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_compatibility/_calendar_id.py` & `pyoda_time-0.8.0/pyoda_time/_compatibility/_calendar_id.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_compatibility/_culture_data.py` & `pyoda_time-0.8.0/pyoda_time/_compatibility/_culture_data.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_compatibility/_culture_info.py` & `pyoda_time-0.8.0/pyoda_time/_compatibility/_culture_info.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_compatibility/_culture_not_found_exception.py` & `pyoda_time-0.8.0/pyoda_time/_compatibility/_culture_not_found_exception.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_compatibility/_culture_types.py` & `pyoda_time-0.8.0/pyoda_time/_compatibility/_culture_types.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_compatibility/_date_time_format_info.py` & `pyoda_time-0.8.0/pyoda_time/_compatibility/_date_time_format_info.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_compatibility/_globalization_mode.py` & `pyoda_time-0.8.0/pyoda_time/_compatibility/_globalization_mode.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_compatibility/_gregorian_calendar.py` & `pyoda_time-0.8.0/pyoda_time/_compatibility/_gregorian_calendar.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_compatibility/_gregorian_calendar_helper.py` & `pyoda_time-0.8.0/pyoda_time/_compatibility/_gregorian_calendar_helper.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_compatibility/_gregorian_calendar_types.py` & `pyoda_time-0.8.0/pyoda_time/_compatibility/_gregorian_calendar_types.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_compatibility/_hebrew_calendar.py` & `pyoda_time-0.8.0/pyoda_time/_compatibility/_hebrew_calendar.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_compatibility/_hijri_calendar.py` & `pyoda_time-0.8.0/pyoda_time/_compatibility/_hijri_calendar.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_compatibility/_i_format_provider.py` & `pyoda_time-0.8.0/pyoda_time/_compatibility/_i_format_provider.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_compatibility/_icu_locale_data.py` & `pyoda_time-0.8.0/pyoda_time/_compatibility/_icu_locale_data.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_compatibility/_interop.py` & `pyoda_time-0.8.0/pyoda_time/_compatibility/_interop.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_compatibility/_japanese_calendar.py` & `pyoda_time-0.8.0/pyoda_time/_compatibility/_japanese_calendar.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_compatibility/_korean_calendar.py` & `pyoda_time-0.8.0/pyoda_time/_compatibility/_korean_calendar.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_compatibility/_number_format_info.py` & `pyoda_time-0.8.0/pyoda_time/_compatibility/_number_format_info.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_compatibility/_persian_calendar.py` & `pyoda_time-0.8.0/pyoda_time/_compatibility/_persian_calendar.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_compatibility/_string_builder.py` & `pyoda_time-0.8.0/pyoda_time/_compatibility/_string_builder.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     @property
     def length(self) -> int:
         return len(self.__string)
 
     @length.setter
     def length(self, value: int) -> None:
-        assert 0 < value <= self.length
+        assert 0 <= value <= self.length
         self.__string = self.__string[:value]
 
     def append(self, string: str) -> Self:
         self.__string += string
         return self
 
     def append_line(self, string: str = "") -> Self:
```

### Comparing `pyoda_time-0.7.1/pyoda_time/_compatibility/_taiwan_calendar.py` & `pyoda_time-0.8.0/pyoda_time/_compatibility/_taiwan_calendar.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_compatibility/_text_info.py` & `pyoda_time-0.8.0/pyoda_time/_compatibility/_text_info.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_compatibility/_thai_buddhist_calendar.py` & `pyoda_time-0.8.0/pyoda_time/_compatibility/_thai_buddhist_calendar.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_compatibility/_um_al_qura_calendar.py` & `pyoda_time-0.8.0/pyoda_time/_compatibility/_um_al_qura_calendar.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_date_interval.py` & `pyoda_time-0.8.0/pyoda_time/_date_interval.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_duration.py` & `pyoda_time-0.8.0/pyoda_time/_duration.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_instant.py` & `pyoda_time-0.8.0/pyoda_time/_instant.py`

 * *Files 2% similar despite different names*

```diff
@@ -468,17 +468,12 @@
 
         offset_date_time = OffsetDateTime._ctor(
             local_date=LocalDate._ctor(days_since_epoch=self.__duration._floor_days),
             offset_time=OffsetTime._ctor(nanosecond_of_day_zero_offset=self.__duration._nanosecond_of_floor_day),
         )
         return ZonedDateTime._ctor(offset_date_time=offset_date_time, zone=DateTimeZone.utc)
 
-    def __str__(self) -> str:
-        if not self._is_valid:
-            if self == self._before_min_value():
-                # TODO: Instant._before_min_value.__str__()
-                return super().__str__()
-            if self == self._after_max_value():
-                # TODO: Instant._after_max_value.__str__()
-                return super().__str__()
-        ldt = self.in_utc().local_date_time
-        return f"{ldt.year:0>4}-{ldt.month:0>2}-{ldt.day:0>2}T{ldt.hour:0>2}:{ldt.minute:0>2}:{ldt.second:0>2}Z"
+    def __repr__(self) -> str:
+        from pyoda_time._compatibility._culture_info import CultureInfo
+        from pyoda_time.text import InstantPattern
+
+        return InstantPattern._bcl_support.format(self, None, CultureInfo.current_culture)
```

### Comparing `pyoda_time-0.7.1/pyoda_time/_local_date.py` & `pyoda_time-0.8.0/pyoda_time/_local_date.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright 2024 The Pyoda Time Authors. All rights reserved.
 # Use of this source code is governed by the Apache License 2.0,
 # as found in the LICENSE.txt file.
 
 from __future__ import annotations
 
-from typing import TYPE_CHECKING, Generator, final, overload
+from typing import TYPE_CHECKING, Callable, Generator, final, overload
 
 from ._calendar_ordinal import _CalendarOrdinal
 from ._calendar_system import CalendarSystem
 from ._iso_day_of_week import IsoDayOfWeek
 from .calendars import Era, WeekYearRules
 from .utility._csharp_compatibility import _sealed
 from .utility._preconditions import _Preconditions
@@ -393,24 +393,79 @@
         return _DatePeriodFields._days_field.add(self, days)
 
     def plus_weeks(self, weeks: int) -> LocalDate:
         from .fields._date_period_fields import _DatePeriodFields
 
         return _DatePeriodFields._weeks_field.add(self, weeks)
 
+    def next(self, target_day_of_week: IsoDayOfWeek) -> LocalDate:
+        """Returns the next ``LocalDate`` falling on the specified ``IsoDayOfWeek``.
+
+        This is a strict "next" - if this date on already falls on the target day of the week, the returned value will
+        be a week later.
+
+        :param target_day_of_week: The ISO day of the week to return the next date of.
+        :return: The next ``LocalDate`` falling on the specified day of the week.
+        :raises RuntimeError: The underlying calendar doesn't use ISO days of the week.
+        :raises ValueError: ``target_day_of_week`` is not a valid day of the week (Monday to Sunday).
+        """
+        if target_day_of_week < IsoDayOfWeek.MONDAY or target_day_of_week > IsoDayOfWeek.SUNDAY:
+            raise ValueError(
+                f"target_day_of_week must be in the range [{IsoDayOfWeek.MONDAY} to {IsoDayOfWeek.SUNDAY}]"
+            )
+        # This will throw the desired exception for calendars with different week systems.
+        this_day = self.day_of_week
+        difference = target_day_of_week - this_day
+        if difference <= 0:
+            difference += 7
+        return self.plus_days(difference)
+
+    def previous(self, target_day_of_week: IsoDayOfWeek) -> LocalDate:
+        """Returns the previous ``LocalDate`` falling on the specified ``IsoDayOfWeek``.
+
+        This is a strict "previous" - if this date on already falls on the target day of the week, the returned value
+        will be a week earlier.
+
+        :param target_day_of_week: The ISO day of the week to return the previous date of.
+        :return: The previous ``LocalDate`` falling on the specified day of the week.
+        :raises RuntimeError: The underlying calendar doesn't use ISO days of the week.
+        :raises ValueError: ``target_day_of_week`` is not a valid day of the week (Monday to Sunday).
+        """
+        if target_day_of_week < IsoDayOfWeek.MONDAY or target_day_of_week > IsoDayOfWeek.SUNDAY:
+            raise ValueError(
+                f"target_day_of_week must be in the range [{IsoDayOfWeek.MONDAY} to {IsoDayOfWeek.SUNDAY}]"
+            )
+        # This will throw the desired exception for calendars with different week systems.
+        this_day = self.day_of_week
+        difference = target_day_of_week - this_day
+        if difference >= 0:
+            difference -= 7
+        return self.plus_days(difference)
+
     def at(self, time: LocalTime) -> LocalDateTime:
         """Combines this ``LocalDate`` with the given ``LocalTime`` into a single ``LocalDateTime``.
 
         Fluent alternative to ``+``.
 
         :param time: The time to combine with this date.
         :return: The ``LocalDateTime`` representation of the given time on this date.
         """
         return self + time
 
+    def with_(self, adjuster: Callable[[LocalDate], LocalDate]) -> LocalDate:
+        """Returns this date, with the given adjuster applied to it.
+
+        If the adjuster attempts to construct an invalid date (such as by trying to set a day-of-month of 30 in
+        February), any exception thrown by that construction attempt will be propagated through this method.
+
+        :param adjuster: The adjuster to apply.
+        :return: The adjusted date.
+        """
+        return _Preconditions._check_not_null(adjuster, "adjuster")(self)
+
     def __iter__(self) -> Generator[int, None, None]:
         """Deconstructs the current instance into its components.
 
         This enables instances of ``LocalDate`` to be unpacked into year, month
         and day, similar to the equivalent ``LocalDate.Deconstruct`` in Noda Time.
 
         :return: A generator which yields the "year", "month" and "day" components of this date.
```

### Comparing `pyoda_time-0.7.1/pyoda_time/_local_date_time.py` & `pyoda_time-0.8.0/pyoda_time/_local_date_time.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import TYPE_CHECKING, final, overload
 
 from ._calendar_system import CalendarSystem
 from .utility._csharp_compatibility import _sealed
 from .utility._preconditions import _Preconditions
 
 if TYPE_CHECKING:
-    from . import Period, ZonedDateTime
+    from . import Offset, OffsetDateTime, Period, ZonedDateTime
     from ._iso_day_of_week import IsoDayOfWeek
     from ._local_date import LocalDate
     from ._local_instant import _LocalInstant
     from ._local_time import LocalTime
     from .calendars import Era
 
 __all__ = ["LocalDateTime"]
@@ -372,14 +372,27 @@
             .plus_weeks(period.weeks)
             .plus_days(period.days + extra_days)
         )
         return LocalDateTime._ctor(local_date=date, local_time=time)
 
     # endregion
 
+    def with_offset(self, offset: Offset) -> OffsetDateTime:
+        """Returns an ``OffsetDateTime`` for this local date/time with the given offset.
+
+        This method is purely a convenient alternative to calling the ``OffsetDateTime`` constructor directly.
+
+        :param offset: The offset to apply.
+        :return: The result of this local date/time offset by the given amount.
+        """
+        from ._offset_date_time import OffsetDateTime
+        from ._offset_time import OffsetTime
+
+        return OffsetDateTime._ctor(local_date=self.__date, offset_time=OffsetTime(self.__time, offset))
+
     def in_utc(self) -> ZonedDateTime:
         """Returns the mapping of this local date/time within ``DateTimeZone.Utc``.
 
         As UTC is a fixed time zone, there is no chance that this local date/time is ambiguous or skipped.
 
         :return: The result of mapping this local date/time in UTC.
         """
```

### Comparing `pyoda_time-0.7.1/pyoda_time/_local_time.py` & `pyoda_time-0.8.0/pyoda_time/_local_time.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Copyright 2024 The Pyoda Time Authors. All rights reserved.
 # Use of this source code is governed by the Apache License 2.0,
 # as found in the LICENSE.txt file.
 
 from __future__ import annotations
 
+import datetime
 import functools
-from typing import TYPE_CHECKING, Generator, final, overload
+from typing import TYPE_CHECKING, Callable, Generator, final, overload
 
 from ._pyoda_constants import PyodaConstants
 from .utility._csharp_compatibility import (
     _csharp_modulo,
     _int32_overflow,
     _int64_overflow,
     _sealed,
@@ -364,14 +365,58 @@
         return _int32_overflow(_csharp_modulo(self.__nanoseconds, PyodaConstants.NANOSECONDS_PER_SECOND))
 
     @property
     def nanosecond_of_day(self) -> int:
         """The nanosecond of this local time within the day, in the range 0 to 86,399,999,999,999 inclusive."""
         return self.__nanoseconds
 
+    def __add__(self, other: Period) -> LocalTime:
+        """Creates a new local time by adding a period to an existing time.
+
+        The period must not contain any date-related units (days etc.) with non-zero values.
+
+        :param other: The period to add
+        :return: The result of adding the period to the time, wrapping via midnight if necessary
+        """
+        from ._period import Period
+
+        if not isinstance(other, Period):
+            return NotImplemented  # type: ignore[unreachable]
+
+        _Preconditions._check_not_null(other, "other")
+        _Preconditions._check_argument(
+            not other.has_date_component, "other", "Cannot add a period with a date component to a time"
+        )
+        return (
+            self.plus_hours(other.hours)
+            .plus_minutes(other.minutes)
+            .plus_seconds(other.seconds)
+            .plus_milliseconds(other.milliseconds)
+            .plus_ticks(other.ticks)
+            .plus_nanoseconds(other.nanoseconds)
+        )
+
+    @staticmethod
+    def add(time: LocalTime, period: Period) -> LocalTime:
+        """Adds the specified period to the time. Friendly alternative to ``+``.
+
+        :param time: The time to add the period to
+        :param period: The period to add. Must not contain any (non-zero) date units.
+        :return: The sum of the given time and period
+        """
+        return time + period
+
+    def plus(self, period: Period) -> LocalTime:
+        """Adds the specified period to this time. Fluent alternative to ``+``.
+
+        :param period: The period to add. Must not contain any (non-zero) date units.
+        :return: The sum of this time and the given period
+        """
+        return self + period
+
     @overload
     def __sub__(self, local_time: LocalTime) -> Period: ...
 
     @overload
     def __sub__(self, period: Period) -> LocalTime: ...
 
     def __sub__(self, other: LocalTime | Period) -> LocalTime | Period:
@@ -388,18 +433,68 @@
                 .plus_seconds(-other.seconds)
                 .plus_milliseconds(-other.milliseconds)
                 .plus_ticks(-other.ticks)
                 .plus_nanoseconds(-other.nanoseconds)
             )
 
         if isinstance(other, LocalTime):
-            return Period.between(self, other)
+            return Period.between(other, self)
 
         return NotImplemented  # type: ignore[unreachable]
 
+    @staticmethod
+    @overload
+    def subtract(time: LocalTime, period: Period, /) -> LocalTime:
+        """Subtracts the specified period from the time. Friendly alternative to ``-``.
+
+        :param time: The time to subtract the period from
+        :param period: The period to subtract. Must not contain any (non-zero) date units.
+        :return: The result of subtracting the given period from the time.
+        """
+        ...
+
+    @staticmethod
+    @overload
+    def subtract(lhs: LocalTime, rhs: LocalTime, /) -> Period:
+        """Subtracts one time from another, returning the result as a ``Period`` with units of years, months and days.
+
+        This is simply a convenience method for calling ``Period.between(LocalTime,LocalTime)``.
+
+        :param lhs: The time to subtract from
+        :param rhs: The time to subtract
+        :return: The result of subtracting one time from another.
+        """
+        ...
+
+    @staticmethod
+    def subtract(lhs: LocalTime, rhs: LocalTime | Period, /) -> LocalTime | Period:
+        return lhs - rhs
+
+    @overload
+    def minus(self, period: Period, /) -> LocalTime:
+        """Subtracts the specified period from this time. Fluent alternative to ``-``.
+
+        :param period: The period to subtract. Must not contain any (non-zero) date units.
+        :return: The result of subtracting the given period from this time.
+        """
+        ...
+
+    @overload
+    def minus(self, time: LocalTime, /) -> Period:
+        """Subtracts the specified time from this time, returning the result as a ``Period``. Fluent alternative to
+        ``-``.
+
+        :param time: The time to subtract from this
+        :return: The difference between the specified time and this one
+        """
+        ...
+
+    def minus(self, period_or_time: Period | LocalTime, /) -> Period | LocalTime:
+        return self - period_or_time
+
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, LocalTime):
             return NotImplemented
         return self.__nanoseconds == other.__nanoseconds
 
     def __ne__(self, other: object) -> bool:
         if not isinstance(other, LocalTime):
@@ -425,16 +520,21 @@
         if not isinstance(other, LocalTime):
             return NotImplemented  # type: ignore[unreachable]
         return self.__nanoseconds >= other.__nanoseconds
 
     def compare_to(self, other: LocalTime | None) -> int:
         if other is None:
             return 1
+        if not isinstance(other, LocalTime):
+            raise TypeError(f"{self.__class__.__name__} cannot be compared to {other.__class__.__name__}")
         return self.__nanoseconds - other.__nanoseconds
 
+    def __hash__(self) -> int:
+        return hash(self.__nanoseconds)
+
     def plus_hours(self, hours: int) -> LocalTime:
         """Returns a new LocalTime representing the current value with the given number of hours added.
 
         If the value goes past the start or end of the day, it wraps - so 11pm plus two hours is 1am, for example.
 
         :param hours: The number of hours to add
         :return: The current value plus the given number of hours.
@@ -474,14 +574,24 @@
         :param milliseconds: The number of milliseconds to add
         :return: The current value plus the given number of milliseconds.
         """
         from pyoda_time.fields._time_period_field import _TimePeriodField
 
         return _TimePeriodField._milliseconds._add_local_time(self, milliseconds)
 
+    def plus_microseconds(self, microseconds: int) -> LocalTime:
+        """Returns a new LocalTime representing the current value with the given number of microseconds added.
+
+        :param microseconds: The number of microseconds to add
+        :return: The current value plus the given number of microseconds.
+        """
+        from pyoda_time.fields._time_period_field import _TimePeriodField
+
+        return _TimePeriodField._microseconds._add_local_time(self, microseconds)
+
     def plus_ticks(self, ticks: int) -> LocalTime:
         """Returns a new LocalTime representing the current value with the given number of ticks added.
 
         :param ticks: The number of ticks to add
         :return: The current value plus the given number of ticks.
         """
         from pyoda_time.fields._time_period_field import _TimePeriodField
@@ -494,14 +604,17 @@
         :param nanoseconds: The number of nanoseconds to add
         :return: The current value plus the given number of ticks.
         """
         from .fields._time_period_field import _TimePeriodField
 
         return _TimePeriodField._nanoseconds._add_local_time(self, nanoseconds)
 
+    def with_(self, adjuster: Callable[[LocalTime], LocalTime]) -> LocalTime:
+        return _Preconditions._check_not_null(adjuster, "adjuster")(self)
+
     def with_offset(self, offset: Offset) -> OffsetTime:
         """Returns an ``OffsetTime`` for this time-of-day with the given offset.
 
         This method is purely a convenient alternative to calling the ``OffsetTime`` constructor directly.
 
         :param offset: The offset to apply.
         :return: The result of this time-of-day offset by the given amount.
@@ -544,7 +657,52 @@
         """Returns the earlier time of the given two.
 
         :param x: The first time to compare.
         :param y: The second time to compare.
         :return: The earlier time of ``x`` or ``y``.
         """
         return x if x < y else y
+
+    # region Formatting
+
+    def __repr__(self) -> str:
+        from pyoda_time._compatibility._culture_info import CultureInfo
+        from pyoda_time.text import LocalTimePattern
+
+        return LocalTimePattern._bcl_support.format(self, None, CultureInfo.current_culture)
+
+    def __format__(self, format_spec: str) -> str:
+        from pyoda_time._compatibility._culture_info import CultureInfo
+        from pyoda_time.text import LocalTimePattern
+
+        return LocalTimePattern._bcl_support.format(self, format_spec, CultureInfo.current_culture)
+
+    # endregion
+
+    def to_time(self) -> datetime.time:
+        """Converts this value to an equivalent ``datetime.time``.
+
+        If the value does not fall on a microsecond boundary, it will be truncated to the earlier microsecond boundary.
+
+        :return: The equivalent ``datetime.time``.
+        """
+
+        return datetime.time(
+            hour=self.hour,
+            minute=self.minute,
+            second=self.second,
+            microsecond=_towards_zero_division(self.nanosecond_of_second, PyodaConstants.NANOSECONDS_PER_MICROSECOND),
+        )
+
+    @classmethod
+    def from_time(cls, time: datetime.time) -> LocalTime:
+        """Constructs a ``LocalTime`` from a ``datetime.time``.
+
+        :param time: The time of day to convert.
+        :return: The ``LocalTime`` equivalent.
+        """
+        return cls.from_ticks_since_midnight(
+            time.hour * PyodaConstants.TICKS_PER_HOUR
+            + time.minute * PyodaConstants.TICKS_PER_MINUTE
+            + time.second * PyodaConstants.TICKS_PER_SECOND
+            + time.microsecond * PyodaConstants.TICKS_PER_MICROSECOND
+        )
```

### Comparing `pyoda_time-0.7.1/pyoda_time/_offset.py` & `pyoda_time-0.8.0/pyoda_time/_offset.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_offset_date_time.py` & `pyoda_time-0.8.0/pyoda_time/_offset_date_time.py`

 * *Files 8% similar despite different names*

```diff
@@ -117,7 +117,21 @@
     def __to_elapsed_time_since_epoch(self) -> Duration:
         # Equivalent to LocalDateTime.ToLocalInstant().Minus(offset)
         days: int = self.__local_date._days_since_epoch
         elapsed_time: Duration = Duration._ctor(days=days, nano_of_day=self.nanosecond_of_day)._minus_small_nanoseconds(
             self.__offset_time._offset_nanoseconds
         )
         return elapsed_time
+
+    # region Operators
+
+    def __eq__(self, other: object) -> bool:
+        """Implements the operator == (equality). See the type documentation for a description of equality semantics.
+
+        :param other: The value to compare this offset date/time with.
+        :return: True if the given value is another offset date/time equal to this one; false otherwise..
+        """
+        if not isinstance(other, OffsetDateTime):
+            return NotImplemented
+        return self.__local_date == other.__local_date and self.__offset_time == other.__offset_time
+
+    # endregion
```

### Comparing `pyoda_time-0.7.1/pyoda_time/_period.py` & `pyoda_time-0.8.0/pyoda_time/_period.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_period_builder.py` & `pyoda_time-0.8.0/pyoda_time/_period_builder.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_period_units.py` & `pyoda_time-0.8.0/pyoda_time/_period_units.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_pyoda_constants.py` & `pyoda_time-0.8.0/pyoda_time/_pyoda_constants.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_year_month.py` & `pyoda_time-0.8.0/pyoda_time/_year_month.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,16 @@
         :param other: The other year/month to compare this one with.
         :return: A value less than zero if this year/month is earlier than ``other``;
             zero if this year/month is the same as ``other``;
             a value greater than zero if this date is later than ``other``.
         """
         if other is None:
             return 1
-        _Preconditions._check_argument(isinstance(other, YearMonth), "other", "Object must be of type YearMonth.")
+        if not isinstance(other, YearMonth):
+            raise TypeError(f"{self.__class__.__name__} cannot be compared to {other.__class__.__name__}")
         _Preconditions._check_argument(
             self.__calendar_ordinal == other.__calendar_ordinal,
             "other",
             "Only values with the same calendar system can be compared",
         )
         return self.__trusted_compare_to(other)
```

### Comparing `pyoda_time-0.7.1/pyoda_time/_year_month_day.py` & `pyoda_time-0.8.0/pyoda_time/_year_month_day.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,15 +69,16 @@
 
     def _with_calendar_ordinal(self, calendar_ordinal: _CalendarOrdinal) -> _YearMonthDayCalendar:
         return _YearMonthDayCalendar._ctor(year_month_day=self.__value, calendar_ordinal=calendar_ordinal)
 
     def compare_to(self, other: _YearMonthDay | None) -> int:
         if other is None:
             return 1
-        # In Noda Time, this method calls `int.CompareTo(otherInt)`
+        if not isinstance(other, _YearMonthDay):
+            raise TypeError(f"{self.__class__.__name__} cannot be compared to {other.__class__.__name__}")
         return self.__value - other.__value
 
     def equals(self, other: _YearMonthDay) -> bool:
         return self == other
 
     def __hash__(self) -> int:
         return self.__value
```

### Comparing `pyoda_time-0.7.1/pyoda_time/_year_month_day_calendar.py` & `pyoda_time-0.8.0/pyoda_time/_year_month_day_calendar.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/_zoned_date_time.py` & `pyoda_time-0.8.0/pyoda_time/_zoned_date_time.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,14 +70,22 @@
         else:
             raise ValueError
 
         self.__offset_date_time: OffsetDateTime = offset_date_time
         self.__zone: DateTimeZone = _Preconditions._check_not_null(zone, "zone")
 
     @property
+    def zone(self) -> DateTimeZone:
+        """Gets the time zone associated with this value.
+
+        :return: The time zone associated with this value.
+        """
+        return self.__zone or DateTimeZone.utc
+
+    @property
     def local_date_time(self) -> LocalDateTime:
         return self.__offset_date_time.local_date_time
 
     @property
     def year(self) -> int:
         """Gets the year of this zoned date and time.
```

### Comparing `pyoda_time-0.7.1/pyoda_time/calendars/__init__.py` & `pyoda_time-0.8.0/pyoda_time/calendars/__init__.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/calendars/_badi_year_month_day_calculator.py` & `pyoda_time-0.8.0/pyoda_time/calendars/_badi_year_month_day_calculator.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/calendars/_coptic_year_month_day_calculator.py` & `pyoda_time-0.8.0/pyoda_time/calendars/_coptic_year_month_day_calculator.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/calendars/_era.py` & `pyoda_time-0.8.0/pyoda_time/calendars/_era.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/calendars/_era_calculator.py` & `pyoda_time-0.8.0/pyoda_time/calendars/_era_calculator.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/calendars/_fixed_month_year_month_day_calculator.py` & `pyoda_time-0.8.0/pyoda_time/calendars/_fixed_month_year_month_day_calculator.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/calendars/_g_j_era_calculator.py` & `pyoda_time-0.8.0/pyoda_time/calendars/_g_j_era_calculator.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/calendars/_g_j_year_month_day_calculator.py` & `pyoda_time-0.8.0/pyoda_time/calendars/_g_j_year_month_day_calculator.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/calendars/_gregorian_year_month_day_calculator.py` & `pyoda_time-0.8.0/pyoda_time/calendars/_gregorian_year_month_day_calculator.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 # Use of this source code is governed by the Apache License 2.0,
 # as found in the LICENSE.txt file.
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Final, final
 
+from ..utility._preconditions import _Preconditions
+
 if TYPE_CHECKING:
     from .._year_month_day import _YearMonthDay
 from .._year_month_day_calendar import _YearMonthDayCalendar
 from ..utility._csharp_compatibility import _towards_zero_division
 from ._g_j_year_month_day_calculator import _GJYearMonthDayCalculator
 
 
@@ -141,22 +143,44 @@
 
     def _get_start_of_year_in_days(self, year: int) -> int:
         if year < self.__FIRST_OPTIMIZED_YEAR or year > self.__LAST_OPTIMIZED_YEAR:
             return super()._get_start_of_year_in_days(year)
         return self.__YEAR_START_DAYS[year - self.__FIRST_OPTIMIZED_YEAR]
 
     def _get_days_since_epoch(self, year_month_day: _YearMonthDay) -> int:
+        # TODO: unchecked
         year = year_month_day._year
         month_of_year = year_month_day._month
         day_of_month = year_month_day._day
         if year < self.__FIRST_OPTIMIZED_YEAR or year > self.__LAST_OPTIMIZED_YEAR:
             return super()._get_days_since_epoch(year_month_day)
         year_month_index = (year - self.__FIRST_OPTIMIZED_YEAR) * 12 + month_of_year
         return self.__MONTH_START_DAYS[year_month_index] + day_of_month
 
+    def _validate_year_month_day(self, year: int, month: int, day: int) -> None:
+        self._validate_gregorian_year_month_day(year, month, day)
+
+    @classmethod
+    def _validate_gregorian_year_month_day(cls, year: int, month: int, day: int) -> None:
+        # Perform quick validation without calling Preconditions, then do it properly if we're going to throw
+        # an exception. Avoiding the method call is pretty extreme, but it does help.
+        if year < cls._MIN_GREGORIAN_YEAR or year > cls._MAX_GREGORIAN_YEAR or month < 1 or month > 12:
+            _Preconditions._check_argument_range("year", year, cls._MIN_GREGORIAN_YEAR, cls._MAX_GREGORIAN_YEAR)
+            _Preconditions._check_argument_range("month", month, 1, 12)
+        # If we've been asked for day 1-28, we're definitely okay regardless of month.
+        if 1 <= day <= 20:
+            return
+        days_in_month = (
+            cls._LEAP_DAYS_PER_MONTH[month]
+            if month == 2 and cls.__is_gregorian_leap_year(year)
+            else cls._NON_LEAP_DAYS_PER_MONTH[month]
+        )
+        if day < 1 or day > days_in_month:
+            _Preconditions._check_argument_range("day", day, 1, days_in_month)
+
     def _calculate_start_of_year_days(self, year: int) -> int:
         leap_years = _towards_zero_division(year, 100)
         if year < 0:
             # Add 3 before shifting right since /4 and >>2 behave differently
             # on negative numbers. When the expression is written as
             # (year / 4) - (year / 100) + (year / 400),
             # it works for both positive and negative values, except this optimization
```

### Comparing `pyoda_time-0.7.1/pyoda_time/calendars/_hebrew_month_converter.py` & `pyoda_time-0.8.0/pyoda_time/calendars/_hebrew_month_converter.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/calendars/_hebrew_month_numbering.py` & `pyoda_time-0.8.0/pyoda_time/calendars/_hebrew_month_numbering.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/calendars/_hebrew_scriptural_calculator.py` & `pyoda_time-0.8.0/pyoda_time/calendars/_hebrew_scriptural_calculator.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/calendars/_hebrew_year_month_day_calculator.py` & `pyoda_time-0.8.0/pyoda_time/calendars/_hebrew_year_month_day_calculator.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/calendars/_i_week_year_rule.py` & `pyoda_time-0.8.0/pyoda_time/calendars/_i_week_year_rule.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/calendars/_islamic_epoch.py` & `pyoda_time-0.8.0/pyoda_time/calendars/_islamic_epoch.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/calendars/_islamic_leap_year_pattern.py` & `pyoda_time-0.8.0/pyoda_time/calendars/_islamic_leap_year_pattern.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/calendars/_islamic_year_month_day_calculator.py` & `pyoda_time-0.8.0/pyoda_time/calendars/_islamic_year_month_day_calculator.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/calendars/_julian_year_month_day_calculator.py` & `pyoda_time-0.8.0/pyoda_time/calendars/_julian_year_month_day_calculator.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/calendars/_persian_year_month_day_calculator.py` & `pyoda_time-0.8.0/pyoda_time/calendars/_persian_year_month_day_calculator.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/calendars/_regular_year_month_day_calculator.py` & `pyoda_time-0.8.0/pyoda_time/calendars/_regular_year_month_day_calculator.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/calendars/_simple_week_year_rule.py` & `pyoda_time-0.8.0/pyoda_time/calendars/_simple_week_year_rule.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/calendars/_single_era_calculator.py` & `pyoda_time-0.8.0/pyoda_time/calendars/_single_era_calculator.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/calendars/_um_al_qura_year_month_day_calculator.py` & `pyoda_time-0.8.0/pyoda_time/calendars/_um_al_qura_year_month_day_calculator.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/calendars/_week_year_rules.py` & `pyoda_time-0.8.0/pyoda_time/calendars/_week_year_rules.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/calendars/_year_month_day_calculator.py` & `pyoda_time-0.8.0/pyoda_time/calendars/_year_month_day_calculator.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/calendars/_year_start_cache_entry.py` & `pyoda_time-0.8.0/pyoda_time/calendars/_year_start_cache_entry.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/fields/_date_period_fields.py` & `pyoda_time-0.8.0/pyoda_time/fields/_date_period_fields.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/fields/_fixed_length_date_period_field.py` & `pyoda_time-0.8.0/pyoda_time/fields/_fixed_length_date_period_field.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/fields/_i_date_period_field.py` & `pyoda_time-0.8.0/pyoda_time/fields/_i_date_period_field.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/fields/_months_period_field.py` & `pyoda_time-0.8.0/pyoda_time/fields/_months_period_field.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/fields/_time_period_field.py` & `pyoda_time-0.8.0/pyoda_time/fields/_time_period_field.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,14 +22,20 @@
         return _TimePeriodField(1)
 
     @property
     def _ticks(self) -> _TimePeriodField:
         return _TimePeriodField(PyodaConstants.NANOSECONDS_PER_TICK)
 
     @property
+    def _microseconds(self) -> _TimePeriodField:
+        # TODO: Investigate where other _TimePeriodFields are used...
+        #  This one is not ported from Noda Time.
+        return _TimePeriodField(PyodaConstants.NANOSECONDS_PER_MICROSECOND)
+
+    @property
     def _milliseconds(self) -> _TimePeriodField:
         return _TimePeriodField(PyodaConstants.NANOSECONDS_PER_MILLISECOND)
 
     @property
     def _seconds(self) -> _TimePeriodField:
         return _TimePeriodField(PyodaConstants.NANOSECONDS_PER_SECOND)
```

### Comparing `pyoda_time-0.7.1/pyoda_time/fields/_years_period_field.py` & `pyoda_time-0.8.0/pyoda_time/fields/_years_period_field.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/globalization/_pattern_resources.py` & `pyoda_time-0.8.0/pyoda_time/globalization/_pattern_resources.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/globalization/_pyoda_format_info.py` & `pyoda_time-0.8.0/pyoda_time/globalization/_pyoda_format_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -187,15 +187,28 @@
                     from ..text._offset_pattern_parser import _OffsetPatternParser
 
                     self.__offset_pattern_parser = _FixedFormatInfoPatternParser(_OffsetPatternParser(), self)
         return self.__offset_pattern_parser
 
     @property
     def _instant_pattern_parser(self) -> _FixedFormatInfoPatternParser[Instant]:
-        raise NotImplementedError
+        if self.__instant_pattern_parser is None:
+            with self.__FIELD_LOCK:
+                if self.__instant_pattern_parser is None:
+                    from pyoda_time.text import InstantPattern, LocalDatePattern
+                    from pyoda_time.text._fixed_format_info_pattern_parser import _FixedFormatInfoPatternParser
+                    from pyoda_time.text._instant_pattern_parser import _InstantPatternParser
+
+                    self.__instant_pattern_parser = _FixedFormatInfoPatternParser(
+                        _InstantPatternParser._ctor(
+                            InstantPattern._DEFAULT_TEMPLATE_VALUE, LocalDatePattern._DEFAULT_TWO_DIGIT_YEAR_MAX
+                        ),
+                        self,
+                    )
+        return self.__instant_pattern_parser
 
     @property
     def _local_time_pattern_parser(self) -> _FixedFormatInfoPatternParser[LocalTime]:
         if self.__local_time_pattern_parser is None:
             with self.__FIELD_LOCK:
                 if self.__local_time_pattern_parser is None:
                     from pyoda_time import LocalTime
```

### Comparing `pyoda_time-0.7.1/pyoda_time/text/__init__.py` & `pyoda_time-0.8.0/pyoda_time/text/__init__.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/text/_composite_pattern_builder.py` & `pyoda_time-0.8.0/pyoda_time/text/_composite_pattern_builder.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/text/_fixed_format_info_pattern_parser.py` & `pyoda_time-0.8.0/pyoda_time/text/_fixed_format_info_pattern_parser.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/text/_format_helper.py` & `pyoda_time-0.8.0/pyoda_time/text/_format_helper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,73 +1,73 @@
 # Copyright 2024 The Pyoda Time Authors. All rights reserved.
 # Use of this source code is governed by the Apache License 2.0,
 # as found in the LICENSE.txt file.
 from pyoda_time._compatibility._string_builder import StringBuilder
 from pyoda_time.utility._csharp_compatibility import _csharp_modulo, _CsharpConstants, _towards_zero_division
 
 
-class FormatHelper:
+class _FormatHelper:
     """Provides helper methods for formatting values using pattern strings."""
 
     @staticmethod
-    def format_2_digits_non_negative(value: int, output_buffer: StringBuilder) -> None:
+    def _format_2_digits_non_negative(value: int, output_buffer: StringBuilder) -> None:
         """Formats the given value to two digits, left-padding with '0' if necessary.
 
         It is assumed that the value is in the range [0, 100). This is usually used for month, day-of-month, hour,
         minute, second and year-of-century values.
         """
         # TODO: Preconditions.DebugCheckArgumentRange
         # TODO: unchecked
         # TODO: This is pretty different (but more idiomatic Python) compared to Noda Time.
         output_buffer.append(f"{value:02}")
 
     @staticmethod
-    def format_4_digits_value_fits(value: int, output_buffer: StringBuilder) -> None:
+    def _format_4_digits_value_fits(value: int, output_buffer: StringBuilder) -> None:
         """Formats the given value to two digits, left-padding with '0' if necessary.
 
         It is assumed that the value is in the range [-9999, 10000). This is usually used for year values. If the value
         is negative, a '-' character is prepended.
         """
         # TODO: Preconditions.DebugCheckArgumentRange
         # TODO: unchecked
         # TODO: This is pretty different (but more idiomatic Python) compared to Noda Time.
         if value < 0:
             value = -value
             output_buffer.append("-")
         output_buffer.append(f"{value:04}")
 
     @classmethod
-    def left_pad(cls, value: int, length: int, output_buffer: StringBuilder) -> None:
+    def _left_pad(cls, value: int, length: int, output_buffer: StringBuilder) -> None:
         """Formats the given value left padded with zeros.
 
         Left pads with zeros the value into a field of ``length`` characters. If the value
         is longer than ``length``, the entire value is formatted. If the value is negative,
         it is preceded by "-" but this does not count against the length.
 
         :param value: The value to format.
         :param length: The length to fill.
         :param output_buffer: The output buffer to add the digits to.
         :return:
         """
         # TODO: Preconditions.DebugCheckArgumentRange(nameof(length), length, 1, MaximumPaddingLength);
         # TODO: unchecked
         if value >= 0:
-            cls.left_pad_non_negative(value, length, output_buffer)
+            cls._left_pad_non_negative(value, length, output_buffer)
             return
         output_buffer.append("-")
         # Special case, as we can't use Math.Abs.
         if value == _CsharpConstants.INT_MIN_VALUE:
             if length > 10:
                 output_buffer.append("000000"[16 - length :])
             output_buffer.append("2147483648")
             return
-        cls.left_pad_non_negative(-value, length, output_buffer)
+        cls._left_pad_non_negative(-value, length, output_buffer)
 
     @staticmethod
-    def left_pad_non_negative(value: int, length: int, output_buffer: StringBuilder) -> None:
+    def _left_pad_non_negative(value: int, length: int, output_buffer: StringBuilder) -> None:
         """Formats the given value left padded with zeros. The value is assumed to be non-negative.
 
         Left pads with zeros the value into a field of ``length`` characters. If the value
         is longer than ``length``, the entire value is formatted. If the value is negative,
         it is preceded by "-" but this does not count against the length.
 
         :param value: The value to format.
@@ -151,7 +151,17 @@
 
         if relevant_length > 0:
             formatted_string = f"{relevant_digits:0{relevant_length}d}"
             output_buffer.append(formatted_string)
         # Check and remove a preceding decimal point if necessary
         elif output_buffer.length > 0 and output_buffer[output_buffer.length - 1] == ".":
             output_buffer.length -= 1
+
+    @classmethod
+    def _format_invariant(cls, value: int, output_buffer: StringBuilder) -> None:
+        """Formats the given value using the invariant culture, with no truncation or padding.
+
+        :param value: The value to format.
+        :param output_buffer: The output buffer to add the digits to.
+        """
+        # TODO: This is very, very different from the Noda Time implementation
+        output_buffer.append(str(value))
```

### Comparing `pyoda_time-0.7.1/pyoda_time/text/_i_partial_pattern.py` & `pyoda_time-0.8.0/pyoda_time/text/_i_partial_pattern.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/text/_i_pattern.py` & `pyoda_time-0.8.0/pyoda_time/text/_i_pattern.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/text/_instant_pattern.py` & `pyoda_time-0.8.0/pyoda_time/text/_instant_pattern.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 
 @final
 @_sealed
 @_private
 class InstantPattern(IPattern[Instant], metaclass=__CombinedMeta):
     """Represents a pattern for parsing and formatting ``Instant`` values."""
 
-    __DEFAULT_TEMPLATE_VALUE: Final[Instant] = Instant.from_utc(2000, 1, 1, 0, 0)
+    _DEFAULT_TEMPLATE_VALUE: Final[Instant] = Instant.from_utc(2000, 1, 1, 0, 0)
 
     __pattern: IPattern[Instant]
     __pattern_text: str
     __template_value: Instant
     __two_digit_year_max: int
     __format_info: _PyodaFormatInfo
 
@@ -160,15 +160,15 @@
         :param pattern_text: Pattern text to create the pattern for
         :param culture_info: The culture to use in the pattern
         :return: A pattern for parsing and formatting instants.
         """
         return cls.__create(
             pattern_text,
             _PyodaFormatInfo._get_format_info(culture_info),
-            cls.__DEFAULT_TEMPLATE_VALUE,
+            cls._DEFAULT_TEMPLATE_VALUE,
             LocalDatePattern._DEFAULT_TWO_DIGIT_YEAR_MAX,
         )
 
     @classmethod
     def create_with_current_culture(cls, pattern_text: str) -> InstantPattern:
         """Creates a pattern for the given pattern text in the current thread's current culture.
 
@@ -178,15 +178,15 @@
 
         :param pattern_text: Pattern text to create the pattern for
         :return: A pattern for parsing and formatting instants.
         """
         return cls.__create(
             pattern_text,
             _PyodaFormatInfo.current_info,
-            cls.__DEFAULT_TEMPLATE_VALUE,
+            cls._DEFAULT_TEMPLATE_VALUE,
             LocalDatePattern._DEFAULT_TWO_DIGIT_YEAR_MAX,
         )
 
     @classmethod
     def create_with_invariant_culture(cls, pattern_text: str) -> InstantPattern:
         """Creates a pattern for the given pattern text in the invariant culture.
 
@@ -194,15 +194,15 @@
 
         :param pattern_text: Pattern text to create the pattern for
         :return: A pattern for parsing and formatting instants.
         """
         return cls.__create(
             pattern_text,
             _PyodaFormatInfo.invariant_info,
-            cls.__DEFAULT_TEMPLATE_VALUE,
+            cls._DEFAULT_TEMPLATE_VALUE,
             LocalDatePattern._DEFAULT_TWO_DIGIT_YEAR_MAX,
         )
 
     def __with_format_info(self, format_info: _PyodaFormatInfo) -> InstantPattern:
         """Creates a pattern for the same original pattern text as this pattern, but with the specified localization
         information.
```

### Comparing `pyoda_time-0.7.1/pyoda_time/text/_instant_pattern_parser.py` & `pyoda_time-0.8.0/pyoda_time/text/_instant_pattern_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
     Supported standard patterns:
         * g: general; the UTC ISO-8601 instant in the style uuuu-MM-ddTHH:mm:ssZ
     """
 
     __GENERAL_PATTERN_TEXT: Final[str] = "uuuu'-'MM'-'dd'T'HH':'mm':'ss'Z'"
     _BEFORE_MIN_VALUE_TEXT: Final[str] = "StartOfTime"
-    _AFTER_MIN_VALUE_TEXT: Final[str] = "EndOfTime"
+    _AFTER_MAX_VALUE_TEXT: Final[str] = "EndOfTime"
 
     __local_template_value: LocalDateTime
     __two_digit_year_max: int
 
     @classmethod
     def _ctor(cls, template_value: Instant, two_digit_year_max: int) -> _InstantPatternParser:
         self = super().__new__(cls)
@@ -77,15 +77,15 @@
         def format(self, value: Instant) -> str:
             # We don't need to be able to parse before-min/after-max values, but it's convenient to be
             # able to format them - mostly for the sake of testing (but also for ZoneInterval).
             if value._is_valid:
                 return self.__pattern.format(value.in_utc().local_date_time)
             if value == Instant._before_min_value():
                 return _InstantPatternParser._BEFORE_MIN_VALUE_TEXT
-            return _InstantPatternParser._AFTER_MIN_VALUE_TEXT
+            return _InstantPatternParser._AFTER_MAX_VALUE_TEXT
 
         def append_format(self, value: Instant, builder: StringBuilder) -> StringBuilder:
             return self.__pattern.append_format(value.in_utc().local_date_time, builder)
 
         def parse(self, text: str) -> ParseResult[Instant]:
             def to_instant(value: LocalDateTime) -> Instant:
                 return Instant._ctor(days=value.date._days_since_epoch, nano_of_day=value.nanosecond_of_day)
```

### Comparing `pyoda_time-0.7.1/pyoda_time/text/_invalid_pattern_exception.py` & `pyoda_time-0.8.0/pyoda_time/text/_invalid_pattern_exception.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/text/_local_date_pattern.py` & `pyoda_time-0.8.0/pyoda_time/text/_local_date_pattern.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/text/_local_date_pattern_parser.py` & `pyoda_time-0.8.0/pyoda_time/text/_local_date_pattern_parser.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/text/_local_date_time_pattern.py` & `pyoda_time-0.8.0/pyoda_time/text/_local_date_time_pattern.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/text/_local_date_time_pattern_parser.py` & `pyoda_time-0.8.0/pyoda_time/text/_local_date_time_pattern_parser.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/text/_local_time_pattern.py` & `pyoda_time-0.8.0/pyoda_time/text/_local_time_pattern.py`

 * *Files 4% similar despite different names*

```diff
@@ -144,32 +144,33 @@
                     if self.__hour_minute_iso_pattern_impl is None:
                         self.__hour_minute_iso_pattern_impl = LocalTimePattern.create_with_invariant_culture("HH':'mm")
             return self.__hour_minute_iso_pattern_impl
 
         @property
         def _variable_precision_iso_pattern_impl(self) -> IPattern[LocalTime]:
             if self.__variable_precision_iso_pattern_impl is None:
+                # Declared outside of the lock being acquired because the properties
+                # it contains *also* try to acquire the lock.
+                patterns = [
+                    self._extended_iso_pattern_impl,
+                    self._hour_minute_iso_pattern_impl,
+                    self._hour_iso_pattern_impl,
+                ]
                 with self.__lock:
                     if self.__variable_precision_iso_pattern_impl is None:
 
                         def format_predicate_for_extended_iso_pattern(time: LocalTime) -> bool:
                             return True
 
                         def format_predicate_for_hour_minute_iso_pattern(time: LocalTime) -> bool:
                             return time.second == 0 and time.nanosecond_of_second == 0
 
                         def format_predicate_for_hour_iso_pattern(time: LocalTime) -> bool:
                             return time.minute == 0 and time.second == 0 and time.nanosecond_of_second == 0
 
-                        patterns = [
-                            self._extended_iso_pattern_impl,
-                            self._hour_minute_iso_pattern_impl,
-                            self._hour_iso_pattern_impl,
-                        ]
-
                         format_predicates = [
                             format_predicate_for_extended_iso_pattern,
                             format_predicate_for_hour_minute_iso_pattern,
                             format_predicate_for_hour_iso_pattern,
                         ]
 
                         self.__variable_precision_iso_pattern_impl = CompositePatternBuilder(
```

### Comparing `pyoda_time-0.7.1/pyoda_time/text/_local_time_pattern_parser.py` & `pyoda_time-0.8.0/pyoda_time/text/_local_time_pattern_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,23 @@
 from pyoda_time.text.patterns._pattern_cursor import _PatternCursor
 from pyoda_time.text.patterns._pattern_fields import _PatternFields
 from pyoda_time.text.patterns._stepped_pattern_builder import _SteppedPatternBuilder
 from pyoda_time.text.patterns._time_pattern_helper import _TimePatternHelper
 from pyoda_time.utility._csharp_compatibility import _csharp_modulo, _private, _sealed, _towards_zero_division
 
 
+def hours_12_getter(value: LocalTime) -> int:
+    return value.clock_hour_of_half_day
+
+
+def hours_12_setter(bucket: _ParseBucket[LocalTime], value: int) -> None:
+    assert isinstance(bucket, _LocalTimePatternParser._LocalTimeParseBucket)
+    bucket._hours_12 = value
+
+
 def hours_24_getter(value: LocalTime) -> int:
     return value.hour
 
 
 def hours_24_setter(bucket: _ParseBucket[LocalTime], value: int) -> None:
     assert isinstance(bucket, _LocalTimePatternParser._LocalTimeParseBucket)
     bucket._hours_24 = value
@@ -43,14 +52,19 @@
 
 
 def seconds_setter(bucket: _ParseBucket[LocalTime], value: int) -> None:
     assert isinstance(bucket, _LocalTimePatternParser._LocalTimeParseBucket)
     bucket._seconds = value
 
 
+def am_pm_setter(bucket: _ParseBucket[LocalTime], value: int) -> None:
+    assert isinstance(bucket, _LocalTimePatternParser._LocalTimeParseBucket)
+    bucket._am_pm = value
+
+
 def nanosecond_of_second_getter(value: LocalTime) -> int:
     return value.nanosecond_of_second
 
 
 def fractional_seconds_setter(bucket: _ParseBucket[LocalTime], value: int) -> None:
     assert isinstance(bucket, _LocalTimePatternParser._LocalTimeParseBucket)
     bucket._fractional_seconds = value
@@ -70,34 +84,36 @@
     """Pattern parser for ``LocalTime`` values."""
 
     __template_value: LocalTime
 
     __pattern_character_handlers: Final[
         Mapping[str, Callable[[_PatternCursor, _SteppedPatternBuilder[LocalTime]], None]]
     ] = {
-        "%": lambda _, __: exec("raise NotImplementedError"),
-        "'": lambda _, __: exec("raise NotImplementedError"),
-        '"': lambda _, __: exec("raise NotImplementedError"),
-        "\\": lambda _, __: exec("raise NotImplementedError"),
+        "%": _SteppedPatternBuilder._handle_percent,
+        "'": _SteppedPatternBuilder._handle_quote,
+        '"': _SteppedPatternBuilder._handle_quote,
+        "\\": _SteppedPatternBuilder._handle_backslash,
         ".": _TimePatternHelper._create_period_handler(9, nanosecond_of_second_getter, fractional_seconds_setter),
-        ";": lambda _, __: exec("raise NotImplementedError"),
+        ";": _TimePatternHelper._create_comma_dot_handler(9, nanosecond_of_second_getter, fractional_seconds_setter),
         ":": _handle_colon,
-        "h": lambda _, __: exec("raise NotImplementedError"),
+        "h": _SteppedPatternBuilder._handle_padded_field(
+            2, _PatternFields.HOURS_12, 1, 12, hours_12_getter, hours_12_setter, LocalTime
+        ),
         "H": _SteppedPatternBuilder._handle_padded_field(
             2, _PatternFields.HOURS_24, 0, 23, hours_24_getter, hours_24_setter, LocalTime
         ),
         "m": _SteppedPatternBuilder._handle_padded_field(
             2, _PatternFields.MINUTES, 0, 59, minutes_getter, minutes_setter, LocalTime
         ),
         "s": _SteppedPatternBuilder._handle_padded_field(
             2, _PatternFields.SECONDS, 0, 59, seconds_getter, seconds_setter, LocalTime
         ),
-        "f": lambda _, __: exec("raise NotImplementedError"),
-        "F": lambda _, __: exec("raise NotImplementedError"),
-        "t": lambda _, __: exec("raise NotImplementedError"),
+        "f": _TimePatternHelper._create_fraction_handler(9, nanosecond_of_second_getter, fractional_seconds_setter),
+        "F": _TimePatternHelper._create_fraction_handler(9, nanosecond_of_second_getter, fractional_seconds_setter),
+        "t": _TimePatternHelper._create_am_pm_handler(hours_24_getter, am_pm_setter),
     }
 
     @classmethod
     def _ctor(cls, template_value: LocalTime) -> _LocalTimePatternParser:
         self = super().__new__(cls)
         self.__template_value = template_value
         return self
```

### Comparing `pyoda_time-0.7.1/pyoda_time/text/_offset_pattern.py` & `pyoda_time-0.8.0/pyoda_time/text/_offset_pattern.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/text/_offset_pattern_parser.py` & `pyoda_time-0.8.0/pyoda_time/text/_offset_pattern_parser.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/text/_parse_bucket.py` & `pyoda_time-0.8.0/pyoda_time/text/_parse_bucket.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/text/_parse_result.py` & `pyoda_time-0.8.0/pyoda_time/text/_parse_result.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/text/_text_cursor.py` & `pyoda_time-0.8.0/pyoda_time/text/_text_cursor.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/text/_text_error_messages.py` & `pyoda_time-0.8.0/pyoda_time/text/_text_error_messages.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/text/_value_cursor.py` & `pyoda_time-0.8.0/pyoda_time/text/_value_cursor.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/text/patterns/_date_pattern_helper.py` & `pyoda_time-0.8.0/pyoda_time/text/patterns/_date_pattern_helper.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/text/patterns/_i_pattern_parser.py` & `pyoda_time-0.8.0/pyoda_time/text/patterns/_i_pattern_parser.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/text/patterns/_pattern_bcl_support.py` & `pyoda_time-0.8.0/pyoda_time/text/patterns/_pattern_bcl_support.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/text/patterns/_pattern_cursor.py` & `pyoda_time-0.8.0/pyoda_time/text/patterns/_pattern_cursor.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/text/patterns/_pattern_fields.py` & `pyoda_time-0.8.0/pyoda_time/text/patterns/_pattern_fields.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/text/patterns/_stepped_pattern_builder.py` & `pyoda_time-0.8.0/pyoda_time/text/patterns/_stepped_pattern_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from ..._compatibility._string_builder import StringBuilder
 from ..._local_date import LocalDate
 from ..._local_date_time import LocalDateTime
 from ..._local_time import LocalTime
 from ...globalization._pyoda_format_info import _PyodaFormatInfo
 from ...utility._csharp_compatibility import _sealed
 from ...utility._preconditions import _Preconditions
-from .._format_helper import FormatHelper
+from .._format_helper import _FormatHelper
 from .._i_partial_pattern import _IPartialPattern
 from .._invalid_pattern_exception import InvalidPatternError
 from .._local_time_pattern import LocalTimePattern
 from .._parse_result import ParseResult
 from .._text_error_messages import _TextErrorMessages
 from ._pattern_cursor import _PatternCursor
 from ._pattern_fields import _PatternFields
@@ -436,39 +436,39 @@
         :param selector: The selector function to apply to obtain a value to format
         :param assume_non_negative: Whether it is safe to assume the value will be non-negative
         :param assume_fits_in_count: Whether it is safe to assume the value will not exceed the specified length
         """
         if count == 2 and assume_non_negative and assume_fits_in_count:
 
             def format_action(value: TResult, sb: StringBuilder) -> None:
-                FormatHelper.format_2_digits_non_negative(selector(value), sb)
+                _FormatHelper._format_2_digits_non_negative(selector(value), sb)
         elif count == 4 and assume_fits_in_count:
 
             def format_action(value: TResult, sb: StringBuilder) -> None:
-                FormatHelper.format_4_digits_value_fits(selector(value), sb)
+                _FormatHelper._format_4_digits_value_fits(selector(value), sb)
         elif assume_non_negative:
 
             def format_action(value: TResult, sb: StringBuilder) -> None:
-                FormatHelper.left_pad_non_negative(selector(value), count, sb)
+                _FormatHelper._left_pad_non_negative(selector(value), count, sb)
         else:
 
             def format_action(value: TResult, sb: StringBuilder) -> None:
-                FormatHelper.left_pad(selector(value), count, sb)
+                _FormatHelper._left_pad(selector(value), count, sb)
 
         self._add_format_action(format_action)
 
     def _add_format_fraction(self, width: int, scale: int, selector: Callable[[TResult], int]) -> None:
         def format_action(value: TResult, sb: StringBuilder) -> None:
-            FormatHelper._append_fraction(selector(value), width, scale, sb)
+            _FormatHelper._append_fraction(selector(value), width, scale, sb)
 
         self._add_format_action(format_action)
 
     def _add_format_fraction_truncate(self, width: int, scale: int, selector: Callable[[TResult], int]) -> None:
         def format_action(value: TResult, sb: StringBuilder) -> None:
-            FormatHelper._append_fraction_truncate(selector(value), width, scale, sb)
+            _FormatHelper._append_fraction_truncate(selector(value), width, scale, sb)
 
         self._add_format_action(format_action)
 
     def _add_embedded_local_partial(
         self,
         pattern: _PatternCursor,
         date_bucket_extractor: Callable[[_ParseBucket[TResult]], _LocalDatePatternParser._LocalDateParseBucket],
```

### Comparing `pyoda_time-0.7.1/pyoda_time/text/patterns/_time_pattern_helper.py` & `pyoda_time-0.8.0/pyoda_time/text/patterns/_time_pattern_helper.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from pyoda_time._compatibility._string_builder import StringBuilder
 from pyoda_time.text import ParseResult
 from pyoda_time.text._parse_bucket import _ParseBucket
 from pyoda_time.text._value_cursor import _ValueCursor
 from pyoda_time.text.patterns._pattern_cursor import _PatternCursor
 from pyoda_time.text.patterns._pattern_fields import _PatternFields
 from pyoda_time.text.patterns._stepped_pattern_builder import _SteppedPatternBuilder
+from pyoda_time.utility._csharp_compatibility import _towards_zero_division
 
 T = TypeVar("T")
 
 
 class _TimePatternHelper:
     """Common methods used when parsing dates.
 
@@ -261,8 +262,26 @@
         count: int,
         specified_designator: str,
         specified_designator_value: int,
         hour_of_day_getter: Callable[[T], int],
         am_pm_setter: Callable[[_ParseBucket[T], int], None],
         builder: _SteppedPatternBuilder[T],
     ) -> None:
-        raise NotImplementedError
+        if count == 1:
+            specified_designator = specified_designator[0]
+
+        def parse_action(cursor: _ValueCursor, bucket: _ParseBucket[T]) -> ParseResult[T] | None:
+            value: int = (
+                specified_designator_value
+                if cursor._match_case_insensitive(specified_designator, True)
+                else 1 - specified_designator_value
+            )
+            am_pm_setter(bucket, value)
+            return None
+
+        def format_action(value: T, sb: StringBuilder) -> None:
+            # Only append anything if it's the non-empty designator.
+            if _towards_zero_division(hour_of_day_getter(value), 12) == specified_designator_value:
+                sb.append(specified_designator)
+
+        builder._add_parse_action(parse_action)
+        builder._add_format_action(format_action)
```

### Comparing `pyoda_time-0.7.1/pyoda_time/time_zones/_i_zone_interval_map.py` & `pyoda_time-0.8.0/pyoda_time/time_zones/_i_zone_interval_map.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/time_zones/_tzdb_zone_1970_location.py` & `pyoda_time-0.8.0/pyoda_time/time_zones/_tzdb_zone_1970_location.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/time_zones/_tzdb_zone_location.py` & `pyoda_time-0.8.0/pyoda_time/time_zones/_tzdb_zone_location.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/time_zones/_zone_interval.py` & `pyoda_time-0.8.0/pyoda_time/time_zones/_zone_interval.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,17 +142,18 @@
         # Do not expose these defaults in the __init__ signature.
         if start is None:
             start = Instant._before_min_value()
         if end is None:
             end = Instant._after_max_value()
 
         _Preconditions._check_not_null(name, "name")
-        _Preconditions._check_argument(
-            start < end, "start", f"The start Instant must be less than the end Instant. start: {start}; end: {end}"
-        )
+        if start >= end:  # Needed to prevent infinite recursion calling Instant.__repr__
+            _Preconditions._check_argument(
+                start < end, "start", f"The start Instant must be less than the end Instant. start: {start}; end: {end}"
+            )
         self.__name: Final[str] = name
         self.__raw_start: Final[Instant] = start
         self.__raw_end: Final[Instant] = end
         self.__wall_offset: Final[Offset] = wall_offset
         self.__savings: Final[Offset] = savings
         # Work out the corresponding local instants, taking care to "go infinite" appropriately.
         self.__local_start: Final[_LocalInstant] = start._safe_plus(wall_offset)
@@ -183,14 +184,15 @@
     def __contains__(self, instant: Instant) -> bool:
         """Determines whether this period contains the given Instant in its range."""
         # Implementation of ``public bool Contains(Instant instant)``
         return self._raw_start <= instant < self._raw_end
 
     def _contains(self, local_instant: _LocalInstant) -> bool:
         """Determines whether this period contains the given LocalInstant in its range."""
+        # TODO: why is this not implemented in __contains__ above?
         # Implementation of ``internal bool Contains(LocalInstant localInstant)``
         return self.__local_start <= local_instant < self.__local_end
 
     def _equal_ignore_bounds(self, other: ZoneInterval) -> bool:
         """Returns whether this zone interval has the same offsets and name as another."""
         # TODO: Preconditions.DebugCheckNotNull(other, nameof(other));
         return other.wall_offset == self.wall_offset and other.savings == self.savings
```

### Comparing `pyoda_time-0.7.1/pyoda_time/time_zones/cldr/_map_zone.py` & `pyoda_time-0.8.0/pyoda_time/time_zones/cldr/_map_zone.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/time_zones/cldr/_windows_zones.py` & `pyoda_time-0.8.0/pyoda_time/time_zones/cldr/_windows_zones.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/time_zones/io/_date_time_zone_reader.py` & `pyoda_time-0.8.0/pyoda_time/time_zones/io/_date_time_zone_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,15 +138,20 @@
     def read_dictionary(self) -> dict[str, str]:
         """Reads a string to string dictionary value from the stream.
 
         The value must have been written by ``_DateTimeZoneWriter.write_dictionary``.
 
         :return: The ``dict[TKey,TValue]`` value from the stream.
         """
-        results = {self.read_string(): self.read_string() for _ in range(self.read_count())}
+        results = {}
+        count = self.read_count()
+        for _ in range(count):
+            key = self.read_string()
+            value = self.read_string()
+            results[key] = value
         return results
 
     def read_zone_interval_transition(self, previous: Instant | None) -> Instant:
         """Reads an instant representing a zone interval transition from the stream.
 
         The value must have been written by ``_DateTimeZoneWriter.write_zone_interval_transition``.
```

### Comparing `pyoda_time-0.7.1/pyoda_time/time_zones/io/_date_time_zone_writer.py` & `pyoda_time-0.8.0/pyoda_time/time_zones/io/_date_time_zone_writer.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/time_zones/io/_i_date_time_zone_reader.py` & `pyoda_time-0.8.0/pyoda_time/time_zones/io/_i_date_time_zone_reader.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/time_zones/io/_i_date_time_zone_writer.py` & `pyoda_time-0.8.0/pyoda_time/time_zones/io/_i_date_time_zone_writer.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/time_zones/io/_tzdb_stream_data.py` & `pyoda_time-0.8.0/pyoda_time/time_zones/io/_tzdb_stream_data.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # Copyright 2024 The Pyoda Time Authors. All rights reserved.
 # Use of this source code is governed by the Apache License 2.0,
 # as found in the LICENSE.txt file.
 from __future__ import annotations
 
-import io
 import struct
 import types
 from typing import Any, BinaryIO, Callable, Final, Sequence, TypeVar, final
 
+from pyoda_time import DateTimeZone
 from pyoda_time.time_zones import TzdbZoneLocation
+from pyoda_time.time_zones._cached_date_time_zone import _CachedDateTimeZone
+from pyoda_time.time_zones._fixed_date_time_zone import _FixedDateTimeZone
+from pyoda_time.time_zones._precalculated_date_time_zone import _PrecalculatedDateTimeZone
 from pyoda_time.time_zones._tzdb_zone_1970_location import TzdbZone1970Location
 from pyoda_time.time_zones.cldr import WindowsZones
 from pyoda_time.time_zones.io._date_time_zone_reader import _DateTimeZoneReader
+from pyoda_time.time_zones.io._date_time_zone_writer import _DateTimeZoneWriter
 from pyoda_time.time_zones.io._tzdb_stream_field import _TzdbStreamField
 from pyoda_time.time_zones.io._tzdb_stream_field_id import _TzdbStreamFieldId
 from pyoda_time.utility import InvalidPyodaDataError
 from pyoda_time.utility._csharp_compatibility import _sealed
 from pyoda_time.utility._preconditions import _Preconditions
 
 T = TypeVar("T")
@@ -116,40 +120,85 @@
     __ACCEPTED_VERSION: Final[int] = 0
 
     @property
     def tzdb_version(self) -> str:
         """Returns the TZDB version string."""
         return self.__tzdb_version
 
+    @property
+    def tzdb_id_map(self) -> types.MappingProxyType[str, str]:
+        """Returns the TZDB ID dictionary (alias to canonical ID)."""
+        return self.__tzdb_id_map
+
+    @property
+    def windows_mapping(self) -> WindowsZones:
+        """Returns the Windows mapping dictionary.
+
+        (As the type is immutable, it can be exposed directly to callers.)
+        """
+        return self.__windows_mapping
+
+    @property
+    def zone_locations(self) -> Sequence[TzdbZoneLocation] | None:
+        """Returns the zone locations for the source, or null if no location data is available."""
+        return self.__zone_locations
+
+    @property
+    def zone_1970_locations(self) -> Sequence[TzdbZone1970Location] | None:
+        """Returns the "zone 1970" locations for the source, or null if no such location data is available."""
+        return self.__zone_1970_locations
+
     def __init__(self, builder: _Builder) -> None:
         self.__string_pool: Sequence[str] = self._check_not_null(builder._string_pool, "string pool")
         mutable_id_map = self._check_not_null(builder._tzdb_id_map, "TZDB alias map")
         self.__tzdb_version = self._check_not_null(builder._tzdb_version, "TZDB version")
         self.__windows_mapping = self._check_not_null(builder._windows_mapping, "CLDR Supplemental Windows Zones")
         self.__zone_fields = builder._zone_fields
         self.__zone_locations = builder._zone_locations
         self.__zone_1970_locations = builder._zone_1970_locations
 
         # Add in the canonical IDs as mappings to themselves
         for zone_id in self.__zone_fields:
             mutable_id_map[zone_id] = zone_id
-        self.__tzdb_id_map = types.MappingProxyType(mutable_id_map)
+        self.__tzdb_id_map: types.MappingProxyType[str, str] = types.MappingProxyType(mutable_id_map)
+
+    def create_zone(self, id_: str, canonical_id: str) -> DateTimeZone:
+        """Creates the ``DateTimeZone`` for the given canonical ID, which will definitely be one of the values of the
+        TzdbAliases dictionary.
+
+        :param id_: ID for the returned zone, which may be an alias.
+        :param canonical_id: Canonical ID for zone data
+        :return: The created ``DateTimeZone`` for the given ID.
+        """
+        _Preconditions._check_not_null(id_, "id_")
+        _Preconditions._check_not_null(canonical_id, "canonical_id")
+        with self.__zone_fields[canonical_id]._create_stream() as stream:
+            reader = _DateTimeZoneReader._ctor(stream, self.__string_pool)
+            # Skip over the ID before the zone data itself
+            reader.read_string()
+            type_ = _DateTimeZoneWriter._DateTimeZoneType(reader.read_byte())
+            match type_:
+                case _DateTimeZoneWriter._DateTimeZoneType.FIXED:
+                    return _FixedDateTimeZone.read(reader, id_)
+                case _DateTimeZoneWriter._DateTimeZoneType.PRECALCULATED:
+                    return _CachedDateTimeZone._for_zone(_PrecalculatedDateTimeZone._read(reader, id_))
+                case _:
+                    raise InvalidPyodaDataError(f"Unknown time zone type {type_.name}")
 
     @staticmethod
     def _check_not_null(input_: T | None, name: str) -> T:
         if input_ is None:
             raise InvalidPyodaDataError(f"Incomplete TZDB data. Missing field: {name}")
         return input_
 
     @classmethod
     def _from_stream(cls, stream: BinaryIO) -> _TzdbStreamData:
         _Preconditions._check_not_null(stream, "stream")
 
-        with io.BytesIO(stream.read()) as reader:
-            version = struct.unpack("i", reader.read(4))[0]
+        version = struct.unpack("i", stream.read(4))[0]
         if version != cls.__ACCEPTED_VERSION:
             raise InvalidPyodaDataError(f"Unable to read stream with version {version}")
 
         builder = cls._Builder()
         for field in _TzdbStreamField._read_fields(stream):
             handler = cls.__FIELD_HANDLERS.get(field.id)
             if handler:
```

### Comparing `pyoda_time-0.7.1/pyoda_time/time_zones/io/_tzdb_stream_field.py` & `pyoda_time-0.8.0/pyoda_time/time_zones/io/_tzdb_stream_field.py`

 * *Files 6% similar despite different names*

```diff
@@ -43,16 +43,18 @@
         self, reader_function: Callable[[_DateTimeZoneReader], T], string_pool: Sequence[str] | None
     ) -> T:
         with self._create_stream() as stream:
             return reader_function(_DateTimeZoneReader._ctor(stream, string_pool))
 
     @classmethod
     def _read_fields(cls, stream: BinaryIO) -> Generator[_TzdbStreamField, None, None]:
-        field_id = stream.read(1)
-        if field_id:
+        while True:
+            field_id = stream.read(1)
+            if not field_id:
+                break
             id_ = _TzdbStreamFieldId(field_id[0])
             # Read 7-bit encoded length
             length = _DateTimeZoneReader._ctor(stream, None).read_count()
             data = bytearray()
             for offset in range(length):
                 bytes_read: bytes = stream.read(1)
                 if not bytes_read:
```

### Comparing `pyoda_time-0.7.1/pyoda_time/time_zones/io/_tzdb_stream_field_id.py` & `pyoda_time-0.8.0/pyoda_time/time_zones/io/_tzdb_stream_field_id.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/utility/_cache.py` & `pyoda_time-0.8.0/pyoda_time/utility/_cache.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/utility/_csharp_compatibility.py` & `pyoda_time-0.8.0/pyoda_time/utility/_csharp_compatibility.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,21 +2,26 @@
 # Use of this source code is governed by the Apache License 2.0,
 # as found in the LICENSE.txt file.
 
 from __future__ import annotations
 
 import datetime
 import decimal
-from typing import Any, Final, Literal, TypeVar
+from collections import defaultdict
+from collections.abc import Mapping
+from types import MappingProxyType
+from typing import Any, Final, Literal, Sequence, TypeVar
 
 __all__: list[str] = []
 
 SEALED_CLASSES: Final[list[type]] = []
 _T = TypeVar("_T")
 _Ttype = TypeVar("_Ttype", bound=type)
+_TKey = TypeVar("_TKey")
+_TValue = TypeVar("_TValue")
 
 
 def _as_span(text: str | None, start: int) -> str:
     """Roughly equivalent to:
     public static ReadOnlySpan<char> AsSpan(this string? text, int start)
     """
     if text is None:
@@ -40,14 +45,23 @@
 
 def _to_ticks(dt: datetime.datetime) -> int:
     """Get a value akin to C#'s DateTime.Ticks property from a python datetime."""
     # Gratefully stolen from https://stackoverflow.com/a/29368771
     return int((dt - datetime.datetime(1, 1, 1, tzinfo=datetime.timezone.utc)).total_seconds() * 10000000)
 
 
+def _to_lookup(mapping: Mapping[_TKey, _TValue]) -> MappingProxyType[_TValue, Sequence[_TKey]]:
+    """Produces a mapping of value->keys, aking to the `.ToLookup()` in dotnet."""
+    # TODO: Make this work for other collections, not just dict.
+    lookup = defaultdict(list)
+    for k, v in mapping.items():
+        lookup[v].append(k)
+    return MappingProxyType(lookup)
+
+
 def _sealed(cls: _Ttype) -> _Ttype:
     """Prevents the decorated class from being subclassed.
 
     This is intended to loosely emulate the behaviour of the ``sealed`` keyword in C#.
     Its use should be accompanied by the ``typing.final`` decorator to aid static analysis.
     """
```

### Comparing `pyoda_time-0.7.1/pyoda_time/utility/_hash_code_helper.py` & `pyoda_time-0.8.0/pyoda_time/utility/_hash_code_helper.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/utility/_preconditions.py` & `pyoda_time-0.8.0/pyoda_time/utility/_preconditions.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyoda_time/utility/_tick_arithmetic.py` & `pyoda_time-0.8.0/pyoda_time/utility/_tick_arithmetic.py`

 * *Files identical despite different names*

### Comparing `pyoda_time-0.7.1/pyproject.toml` & `pyoda_time-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 warn_return_any = true
 warn_unreachable = true
 warn_unused_configs = true
 warn_unused_ignores = true
 
 [tool.poetry]
 name = "pyoda-time"
-version = "0.7.1"
+version = "0.8.0"
 description = "An alternative datetime library for Python."
 authors = ["Christopher McEvoy <12284065+chrisimcevoy@users.noreply.github.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://pyodatime.org/"
 repository = "https://github.com/chrisimcevoy/pyoda-time"
 classifiers = [
@@ -46,19 +46,19 @@
 
 [tool.poetry.dependencies]
 python = "^3.12"
 pyicu = "^2.12"
 
 [tool.poetry.group.dev.dependencies]
 pytest = ">=7.4.3,<9.0.0"
-pytz = ">=2023.3,<2025.0"
 pre-commit = "^3.5.0"
 coverage = "^7.3.2"
 sphinx = "^7.2.6"
 pytest-xdist = "^3.6.1"
+pytest-cov = "^5.0.0"
 
 [tool.ruff]
 line-length = 120
 
 [tool.ruff.lint]
 # Allow fix for all enabled rules (when `--fix`) is provided.
 fixable = ["ALL"]
```

### Comparing `pyoda_time-0.7.1/PKG-INFO` & `pyoda_time-0.8.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoda-time
-Version: 0.7.1
+Version: 0.8.0
 Summary: An alternative datetime library for Python.
 Home-page: https://pyodatime.org/
 License: Apache-2.0
 Author: Christopher McEvoy
 Author-email: 12284065+chrisimcevoy@users.noreply.github.com
 Requires-Python: >=3.12,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -19,14 +19,15 @@
 Description-Content-Type: text/markdown
 
 ![PyPI - Status](https://img.shields.io/pypi/status/pyoda-time)
 ![PyPI - Version](https://img.shields.io/pypi/v/pyoda-time)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pyoda-time)
 ![GitHub License](https://img.shields.io/github/license/chrisimcevoy/pyoda-time)
 [![Documentation Status](https://readthedocs.org/projects/pyoda-time/badge/?version=latest)](https://pyoda-time.readthedocs.io/en/latest/?badge=latest)
+[![codecov](https://codecov.io/github/chrisimcevoy/pyoda-time/graph/badge.svg?token=I1QQES7AVT)](https://codecov.io/github/chrisimcevoy/pyoda-time)
 
 # Pyoda Time
 
 Pyoda Time is an alternative date and time API for Python. 
 
 It helps you to think about your data more clearly, and express operations on that data more precisely.
```

