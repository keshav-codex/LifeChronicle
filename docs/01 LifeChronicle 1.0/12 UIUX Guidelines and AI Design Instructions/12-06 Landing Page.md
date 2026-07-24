12-06 Landing Page

1. Introduction

The Landing Page is the public entry point of the LifeChronicle application.

It introduces the application, allows new users to create an account, provides access to existing users, and displays a small selection of approved user testimonials.

The page shall remain clean, minimal, and focused on helping users begin their journey.

2. Purpose

The Landing Page shall allow users to:

Create a new account.

Access an existing account.

Sign in using supported social providers.

Learn the application's identity through its branding.

Read a few approved testimonials.

3. User Access

User	Access

Guest	Yes

Registered User	Redirect to Timeline

Staff	Redirect to Staff Dashboard

4. Page Layout

Uses:

LYT-01 Public Layout

Sections:

Header

Registration

Testimonials

Footer

5. Front View

────────────────────────────────────────────

LifeChronicle Logo

LifeChronicle

Every Moment.

Every Memory.

One Timeline.

────────────────────────────────────────────

Email Address

Phone Number

Password

Confirm Password

[ Create Account ]

────────── OR ──────────

Continue with Google

Continue with Microsoft

Continue with Apple

Already have an account?

Login

────────────────────────────────────────────

★★★★★

"LifeChronicle helped me preserve my family's memories."

— Random Approved User

────────────────────────────────────────────

Footer

────────────────────────────────────────────

The page should fit comfortably on a laptop screen without excessive scrolling. On mobile, sections stack vertically.

6. Page Sections

6.1 Branding

Displays:

Logo

Application Name

Tagline

Purpose:

Create immediate brand recognition.

6.2 Registration

Fields:

Email Address

Phone Number

Password

Confirm Password

Primary Action:

Create Account

The registration form is the main focus of the page.

6.3 Social Login

Supported providers (Version 1.0):

Google

Microsoft

Apple

Additional providers may be enabled through configuration in future versions.

6.4 Existing User

Display:

Already have an account?

Login

Selecting Login opens the Login page.

6.5 Testimonials

Display:

2–3 approved testimonials.

Randomly selected from approved records.

Automatically refreshed periodically.

Only testimonials approved by Staff shall be displayed.

6.6 Footer

Display:

Privacy Policy

Terms & Conditions

Contact Us

Version (optional)

Copyright

7. Navigation Flow

New User

Landing

      │

Create Account

      │

Email Verification

      │

Birth Profile

      │

Timeline

Existing User

Landing

      │

Login

      │

Timeline

8. Business Rules

Email must be unique.

Phone number must be unique.

Password must satisfy security requirements.

Social login shall create or link an account as applicable.

Testimonials shall only display approved entries.

9. Master Data Dependencies

Code Category	Purpose

BRAND_*	Logo, Name, Tagline

BTN_*	Button Labels

TXT_*	Labels & Links

SOCIAL_*	Enabled Login Providers

FOOTER_*	Footer Content

TESTIMONIAL_*	Display Configuration

10. Components Used

LC-HDR-001 Application Header

LC-INP-002 Email Field

LC-INP-004 Phone Number Field

LC-INP-003 Password Field

LC-BTN-001 Primary Button

LC-BTN-003 Social Login Button

LC-CRD-005 Testimonial Card

LC-FTR-001 Public Footer

11. AI Usage

Version 1.0:

No AI interaction on the page.

Background process:

Testimonials displayed on this page originate from user praise classified by AI and approved by Staff.

12. Responsive Behaviour

Mobile

Single-column layout.

Full-width form fields.

Social login buttons stacked vertically.

Testimonials displayed one at a time in a swipeable carousel.

Tablet

Centered form.

Testimonials displayed one or two at a time depending on available width.

Laptop & Desktop

Centered registration form.

Testimonials displayed below the form in a row or carousel.

The visual style shall remain minimal and uncluttered across all devices.

13. Testing Checklist

Registration form validation.

Social login availability.

Login navigation.

Testimonial rotation.

Responsive layout.

Master Data rendering.

Accessibility verification.

14. Summary

The Landing Page introduces users to LifeChronicle through a clean and focused interface. It emphasizes account creation while providing quick access for existing users and reinforcing trust through approved testimonials. The page follows the application's "Simple by Design. Powerful by Architecture." philosophy and serves as the starting point for every user's journey.