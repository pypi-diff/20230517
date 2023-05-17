# Comparing `tmp/alacorder-80.5.9.tar.gz` & `tmp/alacorder-80.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.5.9.tar", max compression
+gzip compressed data, was "alacorder-80.6.0.tar", max compression
```

## Comparing `alacorder-80.5.9.tar` & `alacorder-80.6.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.5.9/LICENSE
--rw-r--r--   0        0        0     6592 2023-05-11 17:12:36.043202 alacorder-80.5.9/README.md
--rw-r--r--   0        0        0      746 2023-05-17 13:55:00.163468 alacorder-80.5.9/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-17 13:55:53.336379 alacorder-80.5.9/src/alacorder/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.5.9/src/alacorder/__init__.py
--rw-r--r--   0        0        0   235980 2023-05-17 13:55:38.913136 alacorder-80.5.9/src/alacorder/__main__.py
--rw-r--r--   0        0        0   235980 2023-05-17 13:56:07.375052 alacorder-80.5.9/src/alacorder/alac.py
--rw-r--r--   0        0        0     7563 1970-01-01 00:00:00.000000 alacorder-80.5.9/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.6.0/LICENSE
+-rw-r--r--   0        0        0     6592 2023-05-11 17:12:36.043202 alacorder-80.6.0/README.md
+-rw-r--r--   0        0        0      746 2023-05-17 17:55:09.872937 alacorder-80.6.0/pyproject.toml
+-rw-r--r--   0        0        0     6148 2023-05-17 13:55:53.336379 alacorder-80.6.0/src/alacorder/.DS_Store
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.6.0/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   234285 2023-05-17 17:54:48.794246 alacorder-80.6.0/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   234285 2023-05-17 17:54:52.738672 alacorder-80.6.0/src/alacorder/alac.py
+-rw-r--r--   0        0        0     7563 1970-01-01 00:00:00.000000 alacorder-80.6.0/PKG-INFO
```

### Comparing `alacorder-80.5.9/LICENSE` & `alacorder-80.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.5.9/README.md` & `alacorder-80.6.0/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.5.9/pyproject.toml` & `alacorder-80.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.5.9"
+version = "80.6.0"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.5.9/src/alacorder/.DS_Store` & `alacorder-80.6.0/src/alacorder/.DS_Store`

 * *Files identical despite different names*

### Comparing `alacorder-80.5.9/src/alacorder/__main__.py` & `alacorder-80.6.0/src/alacorder/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.5.9"
+version = "80.6.0"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -441,16 +441,14 @@
     overwrite=False,
     no_write=False,
     fetch=False,
     cID="",
     uID="",
     pwd="",
     criminal_only=False,
-    qmax=0,
-    qskip=0,
     pairs=None,
     vrr_summary=False,
     append=False,
     window=None,
     force=False,
     no_update=False,
     now=False,
@@ -470,16 +468,14 @@
         overwrite (bool, optional): Overwrite existing files at output path
         no_write (bool, optional): Do not export to output path
         fetch (bool, optional): Retrieve case detail PDFs from Alacourt.com
         cID (str, optional): Customer ID on Alacourt.com
         uID (str, optional): User ID on Alacourt.com
         pwd (str, optional): Password on Alacourt.com
         criminal_only (bool, optional): Only fetch criminal cases
-        qmax (int, optional): Maximum queries to conduct on Alacourt.com
-        qskip (int, optional): Skip entries at top of query file
         pairs (str, optional): Path to AIS / Unique ID pairs for grouped table functions
         vrr_summary (bool, optional): Create voting rights summary from pairs
         append (bool, optional): Append one archive to another
         window (None, optional): PySimpleGUI window element
         force (bool, optional): Do not raise exceptions
         no_update (bool, optional): Do not mark input query when fetching cases
         now (bool, optional): Start Alacorder upon successful configuration
@@ -496,16 +492,14 @@
         overwrite=overwrite,
         no_write=no_write,
         fetch=fetch,
         cID=cID,
         uID=uID,
         pwd=pwd,
         criminal_only=criminal_only,
-        qmax=qmax,
-        qskip=qskip,
         pairs=pairs,
         vrr_summary=vrr_summary,
         append=append,
         window=window,
         force=force,
         no_update=no_update,
         now=now,
@@ -523,16 +517,14 @@
     debug=False,
     overwrite=False,
     no_write=False,
     fetch=False,
     cID="",
     uID="",
     pwd="",
-    qmax=0,
-    qskip=0,
     criminal_only=False,
     pairs=None,
     vrr_summary=False,
     append=False,
     window=None,
     force=False,
     no_update=False,
@@ -553,16 +545,14 @@
         overwrite (bool, optional): Overwrite existing files at output path
         no_write (bool, optional): Do not export to output path
         fetch (bool, optional): Retrieve case detail PDFs from Alacourt.com
         cID (str, optional): Customer ID on Alacourt.com
         uID (str, optional): User ID on Alacourt.com
         pwd (str, optional): Password on Alacourt.com
         criminal_only (bool, optional): Only fetch criminal cases
-        qmax (int, optional): Maximum queries to conduct on Alacourt.com
-        qskip (int, optional): Skip entries at top of query file
         pairs (str, optional): Path to AIS / Unique ID pairs for grouped table functions
         vrr_summary (bool, optional): Create voting rights summary from pairs
         append (bool, optional): Append one archive to another
         window (None, optional): PySimpleGUI Window element
         force (bool, optional): Do not raise exceptions
         no_update (bool, optional): Do not mark input query when fetching cases
         now (bool, optional): Start Alacorder upon successful configuration
@@ -748,16 +738,14 @@
         "APPEND": append,
         "NO_UPDATE": no_update,
         "FETCH": fetch,
         "ALA_CUSTOMER_ID": cID,
         "ALA_USER_ID": uID,
         "ALA_PASSWORD": pwd,
         "CRIMINAL_ONLY": criminal_only,
-        "FETCH_SKIP": qskip,
-        "FETCH_MAX": qmax,
         "LOG": log,
         "NO_WRITE": no_write,
         "NO_PROMPT": no_prompt,
         "OVERWRITE": overwrite,
         "EXISTING_OUTPUT": existing_output,
         "DEBUG": debug,
         "WINDOW": window,
@@ -2273,15 +2261,15 @@
             .alias("Category"),
             pl.col("RAWDESC")
             .str.contains(r"(A ATT|ATTEMPT|S SOLICIT|CONSP|SOLICITATION)")
             .is_not()
             .alias("A_S_C_DISQ"),
             pl.col("Code")
             .str.contains(
-                r"(OSUA|EGUA|MAN1|MAN2|MANS|ASS1|ASS2|KID1|KID2|HUT1|HUT2|BUR1|BUR2|TOP1|TOP2|TPCS|TPCD|TPC1|TET2|TOD2|ROB1|ROB2|ROB3|FOR1|FOR2|FR2D|MIOB|TRAK|TRAG|VDRU|VDRY|TRAO|TRFT|TRMA|TROP|CHAB|WABC|ACHA|ACAL)"
+                r"(OSUA|EGUA|MAN1|MAN2|MANS|ASS1|ASS2|KID1|KID2|HUT1|HUT2|BUR1|BUR2|TOP1|TOP2|TP2D|TP2G|TPCS|TPCD|TPC1|TET2|TOD2|ROB1|ROB2|ROB3|FOR1|FOR2|FR2D|MIOB|TRAK|TRAG|VDRU|VDRY|TRAO|TRFT|TRMA|TROP|CHAB|WABC|ACHA|ACAL)"
             )
             .alias("CERV_DISQ_MATCH"),
             pl.col("Code")
             .str.contains(
                 r"(RAP1|RAP2|SOD1|SOD2|STSA|SXA1|SXA2|ECHI|SX12|CSSC|FTCS|MURD|MRDI|MURR|FMUR|PMIO|POBM|MIPR|POMA|INCE)"
             )
             .alias("PARDON_DISQ_MATCH"),
@@ -3133,19 +3121,17 @@
     sent = sent.fill_null("")
     return sent
 
 
 #   #   #   #        FETCH (PDF SCRAPER)        #   #   #   #
 
 
-def read_query(path, qmax=0, qskip=0, window=None):
+def read_query(path, window=None):
     if isinstance(path, dict):
         cf = path
-        qmax = cf["FETCH_MAX"]
-        qskip = cf["FETCH_SKIP"]
         path = cf["INPUTS"]
     if os.path.splitext(path)[1] in (".xlsx", ".xls"):
         query = pl.read_excel(
             path,
             xlsx2csv_options={"ignore_errors": True},
             read_csv_options={"ignore_errors": True},
         )
@@ -3167,21 +3153,14 @@
         else:
             raise Exception(
                 "Remove TEMP columns from input query spreadsheet and try again."
             )
 
     found = query.shape[0]
 
-    if qskip > 0:
-        qs = qskip - 1
-        query = query[qs:-1]
-
-    if qmax < query.shape[0] and qmax > 0:
-        query = query.sample(qmax)
-
     pscols = [
         "NAME",
         "PARTY_TYPE",
         "SSN",
         "DOB",
         "COUNTY",
         "DIVISION",
@@ -3224,35 +3203,30 @@
 
     query = query.with_columns(
         [
             pl.col("RETRIEVED").cast(pl.Utf8, strict=False),
         ]
     )
 
-    if goodquery and qmax == 0:
+    if goodquery:
         print(f"{query.shape[0]} queries read from input query file.")
         return query
-    elif goodquery and qmax > 0:
-        print(f"{query.shape[0]} of {found} queries read from input query file.")
-        return query
     else:
         print(
             "Try again with at least one valid column header: [NAME, PARTY_TYPE, SSN, DOB, COUNTY, DIVISION, CASE_YEAR, NO_RECORDS, FILED_BEFORE, FILED_AFTER, RETRIEVED, CASES_FOUND, QUERY_COMPLETE]"
         )
         return None
 
 
 def fetch(
     querypath="",
     dirpath="",
     cID="",
     uID="",
     pwd="",
-    qmax=0,
-    qskip=0,
     criminal_only=False,
     cf=None,
     no_update=False,
     debug=False,
     window=None,
 ):
     """
@@ -3260,43 +3234,37 @@
     Input query spreadsheet with headers NAME, PARTY_TYPE, SSN, DOB, COUNTY, DIVISION, CASE_YEAR, and FILED_BEFORE as `querypath`. Alacorder will Party Search non-blank fields on Alacourt.com and download to `dirpath`.
     Args:
        querypath (str): Path to query table/spreadsheet (.xls, .xlsx)
        dirpath (str): Path to PDF output directory
        cID (str): Customer ID on Alacourt.com
        uID (str): User ID on Alacourt.com
        pwd (str): Password on Alacourt.com
-       qmax (int): Maximum queries to conduct on Alacourt.com
-       qskip (int): Skip entries at top of query file
        no_update (bool): Do not update query template after completion
        debug (bool): Print detailed runtime information to console
     """
     if isinstance(querypath, dict):
         cf = querypath
     if cf != None:
         querypath = cf["INPUTS"]
         dirpath = cf["OUTPUT_PATH"]
         cID = cf["ALA_CUSTOMER_ID"]
         uID = cf["ALA_USER_ID"]
         pwd = cf["ALA_PASSWORD"]
-        qmax = cf["FETCH_MAX"]
-        qskip = cf["FETCH_SKIP"]
         criminal_only = cf["CRIMINAL_ONLY"]
     else:
         cf = {
             "INPUTS": querypath,
             "OUTPUT_PATH": dirpath,
             "ALA_CUSTOMER_ID": cID,
             "ALA_USER_ID": uID,
             "ALA_PASSWORD": pwd,
-            "FETCH_MAX": qmax,
-            "FETCH_SKIP": qskip,
             "CRIMINAL_ONLY": criminal_only,
         }
 
-    query = read_query(cf["INPUTS"], qmax=qmax, qskip=qskip)
+    query = read_query(cf["INPUTS"])
 
     # start browser and authenticate
     opt = webdriver.ChromeOptions()
     opt.add_experimental_option(
         "prefs",
         {
             "download.default_directory": dirpath,  # Set default directory for downloads
@@ -3462,17 +3430,25 @@
             login(driver, cID=cID, uID=uID, pwd=pwd)
             driver.implicitly_wait(1)
         driver.get("https:v2.alacourt.com/frmIndexSearchForm.aspx")
         print("Successfully connected and logged into Alacourt!")
 
     # field search
 
+    time.sleep(0.5)
+
     # name
     if name != "":
-        party_name_box.send_keys(name)
+        driver.implicitly_wait(1)
+        try:
+            party_name_box.send_keys(name)
+        except selenium.common.exceptions.StaleElementReferenceException:
+            time.sleep(2)
+            driver.implicitly_wait(2)
+            party_name_box.send_keys(name)
     # ssn
     if ssn != "":
         ssn_box = driver.find_element(
             by=By.NAME, value="ctl00$ContentPlaceHolder1$txtSSN"
         )
         ssn_box.send_keys(ssn)
     # dob
@@ -3532,20 +3508,24 @@
             by=By.NAME, value="ctl00$ContentPlaceHolder1$txtTo"
         )
         filed_after_box.send_keys(filed_after)
 
     # submit search
     search_button = driver.find_element(by=By.ID, value="searchButton")
 
+    time.sleep(0.25)
+
     try:
         search_button.click()
     except:
         driver.implicitly_wait(2)
         time.sleep(2)
 
+    time.sleep(0.5)
+
     dlog("Submitted party search form...", cf=debug)
 
     # count pages
     try:
         page_counter = driver.find_element(
             by=By.ID, value="ContentPlaceHolder1_dg_tcPageXofY"
         ).text
@@ -3822,21 +3802,14 @@
                 size=[26, 10],
                 key="SQ-OUTPUTPATH",
             ),
             sg.FolderBrowse(
                 button_text="Select Folder", button_color=("white", "black")
             ),
         ],
-        [
-            sg.Text("Max queries: "),
-            sg.Input(key="SQ-MAX", default_text="0", size=[5, 1]),
-            sg.Text("Skip from top: "),
-            sg.Input(key="SQ-SKIP", default_text="0", size=[5, 1]),
-            sg.Checkbox(key="SQ-CRIMINALONLY", text="Criminal Only"),
-        ],
         [sg.Text("Alacourt.com Credentials", font=BODY_FONT)],
         [
             sg.Text("Customer ID: "),
             sg.Input(key="SQ-CUSTOMERID", size=(16, 1)),
         ],
         [
             sg.Text("User ID:"),
@@ -4350,31 +4323,23 @@
                 window["SQ-INPUTPATH"].get() == ""
                 or window["SQ-OUTPUTPATH"].get() == ""
             ):
                 sg.popup("Check configuration and try again.")
                 continue
             try:
                 pwd = window["SQ-PASSWORD"].get()
-                try:
-                    sq_max = int(window["SQ-MAX"].get().strip())
-                    sq_skip = int(window["SQ-SKIP"].get().strip())
-                except:
-                    sq_max = 0
-                    sq_skip = 0
                 window["SQ"].update(disabled=True)
                 thread = threading.Thread(
                     target=fetch,
                     args=(
                         window["SQ-INPUTPATH"].get(),
                         window["SQ-OUTPUTPATH"].get(),
                         window["SQ-CUSTOMERID"].get(),
                         window["SQ-USERID"].get(),
                         pwd,
-                        sq_max,
-                        sq_skip,
                         window["SQ-CRIMINALONLY"].get(),
                         None,
                         False,
                         False,
                         window,
                     ),
                     daemon=True,
@@ -4536,70 +4501,48 @@
     "--criminal-only",
     "-criminal",
     is_flag=True,
     default=False,
     help="Only search criminal cases",
 )
 @click.option(
-    "--max",
-    "-max",
-    "qmax",
-    required=False,
-    type=int,
-    help="Maximum queries to conduct on Alacourt.com",
-    default=0,
-)
-@click.option(
-    "--skip",
-    "-skip",
-    "qskip",
-    required=False,
-    type=int,
-    help="Skip entries at top of query file",
-    default=0,
-)
-@click.option(
     "--no-mark",
     "-n",
     "no_update",
     is_flag=True,
     default=False,
     help="Do not update query template after completion",
 )
 @click.option(
     "--debug",
     is_flag=True,
     default=False,
     help="Print detailed runtime information to console",
 )
 def _cli_fetch(
-    querypath, path, cID, uID, pwd, qmax, qskip, no_update, criminal_only, debug
+    querypath, path, cID, uID, pwd, no_update, criminal_only, debug
 ):
     """
     Fetch case PDFs from Alacourt.com.
     Args:
         querypath (str): Path to query table/spreadsheet (.xls, .xlsx)
         path (str): Path to PDF output directory
         cID (str): Customer ID on Alacourt.com
         uID (str): User ID on Alacourt.com
         pwd (str): Password on Alacourt.com
-        qmax (int): Maximum queries to conduct on Alacourt.com
-        qskip (int): Skip entries at top of query file
         no_update (bool): Do not update query template after completion
         criminal_only (bool): Only search criminal cases
         debug (bool): Print detailed runtime information to console
     """
     fetch(
         querypath=querypath,
         dirpath=path,
         cID=cID,
         uID=uID,
         pwd=pwd,
-        qmax=qmax,
-        qskip=qskip,
         no_update=no_update,
         criminal_only=criminal_only,
         debug=debug,
     )
 
 
 @main.command(name="multi", help="Export all data tables to .xls/.xlsx")
@@ -5867,21 +5810,21 @@
         ).strip()
     except:
         return ""
 
 
 def getDOB(text):
     try:
-        return re.sub(
+        return datetime.strptime(re.sub(
             r"[^\d/]",
             "",
             re.search(r"(\d{2}/\d{2}/\d{4})(?:.{0,5}DOB:)", str(text)).group(1),
-        ).strip()
+        ).strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getPhone(text):
     try:
         text = str(text)
         text = re.sub(r"[^0-9]", "", re.search(r"(Phone: )(.+)", text).group(2)).strip()
         if len(text) < 7 or text[0:10] == "2050000000":
@@ -5997,29 +5940,14 @@
         state = ""
     if len(city) > 3:
         return f"{street1} {street2} {city}, {state} {zipcode}".strip()
     else:
         return f"{street1} {street2} {city} {state} {zipcode}".strip()
 
 
-def getChargesRows(text):
-    m = re.findall(
-        r"(\d{3}\s{1}[A-Z0-9]{4}.{1,200}?.{3}-.{3}-.{3}[^a-z\n]{10,75})", str(text)
-    )
-    return m
-
-
-def getFeeSheetRows(text):
-    m = re.findall(
-        r"(ACTIVE [^\(\n]+\$[^\(\n]+ACTIVE[^\(\n]+[^\n]|Total:.+\$[^A-Za-z\n]*)",
-        str(text),
-    )
-    return m
-
-
 def getTotalRow(text):
     try:
         mmm = re.search(r"(Total:.+\$[^\n]*)", str(text)).group()
         mm = re.sub(r"[^0-9|\.|\s|\$]", "", str(mmm))
         m = re.findall(r"\d+\.\d{2}", str(mm))
         return m
     except:
@@ -6091,17 +6019,17 @@
         )
     except:
         return ""
 
 
 def getCaseYear(text):
     try:
-        return re.search(r"\w{2}\-(\d{4})-\d{6}\.\d{2}", str(text)).group(1)
+        return int(re.search(r"\w{2}\-(\d{4})-\d{6}\.\d{2}", str(text)).group(1))
     except:
-        return ""
+        return None
 
 
 def getLastName(text):
     try:
         return getName(text).split(" ")[0].strip()
     except:
         return ""
@@ -6126,88 +6054,86 @@
 
 def getRelatedCases(text):
     return re.findall(r"(\w{2}\d{12})", str(text))
 
 
 def getFilingDate(text):
     try:
-        return re.sub(
+        return datetime.strptime(re.sub(
             r"Filing Date: ",
             "",
             re.search(r"Filing Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(),
-        ).strip()
+        ).strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getCaseInitiationDate(text):
     try:
-        return re.sub(
+        return datetime.strptime(re.sub(
             r"Case Initiation Date: ",
             "",
             re.search(
                 r"Case Initiation Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)
-            ).group(),
+            ).group(1),  '%m/%d/%Y')
         )
     except:
-        return ""
+        return None
 
 
 def getArrestDate(text):
     try:
-        return re.search(r"Arrest Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+        return datetime.strptime(re.search(r"Arrest Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getOffenseDate(text):
     try:
-        return re.search(r"Offense Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+        return datetime.strptime(re.search(r"Offense Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getIndictmentDate(text):
     try:
-        return re.search(r"Indictment Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+        return datetime.strptime(re.search(r"Indictment Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getYouthfulDate(text):
     try:
-        return re.search(r"Youthful Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+        return datetime.strptime(re.search(r"Youthful Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getRetrieved(text):
     try:
-        return re.search(r"Alacourt\.com (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+        return datetime.strptime(re.search(r"Alacourt\.com (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getCourtAction(text):
     try:
         return re.search(
             r"Court Action: (BOUND|GUILTY PLEA|WAIVED TO GJ|DISMISSED|TIME LAPSED|NOL PROSS|CONVICTED|INDICTED|DISMISSED|FORFEITURE|TRANSFER|REMANDED|WAIVED|ACQUITTED|WITHDRAWN|PETITION|PRETRIAL|COND\. FORF\.)",
             str(text),
         ).group(1)
     except:
         return ""
 
 
 def getCourtActionDate(text):
     try:
-        return re.search(r"Court Action Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(
-            1
-        )
+        return datetime.strptime(re.search(r"Court Action Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getDescription(text):
     try:
         return (
             re.search(r"Charge: ([A-Z\.0-9\-\s]+)", str(text))
             .group(1)
@@ -6424,32 +6350,28 @@
         )
     except:
         return ""
 
 
 def getWarrantIssuanceDate(text):
     try:
-        return (
+        return datetime.strptime(
             re.search(r"(\d\d?/\d\d?/\d\d\d\d) Warrant Issuance Date:", str(text))
             .group(1)
-            .strip()
-        )
+            .strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getWarrantActionDate(text):
     try:
-        return (
-            re.search(r"Warrant Action Date: (\d\d?/\d\d?/\d\d\d\d)", str(text))
-            .group(1)
-            .strip()
-        )
+        return datetime.strptime(
+                re.search(r"Warrant Action Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1).strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getWarrantIssuanceStatus(text):
     try:
         return re.search(r"Warrant Issuance Status: (\w)", str(text)).group(1).strip()
     except:
         return ""
@@ -6510,32 +6432,30 @@
         return re.search(r"Surety Code: ([A-Z0-9]{4})", str(text)).group(1).strip()
     except:
         return ""
 
 
 def getBondReleaseDate(text):
     try:
-        return (
+        return datetime.strptime(
             re.search(r"Release Date: (\d\d?/\d\d?/\d\d\d\d)", str(text))
             .group(1)
-            .strip()
-        )
+            .strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getFailedToAppearDate(text):
     try:
-        return (
+        return datetime.strptime(
             re.search(r"Failed to Appear Date: (\d\d?/\d\d?/\d\d\d\d)", str(text))
             .group(1)
-            .strip()
-        )
+            .strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getBondsmanProcessIssuance(text):
     try:
         return (
             re.search(
                 r"Bondsman Process Issuance: ([^\n]*?) Bondsman Process Return:",
@@ -6557,21 +6477,21 @@
         )
     except:
         return ""
 
 
 def getAppealDate(text):
     try:
-        return re.sub(
+        return datetime.strptime(re.sub(
             r"[\n\s]",
             "",
             re.search(r"([\n\s/\d]*?) Appeal Court:", str(text)).group(1).strip(),
-        )
+        ), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getAppealCourt(text):
     try:
         return re.search(r"([A-Z\-\s]+) Appeal Case Number", str(text)).group(1).strip()
     except:
         return ""
@@ -6619,36 +6539,36 @@
         return re.search(r"Appeal To: (\w?) Appeal", str(text)).group(1).strip()
     except:
         return ""
 
 
 def getLowerCourtAppealDate(text):
     try:
-        return re.sub(
+        return datetime.strptime(re.sub(
             r"[\n\s:\-]",
             "",
             re.search(
                 r"LowerCourt Appeal Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)
             ).group(1),
-        ).strip()
+        ).strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getDispositionDateOfAppeal(text):
     try:
-        return re.sub(
+        return datetime.strptime(re.sub(
             r"[\n\s:\-]",
             "",
             re.search(
                 r"Disposition Date Of Appeal: (\d\d?/\d\d?/\d\d\d\d)", str(text)
             ).group(1),
-        ).strip()
+        ).strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getDispositionTypeOfAppeal(text):
     try:
         return re.sub(
             r"[\n\s:\-]",
             "",
@@ -6676,21 +6596,20 @@
         return re.search(r"Updated By: (\w{3})", str(text)).group(1).strip()
     except:
         return ""
 
 
 def getTransferToAdminDocDate(text):
     try:
-        return (
+        return datetime.strptime(
             re.search(r"Transfer to Admin Doc Date: (\d\d?/\d\d?/\d\d\d\d)", str(text))
             .group(1)
-            .strip()
-        )
+            .strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getTransferDesc(text):
     try:
         return (
             re.search(r"Transfer Desc: ([A-Z\s]{0,15} \d\d?/\d\d?/\d\d\d\d)", str(text))
             .group(1)
@@ -6698,39 +6617,37 @@
         )
     except:
         return ""
 
 
 def getTBNV1(text):
     try:
-        return (
+        return datetime.strptime(
             re.search(r"Date Trial Began but No Verdict \(TBNV1\): ([^\n]+)", str(text))
             .group(1)
-            .strip()
-        )
+            .strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getTBNV2(text):
     try:
-        return (
+        return datetime.strptime(
             re.search(r"Date Trial Began but No Verdict \(TBNV2\): ([^\n]+)", str(text))
             .group(1)
-            .strip()
-        )
+            .strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getTurnOverDate(text):
     try:
-        return re.search(r"TurnOver Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+        return datetime.strptime(re.search(r"TurnOver Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getTurnOverAmt(text):
     try:
         return float(re.search(r"TurnOver Amt\: \$(\d+\.\d\d)", str(text)).group(1))
     except:
         return ""
@@ -6741,24 +6658,24 @@
         return float(re.search(r"Frequency Amt\: \$(\d+\.\d\d)", str(text)).group(1))
     except:
         return ""
 
 
 def getDueDate(text):
     try:
-        return re.search(r"Due Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+        return datetime.strptime(re.search(r"Due Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getLastPaidDate(text):
     try:
-        return re.search(r"Last Paid Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+        return datetime.strptime(re.search(r"Last Paid Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getPayor(text):
     try:
         return re.search(r"Payor\: ([A-Z0-9]{4})", str(text)).group(1)
     except:
         return ""
@@ -6796,87 +6713,85 @@
         return re.search(r"PreTrial\: (YES|NO)", str(text)).group(1)
     except:
         return ""
 
 
 def getPreTrialDate(text):
     try:
-        return re.search(r"PreTrail Date\: (.+)PreTrial", str(text)).group(1).strip()
+        return datetime.strptime(re.search(r"PreTrail Date\: (.+)PreTrial", str(text)).group(1).strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getPreTrialTerms(text):
     try:
         return re.search(r"PreTrial Terms\: (YES|NO)", str(text)).group(1)
     except:
         return ""
 
 
 def getPreTermsDate(text):
     try:
-        return re.search(r"Pre Terms Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+        return datetime.strptime(re.search(r"Pre Terms Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getDelinquent(text):
     try:
         return re.search(r"Delinquent\: (YES|NO)", str(text)).group(1)
     except:
         return ""
 
 
 def getDelinquentDate(text):
     try:
-        return re.search(r"Delinquent Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(
-            1
-        )
+        return datetime.strptime(re.search(r"Delinquent Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getDAMailer(text):
     try:
         return re.search(r"DA Mailer\: (YES|NO)", str(text)).group(1)
     except:
         return ""
 
 
 def getDAMailerDate(text):
     try:
-        return re.search(r"DA Mailer Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+        return datetime.strptime(re.search(r"DA Mailer Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getWarrantMailer(text):
     try:
         return re.search(r"Warrant Mailer\: (YES|NO)", str(text)).group(1)
     except:
         return ""
 
 
 def getWarrantMailerDate(text):
     try:
-        return re.search(
+        return datetime.strptime(re.search(
             r"Warrant Mailer Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)
-        ).group(1)
+        ).group(1), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
-def getEnforcementLastUpdate(text):
+def getLastUpdate(text):
     try:
         return re.search(r"Last Update\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
     except:
         return ""
 
 
-def getEnforcementUpdatedBy(text):
+def getUpdatedBy(text):
     try:
         return re.search(r"Updated By\: ([A-Z]{3})", str(text)).group(1)
     except:
         return ""
 
 
 def getSentencingRequirementsCompleted(text):
@@ -6886,36 +6801,22 @@
             "",
             ", ".join(re.findall(r"(?:Requrements Completed: )([YES|NO]?)", str(text))),
         )
     except:
         return ""
 
 
-def getSentencingRequrementsCompleted(
-    text,
-):  # [sic] On-Line Services doesn't know how to spell requirements lol
-    try:
-        return re.sub(
-            r"[\n:]|Requrements Completed",
-            "",
-            ", ".join(re.findall(r"(?:Requrements Completed: )([YES|NO]?)", str(text))),
-        )
-    except:
-        return ""
-
-
 def getSentenceDate(text):
     try:
-        return (
+        return datetime.strptime(
             re.search(r"(Sentence Date: )(\d\d?/\d\d?/\d\d\d\d)", str(text))
             .group(2)
-            .strip()
-        )
+            .strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None 
 
 
 def getProbationPeriod(text):
     try:
         return "".join(
             re.search(r"Probation Period: ([^\.]+)", str(text)).group(1).strip()
         ).strip()
@@ -6935,86 +6836,64 @@
     except:
         return ""
 
 
 def getJailCreditPeriod(text):
     try:
         return "".join(
-            re.search(r"Jail Credit Period: ([^\.]+)", str(text)).group(1).strip()
+            re.search(r"Days\.\s*(\d+ Years, \d+ Months, \d+ Days\.)\s+", str(text)).group(1).strip()
         )
     except:
         return ""
 
 
 def getSentenceProvisions(text):
     try:
         return re.search(r"Sentence Provisions: ([Y|N]?)", str(text)).group(1).strip()
     except:
         return ""
 
 
 def getSentenceStartDate(text):
     try:
-        return re.sub(
+        return datetime.strptime(re.sub(
             r"(Sentence Start Date:)",
             "",
             ", ".join(
                 re.findall(r"Sentence Start Date: (\d\d?/\d\d?/\d\d\d\d)", str(text))
             ),
-        ).strip()
+        ).strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getSentenceEndDate(text):
     try:
-        return re.sub(
+        return datetime.strptime(re.sub(
             r"(Sentence End Date:)",
             "",
             ", ".join(
                 re.findall(r"Sentence End Date: (\d\d?/\d\d?/\d\d\d\d)", str(text))
             ),
-        ).strip()
+        ).strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getProbationBeginDate(text):
     try:
-        return re.sub(
+        return datetime.strptime(re.sub(
             r"(Probation Begin Date:)",
             "",
             ", ".join(
                 re.findall(r"Probation Begin Date: (\d\d?/\d\d?/\d\d\d\d)", str(text))
             ),
-        ).strip()
-    except:
-        return ""
-
-
-def getSentenceUpdatedBy(text):
-    try:
-        return re.sub(
-            r"(Updated By:)",
-            "",
-            ", ".join(re.findall(r"Updated By: (\w{3}?)", str(text))),
-        ).strip()
+        ).strip(), '%m/%d/%Y')
     except:
-        return ""
-
-
-def getSentenceLastUpdate(text):
-    try:
-        return re.sub(
-            r"(Last Update:)",
-            "",
-            ", ".join(re.findall(r"Last Update: (\d\d?/\d\d?/\d\d\d\d)", str(text))),
-        ).strip()
-    except:
-        return ""
+        return None
 
 
 def getProbationRevoke(text):
     try:
         return re.sub(
             r"(Probation Revoke:)",
             "",
@@ -7055,59 +6934,59 @@
 def getImages(text):
     imgs = re.findall(
         r"(Images\s+?Pages)([^\\n]*)(END OF THE REPORT)", str(text), re.DOTALL
     )
     if len(imgs) > 1:
         imgs = "; ".join(imgs).strip()
     elif len(imgs) == 1:
-        return imgs[0].strip()
+        return imgs[0][1].strip()
     else:
         return ""
 
 
 def getWitnesses(text):
     wit = re.search(r"(Witness.+?Case Action Summary)", str(text), re.DOTALL)
     if wit:
-        wit = re.sub(
-            r"Witness # Date Served Service Type Attorney Issued Type   SJIS Witness List   Date Issued   Subpoena",
-            "",
-            wit,
-            re.DOTALL,
-        )
-        wit = re.sub(
-            r"Date: Time Code Comments   Case Action Summary", "", wit, re.DOTALL
-        )
+        wit = wit.group()
         wit = re.sub(r"© Alacourt.com \d\d?/\d\d?/\d\d\d\d", "", wit, re.DOTALL)
-        wit = re.sub(
-            r"Witness List    4 Requesting Party Name Witness # Date Served Service Type Attorney Issued Type   Date Issued   Subpoena",
-            "",
-            wit,
-            re.DOTALL,
-        )
+        wit = re.sub(r"Witness", "", wit, re.DOTALL)
+        wit = re.sub(r"\#Name", "", wit, re.DOTALL)
+        wit = re.sub(r"Date", "", wit, re.DOTALL)
+        wit = re.sub(r"Served", "", wit, re.DOTALL)
+        wit = re.sub(r"Service", "", wit, re.DOTALL)
+        wit = re.sub(r"Type", "", wit, re.DOTALL)
+        wit = re.sub(r"Attorney", "", wit, re.DOTALL)
+        wit = re.sub(r"Issued", "", wit, re.DOTALL)
+        wit = re.sub(r"Type", "", wit, re.DOTALL)
+        wit = re.sub(r"SJIS", "", wit, re.DOTALL)
+        wit = re.sub(r"Witness", "", wit, re.DOTALL)
+        wit = re.sub(r"List", "", wit, re.DOTALL)
+        wit = re.sub(r"Date Issued", "", wit, re.DOTALL)
+        wit = re.sub(r"Subpoena", "", wit, re.DOTALL)
+        wit = re.sub(r"Date\:", "", wit, re.DOTALL)
+        wit = re.sub(r"Time", "", wit, re.DOTALL)
+        wit = re.sub(r"Code", "", wit, re.DOTALL)
+        wit = re.sub(r"Comments", "", wit, re.DOTALL)
+        wit = re.sub(r"Case Action Summary", "", wit, re.DOTALL)
+        wit = re.sub(r"\:$", "", wit, re.DOTALL)
         return wit.strip()
     else:
         return ""
 
 
 def getSettings(text):
-    settings = re.search(r"(Settings.+Court Action)", str(text), re.DOTALL)
+    settings = re.search(r"(Settings.+?Court Action)", str(text), re.DOTALL)
     if settings:
-        out = settings.group(2)
-        out = re.sub(
-            r"Settings   Date: Que: Time: Description:   Settings", "", out, re.DOTALL
-        )
-        out = re.sub(
-            r"Settings   Settings Date: Que: Time: Description:", "", out, re.DOTALL
-        )
-        out = re.sub(
-            r"Disposition Charges   # Code Court Action Category Cite Court Action",
-            "",
-            out,
-            re.DOTALL,
-        )
+        out = settings.group(1)
+        out = re.sub(r"Settings", "", out, re.DOTALL)
+        out = re.sub(r"Date\:", "", out, re.DOTALL)
+        out = re.sub(r"Que\:", "", out, re.DOTALL)
+        out = re.sub(r"Time\:", "", out, re.DOTALL)
+        out = re.sub(r"Description\:", "", out, re.DOTALL)
+        out = re.sub(r"Court Action", "", out, re.DOTALL)
         return out.strip()
     else:
         return ""
 
 def getBalanceByFeeCode(text, code):
     pat = f"(ACTIVE[^\n]+{code}[^\n]+)"
     rows = re.findall(pat, text)
```

### Comparing `alacorder-80.5.9/src/alacorder/alac.py` & `alacorder-80.6.0/src/alacorder/alac.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.5.9"
+version = "80.6.0"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
@@ -441,16 +441,14 @@
     overwrite=False,
     no_write=False,
     fetch=False,
     cID="",
     uID="",
     pwd="",
     criminal_only=False,
-    qmax=0,
-    qskip=0,
     pairs=None,
     vrr_summary=False,
     append=False,
     window=None,
     force=False,
     no_update=False,
     now=False,
@@ -470,16 +468,14 @@
         overwrite (bool, optional): Overwrite existing files at output path
         no_write (bool, optional): Do not export to output path
         fetch (bool, optional): Retrieve case detail PDFs from Alacourt.com
         cID (str, optional): Customer ID on Alacourt.com
         uID (str, optional): User ID on Alacourt.com
         pwd (str, optional): Password on Alacourt.com
         criminal_only (bool, optional): Only fetch criminal cases
-        qmax (int, optional): Maximum queries to conduct on Alacourt.com
-        qskip (int, optional): Skip entries at top of query file
         pairs (str, optional): Path to AIS / Unique ID pairs for grouped table functions
         vrr_summary (bool, optional): Create voting rights summary from pairs
         append (bool, optional): Append one archive to another
         window (None, optional): PySimpleGUI window element
         force (bool, optional): Do not raise exceptions
         no_update (bool, optional): Do not mark input query when fetching cases
         now (bool, optional): Start Alacorder upon successful configuration
@@ -496,16 +492,14 @@
         overwrite=overwrite,
         no_write=no_write,
         fetch=fetch,
         cID=cID,
         uID=uID,
         pwd=pwd,
         criminal_only=criminal_only,
-        qmax=qmax,
-        qskip=qskip,
         pairs=pairs,
         vrr_summary=vrr_summary,
         append=append,
         window=window,
         force=force,
         no_update=no_update,
         now=now,
@@ -523,16 +517,14 @@
     debug=False,
     overwrite=False,
     no_write=False,
     fetch=False,
     cID="",
     uID="",
     pwd="",
-    qmax=0,
-    qskip=0,
     criminal_only=False,
     pairs=None,
     vrr_summary=False,
     append=False,
     window=None,
     force=False,
     no_update=False,
@@ -553,16 +545,14 @@
         overwrite (bool, optional): Overwrite existing files at output path
         no_write (bool, optional): Do not export to output path
         fetch (bool, optional): Retrieve case detail PDFs from Alacourt.com
         cID (str, optional): Customer ID on Alacourt.com
         uID (str, optional): User ID on Alacourt.com
         pwd (str, optional): Password on Alacourt.com
         criminal_only (bool, optional): Only fetch criminal cases
-        qmax (int, optional): Maximum queries to conduct on Alacourt.com
-        qskip (int, optional): Skip entries at top of query file
         pairs (str, optional): Path to AIS / Unique ID pairs for grouped table functions
         vrr_summary (bool, optional): Create voting rights summary from pairs
         append (bool, optional): Append one archive to another
         window (None, optional): PySimpleGUI Window element
         force (bool, optional): Do not raise exceptions
         no_update (bool, optional): Do not mark input query when fetching cases
         now (bool, optional): Start Alacorder upon successful configuration
@@ -748,16 +738,14 @@
         "APPEND": append,
         "NO_UPDATE": no_update,
         "FETCH": fetch,
         "ALA_CUSTOMER_ID": cID,
         "ALA_USER_ID": uID,
         "ALA_PASSWORD": pwd,
         "CRIMINAL_ONLY": criminal_only,
-        "FETCH_SKIP": qskip,
-        "FETCH_MAX": qmax,
         "LOG": log,
         "NO_WRITE": no_write,
         "NO_PROMPT": no_prompt,
         "OVERWRITE": overwrite,
         "EXISTING_OUTPUT": existing_output,
         "DEBUG": debug,
         "WINDOW": window,
@@ -2273,15 +2261,15 @@
             .alias("Category"),
             pl.col("RAWDESC")
             .str.contains(r"(A ATT|ATTEMPT|S SOLICIT|CONSP|SOLICITATION)")
             .is_not()
             .alias("A_S_C_DISQ"),
             pl.col("Code")
             .str.contains(
-                r"(OSUA|EGUA|MAN1|MAN2|MANS|ASS1|ASS2|KID1|KID2|HUT1|HUT2|BUR1|BUR2|TOP1|TOP2|TPCS|TPCD|TPC1|TET2|TOD2|ROB1|ROB2|ROB3|FOR1|FOR2|FR2D|MIOB|TRAK|TRAG|VDRU|VDRY|TRAO|TRFT|TRMA|TROP|CHAB|WABC|ACHA|ACAL)"
+                r"(OSUA|EGUA|MAN1|MAN2|MANS|ASS1|ASS2|KID1|KID2|HUT1|HUT2|BUR1|BUR2|TOP1|TOP2|TP2D|TP2G|TPCS|TPCD|TPC1|TET2|TOD2|ROB1|ROB2|ROB3|FOR1|FOR2|FR2D|MIOB|TRAK|TRAG|VDRU|VDRY|TRAO|TRFT|TRMA|TROP|CHAB|WABC|ACHA|ACAL)"
             )
             .alias("CERV_DISQ_MATCH"),
             pl.col("Code")
             .str.contains(
                 r"(RAP1|RAP2|SOD1|SOD2|STSA|SXA1|SXA2|ECHI|SX12|CSSC|FTCS|MURD|MRDI|MURR|FMUR|PMIO|POBM|MIPR|POMA|INCE)"
             )
             .alias("PARDON_DISQ_MATCH"),
@@ -3133,19 +3121,17 @@
     sent = sent.fill_null("")
     return sent
 
 
 #   #   #   #        FETCH (PDF SCRAPER)        #   #   #   #
 
 
-def read_query(path, qmax=0, qskip=0, window=None):
+def read_query(path, window=None):
     if isinstance(path, dict):
         cf = path
-        qmax = cf["FETCH_MAX"]
-        qskip = cf["FETCH_SKIP"]
         path = cf["INPUTS"]
     if os.path.splitext(path)[1] in (".xlsx", ".xls"):
         query = pl.read_excel(
             path,
             xlsx2csv_options={"ignore_errors": True},
             read_csv_options={"ignore_errors": True},
         )
@@ -3167,21 +3153,14 @@
         else:
             raise Exception(
                 "Remove TEMP columns from input query spreadsheet and try again."
             )
 
     found = query.shape[0]
 
-    if qskip > 0:
-        qs = qskip - 1
-        query = query[qs:-1]
-
-    if qmax < query.shape[0] and qmax > 0:
-        query = query.sample(qmax)
-
     pscols = [
         "NAME",
         "PARTY_TYPE",
         "SSN",
         "DOB",
         "COUNTY",
         "DIVISION",
@@ -3224,35 +3203,30 @@
 
     query = query.with_columns(
         [
             pl.col("RETRIEVED").cast(pl.Utf8, strict=False),
         ]
     )
 
-    if goodquery and qmax == 0:
+    if goodquery:
         print(f"{query.shape[0]} queries read from input query file.")
         return query
-    elif goodquery and qmax > 0:
-        print(f"{query.shape[0]} of {found} queries read from input query file.")
-        return query
     else:
         print(
             "Try again with at least one valid column header: [NAME, PARTY_TYPE, SSN, DOB, COUNTY, DIVISION, CASE_YEAR, NO_RECORDS, FILED_BEFORE, FILED_AFTER, RETRIEVED, CASES_FOUND, QUERY_COMPLETE]"
         )
         return None
 
 
 def fetch(
     querypath="",
     dirpath="",
     cID="",
     uID="",
     pwd="",
-    qmax=0,
-    qskip=0,
     criminal_only=False,
     cf=None,
     no_update=False,
     debug=False,
     window=None,
 ):
     """
@@ -3260,43 +3234,37 @@
     Input query spreadsheet with headers NAME, PARTY_TYPE, SSN, DOB, COUNTY, DIVISION, CASE_YEAR, and FILED_BEFORE as `querypath`. Alacorder will Party Search non-blank fields on Alacourt.com and download to `dirpath`.
     Args:
        querypath (str): Path to query table/spreadsheet (.xls, .xlsx)
        dirpath (str): Path to PDF output directory
        cID (str): Customer ID on Alacourt.com
        uID (str): User ID on Alacourt.com
        pwd (str): Password on Alacourt.com
-       qmax (int): Maximum queries to conduct on Alacourt.com
-       qskip (int): Skip entries at top of query file
        no_update (bool): Do not update query template after completion
        debug (bool): Print detailed runtime information to console
     """
     if isinstance(querypath, dict):
         cf = querypath
     if cf != None:
         querypath = cf["INPUTS"]
         dirpath = cf["OUTPUT_PATH"]
         cID = cf["ALA_CUSTOMER_ID"]
         uID = cf["ALA_USER_ID"]
         pwd = cf["ALA_PASSWORD"]
-        qmax = cf["FETCH_MAX"]
-        qskip = cf["FETCH_SKIP"]
         criminal_only = cf["CRIMINAL_ONLY"]
     else:
         cf = {
             "INPUTS": querypath,
             "OUTPUT_PATH": dirpath,
             "ALA_CUSTOMER_ID": cID,
             "ALA_USER_ID": uID,
             "ALA_PASSWORD": pwd,
-            "FETCH_MAX": qmax,
-            "FETCH_SKIP": qskip,
             "CRIMINAL_ONLY": criminal_only,
         }
 
-    query = read_query(cf["INPUTS"], qmax=qmax, qskip=qskip)
+    query = read_query(cf["INPUTS"])
 
     # start browser and authenticate
     opt = webdriver.ChromeOptions()
     opt.add_experimental_option(
         "prefs",
         {
             "download.default_directory": dirpath,  # Set default directory for downloads
@@ -3462,17 +3430,25 @@
             login(driver, cID=cID, uID=uID, pwd=pwd)
             driver.implicitly_wait(1)
         driver.get("https:v2.alacourt.com/frmIndexSearchForm.aspx")
         print("Successfully connected and logged into Alacourt!")
 
     # field search
 
+    time.sleep(0.5)
+
     # name
     if name != "":
-        party_name_box.send_keys(name)
+        driver.implicitly_wait(1)
+        try:
+            party_name_box.send_keys(name)
+        except selenium.common.exceptions.StaleElementReferenceException:
+            time.sleep(2)
+            driver.implicitly_wait(2)
+            party_name_box.send_keys(name)
     # ssn
     if ssn != "":
         ssn_box = driver.find_element(
             by=By.NAME, value="ctl00$ContentPlaceHolder1$txtSSN"
         )
         ssn_box.send_keys(ssn)
     # dob
@@ -3532,20 +3508,24 @@
             by=By.NAME, value="ctl00$ContentPlaceHolder1$txtTo"
         )
         filed_after_box.send_keys(filed_after)
 
     # submit search
     search_button = driver.find_element(by=By.ID, value="searchButton")
 
+    time.sleep(0.25)
+
     try:
         search_button.click()
     except:
         driver.implicitly_wait(2)
         time.sleep(2)
 
+    time.sleep(0.5)
+
     dlog("Submitted party search form...", cf=debug)
 
     # count pages
     try:
         page_counter = driver.find_element(
             by=By.ID, value="ContentPlaceHolder1_dg_tcPageXofY"
         ).text
@@ -3822,21 +3802,14 @@
                 size=[26, 10],
                 key="SQ-OUTPUTPATH",
             ),
             sg.FolderBrowse(
                 button_text="Select Folder", button_color=("white", "black")
             ),
         ],
-        [
-            sg.Text("Max queries: "),
-            sg.Input(key="SQ-MAX", default_text="0", size=[5, 1]),
-            sg.Text("Skip from top: "),
-            sg.Input(key="SQ-SKIP", default_text="0", size=[5, 1]),
-            sg.Checkbox(key="SQ-CRIMINALONLY", text="Criminal Only"),
-        ],
         [sg.Text("Alacourt.com Credentials", font=BODY_FONT)],
         [
             sg.Text("Customer ID: "),
             sg.Input(key="SQ-CUSTOMERID", size=(16, 1)),
         ],
         [
             sg.Text("User ID:"),
@@ -4350,31 +4323,23 @@
                 window["SQ-INPUTPATH"].get() == ""
                 or window["SQ-OUTPUTPATH"].get() == ""
             ):
                 sg.popup("Check configuration and try again.")
                 continue
             try:
                 pwd = window["SQ-PASSWORD"].get()
-                try:
-                    sq_max = int(window["SQ-MAX"].get().strip())
-                    sq_skip = int(window["SQ-SKIP"].get().strip())
-                except:
-                    sq_max = 0
-                    sq_skip = 0
                 window["SQ"].update(disabled=True)
                 thread = threading.Thread(
                     target=fetch,
                     args=(
                         window["SQ-INPUTPATH"].get(),
                         window["SQ-OUTPUTPATH"].get(),
                         window["SQ-CUSTOMERID"].get(),
                         window["SQ-USERID"].get(),
                         pwd,
-                        sq_max,
-                        sq_skip,
                         window["SQ-CRIMINALONLY"].get(),
                         None,
                         False,
                         False,
                         window,
                     ),
                     daemon=True,
@@ -4536,70 +4501,48 @@
     "--criminal-only",
     "-criminal",
     is_flag=True,
     default=False,
     help="Only search criminal cases",
 )
 @click.option(
-    "--max",
-    "-max",
-    "qmax",
-    required=False,
-    type=int,
-    help="Maximum queries to conduct on Alacourt.com",
-    default=0,
-)
-@click.option(
-    "--skip",
-    "-skip",
-    "qskip",
-    required=False,
-    type=int,
-    help="Skip entries at top of query file",
-    default=0,
-)
-@click.option(
     "--no-mark",
     "-n",
     "no_update",
     is_flag=True,
     default=False,
     help="Do not update query template after completion",
 )
 @click.option(
     "--debug",
     is_flag=True,
     default=False,
     help="Print detailed runtime information to console",
 )
 def _cli_fetch(
-    querypath, path, cID, uID, pwd, qmax, qskip, no_update, criminal_only, debug
+    querypath, path, cID, uID, pwd, no_update, criminal_only, debug
 ):
     """
     Fetch case PDFs from Alacourt.com.
     Args:
         querypath (str): Path to query table/spreadsheet (.xls, .xlsx)
         path (str): Path to PDF output directory
         cID (str): Customer ID on Alacourt.com
         uID (str): User ID on Alacourt.com
         pwd (str): Password on Alacourt.com
-        qmax (int): Maximum queries to conduct on Alacourt.com
-        qskip (int): Skip entries at top of query file
         no_update (bool): Do not update query template after completion
         criminal_only (bool): Only search criminal cases
         debug (bool): Print detailed runtime information to console
     """
     fetch(
         querypath=querypath,
         dirpath=path,
         cID=cID,
         uID=uID,
         pwd=pwd,
-        qmax=qmax,
-        qskip=qskip,
         no_update=no_update,
         criminal_only=criminal_only,
         debug=debug,
     )
 
 
 @main.command(name="multi", help="Export all data tables to .xls/.xlsx")
@@ -5867,21 +5810,21 @@
         ).strip()
     except:
         return ""
 
 
 def getDOB(text):
     try:
-        return re.sub(
+        return datetime.strptime(re.sub(
             r"[^\d/]",
             "",
             re.search(r"(\d{2}/\d{2}/\d{4})(?:.{0,5}DOB:)", str(text)).group(1),
-        ).strip()
+        ).strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getPhone(text):
     try:
         text = str(text)
         text = re.sub(r"[^0-9]", "", re.search(r"(Phone: )(.+)", text).group(2)).strip()
         if len(text) < 7 or text[0:10] == "2050000000":
@@ -5997,29 +5940,14 @@
         state = ""
     if len(city) > 3:
         return f"{street1} {street2} {city}, {state} {zipcode}".strip()
     else:
         return f"{street1} {street2} {city} {state} {zipcode}".strip()
 
 
-def getChargesRows(text):
-    m = re.findall(
-        r"(\d{3}\s{1}[A-Z0-9]{4}.{1,200}?.{3}-.{3}-.{3}[^a-z\n]{10,75})", str(text)
-    )
-    return m
-
-
-def getFeeSheetRows(text):
-    m = re.findall(
-        r"(ACTIVE [^\(\n]+\$[^\(\n]+ACTIVE[^\(\n]+[^\n]|Total:.+\$[^A-Za-z\n]*)",
-        str(text),
-    )
-    return m
-
-
 def getTotalRow(text):
     try:
         mmm = re.search(r"(Total:.+\$[^\n]*)", str(text)).group()
         mm = re.sub(r"[^0-9|\.|\s|\$]", "", str(mmm))
         m = re.findall(r"\d+\.\d{2}", str(mm))
         return m
     except:
@@ -6091,17 +6019,17 @@
         )
     except:
         return ""
 
 
 def getCaseYear(text):
     try:
-        return re.search(r"\w{2}\-(\d{4})-\d{6}\.\d{2}", str(text)).group(1)
+        return int(re.search(r"\w{2}\-(\d{4})-\d{6}\.\d{2}", str(text)).group(1))
     except:
-        return ""
+        return None
 
 
 def getLastName(text):
     try:
         return getName(text).split(" ")[0].strip()
     except:
         return ""
@@ -6126,88 +6054,86 @@
 
 def getRelatedCases(text):
     return re.findall(r"(\w{2}\d{12})", str(text))
 
 
 def getFilingDate(text):
     try:
-        return re.sub(
+        return datetime.strptime(re.sub(
             r"Filing Date: ",
             "",
             re.search(r"Filing Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(),
-        ).strip()
+        ).strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getCaseInitiationDate(text):
     try:
-        return re.sub(
+        return datetime.strptime(re.sub(
             r"Case Initiation Date: ",
             "",
             re.search(
                 r"Case Initiation Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)
-            ).group(),
+            ).group(1),  '%m/%d/%Y')
         )
     except:
-        return ""
+        return None
 
 
 def getArrestDate(text):
     try:
-        return re.search(r"Arrest Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+        return datetime.strptime(re.search(r"Arrest Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getOffenseDate(text):
     try:
-        return re.search(r"Offense Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+        return datetime.strptime(re.search(r"Offense Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getIndictmentDate(text):
     try:
-        return re.search(r"Indictment Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+        return datetime.strptime(re.search(r"Indictment Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getYouthfulDate(text):
     try:
-        return re.search(r"Youthful Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+        return datetime.strptime(re.search(r"Youthful Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getRetrieved(text):
     try:
-        return re.search(r"Alacourt\.com (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+        return datetime.strptime(re.search(r"Alacourt\.com (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getCourtAction(text):
     try:
         return re.search(
             r"Court Action: (BOUND|GUILTY PLEA|WAIVED TO GJ|DISMISSED|TIME LAPSED|NOL PROSS|CONVICTED|INDICTED|DISMISSED|FORFEITURE|TRANSFER|REMANDED|WAIVED|ACQUITTED|WITHDRAWN|PETITION|PRETRIAL|COND\. FORF\.)",
             str(text),
         ).group(1)
     except:
         return ""
 
 
 def getCourtActionDate(text):
     try:
-        return re.search(r"Court Action Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(
-            1
-        )
+        return datetime.strptime(re.search(r"Court Action Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getDescription(text):
     try:
         return (
             re.search(r"Charge: ([A-Z\.0-9\-\s]+)", str(text))
             .group(1)
@@ -6424,32 +6350,28 @@
         )
     except:
         return ""
 
 
 def getWarrantIssuanceDate(text):
     try:
-        return (
+        return datetime.strptime(
             re.search(r"(\d\d?/\d\d?/\d\d\d\d) Warrant Issuance Date:", str(text))
             .group(1)
-            .strip()
-        )
+            .strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getWarrantActionDate(text):
     try:
-        return (
-            re.search(r"Warrant Action Date: (\d\d?/\d\d?/\d\d\d\d)", str(text))
-            .group(1)
-            .strip()
-        )
+        return datetime.strptime(
+                re.search(r"Warrant Action Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1).strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getWarrantIssuanceStatus(text):
     try:
         return re.search(r"Warrant Issuance Status: (\w)", str(text)).group(1).strip()
     except:
         return ""
@@ -6510,32 +6432,30 @@
         return re.search(r"Surety Code: ([A-Z0-9]{4})", str(text)).group(1).strip()
     except:
         return ""
 
 
 def getBondReleaseDate(text):
     try:
-        return (
+        return datetime.strptime(
             re.search(r"Release Date: (\d\d?/\d\d?/\d\d\d\d)", str(text))
             .group(1)
-            .strip()
-        )
+            .strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getFailedToAppearDate(text):
     try:
-        return (
+        return datetime.strptime(
             re.search(r"Failed to Appear Date: (\d\d?/\d\d?/\d\d\d\d)", str(text))
             .group(1)
-            .strip()
-        )
+            .strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getBondsmanProcessIssuance(text):
     try:
         return (
             re.search(
                 r"Bondsman Process Issuance: ([^\n]*?) Bondsman Process Return:",
@@ -6557,21 +6477,21 @@
         )
     except:
         return ""
 
 
 def getAppealDate(text):
     try:
-        return re.sub(
+        return datetime.strptime(re.sub(
             r"[\n\s]",
             "",
             re.search(r"([\n\s/\d]*?) Appeal Court:", str(text)).group(1).strip(),
-        )
+        ), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getAppealCourt(text):
     try:
         return re.search(r"([A-Z\-\s]+) Appeal Case Number", str(text)).group(1).strip()
     except:
         return ""
@@ -6619,36 +6539,36 @@
         return re.search(r"Appeal To: (\w?) Appeal", str(text)).group(1).strip()
     except:
         return ""
 
 
 def getLowerCourtAppealDate(text):
     try:
-        return re.sub(
+        return datetime.strptime(re.sub(
             r"[\n\s:\-]",
             "",
             re.search(
                 r"LowerCourt Appeal Date: (\d\d?/\d\d?/\d\d\d\d)", str(text)
             ).group(1),
-        ).strip()
+        ).strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getDispositionDateOfAppeal(text):
     try:
-        return re.sub(
+        return datetime.strptime(re.sub(
             r"[\n\s:\-]",
             "",
             re.search(
                 r"Disposition Date Of Appeal: (\d\d?/\d\d?/\d\d\d\d)", str(text)
             ).group(1),
-        ).strip()
+        ).strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getDispositionTypeOfAppeal(text):
     try:
         return re.sub(
             r"[\n\s:\-]",
             "",
@@ -6676,21 +6596,20 @@
         return re.search(r"Updated By: (\w{3})", str(text)).group(1).strip()
     except:
         return ""
 
 
 def getTransferToAdminDocDate(text):
     try:
-        return (
+        return datetime.strptime(
             re.search(r"Transfer to Admin Doc Date: (\d\d?/\d\d?/\d\d\d\d)", str(text))
             .group(1)
-            .strip()
-        )
+            .strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getTransferDesc(text):
     try:
         return (
             re.search(r"Transfer Desc: ([A-Z\s]{0,15} \d\d?/\d\d?/\d\d\d\d)", str(text))
             .group(1)
@@ -6698,39 +6617,37 @@
         )
     except:
         return ""
 
 
 def getTBNV1(text):
     try:
-        return (
+        return datetime.strptime(
             re.search(r"Date Trial Began but No Verdict \(TBNV1\): ([^\n]+)", str(text))
             .group(1)
-            .strip()
-        )
+            .strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getTBNV2(text):
     try:
-        return (
+        return datetime.strptime(
             re.search(r"Date Trial Began but No Verdict \(TBNV2\): ([^\n]+)", str(text))
             .group(1)
-            .strip()
-        )
+            .strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getTurnOverDate(text):
     try:
-        return re.search(r"TurnOver Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+        return datetime.strptime(re.search(r"TurnOver Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getTurnOverAmt(text):
     try:
         return float(re.search(r"TurnOver Amt\: \$(\d+\.\d\d)", str(text)).group(1))
     except:
         return ""
@@ -6741,24 +6658,24 @@
         return float(re.search(r"Frequency Amt\: \$(\d+\.\d\d)", str(text)).group(1))
     except:
         return ""
 
 
 def getDueDate(text):
     try:
-        return re.search(r"Due Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+        return datetime.strptime(re.search(r"Due Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getLastPaidDate(text):
     try:
-        return re.search(r"Last Paid Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+        return datetime.strptime(re.search(r"Last Paid Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getPayor(text):
     try:
         return re.search(r"Payor\: ([A-Z0-9]{4})", str(text)).group(1)
     except:
         return ""
@@ -6796,87 +6713,85 @@
         return re.search(r"PreTrial\: (YES|NO)", str(text)).group(1)
     except:
         return ""
 
 
 def getPreTrialDate(text):
     try:
-        return re.search(r"PreTrail Date\: (.+)PreTrial", str(text)).group(1).strip()
+        return datetime.strptime(re.search(r"PreTrail Date\: (.+)PreTrial", str(text)).group(1).strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getPreTrialTerms(text):
     try:
         return re.search(r"PreTrial Terms\: (YES|NO)", str(text)).group(1)
     except:
         return ""
 
 
 def getPreTermsDate(text):
     try:
-        return re.search(r"Pre Terms Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+        return datetime.strptime(re.search(r"Pre Terms Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getDelinquent(text):
     try:
         return re.search(r"Delinquent\: (YES|NO)", str(text)).group(1)
     except:
         return ""
 
 
 def getDelinquentDate(text):
     try:
-        return re.search(r"Delinquent Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(
-            1
-        )
+        return datetime.strptime(re.search(r"Delinquent Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getDAMailer(text):
     try:
         return re.search(r"DA Mailer\: (YES|NO)", str(text)).group(1)
     except:
         return ""
 
 
 def getDAMailerDate(text):
     try:
-        return re.search(r"DA Mailer Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
+        return datetime.strptime(re.search(r"DA Mailer Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getWarrantMailer(text):
     try:
         return re.search(r"Warrant Mailer\: (YES|NO)", str(text)).group(1)
     except:
         return ""
 
 
 def getWarrantMailerDate(text):
     try:
-        return re.search(
+        return datetime.strptime(re.search(
             r"Warrant Mailer Date\: (\d\d?/\d\d?/\d\d\d\d)", str(text)
-        ).group(1)
+        ).group(1), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
-def getEnforcementLastUpdate(text):
+def getLastUpdate(text):
     try:
         return re.search(r"Last Update\: (\d\d?/\d\d?/\d\d\d\d)", str(text)).group(1)
     except:
         return ""
 
 
-def getEnforcementUpdatedBy(text):
+def getUpdatedBy(text):
     try:
         return re.search(r"Updated By\: ([A-Z]{3})", str(text)).group(1)
     except:
         return ""
 
 
 def getSentencingRequirementsCompleted(text):
@@ -6886,36 +6801,22 @@
             "",
             ", ".join(re.findall(r"(?:Requrements Completed: )([YES|NO]?)", str(text))),
         )
     except:
         return ""
 
 
-def getSentencingRequrementsCompleted(
-    text,
-):  # [sic] On-Line Services doesn't know how to spell requirements lol
-    try:
-        return re.sub(
-            r"[\n:]|Requrements Completed",
-            "",
-            ", ".join(re.findall(r"(?:Requrements Completed: )([YES|NO]?)", str(text))),
-        )
-    except:
-        return ""
-
-
 def getSentenceDate(text):
     try:
-        return (
+        return datetime.strptime(
             re.search(r"(Sentence Date: )(\d\d?/\d\d?/\d\d\d\d)", str(text))
             .group(2)
-            .strip()
-        )
+            .strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None 
 
 
 def getProbationPeriod(text):
     try:
         return "".join(
             re.search(r"Probation Period: ([^\.]+)", str(text)).group(1).strip()
         ).strip()
@@ -6935,86 +6836,64 @@
     except:
         return ""
 
 
 def getJailCreditPeriod(text):
     try:
         return "".join(
-            re.search(r"Jail Credit Period: ([^\.]+)", str(text)).group(1).strip()
+            re.search(r"Days\.\s*(\d+ Years, \d+ Months, \d+ Days\.)\s+", str(text)).group(1).strip()
         )
     except:
         return ""
 
 
 def getSentenceProvisions(text):
     try:
         return re.search(r"Sentence Provisions: ([Y|N]?)", str(text)).group(1).strip()
     except:
         return ""
 
 
 def getSentenceStartDate(text):
     try:
-        return re.sub(
+        return datetime.strptime(re.sub(
             r"(Sentence Start Date:)",
             "",
             ", ".join(
                 re.findall(r"Sentence Start Date: (\d\d?/\d\d?/\d\d\d\d)", str(text))
             ),
-        ).strip()
+        ).strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getSentenceEndDate(text):
     try:
-        return re.sub(
+        return datetime.strptime(re.sub(
             r"(Sentence End Date:)",
             "",
             ", ".join(
                 re.findall(r"Sentence End Date: (\d\d?/\d\d?/\d\d\d\d)", str(text))
             ),
-        ).strip()
+        ).strip(), '%m/%d/%Y')
     except:
-        return ""
+        return None
 
 
 def getProbationBeginDate(text):
     try:
-        return re.sub(
+        return datetime.strptime(re.sub(
             r"(Probation Begin Date:)",
             "",
             ", ".join(
                 re.findall(r"Probation Begin Date: (\d\d?/\d\d?/\d\d\d\d)", str(text))
             ),
-        ).strip()
-    except:
-        return ""
-
-
-def getSentenceUpdatedBy(text):
-    try:
-        return re.sub(
-            r"(Updated By:)",
-            "",
-            ", ".join(re.findall(r"Updated By: (\w{3}?)", str(text))),
-        ).strip()
+        ).strip(), '%m/%d/%Y')
     except:
-        return ""
-
-
-def getSentenceLastUpdate(text):
-    try:
-        return re.sub(
-            r"(Last Update:)",
-            "",
-            ", ".join(re.findall(r"Last Update: (\d\d?/\d\d?/\d\d\d\d)", str(text))),
-        ).strip()
-    except:
-        return ""
+        return None
 
 
 def getProbationRevoke(text):
     try:
         return re.sub(
             r"(Probation Revoke:)",
             "",
@@ -7055,59 +6934,59 @@
 def getImages(text):
     imgs = re.findall(
         r"(Images\s+?Pages)([^\\n]*)(END OF THE REPORT)", str(text), re.DOTALL
     )
     if len(imgs) > 1:
         imgs = "; ".join(imgs).strip()
     elif len(imgs) == 1:
-        return imgs[0].strip()
+        return imgs[0][1].strip()
     else:
         return ""
 
 
 def getWitnesses(text):
     wit = re.search(r"(Witness.+?Case Action Summary)", str(text), re.DOTALL)
     if wit:
-        wit = re.sub(
-            r"Witness # Date Served Service Type Attorney Issued Type   SJIS Witness List   Date Issued   Subpoena",
-            "",
-            wit,
-            re.DOTALL,
-        )
-        wit = re.sub(
-            r"Date: Time Code Comments   Case Action Summary", "", wit, re.DOTALL
-        )
+        wit = wit.group()
         wit = re.sub(r"© Alacourt.com \d\d?/\d\d?/\d\d\d\d", "", wit, re.DOTALL)
-        wit = re.sub(
-            r"Witness List    4 Requesting Party Name Witness # Date Served Service Type Attorney Issued Type   Date Issued   Subpoena",
-            "",
-            wit,
-            re.DOTALL,
-        )
+        wit = re.sub(r"Witness", "", wit, re.DOTALL)
+        wit = re.sub(r"\#Name", "", wit, re.DOTALL)
+        wit = re.sub(r"Date", "", wit, re.DOTALL)
+        wit = re.sub(r"Served", "", wit, re.DOTALL)
+        wit = re.sub(r"Service", "", wit, re.DOTALL)
+        wit = re.sub(r"Type", "", wit, re.DOTALL)
+        wit = re.sub(r"Attorney", "", wit, re.DOTALL)
+        wit = re.sub(r"Issued", "", wit, re.DOTALL)
+        wit = re.sub(r"Type", "", wit, re.DOTALL)
+        wit = re.sub(r"SJIS", "", wit, re.DOTALL)
+        wit = re.sub(r"Witness", "", wit, re.DOTALL)
+        wit = re.sub(r"List", "", wit, re.DOTALL)
+        wit = re.sub(r"Date Issued", "", wit, re.DOTALL)
+        wit = re.sub(r"Subpoena", "", wit, re.DOTALL)
+        wit = re.sub(r"Date\:", "", wit, re.DOTALL)
+        wit = re.sub(r"Time", "", wit, re.DOTALL)
+        wit = re.sub(r"Code", "", wit, re.DOTALL)
+        wit = re.sub(r"Comments", "", wit, re.DOTALL)
+        wit = re.sub(r"Case Action Summary", "", wit, re.DOTALL)
+        wit = re.sub(r"\:$", "", wit, re.DOTALL)
         return wit.strip()
     else:
         return ""
 
 
 def getSettings(text):
-    settings = re.search(r"(Settings.+Court Action)", str(text), re.DOTALL)
+    settings = re.search(r"(Settings.+?Court Action)", str(text), re.DOTALL)
     if settings:
-        out = settings.group(2)
-        out = re.sub(
-            r"Settings   Date: Que: Time: Description:   Settings", "", out, re.DOTALL
-        )
-        out = re.sub(
-            r"Settings   Settings Date: Que: Time: Description:", "", out, re.DOTALL
-        )
-        out = re.sub(
-            r"Disposition Charges   # Code Court Action Category Cite Court Action",
-            "",
-            out,
-            re.DOTALL,
-        )
+        out = settings.group(1)
+        out = re.sub(r"Settings", "", out, re.DOTALL)
+        out = re.sub(r"Date\:", "", out, re.DOTALL)
+        out = re.sub(r"Que\:", "", out, re.DOTALL)
+        out = re.sub(r"Time\:", "", out, re.DOTALL)
+        out = re.sub(r"Description\:", "", out, re.DOTALL)
+        out = re.sub(r"Court Action", "", out, re.DOTALL)
         return out.strip()
     else:
         return ""
 
 def getBalanceByFeeCode(text, code):
     pat = f"(ACTIVE[^\n]+{code}[^\n]+)"
     rows = re.findall(pat, text)
```

### Comparing `alacorder-80.5.9/PKG-INFO` & `alacorder-80.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.5.9
+Version: 80.6.0
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

