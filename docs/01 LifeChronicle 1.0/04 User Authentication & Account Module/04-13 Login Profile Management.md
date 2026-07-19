04-13 Login Profile View & Management
1. Introduction

The Login Profile View & Management module enables authenticated users to view and manage the authentication methods and account-related settings associated with their LifeChronicle account.

This module focuses exclusively on authentication credentials, login methods, account security, and authentication preferences. Personal information such as the user's name, birth details, and profile media is managed separately within the Birth Profile Module.

2. Purpose

The Login Profile View & Management module shall:

View login profile information.

Manage authentication methods.

Link external identity providers.

Unlink authentication providers.

Manage Email & Password authentication.

Control authentication preferences.

Maintain account security.

3. Login Profile Information

The Login Profile may contain the following information.

Account Information

Registered Email Address

Mobile Number (with Country Code)

Preferred Language

Email Verification Status

Account Status

Account Creation Date

Last Login Date and Time

Authentication Methods

Email & Password

Google

Microsoft

Apple

Facebook

GitHub

Security Information

Linked Authentication Providers

Password Status

Authentication History

Recent Login Activity

4. Features

Authenticated users may:

View Login Profile.

Update Login Profile.

View linked authentication methods.

Link new authentication providers.

Remove linked authentication providers.

Add Email & Password authentication to an externally authenticated account.

Change Password.

View authentication history.

View recent login activity.

5. Linked Authentication Providers

A single LifeChronicle account may support multiple authentication methods simultaneously.

Supported providers include:

Email & Password

Google

Microsoft

Apple

Facebook

GitHub

Additional authentication providers may be supported through system configuration.

6. Login Profile Update

Authenticated users may update:

Registered Mobile Number.

Preferred Language.

Linked Authentication Providers.

Email & Password authentication.

Password.

The following information shall not be directly editable:

Account Creation Date.

Authentication Audit History.

Internal User Identifier.

Email Verification History.

Changes to the registered email address, if permitted by system configuration, shall require identity verification.

7. Business Rules

The system shall ensure:

One external identity provider account is linked to only one LifeChronicle account.

One LifeChronicle account may contain multiple linked authentication methods.

At least one authentication method shall always remain active.

Removing the final authentication method shall not be permitted.

Existing accounts shall be linked rather than duplicated whenever applicable.

Sensitive authentication changes shall require user re-authentication before completion.

8. Security

Sensitive operations shall require re-authentication, including:

Password changes.

Linking authentication providers.

Unlinking authentication providers.

Registered email changes.

Removal of Email & Password authentication.

Authentication credentials, passwords, tokens, and provider secrets shall never be displayed to users or administrators.

9. Administrative Access

Authorized administrators may:

View login profile information for administrative, security, or investigation purposes.

View linked authentication providers.

View authentication history.

View login activity.

Administrators shall not be able to:

View passwords.

View password hashes.

View authentication tokens.

View provider credentials.

All administrative access shall be recorded in the audit log.

10. Summary

The Login Profile View & Management module provides authenticated users with centralized control over their authentication methods, account security, and login preferences while ensuring provider independence, strong security, configurable business rules, and complete auditability.

11. Next Document

04-14 Authentication Security