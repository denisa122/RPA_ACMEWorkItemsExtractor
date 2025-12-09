# ACME Work Items Automation
This UiPath RPA project automates the extraction of work item data from the ACME web portal. It handles user authentication, navigates to the Work Items page, extracts data from the table across multiple pages, and writes the results into an Excel workbook.

## Features
- Opens the ACME web portal in Edge.
- Checks if the user is logged in:
  - If not, prompts the user for email and password and performs login.
  - If already logged in, skips login and logs this information.
- Navigates to the Work Items page.
- Extracts all work items including:
  - WIID
  - Description
  - Type
  - Status
  - Date
- Handles multiple pages in the table automatically.
- Saves the extracted data to an Excel workbook (`Work Items.xlsx`).
- Provides user feedback via message boxes during the process.

## Requirements
- UiPath Studio
- UiPath.UIAutomation and UiPath.Excel.Activities packages installed
- Microsoft Edge browser
- Access to the ACME test portal

## Setup
1. Clone or download this repository.
2. Open the project in UiPath Studio.
3. Ensure all dependencies are installed.
4. Run `Main.xaml`.
5. Enter your email and password if prompted.
6. Wait for the process to complete. The extracted data will be saved in `Work Items.xlsx` in the project folder.
