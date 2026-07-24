12-16 Timeline Search & Filter

Page Information

Item	Value

Module	12 – UI/UX

Page Name	Timeline Search & Filter

Page ID	UI-016

Layout	LYT-06 Search Overlay / Filter Panel

Primary User	Registered User

Status	Version 1.0

Design Notes

Search without leaving the Timeline.

Search results never replace the Timeline.

Filters are collapsible.

Mobile-first.

AI-assisted search.

Fast, lightweight, and responsive.

Birth Node always remains visible.

1. Introduction

The Timeline Search & Filter feature enables users to quickly locate memories, events, activities, media, people, and locations within their Timeline.

Rather than navigating to a separate page, searching is performed as an overlay or side panel while keeping the Timeline visible in the background.

2. Purpose

The feature enables users to:

Search Events.

Search Activities.

Search People.

Search Locations.

Search Categories.

Filter Timeline results.

Highlight matching Timeline Nodes.

3. User Access

User	Access

Registered User	✅

Guest	❌

Staff	❌

4. Page Layout

Uses:

LYT-06 Search Overlay

Desktop

Right Side Panel

Mobile

Full Screen Search

5. Front View

🔍 Search Timeline

────────────────────────

Search...

────────────────────────

Filters ▼

────────────────────────

Results (12)

🏛 Graduation

✈ Delhi Trip

🎂 Birthday

🏆 Award Ceremony

────────────────────────

❌ Close

Timeline remains visible behind the search panel.

6. Page Sections

6.1 Search Bar

Users may search by:

Event Title

Description

Activity

Person

Category

Location

Tags

Year

Month

Search begins as the user types.

6.2 Filters

Collapsed by default.

Available filters

Date

Year

Month

Date Range

Category

Parent Category

Child Category

Privacy

Public

Restricted To

Only Visible To

Private

Collaboration

Collaborative Events

Personal Events

Event Status

Draft

Active

Completed

Archived

Media

Images

Videos

Audio

Documents

AI

AI Suggestions Available

AI Alerts

6.3 Search Results

Example

Results (8)

🏛 Graduation

📍 Delhi Trip

🎂 Birthday

🏆 Award

────────────

Load More

Selecting a result

↓

Timeline scrolls

↓

Matching Event highlighted

↓

Preview opens

6.4 AI Search

Users may optionally use

✨ Ask AI

Example

Find my college memories.

Find trips to Delhi.

Show events with Rahul.

Find birthdays before 2010.

Show all temple visits.

AI converts natural language into Timeline filters.

Users may review generated filters before applying them.

7. Navigation Flow

Timeline

↓

🔍 Search

↓

Results

↓

Timeline Scrolls

↓

Highlighted Event

↓

View Event

8. Business Rules

Timeline remains visible during search.

Birth Node always remains visible.

Filters do not permanently change Timeline order.

Search highlights matching nodes.

Multiple filters may be combined.

Clearing filters restores the full Timeline.

9. Global Validation Rules

No mandatory fields.

Search accepts partial matches.

Empty searches return the complete Timeline.

10. Master Data Dependencies

Code	Purpose

CATEGORY_*	Categories

STATUS_*	Event Status

PRIVACY_*	Privacy

BTN_*	Buttons

TXT_*	Labels

AI_LABEL_*	AI Search

FILTER_*	Filter Labels

11. Shared Components Used

LC-SRH-001 Search Bar

LC-FLT-001 Filter Panel

LC-TML-002 Event Node

LC-AI-001 AI Search

LC-BTN-002 Secondary Button

12. AI Usage

AI Search may understand natural language.

Examples

Show my childhood memories.

Find school events.

Show all events with Rahul.

Find temple visits in Bihar.

Show trips during 2024.

AI translates the request into structured Timeline filters.

AI never changes data.

13. Responsive Behaviour

Mobile

Full-screen search.

Bottom-sheet filters.

Swipe to close.

Tablet

Right-side filter panel.

Laptop/Desktop

Floating search panel.

Timeline remains visible.

14. Testing Checklist

Search accuracy.

Multiple filters.

AI Search.

Highlight node.

Timeline scroll.

Empty results.

Performance.

Responsive layout.

Accessibility.

15. Summary

The Timeline Search & Filter feature enables users to quickly rediscover memories without interrupting the Timeline experience. By combining real-time search, structured filters, and optional AI-assisted natural language search, users can efficiently locate events even as their LifeChronicle grows over many years.