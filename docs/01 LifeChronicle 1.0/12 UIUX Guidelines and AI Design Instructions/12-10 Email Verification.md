12-10 Email Verification

Page Information

Item	Value

Module	12 – UI/UX

Page Name	Email Verification

Page ID	UI-010

Layout	LYT-02 Authentication Layout

Primary User	Guest / Registered User

Status	Version 1.0

1. Introduction

The Email Verification page confirms ownership of the user's email address before allowing account activation or password reset.

The verification process protects user accounts while providing a simple and guided experience.

2. Purpose

The page shall:

Inform users that a verification email has been sent.

Allow users to resend the verification email.

Allow users to change their email address if entered incorrectly.

Confirm successful verification.

Redirect users to the next appropriate page.

3. User Access

User	Access

Guest	Yes

Registered User	During verification

Staff	No

Administrator	No

4. Page Layout

Uses:

LYT-02 Authentication Layout

5. Front View (Verification Pending)

LifeChronicle Logo

Verify Your Email

We've sent a verification link to

krishna@example.com

Please check your inbox and click the verification link.

[ Resend Email ]

[ Change Email ]

────────────────────

Back to Login

6. Front View (Verification Successful)

✓

Email Verified Successfully

Your account has been verified.

[ Continue ]

7. Front View (Verification Failed)

⚠

Verification Failed

The verification link is invalid or has expired.

[ Resend Verification ]

Back to Login

8. Page Sections

8.1 Verification Information

Displays:

Registered email address.

Verification instructions.

8.2 Primary Action

Depending on the current state:

Continue

Resend Verification

8.3 Secondary Actions

Change Email

Back to Login

9. Navigation Flow

Registration

Registration

      │

      ▼

Verification Pending

      │

      ▼

User Clicks Email Link

      │

      ▼

Verification Successful

      │

      ▼

Birth Profile

Forgot Password

Forgot Password

      │

      ▼

Verification Pending

      │

      ▼

Verification Successful

      │

      ▼

Create New Password

      │

      ▼

Login

10. Business Rules

Verification links shall expire after the configured validity period.

Expired links shall not activate the account.

Users may request a new verification email.

Email verification is mandatory before account activation.

Verified accounts shall not require repeated verification unless the email address changes.

11. Master Data

Code	Purpose

TXT_*	Labels & Instructions

BTN_*	Button Labels

MSG_*	Success & Error Messages

EMAIL_*	Email Templates

VALIDATION_*	Validation Messages

12. Components Used

LC-INP-002 Email Field (Change Email)

LC-BTN-001 Primary Button

LC-BTN-002 Secondary Button

LC-CRD-004 Information Card

13. AI Usage

None.

14. Responsive Behaviour

The page shall use the standard Authentication Layout across:

Mobile

Tablet

Laptop

Desktop

15. Testing Checklist

Verification email sent.

Resend verification.

Change email.

Successful verification.

Expired link.

Invalid link.

Continue navigation.

Responsive layout.

Accessibility.

16. Summary

The Email Verification page provides a secure and user-friendly verification process. It guides users through email confirmation, supports common recovery actions such as resending or changing the email address, and directs them to the next step in their journey once verification is complete.

Next Document

12-11 Birth Profile