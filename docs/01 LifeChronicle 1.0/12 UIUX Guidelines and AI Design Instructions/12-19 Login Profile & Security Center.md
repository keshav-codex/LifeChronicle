12-19 Login Profile & Security Center

Page Information

Item	Value

Module	12 – UI/UX

Page Name	Login Profile & Security Center

Page ID	UI-019

Layout	LYT-09 Security Layout

Primary User	Registered User

Status	Version 1.0

Design Notes

Security-first design.

Mobile-first.

No AI features.

Progressive disclosure.

Read-only information where appropriate.

Confirmation required for security-sensitive actions.

Simple, modern, and uncluttered.

1. Introduction

The Login Profile & Security Center allows users to manage their authentication methods, login credentials, connected providers, active sessions, and account status.

Unlike the Birth Profile, which represents the user's identity and life journey, the Login Profile manages how the user securely accesses the application.

2. Purpose

The Login Profile enables users to:

Manage email addresses.

Manage phone numbers.

Change password.

Manage connected authentication providers.

View active login sessions.

Review account status.

Temporarily deactivate the account.

Permanently delete the account.

3. User Access

User	Access

Registered User	✅

Guest	❌

Staff	❌

Administrator	Administrative Access Only

4. Page Layout

Uses

LYT-09 Security Layout

The page consists of expandable sections with one primary action per section.

5. Front View

← Back

────────────────────────────

🔐 Login Profile & Security

────────────────────────────

🟢 Account Health (80%)

────────────────────────────

📧 Email Addresses ▼

────────────────────────────

📱 Phone Numbers ▼

────────────────────────────

🔑 Password ▼

────────────────────────────

🔗 Connected Accounts ▼

────────────────────────────

💻 Login Sessions ▼

────────────────────────────

ℹ Account Information ▼

────────────────────────────

⚠ Account Management ▼

6. Page Sections

6.1 Account Health

Displays a simple security summary.

Example

🟢 Account Health

✔ Primary Email Verified

✔ Password Configured

✔ Google Connected

⚠ Phone Number Missing

★★★★☆

Purpose

Help users improve account security.

6.2 Email Addresses

Collapsed by default.

Displays

Primary

krishna@email.com

Verified

────────────────────

Secondary (2)

abc@email.com

Verified

────────────────────

xyz@email.com

Pending Verification

────────────────────

➕ Add Email

Users may:

Add Email

Verify Email

Set Secondary Email as Primary

Delete Secondary Email

Business Rules

Primary Email cannot be edited.

Primary Email cannot be deleted until another verified email becomes Primary.

At least one verified email must always exist.

6.3 Phone Numbers

Displays

Primary

+91 98XXXXXXXX

Verified

────────────────────

➕ Add Phone Number

Users may:

Add Phone Number

Change Phone Number

Delete Phone Number

Phone verification is required.

6.4 Password

Displays

********

Change Password

Users may only:

Change Password

The current password is never displayed.

6.5 Connected Login Providers

Supported providers depend on implementation.

Example

Google

Connected

Disconnect

────────────────────

GitHub

Not Connected

Connect

────────────────────

Microsoft

Not Connected

Connect

Business Rules

The application must always have at least one active authentication method.

Authentication methods include:

Password

Google

Microsoft

GitHub

Apple

Facebook

The system prevents users from removing the final authentication method.

6.6 Login Sessions

Displays

Windows 11

Chrome

Delhi

Current Session

────────────────────

Android

Pixel

Mumbai

Logout Session

Users may:

Logout Individual Session

Logout All Other Sessions

6.7 Account Information

Displays

Account Created On

Last Login

Email Verification Status

Phone Verification Status

Account Status

Read-only.

6.8 Account Management

Displays

⏸ Temporarily Deactivate Account

────────────────────

🗑 Permanently Delete Account

Temporary Deactivation

Effects

Login disabled.

Timeline hidden.

Relationships preserved.

Events preserved.

Collaborations preserved.

Users may reactivate later.

Permanent Deletion

Requires confirmation.

Displays clear warnings before continuing.

Deletion follows the system's data retention policy.

7. Navigation Flow

Timeline

↓

👤 User Menu

↓

Login Profile

↓

Manage Security

↓

Timeline

8. Business Rules

One Primary Email only.

Multiple Secondary Emails allowed.

Email verification required before becoming Primary.

At least one authentication method must always exist.

Password changes require the current password.

Connected providers may be added or removed, subject to the authentication rule.

Temporary deactivation is reversible.

Permanent deletion follows the retention policy.

9. Global Validation Rules

Mandatory

Email verification for new emails.

Phone verification for phone changes.

Current password required to change password.

System Managed

Login sessions.

Authentication providers.

Verification status.

Account status.

10. Master Data Dependencies

Code	Purpose

AUTH_PROVIDER_*	Login Providers

ACCOUNT_STATUS_*	Account Status

BTN_*	Buttons

TXT_*	Labels

MSG_*	Messages

VALIDATION_*	Validation Messages

11. Shared Components Used

LC-ACC-001 Security Card

LC-ACC-002 Authentication Provider Card

LC-ACC-003 Session Card

LC-BTN-001 Primary Button

LC-DLG-001 Confirmation Dialog

LC-LST-001 Expandable List

12. AI Usage


None.

Security-related pages shall not include AI features in Version 1.0.

13. Responsive Behaviour

Mobile

Single-column expandable cards.

Large touch targets.

Tablet

Two-column section layout where space permits.

Laptop/Desktop

Centered security dashboard.

Comfortable spacing.

Expandable cards.

14. Testing Checklist

Add email.

Email verification.

Change primary email.

Phone verification.

Password change.

Connect/disconnect providers.

Login sessions.

Temporary deactivation.

Permanent deletion.

Responsive behaviour.

Accessibility.

15. Summary

The Login Profile & Security Center provides a centralized location for managing account access and security. It separates authentication from personal identity, allowing users to manage emails, phone numbers, passwords, connected providers, login sessions, and account status in a simple, secure, and consistent manner.