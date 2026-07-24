Page Information

Item	Value

Module	12 – UI/UX

Page Name	Registration

Page ID	UI-007

Layout	LYT-02 Authentication Layout

Primary User	Guest

Status	Version 1.0

1. Introduction

The Registration Page allows new users to create a LifeChronicle account.

Registration is intentionally simple. Users only provide the minimum information required to begin their journey.

After successful registration, users proceed to email verification before creating their Birth Profile.

2. Purpose

The Registration Page enables users to:

Create a new account.

Validate basic account information.

Continue to email verification.

Choose an alternative sign-in method using supported social providers.

3. User Access

User	Access

Guest	Yes

Registered User	No (Redirect to Timeline)

Staff	No

4. Page Layout

Uses:

LYT-02 Authentication Layout

5. Front View

LifeChronicle Logo

Create Your Account

Email Address

Phone Number

Password

Confirm Password

[ Create Account ]

──────── OR ────────

Continue with Google

Continue with Microsoft

Continue with Apple

Already have an account?

[ Sign In ]

The page shall remain centered with comfortable spacing and no unnecessary graphics.

6. Page Sections

6.1 Registration Form

Fields:

Email Address

Phone Number

Password

Confirm Password

Required fields shall be clearly indicated.

6.2 Primary Action

Create Account

This is the primary action on the page.

6.3 Social Login

Supported providers:

Google

Microsoft

Apple

Additional providers may be enabled through Master Data.

6.4 Existing User

Display:

Already have an account?

Sign In

Selecting Sign In opens the Login Page.

7. Navigation Flow

Registration Success

Registration

↓

Email Verification

↓

Birth Profile

↓

Timeline Dashboard

Existing User

Registration

↓

Sign In

↓

Login

8. Business Rules

Email address must be unique.

Phone number must be unique.

Password and Confirm Password must match.

Password shall follow the configured password policy.

Registration is not completed until email verification succeeds.

Social login shall create or link an account based on the verified email address.

9. Master Data

Code	Purpose

TXT_*	Labels & Messages

BTN_*	Button Text

SOCIAL_*	Enabled Providers

VALIDATION_*	Validation Messages

PASSWORD_POLICY_*	Password Rules

10. Components Used

LC-INP-002 Email Field

LC-INP-004 Phone Number Field

LC-INP-003 Password Field

LC-BTN-001 Primary Button

LC-BTN-003 Social Login Button

11. AI Usage

None.

The Registration Page does not use AI functionality.

12. Responsive Behaviour

Mobile

Single-column layout.

Full-width fields.

Social buttons stacked vertically.

Tablet

Centered form.

Comfortable spacing.

Laptop/Desktop

Compact centered registration card.

13. Testing Checklist

Required field validation.

Email uniqueness.

Phone uniqueness.

Password validation.

Confirm password validation.

Social login availability.

Responsive layout.

Accessibility.

14. Summary

The Registration Page provides a fast and straightforward account creation experience. By requesting only essential information and supporting social sign-in, it reduces friction while maintaining security and preparing users for the next step of creating their Birth Profile.


Next Document

12-08 Login Page