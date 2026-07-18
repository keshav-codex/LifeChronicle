11-05 Timeline & Events ERD
1. Introduction

The Timeline & Events ERD defines the core entities used to record, organize, and display a user's life journey.

A Timeline belongs to one Birth Profile and contains Events. Each Event may include Activities, Media, Locations, AI suggestions, and Collaboration.

2. Entity Overview

The Timeline domain consists of the following entities:

Timeline
Event
Activity
Collaboration

The domain integrates with:

Media
Location
Master Data
Artificial Intelligence
3. Entity Relationships
BirthProfile (1:1)
        │
        ▼
     Timeline (1)
        │
        ▼
      Event (N)
        │
        ├── Activity (N)
        ├── Media (N)
        ├── Location (N)
        ├── Collaboration (0..1)
        ├── AI Suggestion (N)
        └── Category (Master Data)
4. Entity Responsibilities
Timeline

Represents the user's chronological life journey and acts as the parent of all Events.

Event

Represents a significant life moment recorded by the user.

Activity

Represents an individual activity performed within an Event.

Collaboration

Links independent Events owned by different users to represent a shared real-life experience while preserving individual ownership.

5. Business Rules

The Timeline domain shall ensure:

Every Birth Profile owns one Timeline.
Every Event belongs to one Timeline.
Every Activity belongs to one Event.
Events may contain multiple Media and Locations.
Categories reference Master Data.
Collaborative Events maintain independent ownership.
AI suggestions remain optional.
Configuration-driven limits apply throughout the module.
6. Summary

The Timeline & Events ERD establishes the central business domain of LifeChronicle by organizing life events, activities, media, locations, collaboration, and AI assistance within a normalized and scalable architecture.

7. Next Document

11-06 Timeline & Events Data Dictionary