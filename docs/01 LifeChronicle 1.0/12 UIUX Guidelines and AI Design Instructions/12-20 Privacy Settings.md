12-20 Privacy Settings

Page Information

Item	Value

Module	12 – UI/UX

Page Name	Privacy Settings

Page ID	UI-020

Layout	LYT-10 Settings Layout

Primary User	Registered User

Status	Version 1.0

Design Notes

Privacy-first.

Mobile-first.

Minimal interface.

Plain language instead of technical terminology.

Immediate feedback when privacy changes.

Progressive disclosure.

One setting per purpose.

1. Introduction

The Privacy Settings page allows users to control who can access their personal information and LifeChronicle content.

Rather than configuring privacy individually for every feature, this page provides global privacy defaults while still allowing Event-level overrides where permitted.

Privacy settings are designed to be simple, transparent, and reusable across the application.

2. Purpose

The Privacy Settings page enables users to:

Configure default Event privacy.

Manage default Relationship visibility.

Configure profile visibility.

Manage collaboration permissions.

Control search visibility.

Configure communication preferences.

3. User Access

User	Access

Registered User	✅

Guest	❌

Staff	❌

Administrator	Administrative Access Only

4. Page Layout

Uses

LYT-10 Settings Layout

The page consists of expandable setting cards.

5. Front View

← Back

────────────────────────────

🔒 Privacy Settings

────────────────────────────

🌍 Default Event Privacy ▼

────────────────────────────

👤 Profile Visibility ▼

────────────────────────────

👥 Relationship Privacy ▼

────────────────────────────

🤝 Collaboration Privacy ▼

────────────────────────────

🔍 Search Visibility ▼

────────────────────────────

🔔 Communication Preferences ▼

6. Page Sections

6.1 Default Event Privacy

Sets the default privacy for newly created Events.

Available options

🌍 Public

👥 Restricted To

👤 Only Visible To

🔒 Private

Users can override this while creating or editing an individual Event.

6.2 Profile Visibility

Determines who may view the Birth Profile.

Options

Everyone

Relationships Only

Selected Relationship Groups

Only Selected Users

Only Me

6.3 Relationship Privacy

Controls visibility of:

Relationship List

Relationship Types

Shared Relationship Information

Options

Everyone

Relationships Only

Only Me

6.4 Collaboration Privacy

Controls

Who can invite the user to Collaborations.

Who may see collaborative Events.

Options

Everyone

Relationships Only

Nobody

6.5 Search Visibility

Determines whether other authorized users can discover the user through shared content.

Options

Visible

Limited

Hidden

Business Rule

This setting does not expose the user directory.

Users still cannot search LifeChronicle members directly.

6.6 Communication Preferences

Controls notifications for

Collaboration Invitations

Relationship Invitations

AI Suggestions

Administrative Messages

System Notifications

Users may enable or disable each category independently.

7. Navigation Flow

Timeline

↓

👤 User Menu

↓

Privacy Settings

↓

Save Changes

↓

Timeline

8. Business Rules

Global privacy applies by default.

Individual Events may override the default Event Privacy.

Privacy changes apply immediately after saving.

Relationship Groups are reused from the Relationship module.

Search Visibility does not create a public user directory.

Collaboration permissions respect Relationship Privacy.

9. Global Validation Rules

Mandatory

Default Event Privacy

Optional

Communication preferences.

Search visibility.

System Managed

Privacy inheritance.

Effective visibility calculation.

10. Master Data Dependencies

Code	Purpose

PRIVACY_*	Privacy Levels

COMMUNICATION_*	Notification Categories

BTN_*	Buttons

TXT_*	Labels

MSG_*	Messages

11. Shared Components Used

LC-PRV-001 Privacy Selector

LC-REL-002 Relationship Group Selector

LC-CARD-001 Expandable Settings Card

LC-BTN-001 Primary Button

LC-DLG-001 Confirmation Dialog

12. AI Usage

None.

AI shall not modify privacy settings or recommend privacy changes in Version 1.0.

13. Responsive Behaviour

Mobile

Single-column expandable cards.

Large toggle controls.

Tablet

Centered settings layout.

Laptop/Desktop

Multi-card layout with comfortable spacing.

14. Testing Checklist

Default Event Privacy.

Profile visibility.

Relationship visibility.

Collaboration permissions.

Search visibility.

Communication preferences.

Privacy inheritance.

Responsive behaviour.

Accessibility.

15. Summary

The Privacy Settings page provides a single, centralized location for configuring how personal information and LifeChronicle content are shared. By separating global defaults from Event-level overrides and reusing Relationship Groups throughout the application, it ensures privacy remains consistent, understandable, and easy to manage.

⭐ One architectural improvement (I strongly recommend)

I think we should add a final section called Privacy Preview.

Instead of making users guess what their settings mean, show an immediate summary.

Example:

👁 Privacy Preview

Birth Profile

→ Relationships Only

New Events

→ Restricted To: Family

Relationships

→ Only Me

Collaboration

→ Relationships Only

Search Visibility

→ Limited