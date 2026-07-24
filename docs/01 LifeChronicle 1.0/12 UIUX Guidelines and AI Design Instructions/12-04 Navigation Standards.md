1. Introduction

This document defines the navigation structure and navigation behavior used throughout the LifeChronicle application.

The objective is to provide a simple, predictable, and consistent navigation experience across mobile, tablet, laptop, and desktop devices.

2. Objectives

The navigation system shall:

Be simple and intuitive.

Minimize the number of clicks.

Keep frequently used actions easily accessible.

Remain consistent across all pages.

Adapt automatically to different screen sizes.

3. Navigation Philosophy

LifeChronicle follows a Timeline-first navigation approach.

After login, the Timeline becomes the user's primary workspace.

All major features shall be accessible from the Global Navigation Bar or the User Menu.

4. Navigation Structure

Public Pages

Landing

Registration

Login

Forgot Password

Help

Authenticated User

Timeline

Search

Add Event

Relationships

Notifications

User Menu

Staff

Dashboard

Users

Categories

Reports

Master Data

AI

Notifications

User Menu

5. Timeline Header

Only the Timeline page displays the full two-level header.

────────────────────────────────────────────

LifeChronicle Logo

────────────────────────────────────────────

🏠   🔍   ➕   👥   🔔   👤

────────────────────────────────────────────

Navigation Icons

Icon	Purpose

🏠	Return to Birth Node (Timeline Home)

🔍	Timeline Search & Filter

➕	Create New Event

👥	Relationships

🔔	Notifications (Unread Count)

👤	User Menu

6. Global Navigation

Every page except the Timeline shall display only the Global Navigation Bar.

────────────────────────────────────────────

← Back

🔍   ➕   👥   🔔   👤

────────────────────────────────────────────

The application logo is displayed only on the Timeline page.

7. Scroll Behaviour

To maximize content visibility:

Scroll Down

Hide the logo area (Timeline only).

Hide the navigation bar.

Expand the content area.

Scroll Up

Show the hidden header.

Restore the navigation bar.

The transition shall be smooth and non-distracting.

8. User Menu

Selecting the 👤 icon opens a compact menu.

The menu shall contain:

Menu Item	Purpose

Birth Profile	View/Edit Birth Profile

Login Profile	Manage login credentials

Collaboration Invitations	View collaboration requests

Relationship Invitations	View relationship requests

Privacy Settings	Manage profile privacy

Notifications	View all notifications

AI Suggestions	View AI recommendations

AI Alerts	Review AI-detected issues

Administrative Warnings	View system warnings

Praise Us	Submit praise or appreciation

Help	Help & Support

Logout	Sign out

Menu items shall appear as icon-based cards with labels.

Frequently used items shall appear first.

9. Navigation Rules

Every page shall have a clear way to return to the previous page.

Navigation shall not exceed two levels of depth for common tasks.

Frequently used actions shall always be accessible from the Global Navigation Bar or User Menu.

The Timeline shall always be reachable through the Home icon.

10. Responsive Behaviour

Mobile

Single-row icon navigation.

User Menu opens as a bottom sheet or full-screen menu.

Timeline switches to a vertical layout.

Tablet

Same navigation as mobile with increased spacing.

Laptop & Desktop

Full icon navigation.

User Menu opens as a dropdown panel.

Timeline uses the zig-zag layout.

11. Master Data Dependencies

The following items shall be configurable through Master Data:

Application Logo

Navigation Labels (where applicable)

User Menu Labels

Notification Messages

Help Links

Application Name

12. Shared Components Used

LC-NAV-001 Global Navigation Bar

LC-NAV-002 User Menu

LC-BTN-003 Icon Button

LC-NTF-001 Notification Badge

LC-TML-001 Birth Node

13. Summary

The Navigation Standards establish a consistent, icon-driven navigation system for LifeChronicle. By keeping the Timeline as the primary workspace, limiting navigation complexity, and adapting seamlessly across devices, the application delivers a modern and intuitive user experience while maintaining quick access to essential features.