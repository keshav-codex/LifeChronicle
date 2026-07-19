11-09 Concern ERD

1. Introduction

The Concern ERD defines the entities used to manage user concerns, communication, assignment, escalation, and resolution within LifeChronicle.

The module provides a structured help desk system while integrating with AI, Notifications, Media, and Master Data.

2. Entity Overview

The Concern domain consists of the following entities:

Concern

ConcernConversation

ConcernAssignment

ConcernEscalation

The domain integrates with:

Birth Profile

Administration

Media

Artificial Intelligence

Notification

Master Data

3. Entity Relationships

BirthProfile

      │

      ▼

   Concern (1:N)

      │

      ├── ConcernConversation (1:N)

      ├── ConcernAssignment (1:N)

      ├── ConcernEscalation (1:N)

      ├── Media (1:N)

      └── AI Suggestion (1:N)

      └── UserFeedback (1:N)
      
4. Entity Responsibilities

Concern

Represents a support request submitted by a user.

Stores the concern details, current status, assigned staff member, category, priority, and overall lifecycle.

ConcernConversation

Stores all communication related to a concern.

Supports:

User Messages

Staff Replies

Internal Staff Notes

AI-assisted Draft Responses

ConcernAssignment

Maintains the complete assignment history.

Supports:

Initial Assignment

Reassignment

Assignment History

Only one staff member may be actively assigned at any time.

ConcernEscalation

Maintains the complete escalation history.

Supports:

Manual Escalation

Automatic Escalation

Escalation Reason

Escalation History

5. Business Rules

The Concern domain shall ensure:

Every Concern belongs to one Birth Profile.

Every Concern follows a configurable lifecycle.

Only one active staff member may be assigned at a time.

Reassignment history is permanently preserved.

Escalation history is permanently preserved.

Internal Staff Notes are visible only to authorized staff.

AI suggestions remain optional and editable.

Notifications are delivered through the shared Notification service.

Categories, Priorities, Statuses, and Escalation Levels are maintained through Master Data.

6. Summary

The Concern ERD establishes a scalable help desk architecture supporting user communication, staff assignment, escalation management, AI assistance, and complete operational history while remaining fully configurable through Master Data.

7. Next Document

11-10 Concern Data Dictionary