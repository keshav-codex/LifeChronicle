11-06 Timeline & Events Data Dictionary

1. Introduction

This document defines the data structure for the Timeline & Events domain of LifeChronicle Version 1.0.

The Timeline organizes a user's life chronologically, while Events represent significant life moments. Activities, Media, Locations, Collaboration, and AI integrate with Events through shared services.

2. Timeline

Purpose

Represents the user's personal life timeline.

Primary Key

Timeline ID

Main Information

Timeline Status

Timeline Created On

Timeline Updated On

Relationships

BirthProfile (1:1)

Event (1:N)

3. Event

Purpose

Represents a significant life event belonging to a Timeline.

Primary Key

Event ID

Main Information

Event Title

Event Description

Event Start Date

Event End Date

Same Day Indicator

Event Time (Optional)

Event Privacy

Category

Subcategory

Event Status

Created On

Updated On

Relationships

Timeline (N:1)

Activity (1:N)

Media (1:N)

Location (1:1)

Collaboration (0:1)

AI Suggestion (1)

Category (Master Data) (N:1)

Subcategory (Master Data) (N:1)

4. Activity

Purpose

Represents an individual activity performed within an Event.

Primary Key

Activity ID

Main Information

Activity Title

Activity Description

Activity Date

Activity Time (Optional)

Activity Status

Relationships

Event (N:1)

Media (N)

Location (1:1)

Activity Type (Master Data) (N:1)

5. Collaboration

Purpose

Represents a shared experience that links multiple independent Events belonging to different users.

Primary Key

Collaboration ID

Main Information

Collaboration Status

AI Summary

Created On

Updated On

Relationships

Event (1:N)

6. Business Rules

The system shall ensure:

Every Timeline belongs to one Birth Profile.

Every Event belongs to one Timeline.

Every Activity belongs to one Event.

Events may contain multiple Media and Locations.

Activities may contain multiple Media and Locations.

Collaboration never changes event ownership.

Categories and Activity Types are maintained through Master Data.

7. Summary

The Timeline & Events Data Dictionary defines the core entities responsible for recording, organizing, and presenting a user's life journey while integrating with shared Media, Location, AI, and Master Data services.

8. Next Document

11-07 Relationship ERD