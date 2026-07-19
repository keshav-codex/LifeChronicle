04-09 Account Status Management
1. Introduction

The Account Status Management module defines the lifecycle of a LifeChronicle account after authentication. It governs account accessibility, temporary restrictions, deactivation, reactivation, and permanent deletion according to configurable business policies.

2. Purpose

The module shall:

Control account accessibility.

Support temporary suspension.

Support account deactivation.

Manage account reactivation.

Enforce data retention policies.

Protect user accounts.

3. Account Statuses

A user account may exist in one of the following states:

Pending Email Verification

Active

Temporarily Suspended

Deactivated

Permanently Deleted (Policy Driven)

4. Temporary Suspension

A temporary suspension may be initiated by:

User

Administrator

Business Rules:

Minimum suspension period: 15 days (configurable).

Reactivation is not permitted before the minimum period expires.

After the minimum period:

User-initiated suspension: Direct reactivation is permitted.

Administrator-initiated suspension: A reactivation request shall be submitted and approved by an authorized administrator.

5. Account Deactivation

An account may be deactivated by:

User

Administrator

Business Rules:

Minimum deactivation period: 30 days (configurable).

Reactivation is not permitted before the minimum period expires.

After the minimum period:

User-initiated deactivation: Direct reactivation is permitted.

Administrator-initiated deactivation: A reactivation request shall be submitted and approved by an authorized administrator.

6. Permanent Deletion

Business Rules:

If a deactivated account is not reactivated within 60 days from the date of deactivation (configurable), the account shall be permanently deleted according to the application's data retention policy.

After permanent deletion:

The account cannot be restored.

Associated authentication credentials shall no longer be valid.
Any future registration or authentication using the same email address or external identity provider shall be treated as a new user.

7. Reactivation Process

The reactivation process shall:

Validate the account status.

Verify eligibility for reactivation.

Enforce waiting periods.

Apply administrator approval when required.

Restore account access upon successful reactivation.

8. Administrative Control

Authorized administrators may:

Suspend accounts.

Deactivate accounts.

Approve or reject reactivation requests.

View account status history.

Record administrative remarks.

All administrative actions shall be recorded in audit logs.

9. Configuration

The following values shall be configurable through System Configuration:

Minimum suspension period.

Minimum deactivation period.

Permanent deletion period.

Reactivation approval requirements.

Notification templates.

10. Summary

The Account Status Management module provides a configurable and secure account lifecycle framework that balances user flexibility, administrative control, and long-term data management.

11. Next Document

04-10 Session Management