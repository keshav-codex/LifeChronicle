11-10 Concern Data Dictionary

1. Introduction

This document defines the data structure for the Concern domain of LifeChronicle Version 1.0.

The Concern domain manages user support requests, conversations, staff assignments, escalations, and AI-assisted support while integrating with shared services.

2. Concern

Purpose

Represents a support request submitted by a user.

Primary Key

Concern ID

Main Information

Concern Title

Concern Description

Concern Category

Concern Priority

Concern Status

Current Assigned Staff

Resolution Summary

Created On

Updated On

Closed On (Optional)

Relationships

BirthProfile (N:1)

ConcernConversation (1)

ConcernAssignment (1)

ConcernEscalation (1)

Media (1)

AI Suggestion (1)

Concern Category (Master Data) (N:1)

Concern Priority (Master Data) (N:1)

Concern Status (Master Data) (N:1)

3. ConcernConversation

Purpose

Stores all communication related to a Concern.

Primary Key

Conversation ID

Main Information

Message Type

Conversation Message

Internal Staff Note

AI Draft Indicator

Created On

Relationships

Concern (N:1)

BirthProfile (Optional)

Staff (Optional)

Media (1)

4. ConcernAssignment

Purpose

Maintains the assignment history of a Concern.

Primary Key

Assignment ID

Main Information

Assigned Staff

Assigned By

Assignment Date

Assignment Reason

Assignment Status

Relationships

Concern (N:1)

Staff (N:1)

5. ConcernEscalation

Purpose

Maintains the escalation history of a Concern.

Primary Key

Escalation ID

Main Information

Escalation Level

Escalated By

Escalation Reason

Escalation Date

Relationships

Concern (N:1)

Staff (N:1)

Escalation Level (Master Data) (N:1)

6.UserFeedback

Purpose

Maintain all User Praise/Feedback 

Feedback ID

Birth Profile

Feedback Title (Optional)

Feedback Message

AI Classification

Display on Landing Page

Approval Status

Approved By

Approved On

Created On 

7. Business Rules

The system shall ensure:

Every Concern belongs to one Birth Profile.

Every Conversation belongs to one Concern.

Every Assignment belongs to one Concern.

Every Escalation belongs to one Concern.

Only one staff member may be actively assigned at a time.

Assignment and Escalation history are permanently preserved.

Internal Staff Notes are never visible to users.

AI-generated responses are suggestions only and require staff review before sending.

Categories, Priorities, Statuses, Message Types, Assignment Statuses, and 
Escalation Levels are maintained through Master Data.

7. Summary

The Concern Data Dictionary provides a normalized support management structure that preserves complete communication, assignment history, escalation history, and AI-assisted workflows while integrating with the shared services of the LifeChronicle platform.

8. Next Document

11-11 Administration ERD