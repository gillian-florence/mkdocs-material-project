### Custom Object: Recurring Resource Absence

The Recurring Resource Absence custom object acts as the parent record that stores all related Resource Absence records created as part of a recurring non-availability series.

| **Field Label**                  | **API Name** | **Data Type** | **Description**                                                                 |
|----------------------------------|--------------|---------------|---------------------------------------------------------------------------------|
| Recurring Resource Absence Name | Name         | Auto Number   | Format: `RRA{0000}`                                                             |
| Type                             | Type__c      | Text (30)     | Stores the absence type selected when creating a mass recurring non-availability. |

---

### Custom Fields: Resource Absence Standard Object

The Resource Absence object includes a custom lookup field to associate each absence with its parent Recurring Resource Absence record.

| **Field Label**               | **API Name**                    | **Data Type**                       | **Description**                                                                 |
|-------------------------------|----------------------------------|-------------------------------------|---------------------------------------------------------------------------------|
| Recurring Resource Absence   | Recurring_Resource_Absence__c   | Lookup (Recurring Resource Absence) | Auto-populated with the related Recurring Resource Absence record.              |

---

### Custom Settings

The Mass Recurring NA Settings custom setting controls the maximum number of Resource Absence records that can be created per Service Resource in a single transaction.

- Upon package deployment, the `Max Resource Absence Records Allowed` field is initially `null`.
- However, the **Mass Recurring Non-Availabilities** component restricts users to creating no more than 100 records per Service Resource by default.
- This setting can be configured by an admin to increase or decrease the maximum number of records, up to a hard limit of **999** per Service Resource.
