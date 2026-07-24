12-11 Birth Profile

Page Information

Item	Value

Module	12 – UI/UX

Page Name	Birth Profile

Page ID	UI-011

Layout	LYT-04 Detail Layout

Primary User	Registered User

Status	Version 1.0

Design Notes

Mobile-first design.

Calm, modern and minimal interface.

Large profile photograph as the focal point.

One primary action only.

All visible text comes from Master Data.

Birth Profile creates the Birth Node automatically.

Birth Profile remains editable after creation.

1. Introduction

The Birth Profile is the first personal information page completed after email verification.

It represents the beginning of the user's digital life and creates the permanent Birth Node within the Timeline.

The page should feel welcoming and personal rather than like a traditional registration form.

2. Purpose

The Birth Profile allows users to:

Create their Birth Profile.

Create the Birth Node.

Initialize their Timeline.

Record essential birth information.

Upload a profile photograph.

3. User Access

User	Access

Registered User	Yes

Guest	No

Staff	Read Only (where permitted)

Administrator	Administrative Access

4. Page Layout

Uses:

LYT-04 Detail Layout

Simple centered form.

No sidebars.

No unnecessary widgets.

5. Front View

← Back

                ○

          Profile Photo

          Birth Profile

────────────────────────────

Profile Information

Title

First Name *

Middle Name

Last Name *

Childhood Nickname

────────────────────────────

Birth Information

Birth Date *

Birth Time

Birth Day (Auto)

Gender *

Nationality *

────────────────────────────

Delivery Information

Delivery Type

Delivery Place

Delivery Place Name

────────────────────────────

Address Information

Address Line 1 *

Address Line 2

State / Province *

Country *

Postal / PIN Code

Select Birth Location on Map 📍

────────────────────────────

[ Save Birth Profile ]

6. Page Sections

6.1 Profile Information

Fields

Profile Photo *

Title

First Name *

Middle Name

Last Name *

Childhood Nickname

The profile photograph shall remain the visual focus of the page.

6.2 Birth Information

Fields

Birth Date *

Birth Time

Birth Day (Auto Calculated)

Gender *

Nationality *

Birth Day shall be calculated automatically from the selected Birth Date.

6.3 Delivery Information

Fields

Delivery Type

Delivery Place

Delivery Place Name (Conditional)

Delivery Place Name becomes visible only when applicable.

6.4 Address Information

Fields

Address Line 1 *

Address Line 2

State / Province *

Country *

Postal / PIN Code

These fields capture the descriptive birth address.

6.5 Birth Location

Location shall be selected using:

Google Maps

Location Search

Current map marker

The application shall automatically populate:

Latitude

Longitude

Location Reference

These fields are not editable by users.

6.6 Primary Action

Save Birth Profile

On successful save the application shall:

Create Birth Profile

Create Birth Node

Create Timeline

Display Welcome Screen

Navigate to Timeline Dashboard

7. Navigation Flow

Email Verification

        │

        ▼

Birth Profile

        │

        ▼

Save Birth Profile

        │

        ▼

Welcome to LifeChronicle

        │

        ▼

Timeline Dashboard

Returning User

Timeline

↓

Birth Node

↓

Birth Profile

↓

Edit

↓

Save

8. Business Rules

One Birth Profile per user.

Birth Node is created automatically.

Birth Node cannot be deleted.

Birth Profile remains editable.

Birth Day is system calculated.

Latitude and Longitude are system populated.

Profile Status is system managed.

Timeline is created automatically after successful profile creation.

9. Global Validation Rules

Mandatory Fields

Profile Photo

First Name

Last Name

Birth Date

Gender

Nationality

Address Line 1

State / Province

Country

Birth Location

Optional Fields

Title

Middle Name

Childhood Nickname

Birth Time

Delivery Information

Address Line 2

Postal / PIN Code

System Calculated

Birth Day

System Filled

Birth Profile ID

Birth Location Reference

Latitude

Longitude

Profile Status

Created On

Updated On

10. Master Data

Code	Purpose

TITLE_*	Title List

GENDER_*	Gender Options

NATIONALITY_*	Nationalities

DELIVERY_TYPE_*	Delivery Types

DELIVERY_PLACE_*	Delivery Places

COUNTRY_*	Countries

STATE_*	States / Provinces

BTN_*	Button Labels

TXT_*	Labels

MSG_*	Messages

VALIDATION_*	Validation Messages

11. Components Used

Profile Image Upload

Text Field

Date Picker

Time Picker

Dropdown

Google Map Location Picker

Primary Button

12. AI Usage

Version 1.0

None.

Future versions may assist with:

Address suggestions.

Image enhancement.

Duplicate location detection.

AI shall not modify user data automatically.

13. Responsive Behaviour

Mobile

Single-column layout.

Large profile photo.

Full-width input fields.

Full-screen map picker.

Tablet

Centered form.

Larger map preview.

Laptop/Desktop

Compact centered form.

Inline map preview beside address section (optional).

The overall experience shall remain consistent across all screen sizes.

14. Testing Checklist

Mandatory field validation.

Birth Day calculation.

Profile photo upload.

Google Maps location selection.

Address validation.

Birth Node creation.

Timeline creation.

Welcome screen display.

Responsive layout.

Accessibility verification.

15. Summary

The Birth Profile is the foundation of the LifeChronicle application. It captures the user's essential birth information, creates the permanent Birth Node, initializes the Timeline, and marks the beginning of the user's digital life journey. The interface remains clean, personal, and easy to complete while supporting multilingual content, map integration, and future enhancements.