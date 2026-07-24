12-14 View Event

Page Information

Item	Value

Module	12 – UI/UX

Page Name	View Event

Page ID	UI-014

Layout	LYT-04 Detail Layout

Primary User	Registered User

Status	Version 1.0

Design Notes

Mobile-first design.

Storytelling over form display.

Read-only by default.

Large media with clean typography.

Progressive disclosure.

One primary action.

AI assistance remains optional.

Timeline navigation remains available.

1. Introduction

The View Event page presents a Timeline Event in a rich, readable format.

Rather than displaying raw database fields, the page transforms event information into a chronological story with media, activities, locations, collaborators, and related information.

2. Purpose

The View Event page enables users to:

Read Event details.

View Activities.

Browse Media.

View Event Location.

View Collaborators.

Review Privacy settings.

Review AI Suggestions.

Edit the Event.

Return to the Timeline.

3. User Access

User	Access

Event Owner	Full Access

Authorized User	Read Only

Guest	No

Staff	Administrative Access

Displayed content depends on the Event's privacy settings.

4. Page Layout

Uses:

LYT-04 Detail Layout

The page consists of expandable information sections.

5. Front View

← Back

────────────────────────────

🏛 Graduation Ceremony

15 June 2018

Education → Graduation

────────────────────────────

🖼 Hero Image

────────────────────────────

📝 Description

────────────────────────────

📅 Event Information

────────────────────────────

🎯 Activities (4) ▼

────────────────────────────

📷 Media (26) ▼

────────────────────────────

📍 Location ▼

────────────────────────────

👥 Participants (5) ▼

────────────────────────────

🔒 Privacy ▼

────────────────────────────

✨ AI Suggestions (2) ▼

────────────────────────────

✏ Edit Event

6. Page Sections

6.1 Event Summary

Displays

Hero Image

Event Title

Parent Category

Child Category

Event Date

Event Status

This section is always expanded.

6.2 Description

Displays the Event description.

If unavailable

Display

"No description available."

6.3 Event Information

Displays

Start Date

End Date

Created On

Last Updated

Created By (optional based on privacy)

6.4 Activities

Collapsed by default.

Activities (4) ▼

Opening the section displays:

Activity Title

Date

Thumbnail (optional)

Selecting an Activity opens the View Activity page.

6.5 Media

Collapsed by default.

Displays summary.

Example

Media (26)

22 Photos

3 Videos

1 Audio

Selecting Media opens the Media Gallery.

6.6 Location

Collapsed by default.

Displays

📍 Patna, Bihar, India

▼ Show Map

Selecting Show Map displays the embedded map.

6.7 Collaboration

Collapsed by default.

Displays

Participants (5)

Opening displays

Profile Photo

Name

Relationship

Collaboration Status

6.8 Privacy

Collapsed by default.

Displays

🔒 Private

or

👥 Restricted To

Family

College Friends

The owner may view the complete privacy configuration.

Other users only see the effective privacy level.

6.9 AI Suggestions

Collapsed by default.

Displays

✨ AI Suggestions (2)

Possible suggestions:

Better title

Better description

Better category

Missing location

Missing media

Duplicate event warning

Users may ignore or apply individual suggestions.

7. Primary Action

✏ Edit Event

Available only to users with edit permission.

Selecting Edit opens the Edit Event page.

8. Navigation Flow

Timeline

↓

View Event

↓

Edit Event

↓

Save

↓

View Event

↓

Timeline

9. Business Rules

The Event remains read-only until Edit is selected.

Activities inherit Event privacy.

Media inherits Event privacy.

AI suggestions never modify the Event automatically.

Deleted Events cannot be viewed.

Collaboration details are displayed only to authorized users.

10. Master Data Dependencies

Code	Purpose

CATEGORY_*	Categories

STATUS_*	Event Status

BTN_*	Buttons

TXT_*	Labels

MSG_*	Empty Messages

AI_LABEL_*	AI Labels

PRIVACY_*	Privacy Labels

11. Shared Components Used

LC-EVT-001 Hero Event Card

LC-ACT-001 Activity Card

LC-MED-001 Media Gallery

LC-MAP-001 Map Viewer

LC-COL-001 Participant Card

LC-PRV-001 Privacy Summary

LC-AI-001 AI Suggestion Panel

LC-BTN-002 Secondary Button

12. AI Usage

AI may provide:

Better title suggestions.

Description improvements.

Category recommendations.

Duplicate detection.

Missing information suggestions.

AI suggestions remain optional.

13. Responsive Behaviour

Mobile

Single-column layout.

Media displayed as swipeable cards.

Full-screen image viewer.

Bottom sheet for collapsed sections.

Tablet

Larger media gallery.

Two-column display where appropriate.

Laptop/Desktop

Hero image with structured information.

Responsive cards.

Inline map preview.

14. Testing Checklist

Event display.

Privacy enforcement.

Activities.

Media gallery.

Location map.

Collaboration display.

AI suggestions.

Edit navigation.

Responsive behaviour.

Accessibility.

15. Summary

The View Event page transforms structured event data into a rich and engaging memory experience. By combining media, activities, collaboration, location, privacy, and AI assistance within a clean, read-only interface, it allows users to relive and share important moments while preserving the simplicity and storytelling philosophy of LifeChronicle.


next page 

12-15 Manage Event