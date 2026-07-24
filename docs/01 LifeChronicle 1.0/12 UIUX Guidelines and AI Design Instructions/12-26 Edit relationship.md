12-26 Edit Relationship

Page Information

Item	Value

Module	12 – UI/UX

Page Name	Edit Relationship

Page ID	UI-026

Layout	LYT-13 Relationship Profile Layout

Primary User	Relationship Owner

Status	Version 1.0

Design Philosophy

The Edit Relationship page allows users to update how they organize and identify a relationship within their own LifeChronicle.

Editing a relationship does not modify the other user's account or profile.

The page reuses the View Relationship layout, replacing read-only information with editable controls where permitted.

1. Introduction

The Edit Relationship page enables users to manage relationship information such as nicknames, relationship types, groups, notes, and communication preferences.

It does not allow editing of another user's personal information.

2. Purpose

The page enables users to:

Update the Nickname.

Change the Relationship Type.

Assign or change Relationship Groups.

Add or edit personal notes.

Configure relationship-specific privacy.

Remove or block the relationship.

3. User Access

User	Access

Relationship Owner	Full Access

Related User	No Edit Access

Guest	❌

Staff	Administrative Access

4. Page Layout

Uses

LYT-13 Relationship Profile Layout

The layout matches View Relationship, with editable sections where appropriate.

5. Front View

← Back

====================================================

❤️ Big Brother

Rahul Kumar

Brother

====================================================

Basic Information ▼

====================================================

Relationship Groups ▼

====================================================

Private Notes ▼

====================================================

Relationship Preferences ▼

====================================================

Relationship History ▼

====================================================

🚫 Block Relationship

🗑 Remove Relationship

💾 Save Changes

6. Page Sections

6.1 Basic Information

Editable fields:

Nickname *

Relationship Type *

Read-only fields:

Full Name

Email Address (if visible)

Invitation Status

6.2 Relationship Groups

Users may:

Add to one or more Groups.

Remove from Groups.

Create a new Custom Group.

Example

☑ Family

☑ Close Friends

☐ Office

☐ Photography Club

6.3 Private Notes

Users may maintain personal notes about the relationship.

Examples

Birthday reminders

Favorite memories

Gift ideas

Family information

These notes are:

Visible only to the relationship owner.

Never shared with the other user.

Not included in AI processing in Version 1.0.

6.4 Relationship Preferences

Users may configure:

Default privacy when sharing with this relationship.

Collaboration preferences.

Notification preferences for this relationship.

These settings affect only the user's experience.

6.5 Relationship History

Read-only.

Displays:

Invitation Sent

Invitation Accepted

Relationship Created

Last Updated

7. Primary Actions

💾 Save Changes

Updates the relationship.

Returns to View Relationship.

🚫 Block Relationship

Displays a confirmation dialog.

Effects:

Prevents future invitations.

Prevents future collaboration requests.

Does not delete historical Events or Collaborations.

🗑 Remove Relationship

Displays a confirmation dialog.

Effects:

Removes the relationship connection.

Shared Events remain available according to their privacy settings.

Historical audit records are preserved.

8. Navigation Flow

Relationships

↓

View Relationship

↓

Edit Relationship

↓

Save Changes

↓

View Relationship

9. Business Rules

Nickname belongs to the relationship owner and can be changed at any time.

Changing the Nickname does not affect the other user's account.

Relationship Groups are reusable across the application.

Private Notes are never visible to the other user.

Blocking affects future interactions only.

Removing a relationship does not delete Events, Activities, or Media.

10. Global Validation Rules

Mandatory

Nickname

Relationship Type

Optional

Relationship Groups

Private Notes

Relationship Preferences

System Managed

Invitation Status

Created On

Updated On

11. Master Data Dependencies

Code	Purpose

RELATIONSHIP_TYPE_*	Relationship Types

RELATIONSHIP_GROUP_*	Relationship Groups

BTN_*	Button Labels

TXT_*	Labels

MSG_*	Messages

VALIDATION_*	Validation Messages

12. Shared Components Used

LC-REL-001 Relationship Profile Card

LC-REL-002 Group Selector

LC-TXT-001 Text Area

LC-BTN-001 Primary Button

LC-DLG-001 Confirmation Dialog

13. AI Usage

None.

Relationship editing is entirely user-controlled in Version 1.0.

14. Responsive Behaviour

Mobile

Single-column layout.

Expandable cards.

Large touch targets.

Tablet

Comfortable spacing.

Two-column layout where appropriate.

Laptop/Desktop

Multi-column profile layout.

Side-by-side editable sections where appropriate.

15. Testing Checklist

Nickname update.

Relationship type change.

Group assignment.

Private Notes.

Preferences.

Block workflow.

Remove workflow.

Responsive behaviour.

Accessibility.

16. Summary

The Edit Relationship page allows users to personalize and organize their relationships within LifeChronicle without affecting another user's account. By separating shared relationship data from user-specific information such as nicknames, groups, and private notes, it provides a flexible and privacy-conscious way to manage personal connections.