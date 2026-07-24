12-24 Edit Collaboration

Page Information

Item	Value

Module	12 – UI/UX

Page Name	Edit Collaboration

Page ID	UI-024

Layout	LYT-12 Collaboration Detail Layout

Primary User	Collaboration Owner

Status	Version 1.0

Design Notes

Reuses the View Collaboration layout.

Read-only information remains read-only.

Only collaboration-related information is editable.

Event details are never editable from this page.

Progressive disclosure.

Mobile-first.

1. Introduction

The Edit Collaboration page enables authorized users to manage an existing collaboration associated with a Timeline Event.

This page focuses exclusively on collaboration management, such as participants, invitations, and collaboration settings. Event content remains managed through the Edit Event page.

2. Purpose

Users can:

Invite additional participants.

Remove participants.

Resend pending invitations.

Cancel pending invitations.

Update collaboration information.

Close the collaboration.

3. User Access

User	Access

Collaboration Owner	Full Access

Accepted Participant	Read Only

Pending Participant	No Edit Access

Guest	❌

Staff	Administrative Access

4. Page Layout

Uses

LYT-12 Collaboration Detail Layout

The page reuses the layout from View Collaboration with editable collaboration controls.

5. Front View

← Back

────────────────────────

Edit Collaboration

────────────────────────

Linked Event ▼

(Read Only)

────────────────────────

Participants (5) ▼

────────────────────────

Pending Invitations (2) ▼

────────────────────────

Collaboration Settings ▼

────────────────────────

🗑 Close Collaboration

💾 Save Changes

6. Page Sections

6.1 Linked Event

Displays

Event Title

Event Date

Event Category

Read-only.

Selecting the Event opens View Event.

6.2 Participants

Collapsed by default.

Displays

Profile Photo

Nickname (Primary)

Full Name (Secondary)

Relationship Type

Collaboration Role

Status

Available actions

➕ Invite Participant

➖ Remove Participant

👁 View Relationship

Removing a participant requires confirmation.

6.3 Pending Invitations

Displays all invitations awaiting response.

Each invitation displays

Nickname

Email Address

Invitation Sent

Remaining Time

Status

Available actions

🔄 Resend Invitation

❌ Cancel Invitation

6.4 Collaboration Settings

Displays

Collaboration Status

Total Participants

Accepted Participants

Pending Invitations

Created On

Last Updated

Only editable settings are displayed.

7. Primary Actions

💾 Save Changes

Updates collaboration information.

Returns to View Collaboration.

🗑 Close Collaboration

Displays a confirmation dialog.

Closing the collaboration:

Removes the collaboration record.

Removes participant associations.

Preserves the original Event.

Preserves audit history.

8. Navigation Flow

Timeline

↓

View Event

↓

View Collaboration

↓

Edit Collaboration

↓

Save Changes

↓

View Collaboration

9. Business Rules

Collaboration belongs to exactly one Event.

Editing collaboration never edits Event information.

Only the Collaboration Owner may manage participants.

Pending invitations may be cancelled.

Accepted participants may be removed.

Closed collaborations retain audit records.

Closing a collaboration does not delete the linked Event.

10. Global Validation Rules

Mandatory

At least one Collaboration Owner must exist.

System Managed

Invitation Status.

Participant Count.

Created On.

Updated On.

11. Master Data Dependencies

Code	Purpose

COLLABORATION_STATUS_*	Collaboration Status

INVITATION_STATUS_*	Invitation Status

BTN_*	Buttons

TXT_*	Labels

MSG_*	Messages

VALIDATION_*	Validation Messages

12. Shared Components Used

LC-COL-001 Collaboration Summary Card

LC-REL-001 Participant Card

LC-INV-001 Invitation Card

LC-BTN-001 Primary Button

LC-DLG-001 Confirmation Dialog

13. AI Usage

None.

All collaboration changes are performed manually by authorized users.

14. Responsive Behaviour

Mobile

Single-column expandable sections.

Bottom-sheet confirmation dialogs.

Tablet

Responsive participant cards.

Expandable invitation list.

Laptop/Desktop

Multi-column layout.

Side-by-side participant and invitation panels where space allows.

15. Testing Checklist

Add participant.

Remove participant.

Resend invitation.

Cancel invitation.

Save changes.

Close collaboration.

Permission validation.

Responsive behaviour.

Accessibility.

16. Summary

The Edit Collaboration page provides authorized users with a dedicated workspace for managing collaboration participants and invitations without affecting the associated Timeline Event. By separating collaboration management from event editing, LifeChronicle maintains clear ownership boundaries, consistent business rules, and a simple user experience.