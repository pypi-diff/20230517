# Comparing `tmp/iosense_connect-2.1.4.tar.gz` & `tmp/iosense_connect-2.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iosense_connect-2.1.4.tar", last modified: Tue May 16 09:02:39 2023, max compression
+gzip compressed data, was "dist\iosense_connect-2.1.5.tar", last modified: Tue May 16 12:53:46 2023, max compression
```

## Comparing `iosense_connect-2.1.4.tar` & `iosense_connect-2.1.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-16 09:02:39.244596 iosense_connect-2.1.4/
--rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-2.1.4/LICENSE.txt
--rw-rw-rw-   0        0        0     1062 2023-05-16 09:02:39.242421 iosense_connect-2.1.4/PKG-INFO
--rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-2.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-16 09:02:39.199251 iosense_connect-2.1.4/iosense_connect/
--rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-2.1.4/iosense_connect/__init__.py
--rw-rw-rw-   0        0        0    22624 2023-05-16 08:48:38.000000 iosense_connect-2.1.4/iosense_connect/data_access.py
-drwxrwxrwx   0        0        0        0 2023-05-16 09:02:39.238157 iosense_connect-2.1.4/iosense_connect.egg-info/
--rw-rw-rw-   0        0        0     1062 2023-05-16 09:02:38.000000 iosense_connect-2.1.4/iosense_connect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-05-16 09:02:38.000000 iosense_connect-2.1.4/iosense_connect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-16 09:02:38.000000 iosense_connect-2.1.4/iosense_connect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-16 09:02:38.000000 iosense_connect-2.1.4/iosense_connect.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-16 09:02:39.244596 iosense_connect-2.1.4/setup.cfg
--rw-rw-rw-   0        0        0      614 2023-05-15 07:38:32.000000 iosense_connect-2.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:53:46.589329 iosense_connect-2.1.5/
+-rw-rw-rw-   0        0        0     1087 2023-04-28 09:03:25.000000 iosense_connect-2.1.5/LICENSE.txt
+-rw-rw-rw-   0        0        0     1062 2023-05-16 12:53:46.586773 iosense_connect-2.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      690 2023-04-28 09:03:25.000000 iosense_connect-2.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 12:53:46.500384 iosense_connect-2.1.5/iosense_connect/
+-rw-rw-rw-   0        0        0       37 2023-03-23 09:15:17.000000 iosense_connect-2.1.5/iosense_connect/__init__.py
+-rw-rw-rw-   0        0        0    23452 2023-05-16 12:53:40.000000 iosense_connect-2.1.5/iosense_connect/data_access.py
+drwxrwxrwx   0        0        0        0 2023-05-16 12:53:46.581457 iosense_connect-2.1.5/iosense_connect.egg-info/
+-rw-rw-rw-   0        0        0     1062 2023-05-16 12:53:46.000000 iosense_connect-2.1.5/iosense_connect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-05-16 12:53:46.000000 iosense_connect-2.1.5/iosense_connect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 12:53:46.000000 iosense_connect-2.1.5/iosense_connect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-16 12:53:46.000000 iosense_connect-2.1.5/iosense_connect.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-16 12:53:46.591335 iosense_connect-2.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      614 2023-05-16 12:53:40.000000 iosense_connect-2.1.5/setup.py
```

### Comparing `iosense_connect-2.1.4/LICENSE.txt` & `iosense_connect-2.1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `iosense_connect-2.1.4/PKG-INFO` & `iosense_connect-2.1.5/iosense_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: iosense_connect
-Version: 2.1.4
+Name: iosense-connect
+Version: 2.1.5
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-2.1.4/README.md` & `iosense_connect-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `iosense_connect-2.1.4/iosense_connect/data_access.py` & `iosense_connect-2.1.5/iosense_connect/data_access.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,16 +50,18 @@
         for (value1, value2) in zip(sensor_id_list, sensor_name_list):
             df_meta = pd.DataFrame(data[str(value1)])
             df_meta = df_meta.set_index('paramName').transpose()
 
             if 'm' in df_meta.columns and 'c' in df_meta.columns:
                 m = float(df_meta.iloc[0]['m'])
                 c = int(str(df_meta.iloc[0]['c']).replace(',',''))
+
                 df[str(value2)] = df[str(value2)].replace('BAD 255', '-99999').replace('-', '99999').replace(
-                    'BAD undefined', '-99999').replace('BAD 0', '-99999')
+                    'BAD undefined', '-99999').replace('BAD 0', '-99999').replace('true',True).replace('false',False)
+
                 df[str(value2)] = df[str(value2)].astype('float')
                 df[str(value2)] = (df[str(value2)] * m) + c
                 if 'min' in df_meta.columns:
                     min = int(df_meta.iloc[0]['min'])
                     df[str(value2)] = np.where(df[str(value2)] <= min, min, df[str(value2)])
                 if 'max' in df_meta.columns:
                     max = int(str(df_meta.iloc[0]['max']).replace('-', '99999').replace(
@@ -373,26 +375,35 @@
         If requested data exists in feature store fetch data from the container.
         IF data is not available the data is fetched from influxdb
 
         """
         try:
             df = pd.DataFrame()
             metadata = {}
-            connection_string = self.connection_string
-            blob_svc = BlobServiceClient.from_connection_string(conn_str=connection_string)
+            folder_path = f"{device_id}/"
+            blob_svc = BlobServiceClient.from_connection_string(conn_str=self.connection_string)
+            container_client = blob_svc.get_container_client(self.container_name)
+            processed_blobs = [blob.name[len(folder_path):].lstrip("/").rsplit(".", 1)[0].split("-") for blob in
+                               container_client.list_blobs(name_starts_with=folder_path)]
+            sorted_blobs = sorted(processed_blobs, key=lambda x: (int(x[1]), int(x[0])))
+
+            date_month_list = []
+            for month, year in sorted_blobs:
+                val = f"{month}-{year}"
+                date_month_list.append(val)
 
             def check_device(device_id):
                 flag = False
-                container_client = blob_svc.get_container_client(self.container_name)
                 blob_list = container_client.list_blobs()
                 for blob in blob_list:
                     split_text = blob.name.split('/')
                     if device_id == split_text[0]:
                         flag = True
                 return flag
+
             def get_dates():
                 temp_list = []
                 match_start_str = re.search(r'\d{4}-\d{2}-\d{2}', start_time)
                 match_end_str = re.search(r'\d{4}-\d{2}-\d{2}', end_time)
 
                 start_t = (datetime.strptime(match_start_str.group(), '%Y-%m-%d').date())
                 end_t = (datetime.strptime(match_end_str.group(), '%Y-%m-%d').date())
@@ -407,72 +418,75 @@
                     year_value = date_value.year
                     str_format = str(month_value) + '-' + str(year_value)
                     temp_list.append(str_format)
 
                 def sort_dates(dates):
                     def date_key(date_string):
                         return datetime.strptime(date_string, '%m-%Y')
-
                     return sorted(dates, key=date_key)
 
                 filtered_list = [*set(temp_list)]
-                list_of_dates_in_azure = sort_dates(filtered_list)
+                date_range = sort_dates(filtered_list)
+                list_of_dates_in_azure = list(set(date_month_list).intersection(date_range))
                 return list_of_dates_in_azure
 
             def read_one(blobfile):
                 blob = blob_svc.get_blob_client(self.container_name, device_id + '/' + blobfile + '.parquet')
-
                 with open(blobfile + '.parquet', "wb") as my_blob:
                     blob_data = blob.download_blob()
                     blob_data.readinto(my_blob)
                 df = pd.read_parquet(blobfile + '.parquet')
                 os.remove(blobfile + '.parquet')
                 return df
 
             def thread_read():
                 results = []
                 blob_list = get_dates()
-                with ThreadPoolExecutor(max_workers=40) as executor:  # function to thread
-                    for record in range(len(blob_list)):
-                        sys.stdout.write('\r')
-                        sys.stdout.write("Please Wait .. ")
-                        sys.stdout.flush()
-                    results = executor.map(read_one, blob_list)
-                final_df = pd.concat(results, axis=0)
-                return final_df
+                if len(blob_list) !=0:
+                    with ThreadPoolExecutor(max_workers=40) as executor:  # function to thread
+                        for record in range(len(blob_list)):
+                            sys.stdout.write('\r')
+                            sys.stdout.write("Please Wait .. ")
+                            sys.stdout.flush()
+                        results = executor.map(read_one, blob_list)
+                    fetched_df = pd.concat(results, axis=0)
+                else:
+                    fetched_df=pd.DataFrame()
+                return fetched_df
+
             flag = check_device(device_id)
             if flag:
                 df = thread_read()
-                try:
-                    end_time = str(datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S'))
-                except Exception:
-                    if type(end_time) == str:
-                        end_time = str(end_time) + " 23:59:59"
-                    pass
-                try:
-                    start_time = datetime.strptime(start_time, '%Y-%m-%d %H:%M:%S')
-                    end_time = datetime.strptime(end_time, '%Y-%m-%d %H:%M:%S')
-                    df = df[(df['time'] >= start_time) & (df['time'] <= end_time)]
-                except ValueError:
-                    df = df[(df['time'] >= start_time) & (df['time'] <= end_time)]
-                    pass
-                except Exception as e:
-                    print('Message: \t',e)
-                if sensors is None:
-                    sensors = list(df.columns)
-                    sensors.remove('time')
-                sensor_list_df = list(df.columns)
-                sensor_list_df.remove('time')
-                sensors_filtered = list(set(sensor_list_df).intersection(sensors))
-                if sensors != None and len(sensors_filtered) != 0:
-                    sensors_filtered.insert(0,'time')
-                    df =  df[sensors_filtered]
-                if len(sensors_filtered) == 0:
-                    df = pd.DataFrame()
-                if len(df) !=0:
+                if len(df) != 0:
+                    try:
+                        end_time = str(datetime.strptime(str(end_time), '%Y-%m-%d %H:%M:%S'))
+                    except Exception:
+                        if type(end_time) == str:
+                            end_time = str(end_time) + " 23:59:59"
+                        pass
+                    try:
+                        start_time = datetime.strptime(start_time, '%Y-%m-%d %H:%M:%S')
+                        end_time = datetime.strptime(end_time, '%Y-%m-%d %H:%M:%S')
+                        df = df[(df['time'] >= start_time) & (df['time'] <= end_time)]
+                    except ValueError:
+                        df = df[(df['time'] >= start_time) & (df['time'] <= end_time)]
+                        pass
+                    except Exception as e:
+                        print('Message: \t',e)
+                    if sensors is None:
+                        sensors = list(df.columns)
+                        sensors.remove('time')
+                    sensor_list_df = list(df.columns)
+                    sensor_list_df.remove('time')
+                    sensors_filtered = list(set(sensor_list_df).intersection(sensors))
+                    if sensors != None and len(sensors_filtered) != 0:
+                        sensors_filtered.insert(0,'time')
+                        df =  df[sensors_filtered]
+                    if len(sensors_filtered) == 0:
+                        df = pd.DataFrame()
                     df.reset_index(drop=True, inplace=True)
                     last_date = df['time'].iloc[len(df) - 1]
                     start_date = last_date.date() + timedelta(days=1)
                     end_time = pd.to_datetime(end_time)
                     if last_date.date() != end_time.date():
                         df1 = DataAccess.fetch_data(self, device_id ,start_time=str(start_date), alias=False,end_time=end_time,sensors=sensors, echo=True,onpremise=False,IST=True)
                         df = pd.concat([df, df1])
```

### Comparing `iosense_connect-2.1.4/iosense_connect.egg-info/PKG-INFO` & `iosense_connect-2.1.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: iosense-connect
-Version: 2.1.4
+Name: iosense_connect
+Version: 2.1.5
 Summary: iosense connect library
 Author: Faclon-Labs
 Author-email: reachus@faclon.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `iosense_connect-2.1.4/setup.py` & `iosense_connect-2.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "iosense_connect",
-    version = "2.1.4",
+    version = "2.1.5",
     author = "Faclon-Labs",
     author_email = "reachus@faclon.com",
     description = "iosense connect library",
     packages = ["iosense_connect"],
     long_description = long_description,
     long_description_content_type = "text/markdown",
     classifiers = [
```

