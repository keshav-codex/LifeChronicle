12-27 User Menu

Page Information

Item	Value

Module	12 – UI/UX

Page Name	User Menu

Page ID	UI-027

Layout	LYT-14 User Menu Layout

Primary User	Registered User

Status	Version 1.0

Design Philosophy

The User Menu serves as the Personal Control Center for every registered user.

Unlike traditional dropdown menus, it provides quick access to account management, invitations, notifications, privacy settings, Life Insights, and support without distracting users from the Timeline.

The User Menu should remain compact, intuitive, and consistent across desktop, tablet, and mobile devices.

1. Introduction

The User Menu provides centralized access to user-specific features and settings.

It is available from every authenticated page through the 👤 User Menu icon located in the Global Navigation Bar.

2. Purpose

The User Menu enables users to:

Access Login Profile.

Manage Collaboration Invitations.

Manage Relationship Invitations.

Configure Privacy.

View Notifications.

Access Life Insights.

Review AI Suggestions.

Access Help Center.

Send Praise & Feedback.

Logout.

3. User Access

User	Access

Registered User	✅

Guest	❌

Staff	Separate Staff Menu

Super Administrator	Separate Administration Portal

4. Page Layout

Uses

LYT-14 User Menu Layout

The menu appears as:

Floating popover (Desktop)

Slide-in panel (Tablet)

Bottom sheet or full-screen panel (Mobile)

5. Front View

👤 User Menu

────────────────────────────

🔐 Login Profile

🤝 Collaboration Invitations

👥 Relationship Invitations

🔒 Privacy Settings

🔔 Notifications

📊 Life Insights

✨ AI Suggestions

❓ Help Center

👏 Praise & Feedback

🚪 Logout

Unread notifications and pending invitations display numeric badges.

Example

🔔 Notifications (5)

🤝 Collaboration Invitations (2)

👥 Relationship Invitations (1)

6. Menu Items

6.1 Login Profile

Purpose

Manage account credentials and security.

Destination

12-19 Login Profile & Security Center

6.2 Collaboration Invitations

Purpose

View and respond to collaboration invitations.

Destination

12-21 Collaboration Invitations

6.3 Relationship Invitations

Purpose

Accept or reject relationship requests.

Destination

12-22 Relationship Invitations

6.4 Privacy Settings

Purpose

Manage personal privacy preferences.

Destination

12-20 Privacy Settings

6.5 Notifications

Purpose

View all application notifications.

Destination

12-17 Notifications

Unread notifications display a badge.

6.6 📊 Life Insights

Purpose

Generate personal reports and explore life statistics.

Destination

12-28 Personal Reports (Life Insights)

Examples

Timeline Insights

Travel Insights

Relationship Insights

Media Insights

Collaboration Insights

Education Insights

Custom Reports

6.7 AI Suggestions

Purpose

Review AI-generated recommendations.

Destination

12-31 AI Center

Badge displayed when new suggestions are available.

6.8 Help Center

Purpose

Access documentation, FAQs, and support.

Destination

12-29 Help Center

6.9 Praise & Feedback

Purpose

Submit compliments, suggestions, or general feedback.

Destination

12-30 Praise & Feedback

6.10 Logout

Purpose

Safely end the current session.

Destination

12-33 Logout Confirmation

7. Navigation Flow

Any Authenticated Page

↓

👤 User Menu

↓

Select Menu Item

↓

Destination Page

↓

Return to Previous Page

8. Business Rules

User Menu is available on every authenticated page.

Only authenticated users can access the menu.

Badge counts update automatically.

Menu items respect user permissions.

Selecting a menu item closes the menu before navigation.

The menu remains lightweight and loads instantly.

9. Global Validation Rules

System Managed

Badge Counts

Menu Visibility

User Permissions

Navigation State

No user input is required.

10. Master Data Dependencies

Code	Purpose

MENU_*	Menu Labels

BTN_*	Buttons

TXT_*	Labels

MSG_*	Messages

BADGE_*	Badge Labels

11. Shared Components Used

LC-MNU-001 Menu Item

LC-BDG-001 Notification Badge

LC-ICN-001 Icon Component

LC-PNL-001 Slide Panel

LC-BTN-002 Secondary Button

12. AI Usage

The User Menu does not perform AI operations.

It provides navigation to the AI Suggestions Center when applicable.

13. Responsive Behaviour

Mobile

Full-screen panel or bottom sheet.

Large touch targets.

Scrollable menu.

Tablet

Slide-in side panel.

Laptop/Desktop

Floating popover aligned to the User Menu icon.

14. Testing Checklist

Menu visibility.

Navigation.

Badge updates.

Permission checks.

Responsive behaviour.

Accessibility.

Keyboard navigation.

Touch interaction.

15. Summary

The User Menu serves as the centralized entry point for all user-specific functions within LifeChronicle. By grouping security, invitations, privacy, notifications, Life Insights, AI assistance, and support into a single, consistent interface, it provides fast access to essential features while keeping the primary Timeline experience clean and focused.