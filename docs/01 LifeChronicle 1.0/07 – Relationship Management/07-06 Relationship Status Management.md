07-06 Relationship Status Management
1. Introduction

This document defines the lifecycle and management of relationships within LifeChronicle Version 1.0.

Relationship status determines whether users can interact, view permitted information, and participate in relationship-based features.

2. Supported Statuses

Relationships support the following statuses:

Active
Hold
Delete
Block

Invitation statuses are managed separately.

3. Active

An Active relationship allows:

Relative Profile Viewing
Timeline Viewing (subject to privacy)
Collaborative Invitations
Future relationship features
4. Hold

Hold temporarily hides the relationship.

Characteristics:

No new invitation required.
Relationship can be restored instantly.
Relationship history remains intact.
5. Delete

Deleting a relationship:

Removes the relationship.
Removes it from both users' relationship lists.
Preserves audit logs.

Creating the relationship again requires a new invitation.

6. Block

Blocking a relationship:

Automatically deletes the relationship.
Prevents future relationship invitations.
Prevents collaboration invitations.
Remains effective until manually unblocked.

After unblocking, a new relationship invitation is required.

7. Business Rules

The system shall ensure:

Hold is temporary.
Delete permanently removes the relationship connection.
Block overrides all invitation permissions.
Relationship status changes are recorded in audit logs.
Operational behavior follows configuration and business rules.
8. Summary

Relationship Status Management provides users with flexible control over trusted relationships while preserving privacy, security, auditability, and future extensibility.

9. Next Document

07-07 Relationship Privacy