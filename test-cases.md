

### Test Case 0: Logging In
> [!INFO] Info
> **Test Case ID:** A00
> **Test Designed by:** Ondřej Kulhavý
> **Test Name:** Logging In
> **Brief description:** This test case verifies the ability to log in to the application.
> **Pre-conditions:** User is logged out and on the login window.
> **Dependencies and Requirements:** Default app settings based on official documentation

| Step | Test Steps | Test Data | Expected Result | Passed | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 1 | Enter valid email and password | admin@email.cz, admin | User should be successfully logged in. |  | Ensure correct credentials. |
| 2 | Verify user is on the dashboard | N/A | User should be redirected to the dashboard. |  |  |

---
### Test Case 1: Logging Out
> [!INFO] Info
> **Test Case ID:** A01
> **Test Designed by:** Ondřej Kulhavý
> **Test Name:** Logging Out
> **Brief description:** This test case verifies the ability to log out of the application.
> **Pre-conditions:** User is logged in with default settings and demo data.
> **Dependencies and Requirements:** Default app settings based on official documentation

| Step | Test Steps | Test Data | Expected Result | Passed | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 1 | Verify user is logged in | N/A | User's name and "Log Out" button should be visible in the dashboard. |  |  |
| 2 | Click on "Log Out" | N/A | Application should log out the user. |  | Dashboard should be closed. |
| 3 | Verify user is on the login window | N/A | User should be redirected to the login window. |  |  |

---
### Test Case 2: Printing Prescription
> [!INFO] Info
> **Test Case ID:** A02
> **Test Designed by:** Ondřej Kulhavý
> **Test Name:** Printing Prescription
> **Brief description:** This test case verifies the ability to print the latest prescription in the dashboard.
> **Pre-conditions:** User is logged in with default settings and demo data.
> **Dependencies and Requirements:** Default app settings based on official documentation

| Step | Test Steps | Test Data | Expected Result | Passed | Notes |
| ---- | ---- | ---- | ---- | ---- | ---- |
| 1 | Navigate to the dashboard | N/A | User should be on the dashboard page. |  |  |
| 2 | Click on the latest prescription | N/A | Prescription details should be displayed. |  |  |
| 3 | Click on the "Print" button | N/A | The application should initiate the printing process. |  | Verify successful printing. |

---
### Test Case 3: Failed Log In
> [!INFO] Info
> **Test Case ID:** A03
> **Test Designed by:** Ondřej Kulhavý
> **Test Name:** Failed Log In
> **Brief description:** This test case verifies the handling of failed login attempts.
> **Pre-conditions:** User is not logged in with default settings and demo data.
> **Dependencies and Requirements:** Default app settings based on official documentation

| Step | Test Steps                              | Test Data                            | Expected Result                                       | Passed | Notes                        |
| ---- | --------------------------------------- | ------------------------------------ | ------------------------------------------------------ | ------ | ----------------------------- |
| 1    | Enter incorrect email and password     | fake@fake.fake, fake                 | Login should fail with an appropriate error message.   |        | Ensure proper error handling. |
| 2    | Verify the displayed error message      | N/A                                  | Error message should accurately describe the issue.   |        |                               |

---
### Test Case 4: Adding New Patient
> [!INFO] Info
> **Test Case ID:** A04
> **Test Designed by:** Ondřej Kulhavý
> **Test Name:** Adding New Patient
> **Brief description:** This test case verifies the ability to add a new patient to the system.
> **Pre-conditions:** User is logged in with default settings and demo data.
> **Dependencies and Requirements:** Default app settings based on official documentation

| Step | Test Steps                              | Test Data                            | Expected Result                                       | Passed | Notes                        |
| ---- | --------------------------------------- | ------------------------------------ | ------------------------------------------------------ | ------ | ----------------------------- |
| 1    | Navigate to the dashboard               | N/A                                  | User should be on the dashboard page.                   |        |                               |
| 2    | Click on "Add Patient"                  | N/A                                  | User should be directed to the patient addition form.   |        |                               |
| 3    | Fill in the patient details             | User-specific details               | Patient should be successfully added to the system.    |        | Ensure valid data.            |

---
### Test Case 5: Failed Adding New Patient
> [!INFO] Info
> **Test Case ID:** A05
> **Test Designed by:** Ondřej Kulhavý
> **Test Name:** Failed Adding New Patient
> **Brief description:** This test case verifies the handling of invalid data when adding a new patient.
> **Pre-conditions:** User is logged in with default settings and demo data.
> **Dependencies and Requirements:** Default app settings based on official documentation

| Step | Test Steps                              | Test Data                            | Expected Result                                       | Passed | Notes                        |
| ---- | --------------------------------------- | ------------------------------------ | ------------------------------------------------------ | ------ | ----------------------------- |
| 1    | Navigate to the dashboard               | N/A                                  | User should be on the dashboard page.                   |        |                               |
| 2    | Click on "Add Patient"                  | N/A                                  | User should be directed to the patient addition form.   |        |                               |
| 3    | Fill in the patient details with invalid data | Invalid data                    | Patient addition should fail with an appropriate error message. |        | Ensure proper error handling. |

---
### Test Case 6: Updating Prescription History
> [!INFO] Info
> **Test Case ID:** A06
> **Test Designed by:** Ondřej Kulhavý
> **Test Name:** Updating Prescription History
> **Brief description:** This test case verifies whether the prescription history updates after adding a new record.
> **Pre-conditions:** User is logged in with default settings and demo data.
> **Dependencies and Requirements:** Default app settings based on official documentation

| Step | Test Steps                              | Test Data                            | Expected Result                                       | Passed | Notes                        |
| ---- | --------------------------------------- | ------------------------------------ | ------------------------------------------------------ | ------ | ----------------------------- |
| 1    | Navigate to the dashboard               | N/A                                  | User should be on the dashboard page.                   |        |                               |
| 2    | Click on "Add Prescription"             | N/A                                  | User should be directed to the prescription creation form. |        |                               |
| 3    | Fill in valid prescription details      | Valid prescription data             | Prescription should be successfully created.          |        | Ensure valid data.           |
| 4    | Verify prescription history            | N/A                                  | Prescription history should be updated with the new record. |        | Check for any unexpected issues. |

---
### Test Case 7: Importing Data to MySQL Database
> [!INFO] Info
> **Test Case ID:** A07
> **Test Designed by:** Ondřej Kulhavý
> **Test Name:** Importing Data to MySQL Database
> **Brief description:** This test case verifies the successful import of data to the MySQL database and the application's ability to run with the imported data.
> **Pre-conditions:** MySQL database is set up and configured according to the documentation.
> **Dependencies and Requirements:** MySQL Workbench, Default app settings based on official documentation

| Step | Test Steps                              | Test Data                            | Expected Result                                       | Passed | Notes                        |
| ---- | --------------------------------------- | ------------------------------------ | ------------------------------------------------------ | ------ | ----------------------------- |
| 1    | Import data to MySQL using Workbench    | Data export file                    | Data should be successfully imported to the MySQL database. |        | Follow documentation steps.  |
| 2    | Run the application                     | N/A                                  | Application should run without errors with the imported data. |        |                               |

---
### Test Case 8: Adding a New Drug
> [!INFO] Info
> **Test Case ID:** A08
> **Test Designed by:** Ondřej Kulhavý
> **Test Name:** Adding a New Drug
> **Brief description:** This test case verifies the ability to add a new drug to the system.
> **Pre-conditions:** User is logged in with default settings and demo data.
> **Dependencies and Requirements:** Default app settings based on official documentation

| Step | Test Steps                              | Test Data                            | Expected Result                                       | Passed | Notes                        |
| ---- | --------------------------------------- | ------------------------------------ | ------------------------------------------------------ | ------ | ----------------------------- |
| 1    | Navigate to the dashboard               | N/A                                  | User should be on the dashboard page.                   |        |                               |
| 2    | Click on "Add Drug"                     | N/A                                  | User should be directed to the drug addition form.      |        |                               |
| 3    | Fill in the drug details                | User-specific drug details          | Drug should be successfully added to the system.        |        | Ensure valid data.           |

---
### Test Case 9: Opening Prescription Details
> [!INFO] Info
> **Test Case ID:** A09
> **Test Designed by:** Ondřej Kulhavý
> **Test Name:** Opening Prescription Details
> **Brief description:** This test case verifies the ability to open and view details of a specific prescription in the prescription history.
> **Pre-conditions:** User is logged in with default settings and demo data.
> **Dependencies and Requirements:** Default app settings based on official documentation

| Step | Test Steps                              | Test Data                            | Expected Result                                       | Passed | Notes                        |
| ---- | --------------------------------------- | ------------------------------------ | ------------------------------------------------------ | ------ | ----------------------------- |
| 1    | Navigate to the dashboard               | N/A                                  | User should be on the dashboard page.                   |        |                               |
| 2    | Open the history of prescriptions       | N/A                                  | User should have access to the prescription history.   |        |                               |
| 3    | Click on "Open" for the most recent prescription | N/A                         | Prescription details should be displayed.              |        | Verify accurate details.     |