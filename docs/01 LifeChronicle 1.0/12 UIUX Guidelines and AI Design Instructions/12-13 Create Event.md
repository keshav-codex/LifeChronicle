12-13 Create Event

Page Information

Item	Value

Module	12 – UI/UX

Page Name	Create Event

Page ID	UI-013

Layout	LYT-04 Detail Layout

Primary User	Registered User

Status	Version 1.0

Design Notes

Mobile-first design.

Clean and minimal interface.

One primary action.

Section-based layout.

Progressive disclosure.

Reuse shared UI components.

All visible text managed through Master Data.

Event creation should feel like recording a memory, not filling a form.

1. Introduction

The Create Event page enables users to add a new memory or life event to their Timeline.

Every successfully created Event automatically becomes a new Timeline Node and is displayed chronologically according to its Start Date.

The page is designed to encourage quick and enjoyable memory creation while still supporting rich information such as media, activities, collaboration, location, and privacy.

2. Purpose

The Create Event page allows users to:

Create a Timeline Event.

Categorize the Event.

Record one or more Activities.

Attach Media.

Select a Location.

Invite Collaborators.

Configure Event Privacy.

Save the Event to the Timeline.

3. User Access

User	Access

Registered User	✅

Guest	❌

Staff	❌

Administrator	Administrative Access

4. Page Layout

Uses:

LYT-04 Detail Layout

The page follows a clean vertical layout consisting of expandable sections.

5. Front View

← Back

────────────────────────────────────

Create Event

"Capture another moment from your journey."

────────────────────────────────────

Basic Information

Event Title *

Description

────────────────────────────────────

Category

Parent Category *

Child Category *

────────────────────────────────────

Event Date

Start Date *

End Date

────────────────────────────────────

Activities (0)

➕ Add Activity

────────────────────────────────────

Location

📍 Select Location

────────────────────────────────────

Media

📷 Add Photos / Videos

────────────────────────────────────

Collaboration

👥 Add Participants

────────────────────────────────────

Privacy

🌍 Public

👥 Restricted To

👤 Only Visible To

🔒 Private

────────────────────────────────────

💾 Save Event

6. Page Sections

6.1 Basic Information

Fields

Event Title *

Event Description

6.2 Category

Fields

Parent Category *

Child Category *

Behaviour

Selecting a Parent Category automatically filters the available Child Categories.

Categories are loaded from Master Data.

Users may manually select both Parent and Child Categories.

AI assistance is optional and available before saving the Event.

6.3 Event Date

Fields

Start Date *

End Date

Business Rules

End Date cannot be earlier than Start Date.

Single-day events may omit End Date.

6.4 Activities

Purpose

Activities record smaller moments that occurred during the Event.

Relationship

Event (1)

↓

Activities (N)

Fields

Each Activity may contain

Activity Title

Description

Date & Time (Optional)

Location (Optional)

Media (Optional)

Default View

Activities (3)

────────────────────

🏛 Museum Visit

🍽 Lunch

🚤 Boat Ride

────────────────────

➕ Add Activity

Selecting an Activity opens the Edit Activity page.

Selecting Add Activity opens the Create Activity page.

Activities inherit the Event's Privacy by default.

Activities do not create Timeline Nodes.

6.5 Location

Users may

Search Location

Select on Google Maps

Select Saved Location

System automatically stores

Location Reference

Latitude

Longitude

6.6 Media

Supported Media

Images

Videos

Audio

Documents

Media is managed by the Media Module.

6.7 Collaboration

Users may invite one or more LifeChronicle users to participate.

Invitation Flow

Create Event

↓

Invite Participants

↓

Collaboration Invitation

↓

Accept / Reject

↓

Collaborative Event

Business Rule

If no invited participant accepts within 60 hours, the Collaboration record is automatically removed while audit records are retained.

6.8 Privacy

Every Event shall use one of four privacy modes.

Privacy	Description

🌍 Public	Visible to everyone permitted to view public content.

👥 Restricted To	Visible only to selected Relationship Groups.

👤 Only Visible To	Visible only to selected LifeChronicle users.

🔒 Private	Visible only to the Event Owner.

Restricted To

Restricted To

☑ Family

☑ College Friends

☐ Office Friends

☐ Neighbours

Users may select multiple Relationship Groups.

Only Visible To

Only Visible To

Search User...

☑ Rahul

☑ Amit

☑ Sneha

Users may select multiple LifeChronicle users.

6.9 Primary Action

Save Event

The application shall

Create Event

Create Timeline Node

Store Location

Upload Media

Create Activities

Create Collaboration Invitations

Apply Privacy

Return to Timeline Dashboard

Highlight the newly created Event

7. Navigation Flow

Timeline Dashboard

↓

Create Event

↓

Save Event

↓

Timeline Dashboard

↓

New Event Highlighted

8. Business Rules

Every Event belongs to one Birth Profile.

Every Event belongs to one Parent Category.

Every Event belongs to one Child Category.

Every Event creates exactly one Timeline Node.

Activities belong to one Event.

Activities never appear directly on the Timeline.

Event order is determined by Start Date.

Collaboration is optional.

Privacy is mandatory.

Location and Media are optional unless required by the selected Category.

9. Global Validation Rules

Mandatory

Event Title

Parent Category

Child Category

Start Date

Privacy

Optional

Description

End Date

Activities

Media

Location

Collaboration

System Filled

Event ID

Timeline Node ID

Event Status

Created By

Created On

Updated On

10. Master Data Dependencies

Code	Purpose

CATEGORY_*	Parent & Child Categories

PRIVACY_*	Privacy Options

RELATIONSHIP_GROUP_*	Relationship Groups

BTN_*	Button Labels

TXT_*	Labels

MSG_*	Messages

VALIDATION_*	Validation Messages

ICON_*	Category Icons

11. Shared Components Used

LC-INP-001 Text Field

LC-TXT-001 Text Area

LC-DRP-001 Dropdown

LC-DAT-001 Date Picker

LC-MAP-001 Google Map Picker

LC-MED-001 Media Upload

LC-ACT-001 Activity Card

LC-COL-001 Collaboration Selector

LC-PRV-001 Privacy Selector

LC-BTN-001 Primary Button

12. AI Usage

AI may assist by suggesting:

Better Event Titles

Better Descriptions

Better Categories

Duplicate Event Detection

Missing Media

Missing Location

Missing Date

AI suggestions are optional and never automatically modify user content.

13. Responsive Behaviour

Mobile

Single-column layout.

Bottom sheets for selectors.

Full-screen map picker.

Tablet

Centered layout.

Larger map preview.

Laptop/Desktop

Responsive two-column layout for independent sections such as Media and Location, while maintaining a clear vertical reading order.

14. Testing Checklist

Mandatory field validation.

Category dependency.

Date validation.

Activity creation.

Google Maps integration.

Media upload.

Collaboration invitation.

Privacy selection.

Timeline Node creation.

Responsive behaviour.

Accessibility.

15. Summary

The Create Event page is the primary content creation interface of LifeChronicle. It enables users to capture meaningful life experiences using structured event information, activities, media, locations, collaboration, and flexible privacy controls. Each saved Event becomes a new Timeline Node, allowing the user's life story to grow naturally while maintaining consistency, performance, and ease of use across all supported devices.