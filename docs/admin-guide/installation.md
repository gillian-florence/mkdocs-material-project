# Introduction to Field Service Extensions (Sample)

Field Service Extensions (Sample) enhances Salesforce Field Service by adding capabilities designed to improve technician safety, support mobile productivity, and increase dispatcher visibility.

This managed package provides ready-to-configure features that integrate with an existing Field Service implementation, allowing administrators to enable functionality based on organizational needs.
## Current Features

The current release includes the following features:

- **Working Alone Timer and Alert System**  
Monitor lone worker status and receive alerts when safety timers expire.
- **Mobile Layout**  
Apply mobile-specific layout configurations to improve technician user experience.
- **Mass Recurring Non-Availabilities**  
Schedule large-scale or recurring resource unavailability events.
- **Timesheets Management App**  
Enable resource timesheet tracking, review, and approvals.
- **Union Rules**  
Automatically categorize logged time based on configurable business rules (e.g., Regular, Overtime, Holiday).

## Pre-Installation Requirements
Before installing the package, ensure the following prerequisites are met:

- Salesforce Field Service is enabled in the target org.
- The latest Salesforce Field Service managed package is installed.  
  ➤ [Install the Field Service Package](https://fsl.secure.force.com/install)
- Users are assigned the appropriate Field Service Permission Set Licenses and Permission Sets.
- The Field Service mobile app is configured for technician users:
    - Technicians can log in and use the Field Service mobile app.  
       ➤ [Give Users Access to the Field Service Mobile App](https://help.salesforce.com/s/articleView?id=service.mfs_perms_standard.htm&type=5)
    - The Field Service Connected App is installed in the org.  
       ➤ [Prepare Field Service for Mobile](https://help.salesforce.com/s/articleView?id=sf.mfs_prepare.htm&type=5)
    
## Assign Field Service Permission Sets

Ensure users are assigned the appropriate Field Service Permission Set Licenses and Permission Sets, as outlined below.

| User                     | Permission Set License                         | Permission Sets                                        |
|--------------------------|------------------------------------------------|--------------------------------------------------------|
| **Dispatcher**           | <ul><li>Field Service Dispatcher</li> <li>Field Service Dispatcher Permissions </li></ul>      | <ul><li>Field Service Dispatcher License </li> </ul>    |
| **Technician**           | <ul><li>Field Service Mobile</li> <li>Field Service Scheduling</li>  <ul>                    | <ul><li>Field Service Resource License</li> <li>Field Service Resource Permissions</li> <li>Field Service Mobile License</li></ul>                |  

Refer to Salesforce Help documentation for detailed guidance:

- [Field Service Permission Set Licenses](https://help.salesforce.com/s/articleView?id=sf.field_service_psl.htm)
- [Assign Field Service Permissions](https://help.salesforce.com/s/articleView?id=sf.field_service_permissions.htm)

## Install the Package

To install Field Service Extensions (Sample):

1. Open the installation link provided for your implementation.
2. Log in to the Salesforce org where the package will be installed.
3. Enter the installation password (if required), select **Install for Admin Users Only**, and click **Install**.
> Installation may take several minutes. You will receive an email notification when the process completes.
4. After installation, go to **Setup** and confirm the package appears under **Installed Packages**.

Once installation is complete, proceed to the feature-specific configuration sections.

> **Note:** Available features may vary by implementation. Not all features described in this guide may be enabled in every org.

## Assign Package Licenses

This package uses Salesforce licensing. After installation, assign a license to each user who requires access, including System Administrators, Dispatchers, and Mobile Technicians.

To assign package licenses:

1. From **Setup**, enter **Installed Packages** in the Quick Find box and select **Installed Packages**.
2. Click **Manage Licenses** next to **Field Service Extensions (Sample)**.
3. On the **Package Manager** page, click **Add Users**.
4. Select the users who require access.
5. Click **Add**.

> **Note:** Users without an assigned license will not be able to access package functionality, including administrative configuration.






[def]: https://help.salesforce.com/s/articleView?id=sf.mfs_prepare.htm&type=5