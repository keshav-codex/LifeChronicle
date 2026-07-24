12-22 Relationship Invitations

Relationship Invitation

Connect two LifeChronicle users

User-based

Creates Relationship

Relationship Module

Page Information

Item	Value

Module	12 – UI/UX

Page Name	Relationship Invitations

Page ID	UI-022

Layout	LYT-11 Invitation Layout

Primary User	Registered User

Status	Version 1.0

Design Notes

Mobile-first.

Simple card-based design.

One invitation per card.

Minimal actions.

Friendly language.

Privacy-first.

1. Introduction

The Relationship Invitations page allows users to manage requests from other LifeChronicle users who wish to establish a personal relationship.

Unlike Collaboration Invitations, these invitations create a long-term connection between two users and may later be used for collaboration, privacy groups, and shared memories.

2. Purpose

Users can:

View pending invitations.

Review inviter information.

Accept invitations.

Reject invitations.

View invitation history.

3. User Access

User	Access

Registered User	✅

Guest	❌

Staff	❌

4. Page Layout

Uses

LYT-11 Invitation Layout

Contains

Pending Invitations

Invitation History

5. Front View

← Back

────────────────────────

👥 Relationship Invitations

Pending (2)

────────────────────────

👤 Rahul Kumar

Nickname:

Big Brother

Relationship:

Brother

Sent

Yesterday

────────────────────────

✓ Accept

✖ Reject

────────────────────────

Invitation History ▼

6. Page Sections

6.1 Pending Invitations

Displays

Profile Photo

Full Name

Nickname assigned by inviter

Relationship Type

Date

Invitation Status

6.2 Invitation Details

Selecting a card expands

Displays

Personal Message (Optional)

Relationship Group

Invitation Date

Mutual Collaborations (Future)

6.3 Invitation Actions

Available

✓ Accept

✖ Reject

Accept

Creates

Relationship

Relationship Group Mapping

Privacy Mapping

Updates

Notification Center

Reject

Declines invitation.

No Relationship created.

6.4 Invitation History

Displays

Accepted

Rejected

Cancelled

Expired

History is read-only.

7. Navigation Flow

Notification

↓

Relationship Invitation

↓

View Invitation

↓

Accept / Reject

↓

Relationship Created

↓

Relationships

8. Business Rules

Users cannot send duplicate invitations.

One active invitation per email.

Invitation expires after 30 days (recommended).

Accepted invitations immediately create the Relationship.

Rejected invitations do not create Relationships.

Relationship Groups are automatically linked.

9. Validation Rules

System Managed

Invitation ID

Status

Created On

Updated On

No user input required.

10. Master Data

Code	Purpose

INVITATION_STATUS_*	Status

RELATIONSHIP_TYPE_*	Types

BTN_*	Buttons

TXT_*	Labels

MSG_*	Messages

11. Shared Components

LC-INV-001 Invitation Card

LC-REL-001 Relationship Card

LC-DLG-001 Confirmation Dialog

LC-BTN-001 Primary Button

12. AI Usage

None.

13. Responsive Behaviour

Mobile

Single-column cards.

Tablet

Responsive cards.

Desktop

Grid layout.

14. Testing Checklist

Invitation received.

Accept.

Reject.

Expiry.

Duplicate prevention.

Notification update.

Relationship creation.

Responsive behaviour.

15. Summary

The Relationship Invitations page provides a secure workflow for establishing trusted connections between LifeChronicle users. By separating relationship invitations from collaboration invitations, the application maintains a clear distinction between long-term personal connections and event-specific participation.