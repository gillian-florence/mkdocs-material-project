# Introduction to SFS Extensions (SFS-X) App for Field Service

The SFS Extensions (SFS-X) app enhances Salesforce Field Service by delivering additional capabilities that improve technician safety, boost mobile productivity, and increase dispatcher efficiency.

This managed package offers ready-to-configure features that integrate seamlessly with your existing Field Service setup, allowing for quick deployment and adoption.
## Features

The current release of the SFS-X app includes the following features:

- **Working Alone Timer and Alert System**: Monitor lone worker status and receive alerts when safety timers expire.
- **Mobile Layout**: Apply mobile-specific layout configurations to improve technician user experience.
- **Mass Recurring Non-Availabilities**: Schedule large-scale or recurring resource unavailability events.
- **Timesheets Management App**: Enable resource timesheet tracking, review, and approvals.
- **Union Rules**: Automatically categorize logged time based on configurable business rules (e.g., Regular, Overtime, Holiday).

## Pre-Installation Requirements
Before installing the SFS-X app, ensure the following prerequisites are met:

- Field Service is enabled in your Salesforce org.
- The latest Salesforce Field Service managed package is installed.  
  ➤ [Install the Field Service Package](https://fsl.secure.force.com/install)
- All users are assigned the appropriate Field Service Permission Set Licenses and Permission Sets.  
- The Field Service mobile app is configured for technician users:
     - Technicians must be able to log in and use the Field Service mobile app.
         
          ➤ [Give Users Access to the Field Service Mobile App](https://help.salesforce.com/s/articleView?id=service.mfs_perms_standard.htm&type=5)
     
     - The Field Service Connected App must be installed in your org.  
        ➤ [Download the Field Service Connected App](https://help.salesforce.com/s/articleView?id=sf.mfs_prepare.htm&type=5)  
    
## Assign Field Service Permission Sets

Ensure that users in your org are assigned the appropriate Field Service Permission Set Licenses and Permission Sets, as outlined in the table below.

| User                     | Permission Set License                         | Permission Sets                                        |
|--------------------------|------------------------------------------------|--------------------------------------------------------|
| **Dispatcher**           | <ul><li>Field Service Dispatcher</li> <li>Field Service Dispatcher Permissions </li></ul>      | <ul><li>Field Service Dispatcher License </li> </ul>    |
| **Technician**           | <ul><li>Field Service Mobile</li> <li>Field Service Scheduling</li>  <ul>                    | <ul><li>Field Service Resource License</li> <li>Field Service Resource Permissions</li> <li>Field Service Mobile License</li></ul>                |  

Refer to Salesforce Help documentation:

- [Field Service Permission Set Licenses](https://help.salesforce.com/s/articleView?id=sf.field_service_psl.htm)
- [Assign Field Service Permissions](https://help.salesforce.com/s/articleView?id=sf.field_service_permissions.htm)
## Install the SFS-X Package

To install the SFS Extensions app:

1. Click the installation link provided to you by Diabsolut.
2. Log in to the Salesforce org where you want to install the app.
3. Enter the password provided by Diabsolut, select **Install for Admin Users Only**, then click **Install**.
> The installation may take a while. Check your email for confirmation that the installation was successful.
4. Once installation is complete, go to **Setup** and confirm the SFS-X package appears under **Installed Packages**.

After confirming a successful installation, proceed to configure your org by following the procedures outlined in the feature-specific sections.

> **Note:** With the SFS-X managed package, included features are enabled or disabled by Diabsolut based on your organization’s implementation. You may not have access to all the features described in this document.
## Assign Package Licenses

The SFS-X app is a licensed managed package. After installing the package, you must assign a license to each user who requires access to the app functionality, including System Administrators, Dispatchers, and Mobile Technicians.

To assign package licenses:

1. From **Setup**, enter **Installed Packages** in the Quick Find box and select **Installed Packages**.

2. Click **Manage Licenses** next to **SFS Extensions**.

3. On the **Package Manager** page, click **Add Users**.

4. In the **Available Users** list, check the box next to each user you want to assign a license to.
   Selected users will appear in the Selected Users section.

5. Click **Add** when all required users have been selected.

> **Note:** Users who do not have an assigned license will not be able to access any SFS-X functionality, including System Administrators performing configuration tasks.






[def]: https://help.salesforce.com/s/articleView?id=sf.mfs_prepare.htm&type=5