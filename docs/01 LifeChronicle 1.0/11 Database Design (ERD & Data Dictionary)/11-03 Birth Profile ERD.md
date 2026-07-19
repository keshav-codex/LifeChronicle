11-03 Birth Profile ERD

1. Introduction

The Birth Profile ERD defines the identity domain of LifeChronicle.

A Birth Profile represents the user's personal identity and serves as the starting point of the user's digital life timeline. It is independent of authentication and is linked to exactly one Login Profile.

2. Entity Overview

The Birth Profile domain consists of the following entities:

BirthProfile

The entity integrates with shared services including:

Media

Location

Master Data

3. Entity Relationships


LoginProfile (1:1)

        │
        ▼

BirthProfile
        │

        ├── Media (N:1)

        ├── Location (N:1)

        ├── Gender (Master Data) (N:1)

        ├── Nationality (Master Data) (N:1)

        ├── DeliveryType (Master Data) (N:1)

        └── DeliveryPlace (Master Data) (N:1)

4. Entity Responsibilities

BirthProfile

Represents the user's personal identity.

Stores birth information, delivery information, birth location, and profile information while acting as the root entity for the user's Timeline.

5. Business Rules

The Birth Profile domain shall ensure:

Every Login Profile has exactly one Birth Profile.

Birth Profile completion is mandatory before accessing the Timeline Dashboard.

Users may save partial information and continue later.

The system automatically saves progress during data entry.

Profile Photo is stored using the shared Media service.

Birth Location is stored using the shared Location service.

Gender, Nationality, Delivery Type, and Delivery Place are maintained through 
Master Data.

Birth Day is automatically calculated from Birth Date.

Users may edit Birth Profile information after completion according to 
business rules.

6. Profile Status

The Birth Profile supports the following lifecycle:

Not Started

In Progress

Completed

Users may log out while the profile is in progress and continue editing after logging in again.

7. Visibility Rules

By default, approved relatives may view only:

Profile Photo

Full Name

No other Birth Profile information is shared.

If the relationship status becomes Hold, Delete, or Block, the Birth Profile is no longer visible according to relationship business rules.

8. Summary

The Birth Profile ERD establishes the user's identity within LifeChronicle by separating personal information from authentication while integrating with shared Media, Location, and Master Data services.

9. Next Document

11-04 Birth Profile Data Dictionary