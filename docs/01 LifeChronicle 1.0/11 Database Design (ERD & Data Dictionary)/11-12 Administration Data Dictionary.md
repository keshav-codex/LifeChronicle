11-12 Administration Data Dictionary

1. Introduction

This document defines the data structure for the Administration domain of LifeChronicle Version 1.0.

The Administration domain manages staff members, organizational structure, role-based access, permissions, and operational activities while integrating with shared Audit, AI, and Master Data services.

2. Staff

Purpose

Represents an authorized administrative user of the application.

Primary Key

Staff ID

Main Information

Employee ID

Staff Status

Joining Date

Leaving Date (Optional)

Department

Designation

Created On

Updated On

Relationships

- LoginProfile (1:1)

- StaffRole (1:N)

- Department (Master Data) (N:1)

- Designation (Master Data) (N:1)

- AdministrativeActivityLog (1:N)

3. StaffRole

Purpose

Represents one role assigned to a staff member.

A staff member may have multiple roles.

Primary Key

Staff Role ID

Main Information

Role

Assigned Date

Active Status


Relationships

- Staff (N:1)

- Role (Master Data) (N:1)


5. AdministrativeActivityLog

Purpose

Maintains the operational history of activities performed by staff members.

Primary Key

Administrative Activity Log ID

Main Information

Activity Type

Activity Description

Activity Date & Time

Related Module

Related Record

Activity Status

Relationships

Staff (N:1)

6. Business Rules

The system shall ensure:

Every Staff member is linked to exactly one Login Profile.

A Staff member may have multiple Roles.

Roles determine application permissions.

Permissions are assigned only through Roles.

Departments, Designations, Roles, Permissions, Staff Statuses, and Activity Types are maintained through Master Data.

Dashboard analytics are generated dynamically using application data.

Reports are generated on demand and exported as Excel or PDF.

Staff Activity Logs are permanently preserved.

System-wide auditing is managed through the shared Audit service.

7. Summary

The Administration Data Dictionary provides a normalized structure for managing administrative users, organizational hierarchy, role-based access, staff activities, and operational governance while supporting future organizational expansion.

8. Next Document

11-13 Shared Infrastructure ERD