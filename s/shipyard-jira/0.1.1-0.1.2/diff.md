# Comparing `tmp/shipyard_jira-0.1.1.tar.gz` & `tmp/shipyard_jira-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_jira-0.1.1.tar", max compression
+gzip compressed data, was "shipyard_jira-0.1.2.tar", max compression
```

## Comparing `shipyard_jira-0.1.1.tar` & `shipyard_jira-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      609 2023-05-15 15:13:58.079306 shipyard_jira-0.1.1/README.md
--rw-r--r--   0        0        0      566 2023-05-16 14:47:06.981052 shipyard_jira-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       28 2023-05-12 20:15:15.127680 shipyard_jira-0.1.1/shipyard_jira/__init__.py
--rw-r--r--   0        0        0      932 2023-05-15 19:23:59.579790 shipyard_jira-0.1.1/shipyard_jira/cli/add_comment.py
--rw-r--r--   0        0        0     2283 2023-05-15 19:42:10.388270 shipyard_jira-0.1.1/shipyard_jira/cli/create_ticket.py
--rw-r--r--   0        0        0     1790 2023-05-15 19:42:10.385597 shipyard_jira-0.1.1/shipyard_jira/cli/edit_ticket.py
--rw-r--r--   0        0        0    12490 2023-05-15 19:17:00.981097 shipyard_jira-0.1.1/shipyard_jira/jira.py
--rw-r--r--   0        0        0     1137 1970-01-01 00:00:00.000000 shipyard_jira-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      925 2023-05-17 13:52:05.044803 shipyard_jira-0.1.2/README.md
+-rw-r--r--   0        0        0      538 2023-05-17 13:45:43.414624 shipyard_jira-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       28 2023-05-16 19:54:06.647847 shipyard_jira-0.1.2/shipyard_jira/__init__.py
+-rw-r--r--   0        0        0      962 2023-05-17 13:42:11.918690 shipyard_jira-0.1.2/shipyard_jira/cli/add_comment.py
+-rw-r--r--   0        0        0     2283 2023-05-16 19:54:06.648575 shipyard_jira-0.1.2/shipyard_jira/cli/create_ticket.py
+-rw-r--r--   0        0        0     2290 2023-05-17 13:30:30.655443 shipyard_jira-0.1.2/shipyard_jira/cli/edit_ticket.py
+-rw-r--r--   0        0        0    12673 2023-05-17 13:42:11.929391 shipyard_jira-0.1.2/shipyard_jira/jira.py
+-rw-r--r--   0        0        0     1416 1970-01-01 00:00:00.000000 shipyard_jira-0.1.2/PKG-INFO
```

### Comparing `shipyard_jira-0.1.1/pyproject.toml` & `shipyard_jira-0.1.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 [tool.poetry]
 name = "shipyard-jira"
-version = "0.1.1"
+version = "0.1.2"
 description = "A local client for connecting and working with Jira"
 authors = ["JR <johnathan.rodriguez@shipyardapp.com>"]
 readme = "README.md"
 packages = [{include = "shipyard_jira"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-requests = "2.28.0"
-shipyard-templates = "0.1.2"
+requests = "^2.30.0"
 
 
 [tool.poetry.group.dev.dependencies]
 shipyard-bp-utils = {path = "../shipyard-bp-utils"}
 shipyard-templates = {path = "../../shipyard-templates"}
 
 [build-system]
```

### Comparing `shipyard_jira-0.1.1/shipyard_jira/cli/add_comment.py` & `shipyard_jira-0.1.2/shipyard_jira/cli/add_comment.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,16 @@
     args = get_args()
     jira = JiraClient(access_token=args.access_token,
                       domain=args.domain,
                       email_address=args.email)
 
     try:
         jira.add_comment(ticket_key=args.ticket_key, comment=args.comment)
-    except Exception:
+    except Exception as error:
+        print(error)
         sys.exit(1)
     else:
         sys.exit(0)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `shipyard_jira-0.1.1/shipyard_jira/cli/create_ticket.py` & `shipyard_jira-0.1.2/shipyard_jira/cli/create_ticket.py`

 * *Files identical despite different names*

### Comparing `shipyard_jira-0.1.1/shipyard_jira/jira.py` & `shipyard_jira-0.1.2/shipyard_jira/jira.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         else:
             response = request(
                 url=f'{self.base_url}/{endpoint}',
                 method=method,
                 headers=headers,
                 auth=HTTPBasicAuth(self.email_address, self.access_token))
         if response.status_code == 204:
-            logging.info('Successfully completed request with no response')
+            logging.info('Successfully completed request. Response has no content as expected')
             return {}
 
         response_details = response.json()
 
         if response.ok:
             logging.debug(f"Response: {response.status_code}: {response_details}")
             if response_details:
@@ -114,16 +114,16 @@
         if errors:
             for key, value in errors.items():
                 logging.error(f'An {key} error was encountered: {value}')
                 if key == 'issuetype' and value == 'Specify an issue type':
                     logging.warning(
                         "Please verify that the issue type is spelled correctly and that it's included in the list of "
                         "valid issue types for this project")
-        if not err_msgs and not errors:
-            logging.error(f'Error: {status_code}: {error_details}')
+
+        raise Exception(f'Error: {status_code}: {error_details}')
 
     def create_ticket(self,
                       project_key: str,
                       summary: str,
                       issue_type: str,
                       description: str = None,
                       assignee: str = None,
@@ -141,18 +141,18 @@
         :param kwargs: Any additional fields to be added to the ticket such as labels, priority, etc.
         :return: The response from the request
         """
         if assignee not in ('-1', None):
             logging.info('Retrieving accountId for assignee...')
             try:
                 assignee = self.retrieve_account_id_by_email(assignee)
-            except Exception:
+            except Exception as error:
                 logging.error('Assignee not found. Please verify that the email address is correct.')
                 logging.error('Ticket creation failed')
-                return {}
+                raise Exception(error)
 
         logging.info('Creating Jira Ticket...')
         payload = {
             "fields": {
                 "project": {"key": project_key},
                 "summary": summary,
                 "description": description,
@@ -161,16 +161,17 @@
                 **kwargs
             }
         }
         try:
             response = self._request('issue',
                                      method='POST',
                                      data=payload)
-        except Exception:
+        except Exception as error:
             logging.error('Fail to create Jira ticket')
+            raise Exception(error)
         else:
             logging.info('Jira ticket created successfully')
             return response
 
     def create_subtask(self,
                        parent_ticket_id: str,
                        project_key: str,
@@ -212,20 +213,22 @@
         """
         logging.info('Updating Jira Ticket...')
         data = {
             "update": {
                 **kwargs
             }
         }
+        logging.info(data)
         try:
             response = self._request(f'issue/{ticket_key}',
                                      method='PUT',
                                      data=data)
-        except Exception:
+        except Exception as error:
             logging.error('Fail to update Jira ticket')
+            raise Exception(error)
         else:
             logging.info('Jira ticket updated successfully')
             return response
 
     def get_ticket(self,
                    ticket_id: str
                    ) -> dict:
@@ -233,15 +236,15 @@
         :param ticket_id: The ticket id of the ticket to be retrieved
         :return: The response from the request
         """
         logging.info(f'Getting Jira Ticket {ticket_id}...')
         response = self._request(f'issue/{ticket_id}')
         if response:
             logging.info(f'Jira Ticket {ticket_id} retrieved successfully')
-            logging.info(response)
+            logging.debug(response)
             return response
 
     def find_user_by_email_address(self,
                                    email: str
                                    ) -> dict:
         """
         :param email: The email address of the user to be retrieved
@@ -261,15 +264,15 @@
         """
         :param email: The email address of the user to be retrieved
         :return: The accountId of the user
         """
         try:
             user_details = self.find_user_by_email_address(email)
         except Exception as error:
-            logging.error(error)
+            raise Exception(error)
         else:
             logging.info("Retrieving user's accountId...")
             account_id = user_details.get('accountId')
             if account_id:
                 logging.info('accountId retrieved')
                 return account_id
             else:
@@ -286,16 +289,17 @@
         logging.info('Adding comment to Jira Ticket...')
         try:
             response = self._request(f'issue/{ticket_key}/comment',
                                      method='POST',
                                      data={
                                          'body': comment
                                      })
-        except Exception:
+        except Exception as error:
             logging.error('Fail to add comment to Jira ticket')
+            raise Exception(error)
         else:
             logging.info('Comment added successfully')
             return response
 
     def assign_ticket(self,
                       ticket_key: str,
                       assignee: str
@@ -309,22 +313,22 @@
         :return: The response from the request
         """
         logging.info('Assigning Jira Ticket...')
         if assignee not in ('-1', None):
             try:
                 assignee_id = self.retrieve_account_id_by_email(assignee)
             except Exception as error:
-                logging.error(error)
-                return {}
+                raise Exception(error)
         else:
             assignee_id = assignee
         try:
             response = self._request(f'issue/{ticket_key}/assignee',
                                      method='PUT',
                                      data={
                                          'accountId': assignee_id
                                      })
-        except Exception:
+        except Exception as error:
             logging.error('Fail to assign Jira ticket')
+            raise Exception(error)
         else:
             logging.info('Jira ticket assigned successfully')
             return response
```

### Comparing `shipyard_jira-0.1.1/PKG-INFO` & `shipyard_jira-0.1.2/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 Metadata-Version: 2.1
 Name: shipyard-jira
-Version: 0.1.1
+Version: 0.1.2
 Summary: A local client for connecting and working with Jira
 Author: JR
 Author-email: johnathan.rodriguez@shipyardapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: requests (==2.28.0)
-Requires-Dist: shipyard-templates (==0.1.2)
+Requires-Dist: requests (>=2.30.0,<3.0.0)
 Description-Content-Type: text/markdown
 
-# Create an API token
+# Shipyard Jira
+Shipyard Jira is a Python library that provides a convenient interface for interacting with the Jira issue tracking system. It simplifies the process of managing Jira issues, allowing users to create, update, and query issues programmatically.
+
+## Installation
+```bash
+pip install shipyard-jira
+```
+## Create an API token
 Create an API token from your Atlassian account:
 
 **STEP 1.** Log in to https://id.atlassian.com/manage-profile/security/api-tokens.
 
 **STEP 2.** Click Create API token.
 
 **STEP 3.** From the dialog that appears, enter a memorable and concise Label for your token and click Create.
```

