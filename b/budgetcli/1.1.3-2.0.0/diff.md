# Comparing `tmp/budgetcli-1.1.3.tar.gz` & `tmp/budgetcli-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "budgetcli-1.1.3.tar", last modified: Mon May  8 20:30:58 2023, max compression
+gzip compressed data, was "budgetcli-2.0.0.tar", last modified: Tue May 16 19:06:37 2023, max compression
```

## Comparing `budgetcli-1.1.3.tar` & `budgetcli-2.0.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:30:58.114588 budgetcli-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-08 20:30:29.000000 budgetcli-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-08 20:30:58.114588 budgetcli-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-08 20:30:29.000000 budgetcli-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-08 20:30:29.000000 budgetcli-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-08 20:30:58.114588 budgetcli-1.1.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:30:58.106587 budgetcli-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:30:58.106587 budgetcli-1.1.3/src/budgetcli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:30:58.110587 budgetcli-1.1.3/src/budgetcli/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/cli/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     4699 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    11333 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:30:58.110587 budgetcli-1.1.3/src/budgetcli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-08 20:30:29.000000 budgetcli-1.1.3/src/budgetcli/utils/display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 20:30:58.110587 budgetcli-1.1.3/src/budgetcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-05-08 20:30:58.000000 budgetcli-1.1.3/src/budgetcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-08 20:30:58.000000 budgetcli-1.1.3/src/budgetcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 20:30:58.000000 budgetcli-1.1.3/src/budgetcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-08 20:30:58.000000 budgetcli-1.1.3/src/budgetcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-08 20:30:58.000000 budgetcli-1.1.3/src/budgetcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-08 20:30:58.000000 budgetcli-1.1.3/src/budgetcli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:37.750345 budgetcli-2.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-16 19:06:08.000000 budgetcli-2.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-16 19:06:37.750345 budgetcli-2.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2883 2023-05-16 19:06:08.000000 budgetcli-2.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-16 19:06:08.000000 budgetcli-2.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-16 19:06:37.750345 budgetcli-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:37.746344 budgetcli-2.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:37.746344 budgetcli-2.0.0/src/budgetcli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:08.000000 budgetcli-2.0.0/src/budgetcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-16 19:06:08.000000 budgetcli-2.0.0/src/budgetcli/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:37.750345 budgetcli-2.0.0/src/budgetcli/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:08.000000 budgetcli-2.0.0/src/budgetcli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-16 19:06:08.000000 budgetcli-2.0.0/src/budgetcli/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-16 19:06:08.000000 budgetcli-2.0.0/src/budgetcli/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-16 19:06:08.000000 budgetcli-2.0.0/src/budgetcli/cli/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-05-16 19:06:08.000000 budgetcli-2.0.0/src/budgetcli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-05-16 19:06:08.000000 budgetcli-2.0.0/src/budgetcli/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-16 19:06:08.000000 budgetcli-2.0.0/src/budgetcli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-16 19:06:08.000000 budgetcli-2.0.0/src/budgetcli/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-16 19:06:08.000000 budgetcli-2.0.0/src/budgetcli/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:37.750345 budgetcli-2.0.0/src/budgetcli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:08.000000 budgetcli-2.0.0/src/budgetcli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-16 19:06:08.000000 budgetcli-2.0.0/src/budgetcli/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-16 19:06:08.000000 budgetcli-2.0.0/src/budgetcli/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-16 19:06:08.000000 budgetcli-2.0.0/src/budgetcli/utils/display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:06:37.750345 budgetcli-2.0.0/src/budgetcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-16 19:06:37.000000 budgetcli-2.0.0/src/budgetcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-16 19:06:37.000000 budgetcli-2.0.0/src/budgetcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 19:06:37.000000 budgetcli-2.0.0/src/budgetcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-16 19:06:37.000000 budgetcli-2.0.0/src/budgetcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-16 19:06:37.000000 budgetcli-2.0.0/src/budgetcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 19:06:37.000000 budgetcli-2.0.0/src/budgetcli.egg-info/top_level.txt
```

### Comparing `budgetcli-1.1.3/LICENSE` & `budgetcli-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.3/README.md` & `budgetcli-2.0.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -3,116 +3,107 @@
 [![Build](https://github.com/madalinpopa/budgetcli/actions/workflows/build.yaml/badge.svg)](https://github.com/madalinpopa/budgetcli/actions/workflows/build.yaml) [![Test](https://github.com/coderustle/budgetcli/actions/workflows/test.yaml/badge.svg)](https://github.com/coderustle/budgetcli/actions/workflows/test.yaml) [![License](https://img.shields.io/pypi/l/budgetcli)](https://img.shields.io/pypi/l/budgetcli)
 
 A simple terminal app written in Python to manage budgets and expenses in Google Sheet.
 
 ## Features
 
 - Add income transactions 
-- Add outcome transactions 
-- List transactions by month
+- Add outcome transactions
 - Add spending categories
+- Add budget for category
+- List spending categories
+- List transactions by month
 
 ## Installation
 
 ```
 pip install budgetcli
 ```
 
-In order to use the app you need first to enable Google Spreadsheet API and to generate app credentials with a
-`client_id` and a `client_secret`.
-
-Please follow the following link for more details: [Authorize credentials for a desktop application](https://developers.google.com/sheets/api/quickstart/python)
+In order to use the app you need first to enable Google Spreadsheet API. Please follow this link for more details: [Authorize credentials for a desktop application](https://developers.google.com/sheets/api/quickstart/python)
 
 ## Configuration
-
 Before start adding transactions and data, you need to do the following steps:
 
 **Provide Google spreadsheet id**
+
+The spreadsheet id can be found in the browser url, for example `https://docs.google.com/spreadsheets/d/SPREADSHEET_ID/edit#gid=2121817768`. 
 ```
 budgetcli config spreadsheet-id ID
 ```
 
 **Copy the client_secret_XXX.json to app config**
-```
+```bash
 budgetcli config credentials-file-path /path/to/client_secret.json
 ```
 
 **Authorize the app access to spreadsheet data**
-```
+```bash
 budgetcli auth
 ```
 
-**Init sheet tables headers**
-```
+**Init sheets and tables**
+```bash
 budgetcli init
 ```
-![](https://github.com/coderustle/budgetcli/blob/main/images/commands/init.gif)
 
 ## Usage
 
 The commands follow the below structure.
-```
+```bash
 budgetcli <VERB> <OBJECT> <OPTIONS>
 ```
 ### Incomes
 To add an income you need to provide only an amount and a category. By default, all the income transactions are added
 with default today date and without no description.
 
 **Add an income**
 ```bash
 budgetcli add income 5000 salary
 ```
 
-![](https://github.com/coderustle/budgetcli/blob/main/images/commands/income.gif)
-
 **Add an income with description**
 ```bash
 budgetcli add income 5000 projects --description "Project A"
 ```
 
-![](https://github.com/coderustle/budgetcli/blob/main/images/commands/income-description.gif)
-
 **Add an income with date and description**
 ```bash
 budgetcli add income 500 projects --description "Project A" --date 2023-04-01
 ```
 
-![](https://github.com/coderustle/budgetcli/blob/main/images/commands/income-date.gif)
-
 ### Outcomes
 Same for outcome transactions, you need to provide only an amount and a category. By default, all the outcome transactions are added
 with default today date and without no description.
 
 **Add an outcome**
 ```bash
 budgetcli add outcome 400 rent
 ```
 
-![](https://github.com/coderustle/budgetcli/blob/main/images/commands/outcome.gif)
-
 **Add an outcome with description**
 ```bash
 budgetcli add 400 rent --date 2023-05-01 --description "Rent for May"
 ```
 
-![](https://github.com/coderustle/budgetcli/blob/main/images/commands/outcome-date.gif)
-
 ### List transactions
 
 **List first 100 transactions**
 ```bash
 budgetcli list transactions
 ```
 
-![](https://github.com/coderustle/budgetcli/blob/main/images/commands/transactions.gif)
-
 **List only first 10 transactions**
 ```bash
 budgetcli list transaction --rows 10
 ```
 
-![](https://github.com/coderustle/budgetcli/blob/main/images/commands/transactions-rows.gif)
-
 **List transactions for a specific month**
 ```bash
 budgetcli list transactions --month April 
 ```
+### Budget
+
+**Add budget for category**
+```bash
+budgetcli add budget 400 rent
+```
```

### Comparing `budgetcli-1.1.3/pyproject.toml` & `budgetcli-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.3/setup.cfg` & `budgetcli-2.0.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = budgetcli
-version = 1.1.3
+version = 2.0.0
 author = Code Rustle
 author_email = coderustle@gmail.com
 description = A simple async budgeting app to manage expenses and budgets in google spreadsheets
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 license_file = LICENSE
```

### Comparing `budgetcli-1.1.3/src/budgetcli/auth.py` & `budgetcli-2.0.0/src/budgetcli/auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """
 This module contains the implementation for get_credentials function used
-to autorize the application and to initiate the user that authorization flow.
+to authorize the application and to initiate the user that authorization flow.
 """
 import os
 
 from google.auth.external_account_authorized_user import (
     Credentials as ExCredentials,
 )
 from google.auth.transport.requests import Request
@@ -36,16 +36,14 @@
 
     return credentials
 
 
 def load_user_token() -> Credentials | None:
     """This function is used to get the user data authorization"""
 
-    credentials: Credentials | None = None
-
     # check if token.json exists in the app config dir
     if os.path.exists(AUTH_TOKEN_PATH):
         credentials = Credentials.from_authorized_user_file(
             AUTH_TOKEN_PATH, SCOPES
         )
 
         if not credentials or not credentials.valid:
@@ -57,7 +55,16 @@
                 credentials.refresh(Request())
             else:
                 return None
 
         return credentials
 
     return None
+
+
+def get_auth_headers() -> dict:
+    """Get the authentication headers from Google credentials"""
+    headers = {}
+    credentials: Credentials | None = load_user_token()
+    if credentials:
+        credentials.apply(headers=headers)
+    return headers
```

### Comparing `budgetcli-1.1.3/src/budgetcli/cli/add.py` & `budgetcli-2.0.0/src/budgetcli/cli/add.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,76 +1,101 @@
 """
 This module contains the commands for adding transactions to the Google sheet
 """
+import asyncio
 from datetime import date as date_obj
 from decimal import Decimal
 
 import typer
 
-from ..commands import AddTransactionCommand, AddCategoryCommand
-from ..models import Transaction, Category, validate_amount, validate_date
+from ..commands import (
+    AddTransactionCommand,
+    AddCategoryCommand,
+    AddBudgetCommand,
+)
+from ..models import (
+    Transaction,
+    Category,
+    validate_amount,
+    validate_date,
+    Budget,
+)
 from ..utils.dates import get_today_date
 
 app = typer.Typer()
 
-DateArgument = typer.Option(
-    get_today_date(), help="The date of the transaction"
-)
-CategoryArgument = typer.Argument(..., help="The category of the transaction")
-DescriptionArgument = typer.Option("", help="Transaction description")
-AmountArgument = typer.Argument(..., help="The amount of the transaction")
+DateArgument = typer.Option(get_today_date())
+CategoryArgument = typer.Argument(...)
+DescriptionArgument = typer.Option("")
+AmountArgument = typer.Argument(...)
 
 
-@app.command()
-def category(name: str = CategoryArgument):
-    """Add a category to Google sheet"""
+@app.command(name="category")
+def category_entry(name: str = CategoryArgument):
+    """Add budget/transaction category"""
     if name:
         cat = Category(name)
         command = AddCategoryCommand(cat)
-        command.execute()
+        asyncio.run(command.execute())
+
+
+@app.command(name="budget")
+def budget_entry(
+    amount: str = AmountArgument,
+    category: str = CategoryArgument,
+    date: str = DateArgument,
+):
+    """Add budget for category"""
+    budget_entry_date: date_obj | None = validate_date(date)
+    budget_entry_amount: Decimal | None = validate_amount(amount)
+    if budget_entry_date and budget_entry_amount:
+        budget = Budget(date=budget_entry_date, category=category)
+        budget.amount = budget_entry_amount
+        command = AddBudgetCommand(budget)
+        asyncio.run(command.execute())
 
 
-@app.command()
-def income(
+@app.command(name="income")
+def income_entry(
     amount: str = AmountArgument,
     category: str = CategoryArgument,
     description: str = DescriptionArgument,
     date: str = DateArgument,
 ):
-    """Add an income transaction to the Google sheet"""
+    """Add an income transaction"""
     parsed_date: date_obj | None = validate_date(date)
     parsed_amount: Decimal | None = validate_amount(amount)
 
     if parsed_date and parsed_amount:
         transaction = Transaction(parsed_date, category, description)
         transaction.income = parsed_amount
         command = AddTransactionCommand(transaction)
-        command.execute()
+        asyncio.run(command.execute())
 
 
-@app.command()
-def outcome(
+@app.command(name="outcome")
+def outcome_entry(
     amount: str = AmountArgument,
     category: str = CategoryArgument,
     description: str = DescriptionArgument,
     date: str = DateArgument,
 ):
-    """Add an outcome transaction to the Google sheet"""
+    """Add an outcome transaction"""
     parsed_date: date_obj | None = validate_date(date)
     parsed_amount: Decimal | None = validate_amount(amount)
 
     if parsed_date and parsed_amount:
         transaction = Transaction(parsed_date, category, description)
         transaction.outcome = parsed_amount
         command = AddTransactionCommand(transaction)
-        command.execute()
+        asyncio.run(command.execute())
 
 
 @app.callback(invoke_without_command=True)
 def main(ctx: typer.Context):
-    """Add transactions to the Google sheet"""
+    """Add data to the Google sheet"""
     if not ctx.invoked_subcommand:
         ctx.get_help()
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `budgetcli-1.1.3/src/budgetcli/cli/config.py` & `budgetcli-2.0.0/src/budgetcli/cli/config.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.3/src/budgetcli/cli/display.py` & `budgetcli-2.0.0/src/budgetcli/cli/display.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import calendar
 import typer
 
 from ..utils.config import get_config_list
 from ..commands import ListTransactionCommand, ListCategoryCommand
 from ..utils import dates
 
@@ -36,23 +37,23 @@
 )
 
 
 @app.command()
 def categories(rows: int = RowsOption, name: str = NameOption):
     """List all categories from spreadsheet"""
     command = ListCategoryCommand(rows=rows, name=name)
-    command.execute()
+    asyncio.run(command.execute())
 
 
 @app.command()
 def transactions(rows: int = RowsOption, month: str = MonthOption):
     """List all transactions from spreadsheet"""
     month_number = dates.get_month_number(month)
     command = ListTransactionCommand(rows, month_number)
-    command.execute()
+    asyncio.run(command.execute())
 
 
 @app.command()
 def config():
     """List all the settings from config.json"""
 
     get_config_list()
```

### Comparing `budgetcli-1.1.3/src/budgetcli/data_manager.py` & `budgetcli-2.0.0/src/budgetcli/data_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 import asyncio
 import json
 from abc import ABC, abstractmethod
 from typing import Coroutine, Generic, TypeVar
 
 import httpx
-from google.oauth2.credentials import Credentials
 from rich.pretty import pprint
 
-from .auth import load_user_token
+from .auth import get_auth_headers
 from .settings import API_URL, GVI_URL
-from .utils.config import get_config, update_config
+from .utils.config import get_config
 
 T = TypeVar("T", bound="AbstractDataManager")
 
 SPREADSHEET_ID = get_config("spreadsheet_id")
 
 
+class Client(httpx.AsyncClient):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+
+        self.headers.update(get_auth_headers())
+        self.timeout = 30.0  # default timeout
+
+
 class AbstractDataManager(ABC, Generic[T]):
     """
     Abstract class for data managers
     """
 
-    PARAMS = [
-        "valueInputOption=USER_ENTERED",
-        "includeValuesInResponse=true",
-    ]
-
-    def __init__(self):
+    def __init__(self, session: Client):
+        self.session = session
         self.base_url = f"{API_URL}/{SPREADSHEET_ID}"
         self.gvi_url = f"{GVI_URL}/{SPREADSHEET_ID}/gviz/tq"
-        self.session = httpx.AsyncClient()
-        self.session.headers.update(self.get_auth_headers())
-        self.default_params = "?".join(self.PARAMS)
 
     @abstractmethod
     async def init(self) -> None:
         raise NotImplementedError
 
     @abstractmethod
     async def update(self, values: list[str], a1: str) -> dict[str, str]:
@@ -45,15 +45,19 @@
     async def append(self, values: list[str]) -> dict[str, str]:
         raise NotImplementedError
 
     @abstractmethod
     async def get_records(self, rows: int = 100):
         raise NotImplementedError
 
-    async def _update(self, values: list[str], a1: str) -> dict[str, str]:
+    async def _update(
+        self,
+        values: list[str],
+        a1: str,
+    ) -> dict[str, str]:
         """Update a row or a specific cell"""
         params = "valueInputOption=USER_ENTERED"
         url = f"{self.base_url}/values/{a1}?{params}"
         body = {"range": a1, "majorDimension": "ROWS", "values": [values]}
         response = await self.session.put(url, json=body)
         try:
             response.raise_for_status()
@@ -179,121 +183,147 @@
                 records.append(date)
             elif cel:
                 records.append(cel.get("v"))
             else:
                 records.append("")
         return records
 
-    @staticmethod
-    def get_auth_headers() -> dict:
-        """Get the authentication headers from Google credentials"""
-        headers: dict[str, str] = {}
-        credentials: Credentials | None = load_user_token()
-        if credentials:
-            credentials.apply(headers=headers)
-        return headers
-
 
 class TransactionDataManager(AbstractDataManager):
     SHEET_NAME = "TRANSACTIONS"
-    FIRST_COLUMN = "A"
-    LAST_COLUMN = "E"
+    FIRST_COL = "A"
+    LAST_COL = "E"
     ROW_START = 2
-    TRANSACTIONS_RANGE = (
-        f"{SHEET_NAME}!{FIRST_COLUMN}{ROW_START}:{LAST_COLUMN}"
-    )
+    RANGE = f"{SHEET_NAME}!{FIRST_COL}{ROW_START}:{LAST_COL}"
     HEADERS = ["DATE", "CATEGORY", "DESCRIPTION", "INCOME", "OUTCOME"]
 
     async def init(self) -> None:
         """Create TRANSACTIONS sheet if not exists"""
         a1 = f"{self.SHEET_NAME}!A1"
-        headers = "DATE CATEGORY DESCRIPTION INCOME OUTCOME"
+        headers = "DATE CATEGORY DESCRIPTION INCOME OUTCOME MONTH YEAR"
         sheet_coroutine: Coroutine = self._get_sheet_or_create(self.SHEET_NAME)
         update_coroutine: Coroutine = self._update(headers.split(), a1)
         try:
-            sheet = await asyncio.wait_for(sheet_coroutine, timeout=5)
+            sheet = await asyncio.wait_for(sheet_coroutine, timeout=30.0)
             if sheet:
-                await asyncio.wait_for(update_coroutine, timeout=5)
+                await asyncio.wait_for(update_coroutine, timeout=30.0)
         except asyncio.TimeoutError:
             print("Timeout error")
 
     async def update(self, values: list[str], a1: str) -> dict[str, str]:
         notation = f"{self.SHEET_NAME}!{a1}"
         result = await self._update(values=values, a1=notation)
         return result
 
     async def append(self, values: list) -> dict[str, str]:
         """Add a transaction to the spreadsheet"""
-        result = await self._append(values=values, a1=self.TRANSACTIONS_RANGE)
+        result = await self._append(values=values, a1=self.RANGE)
         return result
 
     async def get_records(self, rows: int = 100) -> list[list[str]]:
         """List transactions. Default 100 rows"""
-        transaction_range = f"{self.TRANSACTIONS_RANGE}{rows + 1}"
+        transaction_range = f"{self.RANGE}{rows + 1}"
         result: list[list[str]] = await self._list(a1=transaction_range)
         return result if result else []
 
     async def get_records_for_month(self, month: int) -> list[list[str]]:
         """Query the transactions for current month"""
         month -= 1  # month query starts from 0 to 11
         query = f"select A,B,C,D,E where month(A)={month}"
         rows = await self._query(query, self.SHEET_NAME)
         transactions = [self._process_row(i) for i in rows] if rows else []
         return transactions
 
 
 class CategoryDataManager(AbstractDataManager):
     SHEET_NAME = "CATEGORIES"
-    FIRST_COLUMN = "A"
-    LAST_COLUMN = "A"
+    FIRST_COL = "A"
+    LAST_COL = "A"
     ROW_START = 2
-    CATEGORY_RANGE = f"{SHEET_NAME}!{FIRST_COLUMN}{ROW_START}:{LAST_COLUMN}"
+    RANGE = f"{SHEET_NAME}!{FIRST_COL}{ROW_START}:{LAST_COL}"
 
     async def init(self) -> None:
         """Create CATEGORY sheet if not exists"""
         a1 = f"{self.SHEET_NAME}!A1"
         headers = "CATEGORY"
         sheet_coroutine: Coroutine = self._get_sheet_or_create(self.SHEET_NAME)
         update_coroutine: Coroutine = self._update([headers], a1)
         try:
-            sheet = await asyncio.wait_for(sheet_coroutine, timeout=5)
+            sheet = await asyncio.wait_for(sheet_coroutine, timeout=30.0)
             if sheet:
-                await asyncio.wait_for(update_coroutine, timeout=5)
+                await asyncio.wait_for(update_coroutine, timeout=30.0)
         except asyncio.TimeoutError:
             print("Timeout error")
 
     async def update(self, values: list[str], a1: str) -> dict[str, str]:
         notation = f"{self.SHEET_NAME}!{a1}"
         result = await self._update(values=values, a1=notation)
         return result
 
     async def append(self, values: list) -> dict[str, str]:
         """Add new category in Google sheet"""
-        result = await self._append(values=values, a1=self.CATEGORY_RANGE)
+        result = await self._append(values=values, a1=self.RANGE)
         return result
 
     async def get_records(self, rows: int = 100):
         """Return all categories"""
-        category_range = f"{self.CATEGORY_RANGE}{rows + 1}"
+        category_range = f"{self.RANGE}{rows + 1}"
         result: list[list[str]] = await self._list(a1=category_range)
         return result if result else []
 
     async def get_records_by_name(self, name: str) -> list[list[str]]:
         """Return a category by a given name"""
         name = name.lower()
         query = f"select A where A='{name}'"
         rows = await self._query(query, self.SHEET_NAME)
         categories = [self._process_row(i) for i in rows] if rows else []
         return categories
 
 
-class ManagerFactory:
-    @staticmethod
-    def create_manager_for(manager_name: str) -> T | None:
-        match manager_name:
-            case "transactions":
-                return TransactionDataManager()
-            case "categories":
-                return CategoryDataManager()
-            case _:
-                pprint("No manager found")
-        return None
+class BudgetDataManager(AbstractDataManager):
+    SHEET_NAME = "BUDGET"
+    FIRST_COL = "A"
+    LAST_COL = "F"
+    ROW_START = 2
+    RANGE = f"{SHEET_NAME}!{FIRST_COL}{ROW_START}:{LAST_COL}"
+
+    async def init(self) -> None:
+        a1 = f"{self.SHEET_NAME}!A1"
+        headers = "DATE CATEGORY PLANNED SPENT"
+        sheet_coroutine = self._get_sheet_or_create(self.SHEET_NAME)
+        update_coroutine = self._update(headers.split(), a1)
+        try:
+            sheet = await asyncio.wait_for(sheet_coroutine, timeout=30.0)
+            if sheet:
+                await asyncio.wait_for(update_coroutine, timeout=30.0)
+        except asyncio.TimeoutError:
+            print("Timeout error")
+
+    async def update(self, values: list[str], a1: str) -> dict[str, str]:
+        notation = f"{self.SHEET_NAME}!{a1}"
+        result = await self._update(values=values, a1=notation)
+        return result
+
+    async def append(self, values: list[str]) -> dict[str, str]:
+        result = await self._append(values=values, a1=self.RANGE)
+        return result
+
+    async def get_records(self, rows: int = 100):
+        budget_range = f"{self.RANGE}{rows + 1}"
+        result: list[list[str]] = await self._list(a1=budget_range)
+        return result if result else []
+
+    async def get_records_by_month(self, month: int) -> list[list[str]]:
+        month -= 1  # month query starts from 0
+        query = f"select A,B,C,D where month(A)={month}"
+        rows = await self._query(query, self.SHEET_NAME)
+        budgets = [self._process_row(i) for i in rows] if rows else []
+        return budgets
+
+    async def get_records_by_month_and_category(
+        self, month: int, cat: str
+    ) -> list[list[str]]:
+        month -= 1  # month array starts from 0
+        query = f"select A,B,C,D where month(A)={month} and B contains '{cat}'"
+        rows = await self._query(query, self.SHEET_NAME)
+        budgets = [self._process_row(i) for i in rows] if rows else []
+        return budgets
```

### Comparing `budgetcli-1.1.3/src/budgetcli/main.py` & `budgetcli-2.0.0/src/budgetcli/main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,29 @@
+import asyncio
 import typer
 from rich import print
 
+from budgetcli.utils.dates import get_today_date
 from .auth import get_user_authorization
 from .cli import add, config, display
 from .commands import InitCommand
 
 # init typer app
 app = typer.Typer()
 
 # register commands
 app.add_typer(config.app, name="config")
 app.add_typer(add.app, name="add")
 app.add_typer(display.app, name="list")
 
+# aliases
+DateArgument = typer.Option(get_today_date())
+CategoryArgument = typer.Argument(...)
+AmountArgument = typer.Argument(...)
+
 
 @app.command()
 def auth():
     """Authorize the app to use the user data"""
     try:
         get_user_authorization()
         print(":heavy_check_mark: User authorized successfully")
@@ -25,15 +32,15 @@
         print(e)
 
 
 @app.command()
 def init():
     """Init the sheets in the Google spreadsheets"""
     command = InitCommand()
-    command.execute()
+    asyncio.run(command.execute())
 
 
 @app.callback(invoke_without_command=True)
 def main(ctx: typer.Context) -> None:
     if ctx.invoked_subcommand is None:
         ctx.get_help()
```

### Comparing `budgetcli-1.1.3/src/budgetcli/models.py` & `budgetcli-2.0.0/src/budgetcli/models.py`

 * *Files 16% similar despite different names*

```diff
@@ -49,14 +49,16 @@
     """
 
     date: date
     category: str
     description: str
     income: Decimal = Decimal(0)
     outcome: Decimal = Decimal(0)
+    month = "=MONTH(TRANSACTIONS!A2:A)"
+    year = "=YEAR(TRANSACTIONS!A2:A)"
 
     @classmethod
     def from_sheet_row(cls, row: list):
         """
         A method to create a transaction from a list of strings
         """
         parsed_date = validate_date(row[0])
@@ -76,14 +78,16 @@
         date_format = "%d-%m-%Y"
         return [
             self.date.strftime(date_format),
             self.category,
             self.description,
             str(self.income),
             str(self.outcome),
+            self.month,
+            self.year,
         ]
 
 
 @dataclass
 class Category:
     """
     Represents a category object
@@ -102,7 +106,48 @@
         return cls(row[0])
 
     def to_sheet_row(self) -> list[str]:
         """
         Return a list with values
         """
         return [self.name]
+
+
+# Google sheet formula to update budget categories
+SUM = "TRANSACTIONS!E2:E"
+CHECK1 = "TRANSACTIONS!B2:B"
+IF1 = 'CONCAT("=";B2:B)'
+CHECK2 = "TRANSACTIONS!F2:F"
+IF2 = 'CONCAT("=";MONTH(A2:A))'
+CHECK3 = "TRANSACTIONS!G2:G"
+IF3 = 'CONCAT("=";YEAR(A2:A))'
+
+
+@dataclass
+class Budget:
+    date: date
+    category: str
+    amount: Decimal = Decimal(0)
+    spent = f"=SUMIFS({SUM};{CHECK1};{IF1};{CHECK2};{IF2};{CHECK3};{IF3})"
+
+    def __post_init__(self):
+        self.category = self.category.lower()
+
+    @classmethod
+    def from_sheet_row(cls, row: list):
+        parsed_date = validate_date(row[0])
+        if parsed_date:
+            return cls(
+                parsed_date,
+                row[1],  # category
+                Decimal(row[2]),  # planned
+                Decimal(row[3]),  # spent
+            )
+
+    def to_sheet_row(self):
+        date_format = "%d-%m-%y"
+        return [
+            self.date.strftime(date_format),
+            self.category,
+            str(self.amount),
+            str(self.spent),
+        ]
```

### Comparing `budgetcli-1.1.3/src/budgetcli/settings.py` & `budgetcli-2.0.0/src/budgetcli/settings.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.3/src/budgetcli/utils/config.py` & `budgetcli-2.0.0/src/budgetcli/utils/config.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.3/src/budgetcli/utils/dates.py` & `budgetcli-2.0.0/src/budgetcli/utils/dates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import calendar
 from datetime import datetime
 
 
 def get_current_month():
-    """An utility function to return the current month number"""
+    """A utility function to return the current month number"""
     now = datetime.now()
     return now.month
 
 
 def get_today_date():
     """An utility function to return today's date"""
     now = datetime.now()
```

### Comparing `budgetcli-1.1.3/src/budgetcli/utils/display.py` & `budgetcli-2.0.0/src/budgetcli/utils/display.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.3/src/budgetcli.egg-info/SOURCES.txt` & `budgetcli-2.0.0/src/budgetcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

