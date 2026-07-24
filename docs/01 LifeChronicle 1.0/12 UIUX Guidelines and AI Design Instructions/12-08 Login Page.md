12-08 Login Page

Page Information

Item	Value

Module	12 – UI/UX

Page Name	Login

Page ID	UI-008

Layout	LYT-02 Authentication Layout

Primary User	Registered User

Status	Version 1.0

1. Introduction

The Login Page allows registered users to securely access their LifeChronicle account.

The page follows the same visual layout as the Registration Page, providing a familiar and consistent authentication experience.

2. Purpose

The Login Page enables users to:

Sign in using their account credentials.

Sign in using supported social providers.

Recover a forgotten password.

Navigate to account registration if they do not already have an account.

3. User Access

User	Access

Guest	Yes

Registered User	Yes

Staff	Yes

Administrator	Yes

Authenticated users attempting to access this page shall be redirected to their appropriate dashboard.

4. Page Layout

Uses:

LYT-02 Authentication Layout

The Login Page shall use the same layout, spacing, and branding as the Registration Page.

5. Front View

LifeChronicle Logo

Welcome Back

Email Address

Password

Forgot Password?

[ Sign In ]

──────── OR ────────

Continue with Google

Continue with Microsoft

Continue with Apple

Don't have an account?

[ Create Account ]

The page shall remain centered with a clean and distraction-free layout.

6. Page Sections

6.1 Login Form

Fields:

Email Address

Password

Both fields are mandatory.

6.2 Primary Action

Sign In

Authenticates the user and redirects them based on their account status.

6.3 Forgot Password

Selecting Forgot Password opens the password recovery page.

6.4 Social Login

Supported providers:

Google

Microsoft

Apple

etc...

Social login shall authenticate users using their linked accounts.

6.5 New User

Display:

Don't have an account?

Create Account

Selecting Create Account opens the Registration Page.

7. Navigation Flow

Successful Login

Login

   │

   ▼

Birth Profile Completed?

      │

 ┌────┴────┐

 │         │

No        Yes

 │         │

 ▼         ▼

Birth     Timeline

Profile   Dashboard

Forgot Password

Login

↓

Forgot Password

↓

Password Recovery

New User

Login

↓

Create Account

↓

Registration

8. Business Rules

Email address must exist.

Password must match the registered account.

Unverified accounts shall complete email verification before access.

Social login shall only authenticate linked accounts.

After successful login:

If the Birth Profile is incomplete, redirect to Birth Profile.

If complete, redirect to the Timeline Dashboard.

9. Master Data

Code	Purpose

TXT_*	Labels & Messages

BTN_*	Button Text

SOCIAL_*	Enabled Social Providers

VALIDATION_*	Validation Messages

10. Components Used

LC-INP-002 Email Field

LC-INP-003 Password Field

LC-BTN-001 Primary Button

LC-BTN-003 Social Login Button

LC-BTN-002 Secondary Button (Create Account)

11. AI Usage

None.

The Login Page does not use AI functionality.

12. Responsive Behaviour

Mobile

Single-column layout.

Full-width input fields.

Social login buttons stacked vertically.

Tablet

Centered authentication form.

Laptop/Desktop

Compact authentication card with balanced spacing.

The layout shall remain visually identical to the Registration Page.

13. Testing Checklist

Email validation.

Password validation.

Successful authentication.

Failed authentication handling.

Forgot Password navigation.

Social login.

Redirect based on Birth Profile status.

Responsive layout.

Accessibility.

14. Summary

The Login Page provides a secure and familiar sign-in experience using the same authentication layout as the Registration Page. After successful authentication, users are guided either to complete their Birth Profile or directly to their Timeline Dashboard, ensuring a smooth and consistent user journey.

Next Document

12-09 Forgot Password