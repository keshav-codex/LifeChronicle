11-01 Accounts ERD

1. Introduction

The Accounts ERD defines the authentication domain of LifeChronicle.

Authentication is intentionally separated from personal identity. A Login Profile represents the permanent application account, while Birth Profile represents the person's identity.

2. Entity Overview

The Accounts domain consists of the following entities:

LoginProfile

AuthenticationProvider

LoginDevice

LoginSession


EmailVerification

PasswordHistory (Future)

3. Entity Relationships

LoginProfile

├── AuthenticationProvider (1:N)

├── LoginDevice (1:N)

├── LoginSession (1:N)

├── EmailVerification (1:N)

├── PasswordHistory (Future) (1:N)

└── BirthProfile (1:1)

4. Entity Responsibilities

LoginProfile

Represents the permanent LifeChronicle account.

Owns authentication settings, security configuration, and links all authentication providers into a single account.

AuthenticationProvider

Represents one authentication method linked to a Login Profile.

Supports Email/Password, Google, GitHub, Facebook, Apple, Microsoft, and future providers while preserving provider-specific information.

LoginDevice

Stores information about devices used to access the application for security monitoring and future device management.

LoginSession

Maintains active and historical login sessions.

Supports future session management and security auditing.

EmailVerification

Tracks verification status for email addresses associated with the Login Profile.

PasswordHistory (Future)

Maintains historical password records for future password reuse policies.

5. Business Rules

The Accounts domain shall ensure:

Every Login Profile has a unique system-generated User ID.

One Login Profile may have multiple Authentication Providers.

The first linked provider becomes the Primary Provider.

If the Primary Provider is removed, another linked provider is automatically 
promoted.

Authentication data is independent of Birth Profile data.

User-entered contact information belongs to the Login Profile.

Provider-specific information belongs to the Authentication Provider.

Accounts follow Soft Delete policies.

6. Summary

The Accounts ERD establishes a provider-independent authentication architecture that separates authentication from identity while supporting multiple login providers, future authentication methods, and enterprise-grade account management.

7. Next Document

11-02 Accounts Data Dictionary