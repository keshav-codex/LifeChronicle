11-02 Accounts Data Dictionary

1. Introduction

This document defines the data structure for the Accounts domain of LifeChronicle Version 1.0.

The Accounts domain manages authentication, linked authentication providers, devices, sessions, and account security independently from the user's Birth Profile.

2. LoginProfile

### Purpose

Represents the permanent LifeChronicle account.

### Primary Key

- Login Profile ID (System Generated)

### Main Information

- System User ID

- Primary Authentication Provider

- Primary Phone Number

- Account Status

- Security Status

- Created On

- Updated On

### Relationships

- AuthenticationProvider (1:N)

- LoginDevice (1:N)

- LoginSession (1:N)

- EmailVerification (1:N)

- PasswordHistory (1:N) *(Future)*

- BirthProfile (1:1)

---

## 3. AuthenticationProvider

### Purpose

Stores authentication information received from each linked authentication provider.

### Primary Key

- Authentication Provider ID

### Authentication Information

- Provider Type

- Login Identifier (Email, Provider ID, etc.)

- Password Hash *(Email/Password provider only)*

- Password Changed On

- Verification Status

- Active Status

### Provider Information

- Provider User ID

- Email

- Phone Number

- Display Name

- Profile Photo

- Language

- Country

### Provider Metadata

- Provider Metadata (JSON)

- Provider Access Token *(Future - Optional)*

- Provider Refresh Token *(Future - Optional)*

### Audit Information

- Linked On

- Last Login

### Relationships

- LoginProfile (N:1)

4. LoginDevice
Purpose

Maintains the history of devices used to access the application.

Primary Key

Login Device ID

Main Information

Device Identifier

Device Name

Device Type

Operating System

Browser

IP Address

Last Login

Device Status

Relationships

LoginProfile (N:1)

5. LoginSession

Purpose

Stores login session information for security monitoring and future session management.

Primary Key

Login Session ID

Main Information

Login Time

Logout Time

Session Status

Session Token

Device Reference

Relationships

LoginProfile (N:1)

LoginDevice (N:1)

6. EmailVerification

Purpose

Tracks verification activities for email addresses associated with the Login Profile.

Primary Key

Email Verification ID

Main Information

Email Address

Verification Token

Verification Status

Verification Date

Expiry Date

Relationships

LoginProfile (N:1)

AuthenticationProvider (Optional)

7. PasswordHistory (Future)

Purpose

Maintains previous password records to support password history policies.

Primary Key

Password History ID

Main Information

Password Hash

Changed Date

Active Status

Relationships

LoginProfile (N:1)

8. Naming Standards

The Accounts domain shall follow:

Singular entity names.

System-generated primary keys.

Audit fields for all entities.

Soft Delete where applicable.

Foreign key naming consistency.

9. Summary

The Accounts Data Dictionary establishes a normalized, provider-independent authentication structure that supports multiple authentication providers, device history, session tracking, account security, and future authentication methods while remaining independent of the user's personal identity.

10. Next Document

11-03 Birth Profile ERD