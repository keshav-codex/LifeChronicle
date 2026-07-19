11-08 Relationship Data Dictionary

1. Introduction

This document defines the data structure for the Relationship domain of LifeChronicle Version 1.0.

The Relationship domain manages invitations, accepted relationships, relationship-specific information, and integration with privacy, collaboration, and notifications.

2. RelationshipInvitation

Purpose

Represents an invitation sent to establish a relationship between two users.

Primary Key

Relationship Invitation ID

Main Information

Invitation Sender

Invitation Receiver

Receiver Email

Sender Nickname

Relationship Category

Invitation Status

Invitation Expiry Date

Created On

Updated On

Relationships

BirthProfile (Sender) (N:1)

BirthProfile (Receiver) (Optional)

Relationship Category (Master Data) (N:1)

Invitation Status (Master Data) (N:1)

3. Relationship

Purpose

Represents an accepted relationship between two Birth Profiles.

Primary Key

Relationship ID

Main Information

Person A

Person B

My Relationship Category

Opposite Relationship Category

My Relationship Nickname

Relationship Status

Timeline Visibility

Accepted On

Updated On

Relationships

BirthProfile (Person A) (N:1)

BirthProfile (Person B) (N:1)

Relationship Category (Master Data) (N:1)

Relationship Status (Master Data) (N:1)

4. Business Rules

The system shall ensure:

Relationships are created only after invitation acceptance.

Every relationship connects exactly two Birth Profiles.

Each user may maintain their own relationship nickname.

Relationship nicknames are visible only to their owner.

Relationship Categories and Opposite Categories are maintained through Master Data.

Relationship Status is maintained through Master Data.

Hold, Delete, and Block follow Relationship Management business rules.

Collaboration eligibility follows Relationship Management rules.

5. Visibility Rules

Relationship visibility depends on the configured Relationship Status.

By default, approved relationships display:

Profile Photo

Full Name

Relationship Category

Relationship Nickname

Additional Timeline information is displayed according to Timeline privacy rules.

6. Summary

The Relationship Data Dictionary provides a normalized structure for managing invitations, accepted relationships, personal nicknames, configurable statuses, and integration with collaboration and privacy while keeping relationship information independent from Birth Profile data.

7. Next Document

11-09 Concern ERD