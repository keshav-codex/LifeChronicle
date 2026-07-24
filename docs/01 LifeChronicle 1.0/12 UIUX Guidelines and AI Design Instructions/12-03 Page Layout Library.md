12-03 Page Layout Library

1. Introduction

The Page Layout Library defines the standard layouts used throughout the LifeChronicle application.

Rather than designing a new page structure for every screen, pages shall reuse one of the predefined layouts described in this document.

This approach ensures visual consistency, simplifies development, and improves the overall user experience.

2. Objectives

The Page Layout Library shall:

Maintain consistent page structure.

Improve usability across all devices.

Reduce UI duplication.

Support responsive design.

Simplify frontend implementation.

3. Standard Layouts

LifeChronicle Version 1.0 uses the following layouts:

Layout ID	Layout Name	Used For

LYT-01	Public Layout	Loading, Landing

LYT-02	Authentication Layout	Registration, Login, Forgot Password

LYT-03	Timeline Layout	Dashboard (Timeline)

LYT-04	Detail Layout	Birth Profile, Event, Relationship, Location

LYT-05	Staff Layout	Staff Portal

LYT-06	Modal / Popup Layout	Dialogs, Confirmations, Quick Views

4. LYT-01 Public Layout

Purpose

Used for public-facing pages before user authentication.

Structure

──────────────────────────────

Logo

Navigation

Main Content

Footer

──────────────────────────────

Pages

Loading

Landing

5. LYT-02 Authentication Layout

Purpose

Used during user authentication.

Structure

──────────────────────────────

Logo

Authentication Form

Social Login

Footer
──────────────────────────────
Pages

Registration

Login

Forgot Password

Email Verification

6. LYT-03 Timeline Layout

Purpose

The primary layout of the application after login.

Structure

────────────────────────────────────

Logo (Timeline only)

Global Navigation

Birth Node

Timeline

Event Nodes

Load More

────────────────────────────────────

Characteristics

Timeline is the main content.

Birth Node always remains at the top.

Lazy loading.

Responsive zig-zag (desktop/tablet).

Vertical timeline (mobile).

Pages

Timeline Dashboard

7. LYT-04 Detail Layout

Purpose

Used to display and manage a single entity.

Structure

──────────────────────────────

Back

Page Title

Content

Primary Action

──────────────────────────────

Pages

Birth Profile

Login Profile

Event

Activity

Relationship

Media

Location

Privacy

8. LYT-05 Staff Layout

Purpose

Used throughout the Staff Portal.

Structure

──────────────────────────────

Global Navigation

Staff Navigation

Content Area

──────────────────────────────
Characteristics

Same design language as the user application.

Different menu options.

Responsive on all devices.

9. LYT-06 Modal / Popup Layout

Purpose

Used for temporary interactions without leaving the current page.

Examples

Delete Confirmation

AI Suggestions

Image Preview

Collaboration Invitation

Relationship Invitation

Quick Event Preview

Characteristics

Focused content.

Dismissible.

Responsive.

Accessible.

10. Responsive Behaviour

Every layout shall support:

Device	Behaviour

Mobile	Single-column layout

Tablet	Adaptive layout

Laptop	Full layout

Desktop	Full layout with optimized spacing

The user experience shall remain consistent regardless of screen size.

11. Layout Selection Rules

Each page shall use one standard layout.

New layouts shall only be introduced when an existing layout cannot satisfy the functional requirements.

12. Summary

The Page Layout Library establishes six reusable layouts that cover all interfaces within LifeChronicle Version 1.0. By standardizing page structures, the application maintains a clean, consistent, and responsive user experience while simplifying frontend development and future maintenance.