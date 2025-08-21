# BillingPlatform Revenue Recognition Reports

This workspace contains configuration files for custom financial reports used in revenue recognition and accounting analysis.

## Reports Overview

### Trial Balance Report
- Summarizes account balances by financial statement and account.
- Includes detail, subtotal, statement total, grand total, and check sum rows.
- Filters out zero-balance rows.
- Supports filtering by accounting period, currency, and account.
- See: [Reports/Trial Balance/TrialBalance](Reports/Trial%20Balance/TrialBalance)

## Usage

- Each report can be exported to Excel or BI tools for further analysis.
- Filters are available for accounting period, currency, and other relevant fields.
- All SQL files are designed for Oracle syntax and BillingPlatform data model.

## Structure

- `Reports/` contains all report definitions and configuration bundles.
- Each report folder includes the main SQL file and, where applicable, supporting bundle/config files.

## Importing Configuration Bundles

To import a configuration bundle into a new environment:

1. Ensure the `.bndl` file is saved in an accessible location.
2. Navigate to `Setup > Configuration Deployment > Deployment Bundles`.
3. Locate the **Import** button or select **Action > Import** from the drop-down list.
4. Click **Browse** and select the `.bndl` file to import.
5. Click **Save**. The bundle is now uploaded, but not yet deployed.

After upload:

- The Bundle detail page opens. All major bundle activity (Build, Import, Deploy, etc.) is tracked in the Bundle History area.
- You can download a log file for each event listed under Bundle History.
- Under **BUNDLE ACTIONS**, click **Deploy**. Status changes to Deployed if successful.
- If deployment takes longer than expected, you can cancel it using **Cancel Deployment** in Actions. All changes will be reverted, and deployment cannot be resumed after canceling.
- In case of failure, an error message appears at the top of the screen with a link to the generated log file. Log files for each event are also available under Bundle History.

> **Note:** Files are checked for integrity before import. Corrupted or altered files will not be imported.

## Author

Patrick Herrmann  
patrick.herrmann@ravusinc.com

---
For questions or enhancements, contact the author
