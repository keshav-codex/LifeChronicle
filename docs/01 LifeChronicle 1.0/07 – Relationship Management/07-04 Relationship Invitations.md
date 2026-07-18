07-04 Relationship Invitations
1. Introduction

This document defines the management of relationship invitations within LifeChronicle Version 1.0.

Relationship invitations allow users to establish trusted connections through a controlled invitation and acceptance process.

2. Invitation Sections

Relationship invitations are organized into:

Sent Invitations

Displays invitations sent by the user.

Received Invitations

Displays invitations received from other users.

3. Sent Invitations

Users may:

View Pending Invitations
View Accepted Invitations
View Rejected Invitations
Cancel Pending Invitations
Delete Invitation Records

Only pending invitations remain active.

4. Received Invitations

Users may:

View Invitation Details
Accept Invitation
Reject Invitation

Upon acceptance:

Relationship becomes Active.
Opposite relationship type is assigned automatically.
Both users receive confirmation notifications.
5. Invitation Status

Supported statuses include:

Pending
Accepted
Rejected
Cancelled
Expired

Invitation expiry and rejection cooldown are controlled through Master Data.

6. Notification Messages

Invitation emails and notifications shall use configurable templates from Master Data.

Messages may include:

Sender Name
Recipient Nickname
Relationship Type
Application Name
7. Business Rules

The system shall ensure:

Pending invitations may be cancelled.
Expired invitations cannot be accepted.
Rejected invitations follow the configured cooldown period.
Accepted invitations cannot be accepted again.
Users may delete invitation history without affecting audit logs.
8. Summary

The Relationship Invitation module manages the complete invitation lifecycle while ensuring secure relationship creation, configurable business rules, and consistent communication through notification and email templates.

9. Next Document

07-05 Relative Profile View