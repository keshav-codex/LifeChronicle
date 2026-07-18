07-03 Add Relationship
1. Introduction

This document defines the functional requirements for adding new relationships in LifeChronicle Version 1.0.

Relationships are created through an invitation process and become active only after acceptance by the recipient.

2. Purpose

The Add Relationship module shall:

Send relationship invitations.
Establish trusted connections.
Prevent unauthorized relationships.
Support configurable relationship types.
3. Information Required

The sender shall provide:

Relative Email Address
Relationship Type
Nickname (Optional)

Relationship Types are managed through Master Data.

4. Invitation Process

The system shall:

Validate the email address.
Verify the relationship type.
Check invitation eligibility.
Generate notifications and email messages using Master Data templates.

If the recipient is already registered:

Send an in-app notification.
Send an email invitation.

If the recipient is not registered:

Send an application invitation email.
Display the relationship invitation after registration.
5. Opposite Relationship Mapping

Upon acceptance, the system shall automatically assign the appropriate opposite relationship using Master Data.

Examples include:

Husband → Wife
Sister → Brother
Father → Son / Daughter
Friend → Friend

The invitee may choose their own nickname.

6. Business Rules

The system shall ensure:

Users cannot invite themselves.
Duplicate active relationships are not permitted.
Invitation expiry is configuration-driven.
Rejection cooldown is configuration-driven.
Maximum relationship limits are configuration-driven.
No global user search is supported.
7. Summary

The Add Relationship module provides a secure, invitation-based process for creating trusted relationships while ensuring configuration-driven validation, privacy, and independent Timeline ownership.

8. Next Document

07-04 Relationship Invitations