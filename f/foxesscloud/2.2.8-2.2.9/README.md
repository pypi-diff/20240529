# Comparing `tmp/foxesscloud-2.2.8.tar.gz` & `tmp/foxesscloud-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "F:\python\FoxESS-Cloud\dist\.tmp-3l5j7lb9\foxesscloud-2.2.8.tar", last modified: Mon May 27 13:12:26 2024, max compression
+gzip compressed data, was "F:\python\FoxESS-Cloud\dist\.tmp-8pnoxowr\foxesscloud-2.2.9.tar", last modified: Tue May 28 11:39:43 2024, max compression
```

## Comparing `foxesscloud-2.2.8.tar` & `foxesscloud-2.2.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-27 13:12:26.000000 foxesscloud-2.2.8/
--rw-rw-rw-   0        0        0     1074 2023-08-27 11:13:04.000000 foxesscloud-2.2.8/LICENCE
--rw-rw-rw-   0        0        0    42891 2024-05-27 13:12:26.000000 foxesscloud-2.2.8/PKG-INFO
--rw-rw-rw-   0        0        0    42336 2024-05-27 11:55:42.000000 foxesscloud-2.2.8/README.md
--rw-rw-rw-   0        0        0      635 2024-05-24 13:57:33.000000 foxesscloud-2.2.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-27 13:12:26.000000 foxesscloud-2.2.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-27 13:12:26.000000 foxesscloud-2.2.8/src/
-drwxrwxrwx   0        0        0        0 2024-05-27 13:12:26.000000 foxesscloud-2.2.8/src/foxesscloud/
--rw-rw-rw-   0        0        0   182371 2024-05-27 12:04:52.000000 foxesscloud-2.2.8/src/foxesscloud/foxesscloud.py
--rw-rw-rw-   0        0        0   176693 2024-05-27 12:04:52.000000 foxesscloud-2.2.8/src/foxesscloud/openapi.py
-drwxrwxrwx   0        0        0        0 2024-05-27 13:12:26.000000 foxesscloud-2.2.8/src/foxesscloud.egg-info/
--rw-rw-rw-   0        0        0    42891 2024-05-27 13:12:26.000000 foxesscloud-2.2.8/src/foxesscloud.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-05-27 13:12:26.000000 foxesscloud-2.2.8/src/foxesscloud.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-27 13:12:26.000000 foxesscloud-2.2.8/src/foxesscloud.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-27 13:12:26.000000 foxesscloud-2.2.8/src/foxesscloud.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-28 11:39:43.000000 foxesscloud-2.2.9/
+-rw-rw-rw-   0        0        0     1074 2023-08-27 11:13:04.000000 foxesscloud-2.2.9/LICENCE
+-rw-rw-rw-   0        0        0    42605 2024-05-28 11:39:43.000000 foxesscloud-2.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0    42050 2024-05-28 11:37:03.000000 foxesscloud-2.2.9/README.md
+-rw-rw-rw-   0        0        0      635 2024-05-28 11:36:16.000000 foxesscloud-2.2.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-28 11:39:43.000000 foxesscloud-2.2.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-28 11:39:43.000000 foxesscloud-2.2.9/src/
+drwxrwxrwx   0        0        0        0 2024-05-28 11:39:43.000000 foxesscloud-2.2.9/src/foxesscloud/
+-rw-rw-rw-   0        0        0   181899 2024-05-28 11:37:50.000000 foxesscloud-2.2.9/src/foxesscloud/foxesscloud.py
+-rw-rw-rw-   0        0        0   176222 2024-05-28 11:37:50.000000 foxesscloud-2.2.9/src/foxesscloud/openapi.py
+drwxrwxrwx   0        0        0        0 2024-05-28 11:39:43.000000 foxesscloud-2.2.9/src/foxesscloud.egg-info/
+-rw-rw-rw-   0        0        0    42605 2024-05-28 11:39:43.000000 foxesscloud-2.2.9/src/foxesscloud.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-05-28 11:39:43.000000 foxesscloud-2.2.9/src/foxesscloud.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-28 11:39:43.000000 foxesscloud-2.2.9/src/foxesscloud.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-28 11:39:43.000000 foxesscloud-2.2.9/src/foxesscloud.egg-info/top_level.txt
```

### Comparing `foxesscloud-2.2.8/LICENCE` & `foxesscloud-2.2.9/LICENCE`

 * *Files identical despite different names*

### Comparing `foxesscloud-2.2.8/PKG-INFO` & `foxesscloud-2.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foxesscloud
-Version: 2.2.8
+Version: 2.2.9
 Summary: library for accessing Fox ESS cloud data using Open API
 Author-email: Tony Matthews <tony@quasair.co.uk>
 Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -460,15 +460,15 @@
 ```
 
 ## Tariffs
 
 Tariffs configure when your battery can be charged and provide time of use (TOU) periods to split your grid import and export into peak, off-peak and shoulder times when data is uploaded to PV Ouptut.
 
 There are a number of different pre-configured tariffs:
-+ Octopus Flux: off-peak from 02:00 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59. Timed work mode change to Self Use at 7am and Feed In First at 4pm.
++ Octopus Flux: off-peak from 02:00 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59. Timed work mode changes to Self Use at 5am and Feed In First at 4pm.
 + Intelligent Octopus: off-peak from 23:30 to 05:30, forecasts from 22:00 to 23:59
 + Octopus Cosy: off-peak from 04:00 to 07:00 and 13:00 to 16:00, peak from 16:00 to 19:00, forecasts from 02:00 to 03:59 and 12:00 to 12:59
 + Octopus Go: off peak from 00:30 to 04:30, forecasts from 22:00 to 23:59
 + Agile Octopus: off-peak from 02:30 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59
 + British Gas Electric Driver: off-peak from 00:00 to 05:00, forecasts from 22:00 to 23:59
 + Eco 7: Economy 7: off-peak from 00:30 to 07:30 GMT (01:30 to 08:30 during BST)
 
@@ -538,19 +538,14 @@
 + times=[("23:00", "8:00", 3), ("12:00", "16:00", 1)]
 
 'strategy' allows you to configure times when work modes will be changed. The format is a list of dictionary items, containing:
 + 'start', 'end': times in decimal hours or time format. The end time is exclusive so setting an end time of '07:00' will set a schedule that ends at '06:59'
 + 'mode': the work mode to be used from 'SelfUse', 'Feedin', 'Backup', 'ForceCharge', 'ForceDischarge'
 + 'min_soc, 'fdsoc', 'fdpwr': optional values for each work mode. The defaults are 10, 10 and 0 respectively.
 
-There are a number of pre-defined strategies:
-+ f.flux_strategy_1: switch to self use at 5am and feed in first at 4pm.
-+ f.flux_strategy_2: as above with force charge between 2am and 4am. Move the AM charge period between 4am and 5am when using this.
-+ f.flux_strategy_3: as above with force discharge between 4pm and 6pm at 6kW with fdsoc at 35%
-
 ```
 f.get_strategy()
 ```
 
 get_strategy() creates a list of time segments from the strategy. If strategy is not provided, it uses the strategy for the current tariff. If a strategy includes settings for the AM/PM charge times for the tariff, the times will be moved so they do not conflict with the charge time used by charge_needed().
 
 
@@ -695,15 +690,16 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
-2.2.8<br>
+2.2.9<br>
+Fix typo in charge_periods() that caused error with timed_mode=2
 ** breaking change ** rename 'groups' to 'periods' for consistency between foxesscloud and openapi.
 Updated management of battery reserve and float charging in charge_needed().
 Added Reserve level to charts in charge_needed().
 Changed bms_power setting to 50W.
 Updated contingency to allow seasonal values for winter, spring, summer and autumn.
 Update strategy mode to support ForceCharge and ForceDischarge work modes.
 Update so min_soc setting in charge_needed() over-rides min_soc in the tariff strategy.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.8 Summary: library for
+Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.9 Summary: library for
 accessing Fox ESS cloud data using Open API Author-email: Tony Matthews
 quasair.co.uk> Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
 Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
 LICENCE # FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code
@@ -334,15 +334,15 @@
 include minutes, ss = include seconds, day = include /n for day when hours > 24
 f.hours_in(h, {'start': a, 'end': b}) # True if decimal hour h is in the time
 period a -> b ``` ## Tariffs Tariffs configure when your battery can be charged
 and provide time of use (TOU) periods to split your grid import and export into
 peak, off-peak and shoulder times when data is uploaded to PV Ouptut. There are
 a number of different pre-configured tariffs: + Octopus Flux: off-peak from 02:
 00 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59. Timed
-work mode change to Self Use at 7am and Feed In First at 4pm. + Intelligent
+work mode changes to Self Use at 5am and Feed In First at 4pm. + Intelligent
 Octopus: off-peak from 23:30 to 05:30, forecasts from 22:00 to 23:59 + Octopus
 Cosy: off-peak from 04:00 to 07:00 and 13:00 to 16:00, peak from 16:00 to 19:
 00, forecasts from 02:00 to 03:59 and 12:00 to 12:59 + Octopus Go: off peak
 from 00:30 to 04:30, forecasts from 22:00 to 23:59 + Agile Octopus: off-peak
 from 02:30 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59 +
 British Gas Electric Driver: off-peak from 00:00 to 05:00, forecasts from 22:00
 to 23:59 + Eco 7: Economy 7: off-peak from 00:30 to 07:30 GMT (01:30 to 08:30
@@ -401,114 +401,111 @@
 between 12 noon and 4pm with a 1 hour period: + times=[("23:00", "8:00", 3),
 ("12:00", "16:00", 1)] 'strategy' allows you to configure times when work modes
 will be changed. The format is a list of dictionary items, containing: +
 'start', 'end': times in decimal hours or time format. The end time is
 exclusive so setting an end time of '07:00' will set a schedule that ends at
 '06:59' + 'mode': the work mode to be used from 'SelfUse', 'Feedin', 'Backup',
 'ForceCharge', 'ForceDischarge' + 'min_soc, 'fdsoc', 'fdpwr': optional values
-for each work mode. The defaults are 10, 10 and 0 respectively. There are a
-number of pre-defined strategies: + f.flux_strategy_1: switch to self use at
-5am and feed in first at 4pm. + f.flux_strategy_2: as above with force charge
-between 2am and 4am. Move the AM charge period between 4am and 5am when using
-this. + f.flux_strategy_3: as above with force discharge between 4pm and 6pm at
-6kW with fdsoc at 35% ``` f.get_strategy() ``` get_strategy() creates a list of
-time segments from the strategy. If strategy is not provided, it uses the
-strategy for the current tariff. If a strategy includes settings for the AM/PM
-charge times for the tariff, the times will be moved so they do not conflict
-with the charge time used by charge_needed(). # PV Output These functions
-produce CSV data for upload to [pvoutput.org](https://pvoutput.org) including
-PV generation, Export, Load and Grid consumption by day in Wh. The functions
-use the energy estimates created from the raw power data (see above). The
-estimates include PV energy generation that are not otherwise available from
-the Fox Cloud. Typically, the energy results are within 3% of the values
-reported by the meters built into the inverter. ## Get PV Output Data Returns
-CSV upload data using the [API format](https://pvoutput.org/help/
-api_specification.html#csv-data-parameter): ``` f.get_pvoutput(d, tou) ``` + d
-is the date or a list of dates, to get data for. The default is yesterday +
-tou: optional, setting tou=1 uploads data with time of use. The default, tou=0
-does not split data and is more accurate. You can copy and paste the output
-data to the pvoutput data CSV Loader, using the following settings: ![image]
-(https://github.com/TonyM1958/FoxESS-Cloud/assets/63789168/21459cdc-a943-4e9d-
-a204-7efd45a422d8) For example, this Jupyer Lab cell will provide a CSV data
-upload for June 2023: ``` f.get_pvoutput(f.date_list('2023-06-01', '2023-06-
-30')) ``` ## Set PV Output Data Loads CSV data directly using the PV Ouput API:
-``` f.set_pvoutput(d, system_id, tou, push) ``` + d is optional and is the
-date, or a list of dates, to upload + system_id is optional and allow you to
-select where data is uploaded to (where you have more than 1 registered system)
-+ tou: optional, setting tou=1 uploads data with time of use. The default,
-tou=0 does not split data and is more accurate + push: optional. 0 = do not
-sent to pushover, 1 = send summary to pushover, 2 = send first day summary only
-# Solar Forecasting # Solcast Get and display solar data from your solcast.com
-account using your API key: ``` f.solcast_api_key = "my.solcast_api_key" fcast
-= f.Solcast() print(fcast) ``` Returns a 7 day forecast. Optional parameters
-are: + days: number of days to get. The default is 7 + estimated: whether to
-get history / estimated data. 1 = yes, 0 = no. Default is 0. + reload: cached
-data handling. 0 = use saved data, 1 = fetch new data, 2 = use saved data for
-today (default) + quiet: True to stop Solcast producing progress messages
-Forecast data is saved to f.solcast_save. The default is 'solcast.txt'. ```
-fcast.plot_daily() fcast.plot_hourly(day) ``` Plots the estimate / forecast
-data. plot_daily() plots the daily yield. plot_hourly() plots each day
-separately. + day: optional. 'today', 'tomorrow', 'all' or a specific list of
-dates. The default is to plot today and tomorrow # Forecast.solar Get and
-display solar data from forecast.solar for today and tomorrow: ```
-f.solar_array('South', lat=51.1789, lon=-1.8262, kwp=6.4) ``` You need to
-configure your solar arrays by calling f.solar_array(). This takes the
-following parameters: + name: the name of each of your arrays + lat: the
-latitude where the array is located. The default is Stonehenge. + lon: the
-longitude where the array is located. The default is Stonehenge. + dec: the
-declination of the array - 0 is lying flat and 90 is vertical. Default is 30 +
-az: azimuth of the array. 0 is pointing due South, -90 is pointing East, 90 is
-pointing West. The default is 0 + kwp: the size of the array in kWp. The
-default is 5kWp + dam: damping factor. Default is None + inv: inverter power
-limit (when the array will clip). The default is None + hor: a list of values
-describing obstructions on the horizon Add one array for each string attached
-to your inverter. If your solar production is limited by clipping, set the
-inverter power so the forecast better matches your generation. See the [API
-documentation](https://doc.forecast.solar/api) for more information on
-parameter values. ``` fcast = f.Solar() print(fcast) ``` Returns a forecast for
-today and tomorrow. Optional parameters are: + reload: cached data handling. 0
-= use saved data, 1 = fetch new data, 2 = use saved data for today (default) +
-quiet: set to True to stop Solar producing progress messages Forecast data is
-saved to f.solar_save. The default is 'solar.txt'. ``` fcast.plot_daily()
+for each work mode. The defaults are 10, 10 and 0 respectively. ```
+f.get_strategy() ``` get_strategy() creates a list of time segments from the
+strategy. If strategy is not provided, it uses the strategy for the current
+tariff. If a strategy includes settings for the AM/PM charge times for the
+tariff, the times will be moved so they do not conflict with the charge time
+used by charge_needed(). # PV Output These functions produce CSV data for
+upload to [pvoutput.org](https://pvoutput.org) including PV generation, Export,
+Load and Grid consumption by day in Wh. The functions use the energy estimates
+created from the raw power data (see above). The estimates include PV energy
+generation that are not otherwise available from the Fox Cloud. Typically, the
+energy results are within 3% of the values reported by the meters built into
+the inverter. ## Get PV Output Data Returns CSV upload data using the [API
+format](https://pvoutput.org/help/api_specification.html#csv-data-parameter):
+``` f.get_pvoutput(d, tou) ``` + d is the date or a list of dates, to get data
+for. The default is yesterday + tou: optional, setting tou=1 uploads data with
+time of use. The default, tou=0 does not split data and is more accurate. You
+can copy and paste the output data to the pvoutput data CSV Loader, using the
+following settings: ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/
+63789168/21459cdc-a943-4e9d-a204-7efd45a422d8) For example, this Jupyer Lab
+cell will provide a CSV data upload for June 2023: ``` f.get_pvoutput
+(f.date_list('2023-06-01', '2023-06-30')) ``` ## Set PV Output Data Loads CSV
+data directly using the PV Ouput API: ``` f.set_pvoutput(d, system_id, tou,
+push) ``` + d is optional and is the date, or a list of dates, to upload +
+system_id is optional and allow you to select where data is uploaded to (where
+you have more than 1 registered system) + tou: optional, setting tou=1 uploads
+data with time of use. The default, tou=0 does not split data and is more
+accurate + push: optional. 0 = do not sent to pushover, 1 = send summary to
+pushover, 2 = send first day summary only # Solar Forecasting # Solcast Get and
+display solar data from your solcast.com account using your API key: ```
+f.solcast_api_key = "my.solcast_api_key" fcast = f.Solcast() print(fcast) ```
+Returns a 7 day forecast. Optional parameters are: + days: number of days to
+get. The default is 7 + estimated: whether to get history / estimated data. 1 =
+yes, 0 = no. Default is 0. + reload: cached data handling. 0 = use saved data,
+1 = fetch new data, 2 = use saved data for today (default) + quiet: True to
+stop Solcast producing progress messages Forecast data is saved to
+f.solcast_save. The default is 'solcast.txt'. ``` fcast.plot_daily()
 fcast.plot_hourly(day) ``` Plots the estimate / forecast data. plot_daily()
 plots the daily yield. plot_hourly() plots each day separately. + day:
 optional. 'today', 'tomorrow', 'all' or a specific list of dates. The default
-is to plot today and tomorrow # Pushover Send messages to a pushover user
-account: ``` f.output_spool(app_key, h) f.output(s) f.output_close(plot, file)
-f.output_message(app_key, message, plot) ``` Calling f.output_spool() with an
-app key will start the system spooling output to send to pushover. h is an
-optional header to add as the first line of the message. H may include \
+is to plot today and tomorrow # Forecast.solar Get and display solar data from
+forecast.solar for today and tomorrow: ``` f.solar_array('South', lat=51.1789,
+lon=-1.8262, kwp=6.4) ``` You need to configure your solar arrays by calling
+f.solar_array(). This takes the following parameters: + name: the name of each
+of your arrays + lat: the latitude where the array is located. The default is
+Stonehenge. + lon: the longitude where the array is located. The default is
+Stonehenge. + dec: the declination of the array - 0 is lying flat and 90 is
+vertical. Default is 30 + az: azimuth of the array. 0 is pointing due South, -
+90 is pointing East, 90 is pointing West. The default is 0 + kwp: the size of
+the array in kWp. The default is 5kWp + dam: damping factor. Default is None +
+inv: inverter power limit (when the array will clip). The default is None +
+hor: a list of values describing obstructions on the horizon Add one array for
+each string attached to your inverter. If your solar production is limited by
+clipping, set the inverter power so the forecast better matches your
+generation. See the [API documentation](https://doc.forecast.solar/api) for
+more information on parameter values. ``` fcast = f.Solar() print(fcast) ```
+Returns a forecast for today and tomorrow. Optional parameters are: + reload:
+cached data handling. 0 = use saved data, 1 = fetch new data, 2 = use saved
+data for today (default) + quiet: set to True to stop Solar producing progress
+messages Forecast data is saved to f.solar_save. The default is 'solar.txt'.
+``` fcast.plot_daily() fcast.plot_hourly(day) ``` Plots the estimate / forecast
+data. plot_daily() plots the daily yield. plot_hourly() plots each day
+separately. + day: optional. 'today', 'tomorrow', 'all' or a specific list of
+dates. The default is to plot today and tomorrow # Pushover Send messages to a
+pushover user account: ``` f.output_spool(app_key, h) f.output(s)
+f.output_close(plot, file) f.output_message(app_key, message, plot) ``` Calling
+f.output_spool() with an app key will start the system spooling output to send
+to pushover. h is an optional header to add as the first line of the message. H
+may include \
 >, \
 > or \
 > and these will be set to current system time and date respectively. When
 spooling is active, any calls to f.output() add lines to the spooled message.
 If appending to the message would exceed 1024 characters, the existing spooled
 message is sent and a new message spool is started. Calling f.output_close()
 will send the spooled message and optionally attach a binary image file. You
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.2.8
-** breaking change ** rename 'groups' to 'periods' for consistency between
-foxesscloud and openapi. Updated management of battery reserve and float
-charging in charge_needed(). Added Reserve level to charts in charge_needed().
-Changed bms_power setting to 50W. Updated contingency to allow seasonal values
-for winter, spring, summer and autumn. Update strategy mode to support
-ForceCharge and ForceDischarge work modes. Update so min_soc setting in
-charge_needed() over-rides min_soc in the tariff strategy. Fix force charge
-strategy mode in charge_neded() to set min_soc correctly. Implement 2 second
-delay between calls that change inverter settings. Added strategy mode
-(timed_mode=2) to charge_needed(). Added set_strategy() and charge_strategy()
-to manage charging schedules and work mode changes. Refactor debug messaging.
-Simplify charge_needed() output. Added 'target_soc' to charge_needed() settings
-Fix bat_info() giving incorrect temperatures when API returns 0 instead of -50
+(verbose) # Version Info 2.2.9
+Fix typo in charge_periods() that caused error with timed_mode=2 ** breaking
+change ** rename 'groups' to 'periods' for consistency between foxesscloud and
+openapi. Updated management of battery reserve and float charging in
+charge_needed(). Added Reserve level to charts in charge_needed(). Changed
+bms_power setting to 50W. Updated contingency to allow seasonal values for
+winter, spring, summer and autumn. Update strategy mode to support ForceCharge
+and ForceDischarge work modes. Update so min_soc setting in charge_needed()
+over-rides min_soc in the tariff strategy. Fix force charge strategy mode in
+charge_neded() to set min_soc correctly. Implement 2 second delay between calls
+that change inverter settings. Added strategy mode (timed_mode=2) to
+charge_needed(). Added set_strategy() and charge_strategy() to manage charging
+schedules and work mode changes. Refactor debug messaging. Simplify
+charge_needed() output. Added 'target_soc' to charge_needed() settings Fix
+bat_info() giving incorrect temperatures when API returns 0 instead of -50
 where there is no battery Fix key error when accessing cell volts and temps
 using an agent / installer account. Ensure output is generated if get_battery()
 fails using battery_info(). Update f.avg() to include calculation of averages
 in lists containng None values. Added 'data_wrap' to charge_config. 2.1.9
 Update get_history() to use GMT or BST when plotting instead of mixed time
 zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
```

### Comparing `foxesscloud-2.2.8/README.md` & `foxesscloud-2.2.9/src/foxesscloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: foxesscloud
+Version: 2.2.9
+Summary: library for accessing Fox ESS cloud data using Open API
+Author-email: Tony Matthews <tony@quasair.co.uk>
+Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
+Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENCE
+
 # FoxESS-Cloud
 
 <a href="https://www.buymeacoffee.com/tonym1958" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174" align="right"></a>
 This site contains sample python code for accessing the Fox cloud data via the REST API used by the Fox ESS Cloud web site and app.
 
 There is also a number of Jupyter Lab notebooks with examples of how to run the sample code.
 
@@ -446,15 +460,15 @@
 ```
 
 ## Tariffs
 
 Tariffs configure when your battery can be charged and provide time of use (TOU) periods to split your grid import and export into peak, off-peak and shoulder times when data is uploaded to PV Ouptut.
 
 There are a number of different pre-configured tariffs:
-+ Octopus Flux: off-peak from 02:00 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59. Timed work mode change to Self Use at 7am and Feed In First at 4pm.
++ Octopus Flux: off-peak from 02:00 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59. Timed work mode changes to Self Use at 5am and Feed In First at 4pm.
 + Intelligent Octopus: off-peak from 23:30 to 05:30, forecasts from 22:00 to 23:59
 + Octopus Cosy: off-peak from 04:00 to 07:00 and 13:00 to 16:00, peak from 16:00 to 19:00, forecasts from 02:00 to 03:59 and 12:00 to 12:59
 + Octopus Go: off peak from 00:30 to 04:30, forecasts from 22:00 to 23:59
 + Agile Octopus: off-peak from 02:30 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59
 + British Gas Electric Driver: off-peak from 00:00 to 05:00, forecasts from 22:00 to 23:59
 + Eco 7: Economy 7: off-peak from 00:30 to 07:30 GMT (01:30 to 08:30 during BST)
 
@@ -524,19 +538,14 @@
 + times=[("23:00", "8:00", 3), ("12:00", "16:00", 1)]
 
 'strategy' allows you to configure times when work modes will be changed. The format is a list of dictionary items, containing:
 + 'start', 'end': times in decimal hours or time format. The end time is exclusive so setting an end time of '07:00' will set a schedule that ends at '06:59'
 + 'mode': the work mode to be used from 'SelfUse', 'Feedin', 'Backup', 'ForceCharge', 'ForceDischarge'
 + 'min_soc, 'fdsoc', 'fdpwr': optional values for each work mode. The defaults are 10, 10 and 0 respectively.
 
-There are a number of pre-defined strategies:
-+ f.flux_strategy_1: switch to self use at 5am and feed in first at 4pm.
-+ f.flux_strategy_2: as above with force charge between 2am and 4am. Move the AM charge period between 4am and 5am when using this.
-+ f.flux_strategy_3: as above with force discharge between 4pm and 6pm at 6kW with fdsoc at 35%
-
 ```
 f.get_strategy()
 ```
 
 get_strategy() creates a list of time segments from the strategy. If strategy is not provided, it uses the strategy for the current tariff. If a strategy includes settings for the AM/PM charge times for the tariff, the times will be moved so they do not conflict with the charge time used by charge_needed().
 
 
@@ -681,15 +690,16 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
-2.2.8<br>
+2.2.9<br>
+Fix typo in charge_periods() that caused error with timed_mode=2
 ** breaking change ** rename 'groups' to 'periods' for consistency between foxesscloud and openapi.
 Updated management of battery reserve and float charging in charge_needed().
 Added Reserve level to charts in charge_needed().
 Changed bms_power setting to 50W.
 Updated contingency to allow seasonal values for winter, spring, summer and autumn.
 Update strategy mode to support ForceCharge and ForceDischarge work modes.
 Update so min_soc setting in charge_needed() over-rides min_soc in the tariff strategy.
```

#### html2text {}

```diff
@@ -1,9 +1,16 @@
-# FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code for
-accessing the Fox cloud data via the REST API used by the Fox ESS Cloud web
+Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.9 Summary: library for
+accessing Fox ESS cloud data using Open API Author-email: Tony Matthews
+quasair.co.uk> Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
+Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
+Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
+Approved :: MIT License Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
+LICENCE # FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code
+for accessing the Fox cloud data via the REST API used by the Fox ESS Cloud web
 site and app. There is also a number of Jupyter Lab notebooks with examples of
 how to run the sample code. This project is not endorsed by, directly
 affiliated with, maintained, authorized, or sponsored by Fox ESS. Please refer
 to the [LICENCE](https://github.com/TonyM1958/FoxESS-Cloud/blob/main/LICENCE)
 for information on copyright, permissions and warranty. # Open API This module
 builds on the Fox Open API to provide a sample code and utilities that can be
 used with your inverter and batteries. + Information on the API can be found
@@ -327,15 +334,15 @@
 include minutes, ss = include seconds, day = include /n for day when hours > 24
 f.hours_in(h, {'start': a, 'end': b}) # True if decimal hour h is in the time
 period a -> b ``` ## Tariffs Tariffs configure when your battery can be charged
 and provide time of use (TOU) periods to split your grid import and export into
 peak, off-peak and shoulder times when data is uploaded to PV Ouptut. There are
 a number of different pre-configured tariffs: + Octopus Flux: off-peak from 02:
 00 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59. Timed
-work mode change to Self Use at 7am and Feed In First at 4pm. + Intelligent
+work mode changes to Self Use at 5am and Feed In First at 4pm. + Intelligent
 Octopus: off-peak from 23:30 to 05:30, forecasts from 22:00 to 23:59 + Octopus
 Cosy: off-peak from 04:00 to 07:00 and 13:00 to 16:00, peak from 16:00 to 19:
 00, forecasts from 02:00 to 03:59 and 12:00 to 12:59 + Octopus Go: off peak
 from 00:30 to 04:30, forecasts from 22:00 to 23:59 + Agile Octopus: off-peak
 from 02:30 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59 +
 British Gas Electric Driver: off-peak from 00:00 to 05:00, forecasts from 22:00
 to 23:59 + Eco 7: Economy 7: off-peak from 00:30 to 07:30 GMT (01:30 to 08:30
@@ -394,114 +401,111 @@
 between 12 noon and 4pm with a 1 hour period: + times=[("23:00", "8:00", 3),
 ("12:00", "16:00", 1)] 'strategy' allows you to configure times when work modes
 will be changed. The format is a list of dictionary items, containing: +
 'start', 'end': times in decimal hours or time format. The end time is
 exclusive so setting an end time of '07:00' will set a schedule that ends at
 '06:59' + 'mode': the work mode to be used from 'SelfUse', 'Feedin', 'Backup',
 'ForceCharge', 'ForceDischarge' + 'min_soc, 'fdsoc', 'fdpwr': optional values
-for each work mode. The defaults are 10, 10 and 0 respectively. There are a
-number of pre-defined strategies: + f.flux_strategy_1: switch to self use at
-5am and feed in first at 4pm. + f.flux_strategy_2: as above with force charge
-between 2am and 4am. Move the AM charge period between 4am and 5am when using
-this. + f.flux_strategy_3: as above with force discharge between 4pm and 6pm at
-6kW with fdsoc at 35% ``` f.get_strategy() ``` get_strategy() creates a list of
-time segments from the strategy. If strategy is not provided, it uses the
-strategy for the current tariff. If a strategy includes settings for the AM/PM
-charge times for the tariff, the times will be moved so they do not conflict
-with the charge time used by charge_needed(). # PV Output These functions
-produce CSV data for upload to [pvoutput.org](https://pvoutput.org) including
-PV generation, Export, Load and Grid consumption by day in Wh. The functions
-use the energy estimates created from the raw power data (see above). The
-estimates include PV energy generation that are not otherwise available from
-the Fox Cloud. Typically, the energy results are within 3% of the values
-reported by the meters built into the inverter. ## Get PV Output Data Returns
-CSV upload data using the [API format](https://pvoutput.org/help/
-api_specification.html#csv-data-parameter): ``` f.get_pvoutput(d, tou) ``` + d
-is the date or a list of dates, to get data for. The default is yesterday +
-tou: optional, setting tou=1 uploads data with time of use. The default, tou=0
-does not split data and is more accurate. You can copy and paste the output
-data to the pvoutput data CSV Loader, using the following settings: ![image]
-(https://github.com/TonyM1958/FoxESS-Cloud/assets/63789168/21459cdc-a943-4e9d-
-a204-7efd45a422d8) For example, this Jupyer Lab cell will provide a CSV data
-upload for June 2023: ``` f.get_pvoutput(f.date_list('2023-06-01', '2023-06-
-30')) ``` ## Set PV Output Data Loads CSV data directly using the PV Ouput API:
-``` f.set_pvoutput(d, system_id, tou, push) ``` + d is optional and is the
-date, or a list of dates, to upload + system_id is optional and allow you to
-select where data is uploaded to (where you have more than 1 registered system)
-+ tou: optional, setting tou=1 uploads data with time of use. The default,
-tou=0 does not split data and is more accurate + push: optional. 0 = do not
-sent to pushover, 1 = send summary to pushover, 2 = send first day summary only
-# Solar Forecasting # Solcast Get and display solar data from your solcast.com
-account using your API key: ``` f.solcast_api_key = "my.solcast_api_key" fcast
-= f.Solcast() print(fcast) ``` Returns a 7 day forecast. Optional parameters
-are: + days: number of days to get. The default is 7 + estimated: whether to
-get history / estimated data. 1 = yes, 0 = no. Default is 0. + reload: cached
-data handling. 0 = use saved data, 1 = fetch new data, 2 = use saved data for
-today (default) + quiet: True to stop Solcast producing progress messages
-Forecast data is saved to f.solcast_save. The default is 'solcast.txt'. ```
-fcast.plot_daily() fcast.plot_hourly(day) ``` Plots the estimate / forecast
-data. plot_daily() plots the daily yield. plot_hourly() plots each day
-separately. + day: optional. 'today', 'tomorrow', 'all' or a specific list of
-dates. The default is to plot today and tomorrow # Forecast.solar Get and
-display solar data from forecast.solar for today and tomorrow: ```
-f.solar_array('South', lat=51.1789, lon=-1.8262, kwp=6.4) ``` You need to
-configure your solar arrays by calling f.solar_array(). This takes the
-following parameters: + name: the name of each of your arrays + lat: the
-latitude where the array is located. The default is Stonehenge. + lon: the
-longitude where the array is located. The default is Stonehenge. + dec: the
-declination of the array - 0 is lying flat and 90 is vertical. Default is 30 +
-az: azimuth of the array. 0 is pointing due South, -90 is pointing East, 90 is
-pointing West. The default is 0 + kwp: the size of the array in kWp. The
-default is 5kWp + dam: damping factor. Default is None + inv: inverter power
-limit (when the array will clip). The default is None + hor: a list of values
-describing obstructions on the horizon Add one array for each string attached
-to your inverter. If your solar production is limited by clipping, set the
-inverter power so the forecast better matches your generation. See the [API
-documentation](https://doc.forecast.solar/api) for more information on
-parameter values. ``` fcast = f.Solar() print(fcast) ``` Returns a forecast for
-today and tomorrow. Optional parameters are: + reload: cached data handling. 0
-= use saved data, 1 = fetch new data, 2 = use saved data for today (default) +
-quiet: set to True to stop Solar producing progress messages Forecast data is
-saved to f.solar_save. The default is 'solar.txt'. ``` fcast.plot_daily()
+for each work mode. The defaults are 10, 10 and 0 respectively. ```
+f.get_strategy() ``` get_strategy() creates a list of time segments from the
+strategy. If strategy is not provided, it uses the strategy for the current
+tariff. If a strategy includes settings for the AM/PM charge times for the
+tariff, the times will be moved so they do not conflict with the charge time
+used by charge_needed(). # PV Output These functions produce CSV data for
+upload to [pvoutput.org](https://pvoutput.org) including PV generation, Export,
+Load and Grid consumption by day in Wh. The functions use the energy estimates
+created from the raw power data (see above). The estimates include PV energy
+generation that are not otherwise available from the Fox Cloud. Typically, the
+energy results are within 3% of the values reported by the meters built into
+the inverter. ## Get PV Output Data Returns CSV upload data using the [API
+format](https://pvoutput.org/help/api_specification.html#csv-data-parameter):
+``` f.get_pvoutput(d, tou) ``` + d is the date or a list of dates, to get data
+for. The default is yesterday + tou: optional, setting tou=1 uploads data with
+time of use. The default, tou=0 does not split data and is more accurate. You
+can copy and paste the output data to the pvoutput data CSV Loader, using the
+following settings: ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/
+63789168/21459cdc-a943-4e9d-a204-7efd45a422d8) For example, this Jupyer Lab
+cell will provide a CSV data upload for June 2023: ``` f.get_pvoutput
+(f.date_list('2023-06-01', '2023-06-30')) ``` ## Set PV Output Data Loads CSV
+data directly using the PV Ouput API: ``` f.set_pvoutput(d, system_id, tou,
+push) ``` + d is optional and is the date, or a list of dates, to upload +
+system_id is optional and allow you to select where data is uploaded to (where
+you have more than 1 registered system) + tou: optional, setting tou=1 uploads
+data with time of use. The default, tou=0 does not split data and is more
+accurate + push: optional. 0 = do not sent to pushover, 1 = send summary to
+pushover, 2 = send first day summary only # Solar Forecasting # Solcast Get and
+display solar data from your solcast.com account using your API key: ```
+f.solcast_api_key = "my.solcast_api_key" fcast = f.Solcast() print(fcast) ```
+Returns a 7 day forecast. Optional parameters are: + days: number of days to
+get. The default is 7 + estimated: whether to get history / estimated data. 1 =
+yes, 0 = no. Default is 0. + reload: cached data handling. 0 = use saved data,
+1 = fetch new data, 2 = use saved data for today (default) + quiet: True to
+stop Solcast producing progress messages Forecast data is saved to
+f.solcast_save. The default is 'solcast.txt'. ``` fcast.plot_daily()
 fcast.plot_hourly(day) ``` Plots the estimate / forecast data. plot_daily()
 plots the daily yield. plot_hourly() plots each day separately. + day:
 optional. 'today', 'tomorrow', 'all' or a specific list of dates. The default
-is to plot today and tomorrow # Pushover Send messages to a pushover user
-account: ``` f.output_spool(app_key, h) f.output(s) f.output_close(plot, file)
-f.output_message(app_key, message, plot) ``` Calling f.output_spool() with an
-app key will start the system spooling output to send to pushover. h is an
-optional header to add as the first line of the message. H may include \
+is to plot today and tomorrow # Forecast.solar Get and display solar data from
+forecast.solar for today and tomorrow: ``` f.solar_array('South', lat=51.1789,
+lon=-1.8262, kwp=6.4) ``` You need to configure your solar arrays by calling
+f.solar_array(). This takes the following parameters: + name: the name of each
+of your arrays + lat: the latitude where the array is located. The default is
+Stonehenge. + lon: the longitude where the array is located. The default is
+Stonehenge. + dec: the declination of the array - 0 is lying flat and 90 is
+vertical. Default is 30 + az: azimuth of the array. 0 is pointing due South, -
+90 is pointing East, 90 is pointing West. The default is 0 + kwp: the size of
+the array in kWp. The default is 5kWp + dam: damping factor. Default is None +
+inv: inverter power limit (when the array will clip). The default is None +
+hor: a list of values describing obstructions on the horizon Add one array for
+each string attached to your inverter. If your solar production is limited by
+clipping, set the inverter power so the forecast better matches your
+generation. See the [API documentation](https://doc.forecast.solar/api) for
+more information on parameter values. ``` fcast = f.Solar() print(fcast) ```
+Returns a forecast for today and tomorrow. Optional parameters are: + reload:
+cached data handling. 0 = use saved data, 1 = fetch new data, 2 = use saved
+data for today (default) + quiet: set to True to stop Solar producing progress
+messages Forecast data is saved to f.solar_save. The default is 'solar.txt'.
+``` fcast.plot_daily() fcast.plot_hourly(day) ``` Plots the estimate / forecast
+data. plot_daily() plots the daily yield. plot_hourly() plots each day
+separately. + day: optional. 'today', 'tomorrow', 'all' or a specific list of
+dates. The default is to plot today and tomorrow # Pushover Send messages to a
+pushover user account: ``` f.output_spool(app_key, h) f.output(s)
+f.output_close(plot, file) f.output_message(app_key, message, plot) ``` Calling
+f.output_spool() with an app key will start the system spooling output to send
+to pushover. h is an optional header to add as the first line of the message. H
+may include \
 >, \
 > or \
 > and these will be set to current system time and date respectively. When
 spooling is active, any calls to f.output() add lines to the spooled message.
 If appending to the message would exceed 1024 characters, the existing spooled
 message is sent and a new message spool is started. Calling f.output_close()
 will send the spooled message and optionally attach a binary image file. You
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.2.8
-** breaking change ** rename 'groups' to 'periods' for consistency between
-foxesscloud and openapi. Updated management of battery reserve and float
-charging in charge_needed(). Added Reserve level to charts in charge_needed().
-Changed bms_power setting to 50W. Updated contingency to allow seasonal values
-for winter, spring, summer and autumn. Update strategy mode to support
-ForceCharge and ForceDischarge work modes. Update so min_soc setting in
-charge_needed() over-rides min_soc in the tariff strategy. Fix force charge
-strategy mode in charge_neded() to set min_soc correctly. Implement 2 second
-delay between calls that change inverter settings. Added strategy mode
-(timed_mode=2) to charge_needed(). Added set_strategy() and charge_strategy()
-to manage charging schedules and work mode changes. Refactor debug messaging.
-Simplify charge_needed() output. Added 'target_soc' to charge_needed() settings
-Fix bat_info() giving incorrect temperatures when API returns 0 instead of -50
+(verbose) # Version Info 2.2.9
+Fix typo in charge_periods() that caused error with timed_mode=2 ** breaking
+change ** rename 'groups' to 'periods' for consistency between foxesscloud and
+openapi. Updated management of battery reserve and float charging in
+charge_needed(). Added Reserve level to charts in charge_needed(). Changed
+bms_power setting to 50W. Updated contingency to allow seasonal values for
+winter, spring, summer and autumn. Update strategy mode to support ForceCharge
+and ForceDischarge work modes. Update so min_soc setting in charge_needed()
+over-rides min_soc in the tariff strategy. Fix force charge strategy mode in
+charge_neded() to set min_soc correctly. Implement 2 second delay between calls
+that change inverter settings. Added strategy mode (timed_mode=2) to
+charge_needed(). Added set_strategy() and charge_strategy() to manage charging
+schedules and work mode changes. Refactor debug messaging. Simplify
+charge_needed() output. Added 'target_soc' to charge_needed() settings Fix
+bat_info() giving incorrect temperatures when API returns 0 instead of -50
 where there is no battery Fix key error when accessing cell volts and temps
 using an agent / installer account. Ensure output is generated if get_battery()
 fails using battery_info(). Update f.avg() to include calculation of averages
 in lists containng None values. Added 'data_wrap' to charge_config. 2.1.9
 Update get_history() to use GMT or BST when plotting instead of mixed time
 zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
```

### Comparing `foxesscloud-2.2.8/pyproject.toml` & `foxesscloud-2.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "foxesscloud"
-version = "2.2.8"
+version = "2.2.9"
 authors = [
   {name="Tony Matthews", email="tony@quasair.co.uk"},
 ]
 description = "library for accessing Fox ESS cloud data using Open API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `foxesscloud-2.2.8/src/foxesscloud/foxesscloud.py` & `foxesscloud-2.2.9/src/foxesscloud/foxesscloud.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################################
 """
 Module:   Fox ESS Cloud
-Updated:  24 May 2024
+Updated:  28 May 2024
 By:       Tony Matthews
 """
 ##################################################################################################
 # Code for getting and setting inverter data via the Fox ESS cloud web site, including
 # getting forecast data from solcast.com.au and sending inverter data to pvoutput.org
 # ALL RIGHTS ARE RESERVED © Tony Matthews 2023
 ##################################################################################################
 
-version = "1.4.0"
+version = "1.4.1"
 print(f"FoxESS-Cloud version {version}")
 
 debug_setting = 1
 
 # constants
 month_names = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December']
 day_names = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']
@@ -1168,15 +1168,15 @@
 
 # create a period structure. Note: end time is exclusive.
 def set_period(start=None, end=None, mode=None, min_soc=None, fdsoc=None, fdpwr=None, segment=None, quiet=1):
     if segment is not None and type(segment) is dict:
         start = segment.get('start')
         end = segment.get('end')
         mode = segment.get('mode')
-        min_soc = segement.get('min_soc')
+        min_soc = segment.get('min_soc')
         fdsoc = segment.get('fdsoc')
         fdpwr = segmenet.get('fdsoc')
     start = time_hours(start)
     end = time_hours(end)
     if start is None or end is None or start >= end:
         return None
     end = round_time(end - 1/60)        # adjust exclusive time to inclusive
@@ -1941,14 +1941,18 @@
 octopus_flux = {
     'name': 'Octopus Flux',
     'off_peak1': {'start': 2.0, 'end': 5.0, 'force': 1},        # off-peak period 1 / am charging period
     'off_peak2': {'start': 0.0, 'end': 0.0, 'force': 0},        # off-peak period 2 / pm charging period
     'peak': {'start': 16.0, 'end': 19.0 },                      # peak period 1
     'peak2': {'start': 0.0, 'end': 0.0 },                       # peak period 2
     'forecast_times': [22, 23],                                 # hours in a day to get a forecast
+    'strategy': [
+        {'start': 0.0, 'end': 2.0, 'mode': 'Feedin'},
+        {'start': 5.0, 'end': 6.0, 'mode': 'SelfUse'},
+        {'start': 16.0, 'end': 24.0, 'mode': 'Feedin'}]
     }
 
 # time periods for Intelligent Octopus
 intelligent_octopus = {
     'name': 'Intelligent Octopus',
     'off_peak1': {'start': 23.5, 'end': 5.5, 'force': 1},
     'off_peak2': {'start': 0.0, 'end': 0.0, 'force': 0},
@@ -2019,33 +2023,15 @@
 tariff_list = [octopus_flux, intelligent_octopus, octopus_cosy, octopus_go, agile_octopus, bg_driver, economy_7, custom_periods]
 tariff = octopus_flux
 
 ##################################################################################################
 # Strategy - schedule templates
 ##################################################################################################
 
-# summer strategy for Flux
-flux_strategy_1 = [
-        {'start': 5, 'end': 6, 'mode': 'SelfUse'},
-        {'start': 16, 'end': 24, 'mode': 'Feedin'}]
-
-# winter strategy for Flux
-flux_strategy_2 = [
-        {'start': 2, 'end': 4, 'mode': 'ForceCharge'},
-        {'start': 5, 'end': 6, 'mode': 'SelfUse'},
-        {'start': 16, 'end': 24, 'mode': 'Feedin'}]
-
-# revenue strategy for Flux
-flux_strategy_3 = [
-        {'start': 2, 'end': 4, 'mode': 'ForceCharge'},
-        {'start': 5, 'end': 6, 'mode': 'SelfUse'},
-        {'start': 16, 'end': 18, 'mode': 'ForceDischarge', 'fdsoc': 35, 'fdpwr': 6000},
-        {'start': 18, 'end': 24, 'mode': 'Feedin'}]
-
-flux_strategy_x = [
+test_strategy = [
         {'start': 2, 'end': 11, 'mode': 'SelfUse', 'min_soc': 80},
         {'start': 11, 'end': 14, 'mode': 'SelfUse', 'min_soc': 10},
         {'start': 16, 'end': 24, 'mode': 'Feedin'}]
 
 # return an updated strategy from the tariff strategy that has been filtered for charge times:
 def get_strategy(use=None, strategy=None, min_soc=10, quiet=1):
     global tariff
```

### Comparing `foxesscloud-2.2.8/src/foxesscloud/openapi.py` & `foxesscloud-2.2.9/src/foxesscloud/openapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################################
 """
 Module:   Fox ESS Cloud using Open API
-Updated:  24 May 2024
+Updated:  28 May 2024
 By:       Tony Matthews
 """
 ##################################################################################################
 # Code for getting and setting inverter data via the Fox ESS cloud api site, including
 # getting forecast data from solcast.com.au and sending inverter data to pvoutput.org
 # ALL RIGHTS ARE RESERVED © Tony Matthews 2024
 ##################################################################################################
 
-version = "2.2.8"
+version = "2.2.9"
 print(f"FoxESS-Cloud Open API version {version}")
 
 debug_setting = 1
 
 # constants
 month_names = ['January', 'February', 'March', 'April', 'May', 'June', 'July', 'August', 'September', 'October', 'November', 'December']
 day_names = ['Monday', 'Tuesday', 'Wednesday', 'Thursday', 'Friday', 'Saturday', 'Sunday']
@@ -1051,15 +1051,15 @@
 
 # create time segment structure. Note: end time is exclusive.
 def set_period(start=None, end=None, mode=None, min_soc=None, fdsoc=None, fdpwr=None, segment=None, enable=1, quiet=1):
     if segment is not None and type(segment) is dict:
         start = segment.get('start')
         end = segment.get('end')
         mode = segment.get('mode')
-        min_soc = segement.get('min_soc')
+        min_soc = segment.get('min_soc')
         fdsoc = segment.get('fdsoc')
         fdpwr = segmenet.get('fdsoc')
     start = time_hours(start)
     end = time_hours(end)
     if start is None or end is None or start >= end:
         return None
     end = round_time(end - 1/60)        # adjust exclusive time to inclusive
@@ -1815,16 +1815,21 @@
 octopus_flux = {
     'name': 'Octopus Flux',
     'off_peak1': {'start': 2.0, 'end': 5.0, 'force': 1},        # off-peak period 1 / am charging period
     'off_peak2': {'start': 0.0, 'end': 0.0, 'force': 0},        # off-peak period 2 / pm charging period
     'peak': {'start': 16.0, 'end': 19.0 },                      # peak period 1
     'peak2': {'start': 0.0, 'end': 0.0 },                       # peak period 2
     'forecast_times': [22, 23],                                 # hours in a day to get a forecast
+    'strategy': [
+        {'start': 0.0, 'end': 2.0, 'mode': 'Feedin'},
+        {'start': 5.0, 'end': 6.0, 'mode': 'SelfUse'},
+        {'start': 16.0, 'end': 24.0, 'mode': 'Feedin'}]
     }
 
+
 # time periods for Intelligent Octopus
 intelligent_octopus = {
     'name': 'Intelligent Octopus',
     'off_peak1': {'start': 23.5, 'end': 5.5, 'force': 1},
     'off_peak2': {'start': 0.0, 'end': 0.0, 'force': 0},
     'peak': {'start': 0.0, 'end': 0.0 },
     'peak2': {'start': 0.0, 'end': 0.0 },
@@ -1893,33 +1898,15 @@
 tariff_list = [octopus_flux, intelligent_octopus, octopus_cosy, octopus_go, agile_octopus, bg_driver, economy_7, custom_periods]
 tariff = octopus_flux
 
 ##################################################################################################
 # Strategy - schedule templates
 ##################################################################################################
 
-# summer strategy for Flux
-flux_strategy_1 = [
-        {'start': 5, 'end': 6, 'mode': 'SelfUse'},
-        {'start': 16, 'end': 24, 'mode': 'Feedin'}]
-
-# winter strategy for Flux
-flux_strategy_2 = [
-        {'start': 2, 'end': 4, 'mode': 'ForceCharge'},
-        {'start': 5, 'end': 6, 'mode': 'SelfUse'},
-        {'start': 16, 'end': 24, 'mode': 'Feedin'}]
-
-# revenue strategy for Flux
-flux_strategy_3 = [
-        {'start': 2, 'end': 4, 'mode': 'ForceCharge'},
-        {'start': 5, 'end': 6, 'mode': 'SelfUse'},
-        {'start': 16, 'end': 18, 'mode': 'ForceDischarge', 'fdsoc': 35, 'fdpwr': 6000},
-        {'start': 18, 'end': 24, 'mode': 'Feedin'}]
-
-flux_strategy_x = [
+test_strategy = [
         {'start': 2, 'end': 11, 'mode': 'SelfUse', 'min_soc': 80},
         {'start': 11, 'end': 14, 'mode': 'SelfUse', 'min_soc': 10},
         {'start': 16, 'end': 24, 'mode': 'Feedin'}]
 
 # return an updated strategy from the tariff strategy that has been filtered for charge times:
 def get_strategy(use=None, strategy=None, min_soc=10, quiet=1):
     global tariff
```

### Comparing `foxesscloud-2.2.8/src/foxesscloud.egg-info/PKG-INFO` & `foxesscloud-2.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: foxesscloud
-Version: 2.2.8
-Summary: library for accessing Fox ESS cloud data using Open API
-Author-email: Tony Matthews <tony@quasair.co.uk>
-Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
-Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENCE
-
 # FoxESS-Cloud
 
 <a href="https://www.buymeacoffee.com/tonym1958" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174" align="right"></a>
 This site contains sample python code for accessing the Fox cloud data via the REST API used by the Fox ESS Cloud web site and app.
 
 There is also a number of Jupyter Lab notebooks with examples of how to run the sample code.
 
@@ -460,15 +446,15 @@
 ```
 
 ## Tariffs
 
 Tariffs configure when your battery can be charged and provide time of use (TOU) periods to split your grid import and export into peak, off-peak and shoulder times when data is uploaded to PV Ouptut.
 
 There are a number of different pre-configured tariffs:
-+ Octopus Flux: off-peak from 02:00 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59. Timed work mode change to Self Use at 7am and Feed In First at 4pm.
++ Octopus Flux: off-peak from 02:00 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59. Timed work mode changes to Self Use at 5am and Feed In First at 4pm.
 + Intelligent Octopus: off-peak from 23:30 to 05:30, forecasts from 22:00 to 23:59
 + Octopus Cosy: off-peak from 04:00 to 07:00 and 13:00 to 16:00, peak from 16:00 to 19:00, forecasts from 02:00 to 03:59 and 12:00 to 12:59
 + Octopus Go: off peak from 00:30 to 04:30, forecasts from 22:00 to 23:59
 + Agile Octopus: off-peak from 02:30 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59
 + British Gas Electric Driver: off-peak from 00:00 to 05:00, forecasts from 22:00 to 23:59
 + Eco 7: Economy 7: off-peak from 00:30 to 07:30 GMT (01:30 to 08:30 during BST)
 
@@ -538,19 +524,14 @@
 + times=[("23:00", "8:00", 3), ("12:00", "16:00", 1)]
 
 'strategy' allows you to configure times when work modes will be changed. The format is a list of dictionary items, containing:
 + 'start', 'end': times in decimal hours or time format. The end time is exclusive so setting an end time of '07:00' will set a schedule that ends at '06:59'
 + 'mode': the work mode to be used from 'SelfUse', 'Feedin', 'Backup', 'ForceCharge', 'ForceDischarge'
 + 'min_soc, 'fdsoc', 'fdpwr': optional values for each work mode. The defaults are 10, 10 and 0 respectively.
 
-There are a number of pre-defined strategies:
-+ f.flux_strategy_1: switch to self use at 5am and feed in first at 4pm.
-+ f.flux_strategy_2: as above with force charge between 2am and 4am. Move the AM charge period between 4am and 5am when using this.
-+ f.flux_strategy_3: as above with force discharge between 4pm and 6pm at 6kW with fdsoc at 35%
-
 ```
 f.get_strategy()
 ```
 
 get_strategy() creates a list of time segments from the strategy. If strategy is not provided, it uses the strategy for the current tariff. If a strategy includes settings for the AM/PM charge times for the tariff, the times will be moved so they do not conflict with the charge time used by charge_needed().
 
 
@@ -695,15 +676,16 @@
 + 1: information reporting (default)
 + 2: more debug information, updating of inverter settings is disabled
 + 3: internal variables and values are displayed (verbose)
 
 
 # Version Info
 
-2.2.8<br>
+2.2.9<br>
+Fix typo in charge_periods() that caused error with timed_mode=2
 ** breaking change ** rename 'groups' to 'periods' for consistency between foxesscloud and openapi.
 Updated management of battery reserve and float charging in charge_needed().
 Added Reserve level to charts in charge_needed().
 Changed bms_power setting to 50W.
 Updated contingency to allow seasonal values for winter, spring, summer and autumn.
 Update strategy mode to support ForceCharge and ForceDischarge work modes.
 Update so min_soc setting in charge_needed() over-rides min_soc in the tariff strategy.
```

#### html2text {}

```diff
@@ -1,16 +1,9 @@
-Metadata-Version: 2.1 Name: foxesscloud Version: 2.2.8 Summary: library for
-accessing Fox ESS cloud data using Open API Author-email: Tony Matthews
-quasair.co.uk> Project-URL: Homepage, https://github.com/TonyM1958/FoxESS-Cloud
-Project-URL: Bug Tracker, https://github.com/TonyM1958/FoxESS-Cloud/issues
-Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
-Approved :: MIT License Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7 Description-Content-Type: text/markdown License-File:
-LICENCE # FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code
-for accessing the Fox cloud data via the REST API used by the Fox ESS Cloud web
+# FoxESS-Cloud _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]This site contains sample python code for
+accessing the Fox cloud data via the REST API used by the Fox ESS Cloud web
 site and app. There is also a number of Jupyter Lab notebooks with examples of
 how to run the sample code. This project is not endorsed by, directly
 affiliated with, maintained, authorized, or sponsored by Fox ESS. Please refer
 to the [LICENCE](https://github.com/TonyM1958/FoxESS-Cloud/blob/main/LICENCE)
 for information on copyright, permissions and warranty. # Open API This module
 builds on the Fox Open API to provide a sample code and utilities that can be
 used with your inverter and batteries. + Information on the API can be found
@@ -334,15 +327,15 @@
 include minutes, ss = include seconds, day = include /n for day when hours > 24
 f.hours_in(h, {'start': a, 'end': b}) # True if decimal hour h is in the time
 period a -> b ``` ## Tariffs Tariffs configure when your battery can be charged
 and provide time of use (TOU) periods to split your grid import and export into
 peak, off-peak and shoulder times when data is uploaded to PV Ouptut. There are
 a number of different pre-configured tariffs: + Octopus Flux: off-peak from 02:
 00 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59. Timed
-work mode change to Self Use at 7am and Feed In First at 4pm. + Intelligent
+work mode changes to Self Use at 5am and Feed In First at 4pm. + Intelligent
 Octopus: off-peak from 23:30 to 05:30, forecasts from 22:00 to 23:59 + Octopus
 Cosy: off-peak from 04:00 to 07:00 and 13:00 to 16:00, peak from 16:00 to 19:
 00, forecasts from 02:00 to 03:59 and 12:00 to 12:59 + Octopus Go: off peak
 from 00:30 to 04:30, forecasts from 22:00 to 23:59 + Agile Octopus: off-peak
 from 02:30 to 05:00, peak from 16:00 to 19:00, forecasts from 22:00 to 23:59 +
 British Gas Electric Driver: off-peak from 00:00 to 05:00, forecasts from 22:00
 to 23:59 + Eco 7: Economy 7: off-peak from 00:30 to 07:30 GMT (01:30 to 08:30
@@ -401,114 +394,111 @@
 between 12 noon and 4pm with a 1 hour period: + times=[("23:00", "8:00", 3),
 ("12:00", "16:00", 1)] 'strategy' allows you to configure times when work modes
 will be changed. The format is a list of dictionary items, containing: +
 'start', 'end': times in decimal hours or time format. The end time is
 exclusive so setting an end time of '07:00' will set a schedule that ends at
 '06:59' + 'mode': the work mode to be used from 'SelfUse', 'Feedin', 'Backup',
 'ForceCharge', 'ForceDischarge' + 'min_soc, 'fdsoc', 'fdpwr': optional values
-for each work mode. The defaults are 10, 10 and 0 respectively. There are a
-number of pre-defined strategies: + f.flux_strategy_1: switch to self use at
-5am and feed in first at 4pm. + f.flux_strategy_2: as above with force charge
-between 2am and 4am. Move the AM charge period between 4am and 5am when using
-this. + f.flux_strategy_3: as above with force discharge between 4pm and 6pm at
-6kW with fdsoc at 35% ``` f.get_strategy() ``` get_strategy() creates a list of
-time segments from the strategy. If strategy is not provided, it uses the
-strategy for the current tariff. If a strategy includes settings for the AM/PM
-charge times for the tariff, the times will be moved so they do not conflict
-with the charge time used by charge_needed(). # PV Output These functions
-produce CSV data for upload to [pvoutput.org](https://pvoutput.org) including
-PV generation, Export, Load and Grid consumption by day in Wh. The functions
-use the energy estimates created from the raw power data (see above). The
-estimates include PV energy generation that are not otherwise available from
-the Fox Cloud. Typically, the energy results are within 3% of the values
-reported by the meters built into the inverter. ## Get PV Output Data Returns
-CSV upload data using the [API format](https://pvoutput.org/help/
-api_specification.html#csv-data-parameter): ``` f.get_pvoutput(d, tou) ``` + d
-is the date or a list of dates, to get data for. The default is yesterday +
-tou: optional, setting tou=1 uploads data with time of use. The default, tou=0
-does not split data and is more accurate. You can copy and paste the output
-data to the pvoutput data CSV Loader, using the following settings: ![image]
-(https://github.com/TonyM1958/FoxESS-Cloud/assets/63789168/21459cdc-a943-4e9d-
-a204-7efd45a422d8) For example, this Jupyer Lab cell will provide a CSV data
-upload for June 2023: ``` f.get_pvoutput(f.date_list('2023-06-01', '2023-06-
-30')) ``` ## Set PV Output Data Loads CSV data directly using the PV Ouput API:
-``` f.set_pvoutput(d, system_id, tou, push) ``` + d is optional and is the
-date, or a list of dates, to upload + system_id is optional and allow you to
-select where data is uploaded to (where you have more than 1 registered system)
-+ tou: optional, setting tou=1 uploads data with time of use. The default,
-tou=0 does not split data and is more accurate + push: optional. 0 = do not
-sent to pushover, 1 = send summary to pushover, 2 = send first day summary only
-# Solar Forecasting # Solcast Get and display solar data from your solcast.com
-account using your API key: ``` f.solcast_api_key = "my.solcast_api_key" fcast
-= f.Solcast() print(fcast) ``` Returns a 7 day forecast. Optional parameters
-are: + days: number of days to get. The default is 7 + estimated: whether to
-get history / estimated data. 1 = yes, 0 = no. Default is 0. + reload: cached
-data handling. 0 = use saved data, 1 = fetch new data, 2 = use saved data for
-today (default) + quiet: True to stop Solcast producing progress messages
-Forecast data is saved to f.solcast_save. The default is 'solcast.txt'. ```
-fcast.plot_daily() fcast.plot_hourly(day) ``` Plots the estimate / forecast
-data. plot_daily() plots the daily yield. plot_hourly() plots each day
-separately. + day: optional. 'today', 'tomorrow', 'all' or a specific list of
-dates. The default is to plot today and tomorrow # Forecast.solar Get and
-display solar data from forecast.solar for today and tomorrow: ```
-f.solar_array('South', lat=51.1789, lon=-1.8262, kwp=6.4) ``` You need to
-configure your solar arrays by calling f.solar_array(). This takes the
-following parameters: + name: the name of each of your arrays + lat: the
-latitude where the array is located. The default is Stonehenge. + lon: the
-longitude where the array is located. The default is Stonehenge. + dec: the
-declination of the array - 0 is lying flat and 90 is vertical. Default is 30 +
-az: azimuth of the array. 0 is pointing due South, -90 is pointing East, 90 is
-pointing West. The default is 0 + kwp: the size of the array in kWp. The
-default is 5kWp + dam: damping factor. Default is None + inv: inverter power
-limit (when the array will clip). The default is None + hor: a list of values
-describing obstructions on the horizon Add one array for each string attached
-to your inverter. If your solar production is limited by clipping, set the
-inverter power so the forecast better matches your generation. See the [API
-documentation](https://doc.forecast.solar/api) for more information on
-parameter values. ``` fcast = f.Solar() print(fcast) ``` Returns a forecast for
-today and tomorrow. Optional parameters are: + reload: cached data handling. 0
-= use saved data, 1 = fetch new data, 2 = use saved data for today (default) +
-quiet: set to True to stop Solar producing progress messages Forecast data is
-saved to f.solar_save. The default is 'solar.txt'. ``` fcast.plot_daily()
+for each work mode. The defaults are 10, 10 and 0 respectively. ```
+f.get_strategy() ``` get_strategy() creates a list of time segments from the
+strategy. If strategy is not provided, it uses the strategy for the current
+tariff. If a strategy includes settings for the AM/PM charge times for the
+tariff, the times will be moved so they do not conflict with the charge time
+used by charge_needed(). # PV Output These functions produce CSV data for
+upload to [pvoutput.org](https://pvoutput.org) including PV generation, Export,
+Load and Grid consumption by day in Wh. The functions use the energy estimates
+created from the raw power data (see above). The estimates include PV energy
+generation that are not otherwise available from the Fox Cloud. Typically, the
+energy results are within 3% of the values reported by the meters built into
+the inverter. ## Get PV Output Data Returns CSV upload data using the [API
+format](https://pvoutput.org/help/api_specification.html#csv-data-parameter):
+``` f.get_pvoutput(d, tou) ``` + d is the date or a list of dates, to get data
+for. The default is yesterday + tou: optional, setting tou=1 uploads data with
+time of use. The default, tou=0 does not split data and is more accurate. You
+can copy and paste the output data to the pvoutput data CSV Loader, using the
+following settings: ![image](https://github.com/TonyM1958/FoxESS-Cloud/assets/
+63789168/21459cdc-a943-4e9d-a204-7efd45a422d8) For example, this Jupyer Lab
+cell will provide a CSV data upload for June 2023: ``` f.get_pvoutput
+(f.date_list('2023-06-01', '2023-06-30')) ``` ## Set PV Output Data Loads CSV
+data directly using the PV Ouput API: ``` f.set_pvoutput(d, system_id, tou,
+push) ``` + d is optional and is the date, or a list of dates, to upload +
+system_id is optional and allow you to select where data is uploaded to (where
+you have more than 1 registered system) + tou: optional, setting tou=1 uploads
+data with time of use. The default, tou=0 does not split data and is more
+accurate + push: optional. 0 = do not sent to pushover, 1 = send summary to
+pushover, 2 = send first day summary only # Solar Forecasting # Solcast Get and
+display solar data from your solcast.com account using your API key: ```
+f.solcast_api_key = "my.solcast_api_key" fcast = f.Solcast() print(fcast) ```
+Returns a 7 day forecast. Optional parameters are: + days: number of days to
+get. The default is 7 + estimated: whether to get history / estimated data. 1 =
+yes, 0 = no. Default is 0. + reload: cached data handling. 0 = use saved data,
+1 = fetch new data, 2 = use saved data for today (default) + quiet: True to
+stop Solcast producing progress messages Forecast data is saved to
+f.solcast_save. The default is 'solcast.txt'. ``` fcast.plot_daily()
 fcast.plot_hourly(day) ``` Plots the estimate / forecast data. plot_daily()
 plots the daily yield. plot_hourly() plots each day separately. + day:
 optional. 'today', 'tomorrow', 'all' or a specific list of dates. The default
-is to plot today and tomorrow # Pushover Send messages to a pushover user
-account: ``` f.output_spool(app_key, h) f.output(s) f.output_close(plot, file)
-f.output_message(app_key, message, plot) ``` Calling f.output_spool() with an
-app key will start the system spooling output to send to pushover. h is an
-optional header to add as the first line of the message. H may include \
+is to plot today and tomorrow # Forecast.solar Get and display solar data from
+forecast.solar for today and tomorrow: ``` f.solar_array('South', lat=51.1789,
+lon=-1.8262, kwp=6.4) ``` You need to configure your solar arrays by calling
+f.solar_array(). This takes the following parameters: + name: the name of each
+of your arrays + lat: the latitude where the array is located. The default is
+Stonehenge. + lon: the longitude where the array is located. The default is
+Stonehenge. + dec: the declination of the array - 0 is lying flat and 90 is
+vertical. Default is 30 + az: azimuth of the array. 0 is pointing due South, -
+90 is pointing East, 90 is pointing West. The default is 0 + kwp: the size of
+the array in kWp. The default is 5kWp + dam: damping factor. Default is None +
+inv: inverter power limit (when the array will clip). The default is None +
+hor: a list of values describing obstructions on the horizon Add one array for
+each string attached to your inverter. If your solar production is limited by
+clipping, set the inverter power so the forecast better matches your
+generation. See the [API documentation](https://doc.forecast.solar/api) for
+more information on parameter values. ``` fcast = f.Solar() print(fcast) ```
+Returns a forecast for today and tomorrow. Optional parameters are: + reload:
+cached data handling. 0 = use saved data, 1 = fetch new data, 2 = use saved
+data for today (default) + quiet: set to True to stop Solar producing progress
+messages Forecast data is saved to f.solar_save. The default is 'solar.txt'.
+``` fcast.plot_daily() fcast.plot_hourly(day) ``` Plots the estimate / forecast
+data. plot_daily() plots the daily yield. plot_hourly() plots each day
+separately. + day: optional. 'today', 'tomorrow', 'all' or a specific list of
+dates. The default is to plot today and tomorrow # Pushover Send messages to a
+pushover user account: ``` f.output_spool(app_key, h) f.output(s)
+f.output_close(plot, file) f.output_message(app_key, message, plot) ``` Calling
+f.output_spool() with an app key will start the system spooling output to send
+to pushover. h is an optional header to add as the first line of the message. H
+may include \
 >, \
 > or \
 > and these will be set to current system time and date respectively. When
 spooling is active, any calls to f.output() add lines to the spooled message.
 If appending to the message would exceed 1024 characters, the existing spooled
 message is sent and a new message spool is started. Calling f.output_close()
 will send the spooled message and optionally attach a binary image file. You
 can set plot=1 to attach the last plot file created (when f.plot_file is set)
 or specify a file. f.output_message() is a shorcut to send a message without
 spooling output. # Troubleshooting If needed, you can add the following setting
 to increase the level of information reported by the foxesscloud module: ```
 f.debug_setting = 2 ``` This setting can be: + 0: silent mode (minimal output)
 + 1: information reporting (default) + 2: more debug information, updating of
 inverter settings is disabled + 3: internal variables and values are displayed
-(verbose) # Version Info 2.2.8
-** breaking change ** rename 'groups' to 'periods' for consistency between
-foxesscloud and openapi. Updated management of battery reserve and float
-charging in charge_needed(). Added Reserve level to charts in charge_needed().
-Changed bms_power setting to 50W. Updated contingency to allow seasonal values
-for winter, spring, summer and autumn. Update strategy mode to support
-ForceCharge and ForceDischarge work modes. Update so min_soc setting in
-charge_needed() over-rides min_soc in the tariff strategy. Fix force charge
-strategy mode in charge_neded() to set min_soc correctly. Implement 2 second
-delay between calls that change inverter settings. Added strategy mode
-(timed_mode=2) to charge_needed(). Added set_strategy() and charge_strategy()
-to manage charging schedules and work mode changes. Refactor debug messaging.
-Simplify charge_needed() output. Added 'target_soc' to charge_needed() settings
-Fix bat_info() giving incorrect temperatures when API returns 0 instead of -50
+(verbose) # Version Info 2.2.9
+Fix typo in charge_periods() that caused error with timed_mode=2 ** breaking
+change ** rename 'groups' to 'periods' for consistency between foxesscloud and
+openapi. Updated management of battery reserve and float charging in
+charge_needed(). Added Reserve level to charts in charge_needed(). Changed
+bms_power setting to 50W. Updated contingency to allow seasonal values for
+winter, spring, summer and autumn. Update strategy mode to support ForceCharge
+and ForceDischarge work modes. Update so min_soc setting in charge_needed()
+over-rides min_soc in the tariff strategy. Fix force charge strategy mode in
+charge_neded() to set min_soc correctly. Implement 2 second delay between calls
+that change inverter settings. Added strategy mode (timed_mode=2) to
+charge_needed(). Added set_strategy() and charge_strategy() to manage charging
+schedules and work mode changes. Refactor debug messaging. Simplify
+charge_needed() output. Added 'target_soc' to charge_needed() settings Fix
+bat_info() giving incorrect temperatures when API returns 0 instead of -50
 where there is no battery Fix key error when accessing cell volts and temps
 using an agent / installer account. Ensure output is generated if get_battery()
 fails using battery_info(). Update f.avg() to include calculation of averages
 in lists containng None values. Added 'data_wrap' to charge_config. 2.1.9
 Update get_history() to use GMT or BST when plotting instead of mixed time
 zones. Added 'economy_7' tariff that charges using GMT when clocks change.
 Updated charge / discharge profiles for charge_needed() to show power flow in
```

