
> [!ERROR] Header
> - Tester is Ondřej Kulhavý
> - Tests are combination of the tester and author of the app
> - Everything was tested on school computer PC956

# Test cases

> [!INFO] Info
> **Test Case ID:** TC_001
> **Test Designed by:** Ondřej Kulhavý
> **Test Name:** App Execution with Missing MySQL in XAMPP Workbench
> **Brief description:** Verify the behavior of the app when attempting to run it based on the instructions in the README with MySQL missing in XAMPP Workbench.
> **Pre-conditions:** XAMPP installed on school PCs according to the README instructions.
> **Dependencies and Requirements:** XAMPP, App as per README instructions.

| Step | Test Steps | Test Data | Expected Result | Passed | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 1 | Follow the instructions in the README to run |  | App execution command executed as per README | ⛔ |  |
| 2 | Check the XAMPP Workbench for MySQL presence |  | MySQL is NOT missing in XAMPP Workbench | ⛔ |  |

---

> [!INFO] Info
> **Test Case ID:** TC_002
> **Test Designed by:** Ondřej Kulhavý
> **Test Name:** Manual Database Import Error Resolution
> **Brief description:** Verify the behavior when attempting to manually import the database through MySQL Workbench to resolve the issue mentioned in TC_001, and encountering an error in the SQL dump file.
> **Pre-conditions:** XAMPP installed on school PCs according to the README instructions.
> **Dependencies and Requirements:** XAMPP, MySQL Workbench, SQL dump file.

| Step | Test Steps | Test Data | Expected Result | Passed | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 1 | Open MySQL Workbench | SQL dump | MySQL Workbench application launched | ✅ |  |
| 2 | Attempt to import the SQL dump file | SQL dump | Successful import of database | ⛔ |  |
| 3 | Running app based on readme |  | Successful start of app | ⛔ |  |

---


> [!INFO] Info
> **Test Case ID:** TC_003
> **Test Designed by:** Ondřej Kulhavý
> **Test Name:** Manual Database Import Error Resolution
> **Brief description:** Verify the behavior when attempting to manually import the database through MySQL Workbench to resolve the issue mentioned in TC_001, and encountering an error in the SQL dump file.
> **Pre-conditions:** XAMPP installed on school PCs according to the README instructions.
> **Dependencies and Requirements:** XAMPP, MySQL Workbench, SQL dump file.

| Step | Test Steps | Test Data | Expected Result | Passed | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 1 | Open MySQL Workbench |  | MySQL Workbench application launched | ✅ |  |
| 2 | Navigate to line 29 of the SQL dump file | SQL Dump file | Line 29 of the SQL dump file located | ✅ |  |
| 3 | Identify and analyze the error at line 29 |  | Error in the SQL dump file at line 29 identified | ✅ | Attempting to add privileges to user |
| 4 | Attempt to resolve the error (e.g., correct syntax) |  | Error in the SQL dump file resolved | ✅ | By removing this call |
| 5 | Retry importing the SQL dump file |  | SQL dump file imported successfully after error resolution | ✅ |  |
| 6 | Verify the database imported successfully |  | Database imported without errors | ✅ |  |
| 7 | Attempt to execute the app again |  | App executed successfully after database import | ⛔ | Unsupported version of SQL |

---
|
> [!INFO] Info
> **Test Case ID:** TCO_001
> **Test Designed by:** Erik Vaněk
> **Test Name:** Edit Řidiči Data
> **Brief description:** Verify the behavior when editing Řidiči data by clicking on the pencil icon, modifying the data, and submitting the changes.
> **Pre-conditions:** Řidiči page accessible with editable data.
> **Dependencies and Requirements:** Access to Řidiči page, existing data in the table.

| Step | Test Steps | Test Data | Expected Result | Passed | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 1 | Click on link Řidiči |  | You'll be redirected to page Řidiči. | ⛔ | Bug I001 |
| 2 | Pick any of the shown Řidiči in the table |  | data table. | ⛔ | Bug I001 |
| 3 | Click on the little pencil ✏ |  | The editing window will be shown. | ⛔ | Bug I001 |
| 4 | Edit data in input however you want |  |  | ⛔ | Bug I001 |
| 5 | Click on submit |  | The data will be submitted and successfully edited in the database. | ⛔ | Bug I001 |


# Summery table
| Test Case Id | Test Results | Bugs |
| ---- | ---- | ---- |
| TC_001 | ⛔ | I001 |
| TC_002 | ⛔ | I001 |
| TC_003 | ⛔ | I001 |
| TCO_001 |  | I001 |
|  |  | I001 |

# Incidents

| Incident ID | Summary | Expected Result | Test result | Repro steps | Note |
| ---- | ---- | ---- | ---- | ---- | ---- |
| I001 | Error when loading databases by app | Successfully loaded database and initialized app | ⛔ | TC_001, TC_002, TC_003 |  |
