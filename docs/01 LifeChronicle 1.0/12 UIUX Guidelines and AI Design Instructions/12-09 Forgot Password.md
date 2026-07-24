12-09 Forgot Password

Page Information

Item	Value

Module	12 – UI/UX

Page Name	Forgot Password

Page ID	UI-009

Layout	LYT-02 Authentication Layout

Primary User	Registered User

Status	Version 1.0

1. Introduction

The Forgot Password Page allows registered users to securely reset their account password when they can no longer access their account.

The process is simple, secure, and requires email verification before a new password can be created.

2. Purpose

The page enables users to:

Request a password reset.

Verify their identity through email.

Continue to create a new password.

3. User Access

User	Access

Guest	Yes

Registered User	Yes

Staff	Yes

Administrator	Yes

4. Page Layout

Uses:

LYT-02 Authentication Layout

The page follows the same layout as the Registration and Login pages.

5. Front View

LifeChronicle Logo

Forgot Password

Enter your registered email address.

Email Address

[ Send Verification Link ]

──────────────

Remember your password?

[ Sign In ]

6. Page Sections

6.1 Email Address

User enters the registered email address.

6.2 Primary Action

Send Verification Link

A secure verification email is sent to the registered email address.

6.3 Return to Login

Display:

Remember your password?

Sign In

7. Navigation Flow

Forgot Password

        │

        ▼

Verification Email Sent

        │

        ▼

Email Verification

        │

        ▼

Create New Password

        │

        ▼
Login

8. Business Rules

The email address must exist.

The verification link shall expire after the configured time.

Expired or invalid links shall require a new request.

Password reset is completed only after successful email verification.

9. Master Data

Code	Purpose

TXT_*	Labels

BTN_*	Button Text

MSG_*	Success & Error Messages

EMAIL_*	Email Template

VALIDATION_*	Validation Messages

10. Components Used

LC-INP-002 Email Field

LC-BTN-001 Primary Button

LC-BTN-002 Secondary Button

11. AI Usage

None.

12. Responsive Behaviour

The page shall maintain the same responsive authentication layout used by the Registration and Login pages.

13. Testing Checklist

Registered email validation.

Unknown email handling.

Verification email delivery.

Expired link handling.

Navigation to Login.

Responsive layout.

Accessibility.

14. Summary

The Forgot Password Page provides a secure and straightforward password recovery process. By verifying ownership through the registered email address, it ensures account security while maintaining a familiar authentication experience.

Next Document

12-10 Email Verification