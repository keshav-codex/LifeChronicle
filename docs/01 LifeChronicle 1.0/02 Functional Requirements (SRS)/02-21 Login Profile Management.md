02-21 Login Profile Management

1. Introduction

The Login Profile stores account-related information required for authentication, communication, and account management. It is separate from the Birth Profile, which stores personal life information.

2. Purpose

The Login Profile shall:

Manage authentication information.

Store contact information.

Manage security settings.

Support account maintenance.

3. Actors

Primary Actor:

Registered User

Secondary Actor:

System

4. Functional Requirements

Users shall be able to:

View Login Profile.

Edit Login Profile.

Change Password.

Update Email Address (subject to verification).

Update Mobile Number.

Manage Language Preference.

View Login History.

Temporarily Suspend Account.

Deactivate Account.

Reactivate Account (subject to business rules).

5. Login Profile Information

The profile may contain:

Email Address

Mobile Number (with Country Code)

Preferred Language

Preferred Time Zone (Future)

Account Status

Email Verification Status

Last Login

Login History

6. Security Features

Users shall be able to:

Change Password.

Request Password Reset.

Review Recent Logins.

Review Security Alerts.

Manage Active Sessions (Future).

7. Business Rules

Email must remain unique.

Email changes require verification.

Mobile numbers shall be stored with country codes.

Account suspension and deactivation follow approved business rules.

Security events shall be logged.

8. Validation Rules

The system shall validate:

Email Address.

Mobile Number.

Password Policy.

Account Status.

9. Error Handling

Examples:

Invalid email.

Email already exists.

Invalid mobile number.

Verification failed.

10. Future Enhancements

Multi-factor Authentication.

Device Management.

Trusted Devices.

Passkey Authentication.

11. Summary

The Login Profile manages authentication, communication, and account security while remaining independent of the user's personal life information.

12. Next Document

02-22 Relationship Profile Management