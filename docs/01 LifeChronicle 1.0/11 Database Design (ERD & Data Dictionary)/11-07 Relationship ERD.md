11-07 Relationship ERD

1. Introduction

The Relationship ERD defines how users establish, manage, and maintain  relationships within LifeChronicle.

Relationships are created only after a Relationship Invitation is accepted. 

Each relationship is independent and follows configurable business rules.

2. Entity Overview

The Relationship domain consists of the following entities:

RelationshipInvitation

Relationship

The domain integrates with:

Birth Profile

Master Data

Notification

3. Entity Relationships

BirthProfile

      │

      ├── RelationshipInvitation (1:N)

      │

      └── Relationship (1:N)
 
RelationshipInvitation

↓

Accepted

↓

Relationship

4. Entity Responsibilities

RelationshipInvitation

Represents an invitation sent to establish a relationship between two users.

Relationship

Represents an active relationship between two Birth Profiles.

Stores relationship-specific information such as category, nickname, status, and visibility settings.

5. Business Rules

The Relationship domain shall ensure:

Relationships are created only after an invitation is accepted.

Relationship Categories are maintained through Master Data.

Opposite Relationship Categories are maintained through Master Data.

Relationship Status is maintained through Master Data.

Users may assign personal nicknames to their relatives.

Relationship nicknames are visible only to the owner of the relationship.

Relationship status controls visibility and collaboration eligibility.

Notifications are handled through the shared Notification service.

6. Summary

The Relationship ERD provides a flexible and configurable structure for managing relationships while maintaining independent relationship data, configurable statuses, and integration with collaboration and privacy features.

7. Next Document

11-08 Relationship Data Dictionary