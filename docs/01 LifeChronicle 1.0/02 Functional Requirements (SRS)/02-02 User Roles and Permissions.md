# 02-02 User Roles and Actors

## 1. Introduction

This document defines all actors who interact with the LifeChronicle system. An actor is any person or system component that performs actions within the application.

Clearly identifying actors helps establish permissions, responsibilities, workflows, and access control throughout the application.

---

# 2. Purpose

The objectives of this document are to:

* Identify all system actors.
* Define responsibilities for each actor.
* Establish role-based access control.
* Support secure authorization.
* Guide functional implementation.

---

# 3. Actor Categories

LifeChronicle consists of four primary actor groups:

* Public Visitors
* Registered Users
* Administrative Staff
* System Services

---

# 4. Public Visitor

A Public Visitor is a person who has not yet authenticated.

### Responsibilities

* View Landing Page
* Read public information
* Register
* Login
* Access Forgot Password
* View legal documents

### Restrictions

A Public Visitor cannot access any user data or administrative functions.

---

# 5. 5. Registered User

A Registered User is an authenticated individual who uses LifeChronicle to preserve, organize, and manage their digital life.

Responsibilities
Manage Birth Profile.
Create, edit, and manage events.
Upload and manage images.
Manage relationships.
View relative profiles (subject to privacy settings).
Send and receive relationship invitations.
Send collaborative event invitations.
Accept, reject, or participate in collaborative events.
Manage notifications.
Submit concerns through the Help Desk.
Submit appreciation and feedback.
Receive AI suggestions and recommendations.
Manage account settings.
Change password.
Temporarily suspend or deactivate their account.
Reactivate their account (subject to account status and business rules).
Restrictions

A Registered User cannot:

Access administrative functions.
Access another user's private information beyond the permissions granted by that user's privacy settings.
Modify or delete another user's data.
Perform actions restricted by system business rules or security policies.

---

# 6. Super Admin

The Super Admin is the highest administrative authority within the LifeChronicle system and has complete control over platform administration, governance, security, and system configuration.

Responsibilities
Complete system administration.
Manage Admin accounts.
Manage departments.
Configure the application.
Manage system settings.
Access all reports and analytics.
Manage AI governance.
View audit logs.
Override administrative actions.
View appreciation and user feedback.
View concern reports.
Monitor overall system health and analytics.
View user account information when required.
View user activity logs when required.
View user-generated content only for legitimate administrative purposes, including:
Concern resolution.
Content moderation.
Policy violation investigations.
Legal, security, or compliance requirements.
Restrictions

The Super Admin shall not:

Edit user events on behalf of users except through approved administrative procedures.
Modify personal memories or user-generated content without authorization.
Access sensitive user information without creating an audit log entry.

Every administrative access to sensitive user information must be recorded in the system audit logs for accountability and security.

Only one Super Admin account exists within the system.

---

# 7. Admin

The Admin manages the day-to-day operation of the platform.

### Responsibilities

* Manage users
* Manage department staff
* Assign work
* View reports
* Configure operational settings
* Review AI recommendations
* Override department-level decisions

Only one Admin account exists within the system.

---

# 8. Department Head

Each department has one Department Head.

### Responsibilities

* Lead the department
* Manage department staff
* Approve department activities
* Assign work
* Review completed tasks
* Generate department reports

Department Heads have authority only within their assigned department.

---

# 9. Department Manager

Multiple Department Managers may exist within a department.

### Responsibilities

* Supervise executives
* Manage assigned work
* Reassign tasks
* Review task completion
* Monitor departmental workload
* Approve delegated operations

---

# 10. Executive

Executives perform operational work assigned by management.

### Responsibilities

* Execute assigned tasks
* Update task progress
* Submit completed work
* Request reassignment
* Mark leave availability

Executives cannot perform administrative configuration.

---

# 11. Artificial Intelligence

AI acts as an intelligent assistant rather than an autonomous decision-maker.

### Responsibilities

* Improve descriptions
* Suggest categories
* Review content quality
* Monitor safety
* Generate reports
* Assist administrators
* Recommend new categories
* Detect abnormal patterns

AI cannot perform destructive actions without human approval.

---

# 12. System Services

Automated background services perform internal operations.

Examples include:

* Email Delivery
* Notification Processing
* Scheduled Tasks
* Security Monitoring
* Audit Logging
* Data Validation
* Configuration Loading
* Backup Operations

---

# 13. Role Hierarchy

The administrative hierarchy is:

```text
Super Admin
        ↓
Admin
        ↓
Department Head
        ↓
Department Manager
        ↓
Executive
```

Reporting relationships are maintained dynamically using the **Reports To** structure rather than fixed hierarchy rules.

---

# 14. Role-Based Access Control

Access throughout the application follows Role-Based Access Control (RBAC).

Permissions are determined by:

* Role
* Department
* Assigned Responsibilities
* Business Rules
* Security Policies

Every request is validated before execution.

---

# 15. Summary

LifeChronicle defines a clear separation of responsibilities between public visitors, registered users, administrative staff, AI services, and automated system processes.

This structured approach improves security, scalability, maintainability, and operational efficiency.

---

# 16. Next Document

**02-03 Landing Page**

The next document specifies the functional requirements for the public landing page, including navigation, authentication entry points, and visitor interactions.
