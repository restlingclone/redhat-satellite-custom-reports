# Red Hat Satellite Custom Reports

## Introduction
This repository provides detailed instructions on how to use custom reports in Red Hat Satellite. These reports are designed to help administrators monitor and manage their environments more efficiently by providing insights into various aspects like system configurations, errata, package installations, and more.

## Prerequisites
Before you begin, ensure that you have:
- **Red Hat Satellite** installed and configured (version 6.14 or later recommended).
- Proper permissions to create and run reports in Satellite.
- Basic knowledge of ERB template syntax.

## Custom Reports Overview
The custom reports provided in this repository cover the following areas:
1. **Host Status Reports**: Includes details like Host Name, IP Address, OS Version, Kernel, Content View, Hostgroup, and more.
2. **Errata Reports**: Tracks the application status of specific errata on hosts.
3. **Package Installation Reports**: Verifies whether particular packages are installed on hosts.

## Installation
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/restlingclone/redhat-satellite-custom-reports.git
   cd redhat-satellite-custom-reports
2. **Import Reports into Red Hat Satellite**:
  - Navigate to the Monitor > Reports section in the Red Hat Satellite web UI.
  - Use the import option to upload each .erb template file from the reports/ directory.
  - Assign relevant roles and permissions as needed.
3. **Configure Report Parameters**:
  - Each report template might have inputs such as Host filter, Errata filter, etc.
  - Customize these inputs based on your environment to refine the report output.

##Usage
1. **Running a report**:
  - Go to Monitor > Reports in the Satellite UI.
  - Select the custom report you wish to run.
  - Input the required parameters (e.g., Host filter, Errata ID) and click Generate.
2. **Exporting Results**:
  - Once the report is generated, you can export it in various formats like CSV, JSON, or HTML for further analysis or record-keeping.

##Customization
If you need to modify an existing report:

1. Edit the .erb template file with your preferred text editor.
2. Make necessary changes (e.g., adding/removing fields, altering filters).
3. Re-import the modified template into Red Hat Satellite.

##Troubleshooting
. No Data Returned: Ensure that the parameters used are correct and applicable to your environment.
. Template Errors: Review the ERB syntax for any mistakes or missing variables.
. Permissions Issues: Verify that the user running the report has sufficient permissions

##Contribution
If you have improvements or new report templates, feel free to fork this repository, make your changes, and submit a pull request.

For more details on creating and using custom reports, refer to the Red Hat Satellite documentation.
