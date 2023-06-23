# Comparing `tmp/pyThorlabsTC300-0.2.tar.gz` & `tmp/pyThorlabsTC300-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyThorlabsTC300-0.2.tar", last modified: Thu Jun  8 23:07:40 2023, max compression
+gzip compressed data, was "pyThorlabsTC300-0.3.tar", last modified: Fri Jun 23 22:17:07 2023, max compression
```

## Comparing `pyThorlabsTC300-0.2.tar` & `pyThorlabsTC300-0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 23:07:40.337226 pyThorlabsTC300-0.2/
--rw-rw-rw-   0        0        0       97 2023-06-08 23:07:04.000000 pyThorlabsTC300-0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     7592 2023-06-08 23:07:40.336222 pyThorlabsTC300-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     7263 2022-10-06 04:44:02.000000 pyThorlabsTC300-0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 23:07:40.194221 pyThorlabsTC300-0.2/pyThorlabsTC300/
--rw-rw-rw-   0        0        0   258560 2021-12-03 07:56:46.000000 pyThorlabsTC300-0.2/pyThorlabsTC300/TC300COMMANDLIB_win32.dll
--rw-rw-rw-   0        0        0   312832 2021-12-03 07:56:46.000000 pyThorlabsTC300-0.2/pyThorlabsTC300/TC300COMMANDLIB_win64.dll
--rw-rw-rw-   0        0        0    40834 2023-06-07 20:01:07.000000 pyThorlabsTC300-0.2/pyThorlabsTC300/TC300_COMMAND_LIB.py
--rw-rw-rw-   0        0        0    17045 2021-12-03 07:56:46.000000 pyThorlabsTC300-0.2/pyThorlabsTC300/TC300_COMMAND_LIB_EXAMPLE.py
--rw-rw-rw-   0        0        0      330 2022-10-03 21:45:25.000000 pyThorlabsTC300-0.2/pyThorlabsTC300/__init__.py
--rw-rw-rw-   0        0        0      405 2023-06-08 20:59:24.000000 pyThorlabsTC300-0.2/pyThorlabsTC300/config.json
--rw-rw-rw-   0        0        0     9437 2023-06-08 04:34:41.000000 pyThorlabsTC300-0.2/pyThorlabsTC300/driver.py
-drwxrwxrwx   0        0        0        0 2023-06-08 23:07:40.264529 pyThorlabsTC300-0.2/pyThorlabsTC300/graphics/
--rw-rw-rw-   0        0        0     7799 2021-08-31 16:42:47.000000 pyThorlabsTC300-0.2/pyThorlabsTC300/graphics/pause.png
--rw-rw-rw-   0        0        0     9320 2021-08-31 16:41:38.000000 pyThorlabsTC300-0.2/pyThorlabsTC300/graphics/play.png
--rw-rw-rw-   0        0        0     3439 2021-08-29 03:28:31.000000 pyThorlabsTC300-0.2/pyThorlabsTC300/graphics/refresh.png
--rw-rw-rw-   0        0        0     7522 2021-08-31 16:43:00.000000 pyThorlabsTC300-0.2/pyThorlabsTC300/graphics/stop.png
--rw-rw-rw-   0        0        0    48530 2023-06-08 20:39:00.000000 pyThorlabsTC300-0.2/pyThorlabsTC300/main.py
-drwxrwxrwx   0        0        0        0 2023-06-08 23:07:40.242555 pyThorlabsTC300-0.2/pyThorlabsTC300.egg-info/
--rw-rw-rw-   0        0        0     7592 2023-06-08 23:07:40.000000 pyThorlabsTC300-0.2/pyThorlabsTC300.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      678 2023-06-08 23:07:40.000000 pyThorlabsTC300-0.2/pyThorlabsTC300.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 23:07:40.000000 pyThorlabsTC300-0.2/pyThorlabsTC300.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-06-08 23:07:40.000000 pyThorlabsTC300-0.2/pyThorlabsTC300.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-08 23:04:07.000000 pyThorlabsTC300-0.2/pyThorlabsTC300.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       16 2023-06-08 23:07:40.000000 pyThorlabsTC300-0.2/pyThorlabsTC300.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 23:07:40.338221 pyThorlabsTC300-0.2/setup.cfg
--rw-rw-rw-   0        0        0      982 2023-06-08 23:07:16.000000 pyThorlabsTC300-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-23 22:17:07.025403 pyThorlabsTC300-0.3/
+-rw-rw-rw-   0        0        0       97 2023-06-08 23:07:04.000000 pyThorlabsTC300-0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     7592 2023-06-23 22:17:07.025403 pyThorlabsTC300-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7263 2022-10-06 04:44:02.000000 pyThorlabsTC300-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-23 22:17:06.528277 pyThorlabsTC300-0.3/pyThorlabsTC300/
+-rw-rw-rw-   0        0        0   258560 2021-12-03 07:56:46.000000 pyThorlabsTC300-0.3/pyThorlabsTC300/TC300COMMANDLIB_win32.dll
+-rw-rw-rw-   0        0        0   312832 2021-12-03 07:56:46.000000 pyThorlabsTC300-0.3/pyThorlabsTC300/TC300COMMANDLIB_win64.dll
+-rw-rw-rw-   0        0        0    40834 2023-06-07 20:01:07.000000 pyThorlabsTC300-0.3/pyThorlabsTC300/TC300_COMMAND_LIB.py
+-rw-rw-rw-   0        0        0    17045 2021-12-03 07:56:46.000000 pyThorlabsTC300-0.3/pyThorlabsTC300/TC300_COMMAND_LIB_EXAMPLE.py
+-rw-rw-rw-   0        0        0      330 2022-10-03 21:45:25.000000 pyThorlabsTC300-0.3/pyThorlabsTC300/__init__.py
+-rw-rw-rw-   0        0        0      405 2023-06-23 19:28:12.000000 pyThorlabsTC300-0.3/pyThorlabsTC300/config.json
+-rw-rw-rw-   0        0        0     9437 2023-06-08 04:34:41.000000 pyThorlabsTC300-0.3/pyThorlabsTC300/driver.py
+drwxrwxrwx   0        0        0        0 2023-06-23 22:17:06.963566 pyThorlabsTC300-0.3/pyThorlabsTC300/graphics/
+-rw-rw-rw-   0        0        0     7799 2021-08-31 16:42:47.000000 pyThorlabsTC300-0.3/pyThorlabsTC300/graphics/pause.png
+-rw-rw-rw-   0        0        0     9320 2021-08-31 16:41:38.000000 pyThorlabsTC300-0.3/pyThorlabsTC300/graphics/play.png
+-rw-rw-rw-   0        0        0     3439 2021-08-29 03:28:31.000000 pyThorlabsTC300-0.3/pyThorlabsTC300/graphics/refresh.png
+-rw-rw-rw-   0        0        0     7522 2021-08-31 16:43:00.000000 pyThorlabsTC300-0.3/pyThorlabsTC300/graphics/stop.png
+-rw-rw-rw-   0        0        0    40674 2023-06-23 22:15:26.000000 pyThorlabsTC300-0.3/pyThorlabsTC300/main.py
+drwxrwxrwx   0        0        0        0 2023-06-23 22:17:06.595788 pyThorlabsTC300-0.3/pyThorlabsTC300.egg-info/
+-rw-rw-rw-   0        0        0     7592 2023-06-23 22:17:06.000000 pyThorlabsTC300-0.3/pyThorlabsTC300.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      678 2023-06-23 22:17:06.000000 pyThorlabsTC300-0.3/pyThorlabsTC300.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-23 22:17:06.000000 pyThorlabsTC300-0.3/pyThorlabsTC300.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-06-23 22:17:06.000000 pyThorlabsTC300-0.3/pyThorlabsTC300.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-23 22:17:06.000000 pyThorlabsTC300-0.3/pyThorlabsTC300.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       16 2023-06-23 22:17:06.000000 pyThorlabsTC300-0.3/pyThorlabsTC300.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-23 22:17:07.026400 pyThorlabsTC300-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      982 2023-06-23 22:15:48.000000 pyThorlabsTC300-0.3/setup.py
```

### Comparing `pyThorlabsTC300-0.2/PKG-INFO` & `pyThorlabsTC300-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyThorlabsTC300
-Version: 0.2
+Version: 0.3
 Summary: A python library/GUI to access and control the TC300 Temperature Controller of Thorlabs.
 Home-page: https://github.com/MicheleCotrufo/
 Author: Michele Cotrufo
 Author-email: michele.cotrufo@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `pyThorlabsTC300-0.2/README.md` & `pyThorlabsTC300-0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyThorlabsTC300-0.2/pyThorlabsTC300/TC300COMMANDLIB_win32.dll` & `pyThorlabsTC300-0.3/pyThorlabsTC300/TC300COMMANDLIB_win32.dll`

 * *Files identical despite different names*

### Comparing `pyThorlabsTC300-0.2/pyThorlabsTC300/TC300COMMANDLIB_win64.dll` & `pyThorlabsTC300-0.3/pyThorlabsTC300/TC300COMMANDLIB_win64.dll`

 * *Files identical despite different names*

### Comparing `pyThorlabsTC300-0.2/pyThorlabsTC300/TC300_COMMAND_LIB.py` & `pyThorlabsTC300-0.3/pyThorlabsTC300/TC300_COMMAND_LIB.py`

 * *Files identical despite different names*

### Comparing `pyThorlabsTC300-0.2/pyThorlabsTC300/TC300_COMMAND_LIB_EXAMPLE.py` & `pyThorlabsTC300-0.3/pyThorlabsTC300/TC300_COMMAND_LIB_EXAMPLE.py`

 * *Files identical despite different names*

### Comparing `pyThorlabsTC300-0.2/pyThorlabsTC300/driver.py` & `pyThorlabsTC300-0.3/pyThorlabsTC300/driver.py`

 * *Files identical despite different names*

### Comparing `pyThorlabsTC300-0.2/pyThorlabsTC300/graphics/pause.png` & `pyThorlabsTC300-0.3/pyThorlabsTC300/graphics/pause.png`

 * *Files identical despite different names*

### Comparing `pyThorlabsTC300-0.2/pyThorlabsTC300/graphics/play.png` & `pyThorlabsTC300-0.3/pyThorlabsTC300/graphics/play.png`

 * *Files identical despite different names*

### Comparing `pyThorlabsTC300-0.2/pyThorlabsTC300/graphics/refresh.png` & `pyThorlabsTC300-0.3/pyThorlabsTC300/graphics/refresh.png`

 * *Files identical despite different names*

### Comparing `pyThorlabsTC300-0.2/pyThorlabsTC300/graphics/stop.png` & `pyThorlabsTC300-0.3/pyThorlabsTC300/graphics/stop.png`

 * *Files identical despite different names*

### Comparing `pyThorlabsTC300-0.2/pyThorlabsTC300/main.py` & `pyThorlabsTC300-0.3/pyThorlabsTC300/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -60,36 +60,33 @@
     
         
     update()
         This method also calls the update() method defined in abstract_instrument_interface.abstract_interface
 
     """
 
-    output = {'Power':0}  #We define this also as class variable. This makes it possible to see which data is produced by this interface without having to create an object
+    output = {'T1':0, 'T2':0, 'i1':0, 'i2':0}   #We define this also as class variable. This makes it possible to see which data is produced by this interface without having to create an object
 
     ## SIGNALS THAT WILL BE USED TO COMMUNICATE WITH THE GUI
     #                                                               | Triggered when ...                                        | Parameter(s) Sent     
     #                                                           #   -----------------------------------------------------------------------------------------------------------------------         
     sig_list_devices_updated = QtCore.pyqtSignal(list)          #   | List of devices is updated                                | List of devices   
     sig_channel_mode_changed = QtCore.pyqtSignal(int,int)       #   | The mode of one channel changed (or was read)             | Channel number, Channel mode [0: Heater; 1: Tec; 2: Constant current; 3: Synchronize with Ch1(only for channel 2)]
     sig_temperature_read = QtCore.pyqtSignal(int,float)         #   | The actual tempereature of a channel was read             | Channel number, Actual Temperature
     sig_current_read = QtCore.pyqtSignal(int,float)             #   | The actual current of a channel was read                  | Channel number, Actual Current
     sig_target_temperature_read = QtCore.pyqtSignal(int,float)  #   | The target temperature of a channel was read              | Channel number, Target Temperature
     sig_target_current_read = QtCore.pyqtSignal(int,float)      #   | The target current of a channel was read                  | Channel number, Target Current
     sig_channel_enabled = QtCore.pyqtSignal(int)                #   | A channel has been enabled                                | Channel number
-    sig_enabled_state_change = QtCore.pyqtSignal(int,int)
+    sig_enabled_state_change = QtCore.pyqtSignal(int,int)       #   | A channel has been enabled or disabled                    | Channel number, 1 = Enabled, 0 = Disabled
     sig_change_moving_status = QtCore.pyqtSignal(int)           #   | A step (either of temperature or current) initiated by ramp has started or ended | self.interface.SIG_MOVEMENT_STARTED, self.interface.SIG_MOVEMENT_ENDED
     
     sig_reading = QtCore.pyqtSignal(int)                    #   | Reading status changes                                    | 1 = Started Reading, 2 = Paused Reading, 3 Stopped Reading
     sig_updated_data = QtCore.pyqtSignal(object)            #   | Data is read from instrument                              | Acquired data 
-    sig_wavelength = QtCore.pyqtSignal(int)                 #   | Wavelength is changed                                     | Current Wavelength
-    sig_min_max_wavelength = QtCore.pyqtSignal(int,int)     #   | Min and max wavelengths supported by this device are read | Current Min and max wavelengths
-    sig_refreshtime = QtCore.pyqtSignal(float)              #   | Refresh time is changed                                   | Current Refresh time 
-    sig_power_range = QtCore.pyqtSignal(float)              #   | Power range is changed                                    | Current Power range
-    sig_auto_power_range = QtCore.pyqtSignal(bool)          #   | Auto power range setting is changed                       | Current Status of auto power range (true/false)
+    
+    
     ##
     # Identifier codes used for view-model communication. Other general-purpose codes are specified in abstract_instrument_interface
     SIG_READING_START = 1
     SIG_READING_PAUSE = 2
     SIG_READING_STOP = 3
 
     SIG_MOVEMENT_STARTED = 1
@@ -135,15 +132,15 @@
         super().__init__(**kwargs)
 
         # Setting up the ramp object, which is defined in the package abstract_instrument_interface
         self.ramp = abstract_instrument_interface.ramp(interface=self)  
         self.ramp.set_ramp_settings(self.settings['ramp'])
         self.ramp.set_ramp_functions(func_move = self.increase_target_by,
                                      func_check_step_has_ended = self.step_has_ended, 
-                                     func_trigger = super().update(), 
+                                     func_trigger = super().update, 
                                      func_trigger_continue_ramp = None,
                                      func_set_value = self.set_target_value, 
                                      func_read_current_value = self.get_target_value, 
                                      list_functions_step_not_ended = [],  
                                      list_functions_step_has_ended = [self.read_output_channel],#lambda:self.end_movement(send_signal=False)],  
                                      list_functions_ramp_started = [self.pause_reading],
                                      list_functions_ramp_ended = [self.start_reading])
@@ -386,108 +383,15 @@
         if channel == None: channel = self.channel_controlled_by_ramp
         self.set_target_channel(channel,target)
 
     def step_has_ended(self):
         # This function is used by the ramp to check if a step has ended. For now it is a placeholder and always returns True
         return True
 
-
-    ###
-
-    #def set_wavelength(self, wl):
-    #    try:
-    #        if int(self.instrument.wavelength) == int(float(wl)): #in this case the number in the refresh time edit box is the same as the wavelength currently set
-    #                return True
-    #        self.logger.info(f"Setting the wavelength to {wl} for the device {self.connected_device_name}...")
-    #    except ValueError as e:
-    #        self.logger.error(f"The wavelength must be a valid number.")
-    #        self.sig_wavelength.emit(self.instrument.wavelength)
-    #        return False
-    #    try: 
-    #        self.instrument.wavelength = int(float(wl))
-    #        self.logger.info(f"Wavelength set correctly.")
-    #    except Exception as e:
-    #        self.logger.error(f"An error occurred while setting the wavelength: {e}")
-    #        self.sig_wavelength.emit(self.instrument.wavelength)
-    #        return False
-    #    self.read_power_range() #The boundaries of the power ranges might change when the wavelength is changed, so we need to update it after changing the wavelength
-    #    return True
-  
-    #def read_wavelength(self):
-    #    self.logger.info(f"Reading current wavelength from device {self.connected_device_name}...") 
-    #    self.wavelength = int(self.instrument.wavelength)
-    #    if self.wavelength == None:
-    #        self.logger.error(f"An error occurred while reading the wavelength from this device.")
-    #        return
-    #    self.sig_wavelength.emit(self.instrument.wavelength)
-    #    self.logger.info(f"Current wavelength is {self.wavelength}.") 
-    #    return
-      
-    #def read_min_max_wavelength(self):
-    #    self.logger.info(f"Reading min and max wavelength supported by device {self.connected_device_name}...") 
-    #    self.min_max_wls =  (self.instrument.min_wavelength,self.instrument.max_wavelength)
-    #    self.sig_min_max_wavelength.emit(self.min_max_wls[0],self.min_max_wls[1])
-    #    self.logger.info(f"Wavelength range: {self.min_max_wls[0]}-{self.min_max_wls[1]} nm") 
-
-    #def change_power_range(self,direction):
-    #    if direction == +1:
-    #        string = 'increase'
-    #    else: 
-    #        string = 'decrease'
-    #    self.logger.info(f"Trying to {string} the power range...")
-    #    self.instrument.move_to_next_power_range(direction)
-    #    self.read_power_range()
-    #    return
-
-    #def read_power_range(self):
-    #    self.logger.info(f"Reading current power range from device {self.connected_device_name}...") 
-    #    self.power_range = self.instrument.power_range
-    #    if self.power_range == None:
-    #        self.logger.error(f"An error occurred while reading the power range from this device.")
-    #        return
-    #    self.sig_power_range.emit(self.power_range)
-    #    self.logger.info(f"Current power range is {self.power_range}.") 
-
-    #def set_auto_power_range(self,auto_power_range):
-    #    auto_power_range = bool(auto_power_range)
-    #    status_string = 'ON' if auto_power_range else 'OFF'
-    #    self.logger.info(f"Setting the auto-ranging function to {status_string} for the device {self.connected_device_name}...")    
-    #    try:
-    #        self.instrument.auto_power_range  = auto_power_range
-    #        self.sig_auto_power_range.emit(auto_power_range)
-    #        self.logger.info(f"Setting changed succesfully.")
-    #        self.settings['auto_power_range'] = auto_power_range
-    #    except Exception as e:
-    #        self.logger.error(f"An error occurred while setting the auto-ranging status: {e}")
-    #    #self.read_auto_power_range()
-    #    self.read_power_range()
-
-    #def read_auto_power_range(self):
-    #    self.logger.info(f"Reading the status of the auto-ranging function for the device {self.connected_device_name}...")   
-    #    try:
-    #        auto_power_range = self.instrument.auto_power_range
-    #        status_string = 'ON' if auto_power_range else 'OFF'
-    #        self.sig_auto_power_range.emit(auto_power_range)
-    #        self.logger.info(f"The auto-ranging function is currently set to {status_string}.")
-    #        self.settings['auto_power_range'] = auto_power_range
-    #        return auto_power_range
-    #    except Exception as e:
-    #        self.logger.error(f"An error occurred while reading the auto-ranging status: {e}")
-
-    #def set_zero_powermeter(self):
-    #    try: 
-    #        ID = self.instrument.set_zero()
-    #        self.logger.info(f"Zero-ing the device {self.connected_device_name}...")
-    #        if ID == 1:
-    #            self.logger.info(f"Device was succesfully zeroed.")
-    #        else:
-    #            self.logger.error(f"An error occurred while zero-ing this device.")
-    #    except Exception as e:
-    #        self.logger.error(f"An error occurred while zero-ing this device: {e}")
-    #    return
+    ### END Functions mainly used for interface with ramp
 
     def start_reading(self):
         if(self.instrument.connected == False):
             self.logger.error(f"No device is connected.")
             return
         #self.logger.info(f"Updating wavelength and refresh time before starting reading...")       
         self.sig_reading.emit(self.SIG_READING_START) # This signal will be caught by the GUI
@@ -515,23 +419,17 @@
         
     def update(self):
         '''
 
         '''
         if(self.continuous_read == True):
             self.read_output_channel()
-            #(currentPower,power_units) = self.instrument.power
-            #self.output['Power'] = currentPower
-            #self.power_units = power_units
-            #self.stored_data.append(currentPower)
-            #self.output['PowerUnits'] = power_units
-
-            super().update()    
+  
+            #super().update()    
 
-            #self.sig_updated_data.emit([currentPower, power_units])
             QtCore.QTimer.singleShot(int(self.settings['refresh_time']*1e3), self.update)
            
         return
     
     
 class gui(abstract_instrument_interface.abstract_gui):
      
@@ -559,23 +457,16 @@
         self.interface.sig_temperature_read.connect(self.on_actual_temperature_changed)
         self.interface.sig_current_read.connect(self.on_actual_current_changed)
         self.interface.sig_target_temperature_read.connect(self.on_target_temperature_changed)
         self.interface.sig_target_current_read.connect(self.on_target_current_changed)
         self.interface.sig_enabled_state_change.connect(self.on_enabled_state_change)
         #self.interface.sig_reading.connect(self.on_reading_status_change) 
         #self.interface.sig_updated_data.connect(self.on_data_change) 
-        #self.interface.sig_refreshtime.connect(self.on_refreshtime_change)
-        #self.interface.sig_wavelength.connect(self.on_wavelength_change)
-        #self.interface.sig_min_max_wavelength.connect(self.on_min_max_wavelength_update)
-        #self.interface.sig_auto_power_range.connect(self.on_auto_power_range_change)
-        #self.interface.sig_power_range.connect(self.on_power_range_change)
-        #self.interface.sig_close.connect(self.on_close)
 
         ### SET INITIAL STATE OF WIDGETS
-        #self.edit_RefreshTime.setText(f"{self.interface.settings['refresh_time']:.3f}")
         self.interface.send_list_devices()  
         #self.on_connection_status_change(self.interface.SIG_DISCONNECTED) #When GUI is created, all widgets are set to the "Disconnected" state              
         ###
 
     def create_panel_channel(self,channel_name = 'CH'):
 
         QGroupBoxStyle = """ {
@@ -774,37 +665,19 @@
     #    #Data is (in this case) a string
     #    current_power_string = f"{data[0]:.2e}" + ' ' +  data[1]
     #    self.edit_Power.setText(current_power_string)
 
     #def on_refreshtime_change(self,value):
     #    self.edit_RefreshTime.setText(f"{value:.3f}")
 
-    #def on_wavelength_change(self,value):
-    #    self.edit_Wavelength.setText(str(int(value)))
-
-    #def on_min_max_wavelength_update(self,min,max):
-    #    self.label_Wavelength.setText(f"Wavelength<br>(<b>{min}-{max}</b>): ")
     
-    #def on_power_range_change(self,value):
-    #    self.edit_PowerRange.setText(f"{value:.2e}")
-    #    self.edit_PowerRange.setCursorPosition(1)
-
-    #def on_auto_power_range_change(self,value):
-    #    self.set_auto_power_range_state(value)
-    #    self.box_PowerRangeAuto.setChecked(value)
 
     #def on_close(self):
     #    return
 
-    #def set_auto_power_range_state(self,auto_power_range):
-    #    if auto_power_range:
-    #        self.disable_widget([self.edit_PowerRange,self.button_IncreasePowerRange, self.button_DecreasePowerRange])
-    #    else:
-    #        self.enable_widget([self.edit_PowerRange,self.button_IncreasePowerRange, self.button_DecreasePowerRange])
-
 #######################
 ### END Event Slots ###
 #######################
 
             
 ###################################################################################################################################################
 ### GUI Events Functions. They are triggered by direct interaction with the GUI, and they call methods of the interface (i.e. the model) object.###
@@ -829,29 +702,14 @@
         mode = keys[0]
         self.interface.set_mode_channel(channel,mode)
 
     def press_enter_edit_target(self,channel):
         target = self.widgets_channels[channel]['edit_target'].text()
         self.interface.set_target_channel(channel,target)
 
-    #def click_box_PowerRangeAuto(self, state):
-    #    if state == QtCore.Qt.Checked:
-    #        status_bool = True
-    #    else:
-    #        status_bool = False
-    #    self.interface.set_auto_power_range(status_bool)
-
-    #def click_button_set_zero_powermeter(self):
-    #    self.interface.set_zero_powermeter()
-
-    #def press_enter_wavelength(self):
-    #    return self.interface.set_wavelength(self.edit_Wavelength.text())
-        
-    #def click_button_change_power_range(self,direction):
-    #    self.interface.change_power_range(direction)
        
     #def click_button_StartPauseReading(self): 
     #    if(self.interface.continuous_read == False):
     #        if not(self.press_enter_refresh_time()): #read the current value in the refresh_time textbox, and validates it. The function returns True/False if refresh_time was valid
     #            return
     #        if not(self.press_enter_wavelength()): #read the current value in the wavelength textbox, and validates it. The function returns True/False if refresh_time was valid
     #            return
```

### Comparing `pyThorlabsTC300-0.2/pyThorlabsTC300.egg-info/PKG-INFO` & `pyThorlabsTC300-0.3/pyThorlabsTC300.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyThorlabsTC300
-Version: 0.2
+Version: 0.3
 Summary: A python library/GUI to access and control the TC300 Temperature Controller of Thorlabs.
 Home-page: https://github.com/MicheleCotrufo/
 Author: Michele Cotrufo
 Author-email: michele.cotrufo@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
```

### Comparing `pyThorlabsTC300-0.2/pyThorlabsTC300.egg-info/SOURCES.txt` & `pyThorlabsTC300-0.3/pyThorlabsTC300.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyThorlabsTC300-0.2/setup.py` & `pyThorlabsTC300-0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open(path.join(this_directory, 'README.md'),encoding ='unicode_escape') as f:
     long_description = f.read()
 
 with open("requirements_strict.txt") as f:
     required_packages = f.read().splitlines()
 
 setuptools.setup(name='pyThorlabsTC300',
-      version='0.2',
+      version='0.3',
       description='A python library/GUI to access and control the TC300 Temperature Controller of Thorlabs.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/MicheleCotrufo/',
       author='Michele Cotrufo',
       author_email='michele.cotrufo@gmail.com',
       license='MIT',
```

