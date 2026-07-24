12-15 Manage Event

Page Information

Item	Value

Module	12 – UI/UX

Page Name	Manage Event

Page ID	UI-015

Layout	LYT-04 Detail Layout

Primary User	Event Owner, Authorized Collaborator

Status	Version 1.0

Design Philosophy

The Manage Event page extends the View Event experience by allowing authorized users to update an existing Timeline Event while preserving the familiar page layout.

The page follows LifeChronicle's design principles:

Clean and minimal interface

Content-first design

Premium but lightweight appearance

Reuse existing layouts whenever possible

Progressive disclosure through collapsible sections

Consistent navigation across all Event pages

AI acts only as an assistant

No unnecessary animations or visual distractions

1. Introduction

The Manage Event page enables authorized users to modify an existing Timeline Event.

Rather than presenting a completely different interface, the page reuses the View Event layout and converts appropriate sections into editable components.

This approach minimizes the learning curve while maintaining consistency throughout the Event module.

The page focuses on managing event information rather than creating new content.

2. Purpose

The Manage Event page allows users to:

Update event information

Modify event dates

Update category

Manage personal activities

Manage personal media

Update event location

View collaboration details

Modify privacy settings

Review AI recommendations

Preview changes

Save changes

Delete or archive the event (subject to business rules)

3. User Access

User	Access

Event Owner	Full Event Management

Authorized Collaborator	Limited (based on ownership and permissions)

Guest	No Access

Staff	Administrative Access

4. Ownership Principle

LifeChronicle follows a contribution ownership model.

Every Activity, Media item, Comment, and Note belongs to its creator.

Users may edit or delete only their own contributions.

The Event Owner manages the Event itself but cannot modify another collaborator's personal contribution.

This preserves ownership, accountability, and collaboration integrity.

5. Page Layout

Uses:

LYT-04 Detail Layout

The page reuses the View Event layout while replacing read-only fields with editable controls where appropriate.

The page consists of:

Event Overview

AI Overview

Basic Information

Category

Event Date

Activities

Media

Location

Collaboration

Privacy

AI Suggestions

Action Bar

Advanced sections remain collapsed until needed.

6. Front View

← Timeline

────────────────────────────────────────────

Manage Event

────────────────────────────────────────────

Event Overview

────────────────────────────────────────────

AI Overview

────────────────────────────────────────────

Basic Information ▼

────────────────────────────────────────────

Category ▼

────────────────────────────────────────────

Event Date ▼

────────────────────────────────────────────

Activities (4) ▼

────────────────────────────────────────────

Media (26) ▼

────────────────────────────────────────────

Location ▼

────────────────────────────────────────────

View Collaboration →

────────────────────────────────────────────

Privacy ▼

────────────────────────────────────────────

AI Suggestions (3) ▼

────────────────────────────────────────────

Delete     Cancel     Preview     Save Changes

7. Event Overview

Displayed at the top of the page.

Provides a quick summary before editing begins.

Displays:

Cover Image

Event Title

Category

Event Duration

Location

Activity Count

Media Count

Participant Count

Current Privacy

Last Updated Date

Last Modified By

This section is read-only.

Its purpose is to provide context throughout the editing process.

8. AI Overview

Displayed immediately below the Event Overview.

AI may generate:

Suggested Event Title

Suggested Description

Event Completeness Score

Missing Information Summary

Example:

AI Summary

Suggested Title

Family Vacation to Jaipur

Suggested Description

A memorable family trip exploring

historical places, local culture,

and shared experiences.

Event Completeness

92%

Missing

• Cover Image

• Expense Details

[ Apply ]

[ Ignore ]

Business Rules

AI suggestions are optional.

AI never changes user content automatically.

Users decide whether to apply recommendations.

AI suggestions are regenerated only when requested.

9. Basic Information

Editable fields:

Event Title

Event Description

Users may:

Update the title

Update the description

Validation rules follow those defined in Create Event.

AI may recommend improved wording but never overwrite existing content.

10. Category

Editable fields:

Parent Category

Child Category

Optional AI Assistance:

Suggest Better Category

AI recommendations may consider:

Event Title

Description

Activities

Media

Location

Users may:

Accept recommendation

Ignore recommendation

Category changes update the Event classification immediately after saving.

11. Event Date

Editable fields:

Start Date

End Date

Validation follows Create Event.

If the Start Date changes,

the Timeline automatically reorders the Event after saving.

Users cannot create invalid date ranges.

12. Activities

Activities describe the individual moments that make up an Event.

Examples:

Museum Visit

Lunch

Boat Ride

Coffee Break

The Activities section remains collapsed by default to reduce visual clutter.

Display

Activities (4)

🏛 Museum Visit

Added by: Rahul

🍽 Lunch

Added by: Keshav

🚤 Boat Ride

Added by: Rahul

☕ Coffee Break

Added by: Keshav

+ Add Activity

User Actions

Users may:

Add Activity

Edit their own Activity

Delete their own Activity

View Activities added by other collaborators

Ownership Rules

Each Activity belongs to its creator.

Users:

✅ May edit their own Activities.

✅ May delete their own Activities.

❌ Cannot edit Activities created by another collaborator.

❌ Cannot delete Activities created by another collaborator.

The Event Owner follows the same ownership rules.

Business Rules

Activities never become Timeline Nodes.

Deleting an Activity removes only that Activity.

Deleting an Activity never deletes the Event.

Activity privacy always inherits the Event privacy.

13. Media

The Media section allows users to manage files associated with the Event.

Supported media include:

Photos

Videos

Audio

Documents

The section remains collapsed by default.

Display

Media (26)

□□□□□□□□□□□□□□□□

Photo  Photo  Video  Audio

□□□□□□□□□□□□□□□□

+ Upload Media

User Actions

Users may:

Upload Media

Replace their own Media

Delete their own Media

Change Caption

Set Cover Image (Event Owner only)

Ownership Rules

Each uploaded file belongs to its uploader.

Users:

✅ May edit their own Media.

✅ May delete their own Media.

❌ Cannot modify Media uploaded by another collaborator.

Business Rules

Cover Image may be changed only by the Event Owner.

Deleting Media never deletes the Event.

Media privacy always follows the Event privacy.

14. Location

Displays the Event Location.

The page integrates with Google Maps Platform.

Editable Fields

Location Name

Address

Coordinates (System Managed)

Display

Current Location

Jaipur, Rajasthan

────────────────────

Map Preview

────────────────────

Search Location

Open Google Maps

Change Location

User Actions

Users may:

Search a new location

Select a place from Google Maps

Change Event Location

Business Rules

Changing the Location automatically updates:

Address

Coordinates

Location Reference

The Timeline remains unaffected.

15. Collaboration

Collaboration is managed through a dedicated page.

The Manage Event page provides quick access only.

Display

Participants (5)

View Collaboration →

Selecting View Collaboration opens the Collaboration Management page.

Collaboration Page

Users may:

View Participants

View Invitation Status

View Contribution Summary

View Permissions

The Collaboration page handles:

Invitations

Permissions

Contribution History

This keeps the Manage Event page focused on Event editing.

Ownership Rules

The Event Owner cannot edit another user's:

Activities

Media

Notes

Comments

Every contribution remains owned by its creator.

16. Privacy

Users may modify the Event Privacy.

Available options:

🌍 Public

👥 Restricted

👤 Only Visible To

🔒 Private

Business Rules

Privacy changes affect:

Activities

Media

Attachments

Changes become effective immediately after saving.

17. AI Suggestions

The AI Suggestions section provides optional recommendations to improve Event quality.

The section remains collapsed by default.

Possible Suggestions

Better Title

Better Description

Better Category

Missing Activity

Missing Media

Missing Location

Duplicate Event

Timeline Conflict

User Actions

Users may:

Apply individual suggestions

Ignore suggestions

Request new suggestions

Business Rules

AI never:

Changes user content automatically

Deletes user data

Saves modifications

All AI recommendations require explicit user approval.

18. Primary Actions

Action	Purpose

Preview	Review changes before saving

Save Changes	Save all modifications

Cancel	Discard unsaved changes

Delete Event	Archive or delete (subject to business rules)

Delete Confirmation

Deleting an Event always requires confirmation.

Example:

Delete Event?

This action cannot be undone.

[ Cancel ]

[ Delete ]

19. Navigation Flow

Timeline

↓

View Event

↓

Manage Event

↓

Preview Changes

↓

Save Changes

↓

View Event

↓

Timeline

20. Business Rules

Only authorized users may access the page.

Every change is recorded in the audit log.

Timeline order updates automatically if the Event Date changes.

Activities inherit Event Privacy.

Media inherit Event Privacy.

Users may edit only their own contributions.

AI recommendations are always optional.

Google Maps updates Location information automatically.

Delete operations always require confirmation.

Unsaved changes trigger a warning before leaving the page.

21. Global Validation Rules

The Manage Event page inherits all validation rules defined in 12-13 Create Event.

Additional validation applies only to modifications performed on an existing Event.

Event Validation

Event Title cannot be empty.

Event Date must remain valid.

End Date cannot be earlier than Start Date.

Category must be valid.

Privacy option must be selected.

Activity Validation

Users cannot edit another contributor's Activity.

Deleted Activities are removed only after confirmation.

Empty Activities are not permitted.

Media Validation

Users cannot modify Media uploaded by another contributor.

Cover Image must belong to the current Event.

Unsupported file types are rejected.

Location Validation

A valid Location must be selected.

Google Maps lookup failures do not remove the existing Location.

Coordinates are system managed.

Privacy Validation

Privacy changes apply to all Event content.

Restricted visibility must include at least one authorized user.

Save Validation

The Event cannot be saved until all required validations are satisfied.

22. Master Data Dependencies

Code	Purpose

CATEGORY_*	Categories

PRIVACY_*	Privacy Options

BTN_*	Button Labels

TXT_*	Labels

MSG_*	System Messages

AI_LABEL_*	AI Labels

VALIDATION_*	Validation Messages

23. Shared Components

The page reuses existing UI components to maintain consistency throughout the Event module.

Components reused:

Event Overview Card

Basic Information Card

Category Card

Event Date Card

Activities Card

Media Card

Location Card

Privacy Card

AI Suggestion Card

Confirmation Dialog

Google Maps Selector

Sticky Action Bar

The page shares its layout with:

12-13 Create Event

12-14 View Event

24. AI Usage

Artificial Intelligence assists users by providing recommendations only.

AI may generate suggestions for:

Event Title

Event Description

Event Category

Missing Activities

Missing Media

Missing Location

Duplicate Event Detection

AI suggestions are generated using the available Event information.

Users may:

Apply a suggestion

Ignore a suggestion

Request new suggestions

AI never:

Creates content automatically

Deletes content

Saves changes

Overrides user input

25. Responsive Behaviour

The page follows the standard LifeChronicle responsive design.

Desktop

Two-column layout where appropriate.

Sticky Action Bar remains visible.

Google Maps preview displayed beside Location details.

Tablet

Single-column content.

Cards stack vertically.

Action Bar remains fixed at the bottom.

Mobile

Single-column layout.

All sections collapse by default.

Full-width buttons.

Optimized spacing for touch interaction.

No separate layouts are required.

26. Accessibility

The page follows LifeChronicle accessibility standards.

Requirements:

Keyboard navigation supported.

Logical tab order.

Screen reader friendly labels.

Sufficient color contrast.

Visible focus indicators.

Accessible form validation messages.

27. Audit Trail

All modifications are recorded for future reference.

Examples include:

Event updated

Category changed

Activity added

Activity deleted

Media uploaded

Media removed

Location updated

Privacy changed

Each audit record stores:

User

Action

Date & Time

Previous Value

Updated Value

Audit information is system managed and cannot be modified by users.

28. Performance Considerations

To maintain a responsive user experience:

Activities are loaded only when expanded.

Media thumbnails are lazy loaded.

Google Maps loads only when the Location section is opened.

AI suggestions are generated only on user request.

Large media collections support pagination or incremental loading.

29. Security Considerations

Authentication is required.

Authorization is verified before every update.

Ownership rules are enforced.

CSRF protection applies to all form submissions.

Input validation is performed on both client and server.

Unauthorized modification attempts are rejected and logged.

30. Testing Checklist

Functional Testing

User permissions

Ownership validation

Event updates

Save changes

Cancel changes

Delete confirmation

Preview functionality

Activity Testing

Add Activity

Edit own Activity

Delete own Activity

Prevent editing another user's Activity

Media Testing

Upload Media

Replace Media

Delete own Media

Change Cover Image

Prevent editing another user's Media

Location Testing

Search Location

Google Maps selection

Change Location

Coordinate update

Privacy Testing

Privacy changes

Visibility updates

Restricted access validation

AI Testing

AI summary generation

AI suggestions

Apply suggestion

Ignore suggestion

Responsive Testing

Mobile

Tablet

Laptop

Desktop

Accessibility Testing

Keyboard navigation

Screen reader compatibility

Focus order

Color contrast

31. Summary

The Manage Event page provides a consistent and intuitive interface for updating an existing Timeline Event while preserving the familiar structure of the View Event page.

The page emphasizes clarity, ownership, and simplicity by allowing users to manage Event details, Activities, Media, Location, Privacy, and AI recommendations without introducing unnecessary complexity. Collaboration is handled through a dedicated page, ensuring that contribution ownership remains protected and that each collaborator maintains control over their own content.

By reusing common layouts and components across the Event module, the Manage Event page delivers a clean, professional, and maintainable user experience that aligns with LifeChronicle's overall design philosophy of minimal, elegant, and specification-driven software.

next page 

12-16 Timeline Search & Filter