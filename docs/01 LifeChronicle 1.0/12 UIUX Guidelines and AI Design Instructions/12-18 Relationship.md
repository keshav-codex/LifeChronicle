12-18 Relationships

Page Information

Item	Value

Module	12 – UI/UX

Page Name	Relationship Management

Page ID	UI-018

Layout	LYT-08 Relationship Layout

Primary User	Registered User

Status	Version 1.0

Design Notes

Mobile-first.

Relationship cards.

Progressive disclosure.

Search-first experience.

Relationship Groups are first-class objects.

Simple enough for non-technical users.

1. Introduction

The Relationship Management page allows users to create and manage personal relationships within LifeChronicle.

Relationships enable collaboration, privacy control, invitations, shared memories, and future family tree functionality.

Relationships are independent of Timeline Events but can be associated with Events and Activities.

2. Purpose

The Relationship module enables users to:

View Relationships.

Add Relationships.

Search Relationships.

Group Relationships.

Accept Invitations.

Manage Privacy Groups.

View shared Events.

3. User Access

User	Access

Registered User	✅

Guest	❌

Staff	❌

4. Page Layout

Uses

LYT-08 Relationship Layout

The page consists of:

Search Bar

Relationship Summary

Relationship Groups

Relationship Cards

5. Front View

← Back

────────────────────────

👥 Relationships

Search...

────────────────────────

Family (8)

Friends (22)

Education (34)

Office (16)

Neighbours (5)

Others (3)

────────────────────────

👤 Rahul Kumar

Brother

Accepted

────────────────────────

👤 Amit Sharma

College Friend

Invitation Pending

────────────────────────

➕ Add Relationship

6. Page Sections

6.1 Search

Search by

Name

Nickname

Relationship Type

Group

Email

Phone Number

Search begins while typing.

6.2 Relationship Groups

Default Groups - 

Family

Friends

Education

Office

Neighbours

Others

Users may create additional custom groups.

Example

Groups

Family (8)

Friends (22)

Office (16)

Cricket Team (12)

Photography Club (9)

6.3 Relationship Card

Each Relationship Card displays:

Profile Photo (if available)

Nickname (Always displayed as the primary name)

Full Name (Secondary information, displayed when available)

Relationship Type

Invitation Status

Shared Event Count

Example (User has joined)

👤

❤️ Chintu Mama

Rahul Kumar

Relationship: Maternal Uncle

Shared Events (28)

Accepted

Example (Invitation Pending)

👤

❤️ Chintu Mama

Invitation Pending

Relationship: Maternal Uncle

The Nickname always remains the primary identity because it represents how the user personally knows that individual.

6.4 Add Relationship

Selecting

➕ Add Relationship

opens the Add Relationship page.

Fields

Email Address *

Nickname *

Relationship Type *

Relationship Group (Optional)

Personal Notes (Optional)

6.5 Invitations

Invitation Status

Pending

Accepted

Rejected

Expired

Cancelled

Pending invitations display:

Invitation Pending

Cancel Invitation

6.6 Shared Events

Each relationship displays

Shared Events (12)

Selecting opens filtered Timeline results showing only shared events with that relationship.

6.7 Privacy Groups

Relationship Groups are reused by Event Privacy.

Example

👥 Restricted To

☑ Family

☑ Office

☐ Cricket Team

No duplicate group management is required.

7. Navigation Flow

Timeline

↓

👥 Relationships

↓

Relationship List

↓

View Relationship

↓

Edit Relationship

↓

Timeline

8. Business Rules

Relationship invitations require acceptance.

One invitation exists per relationship request.

Custom Relationship Groups may be created.

Relationship Groups are reusable across privacy settings.

Shared Events respect Event Privacy.

Removing a relationship does not delete Events.

9. Global Validation Rules

Mandatory

Name (or selected LifeChronicle user)

Relationship Type

Optional

Group

Notes

Nickname

System Filled

Relationship ID

Invitation Status

Created On

Updated On

10. Master Data Dependencies

Code	Purpose

RELATIONSHIP_TYPE_*	Relationship Types

RELATIONSHIP_GROUP_*	Default Groups

INVITATION_STATUS_*	Invitation Status

BTN_*	Buttons

TXT_*	Labels

MSG_*	Messages

11. Shared Components Used

LC-SRH-001 Search Bar

LC-REL-001 Relationship Card

LC-REL-002 Group Card

LC-REL-003 Invitation Status Badge

LC-BTN-001 Primary Button

12. AI Usage

Version 1.0

AI does not create or modify relationships.

Future versions may suggest:

Possible duplicate relationships.

Frequently collaborating users.

Recommended privacy groups.

All suggestions remain optional.

13. Responsive Behaviour

Mobile

Single-column cards.

Full-screen search.

Expandable group lists.

Tablet

Two-column cards.

Laptop/Desktop

Multi-column responsive grid.

Persistent search panel.

14. Testing Checklist

Relationship creation.

Invitation workflow.

Search.

Group management.

Shared Events.

Privacy group reuse.

Responsive behaviour.

Accessibility.

15. Summary

The Relationship Management page provides a centralized interface for managing personal connections within LifeChronicle. By combining relationship groups, invitations, shared events, and reusable privacy groups, it supports collaboration and controlled content sharing while maintaining a simple and scalable user experience.