11-04 Birth Profile Data Dictionary

1. Introduction

This document defines the data structure for the Birth Profile domain of LifeChronicle Version 1.0.

The Birth Profile stores the user's personal identity and serves as the foundation of the Timeline. Authentication information is maintained separately within the Accounts domain.

2. BirthProfile

Purpose

Represents the user's personal identity and the starting point of the Timeline.

Primary Key

Birth Profile ID

Main Information

Profile Information

Profile Photo (Media Reference)

Title (Optional)

First Name

Middle Name (Optional)

Last Name

Childhood Nickname (Optional)

Birth Information

Birth Date

Birth Time (Optional)

Birth Day (System Calculated)

Gender 

Nationality

Delivery Information

Delivery Type

Delivery Place

Delivery Place Name (Conditional)

Birth Location

Birth Location (Location Reference)

Profile Status

Not Started

In Progress

Completed

Audit Information

Created On

Updated On

3. Relationships

LoginProfile (1:1)

Timeline (1:1)

Event (1)

Relationship (1)

Media (N:1)

Location (N:1)

Gender (Master Data) (N:1)

Nationality (Master Data) (N:1)

Delivery Type (Master Data) (N:1)

Delivery Place (Master Data) (N:1)

4. Business Rules

The system shall ensure:

Every Login Profile owns exactly one Birth Profile.

Birth Profile is required before Timeline initialization.

Users may save incomplete information and continue later.

Birth Day is automatically calculated from Birth Date.

Profile Photo references the shared Media entity.

Birth Location references the shared Location entity.

Gender, Nationality, Delivery Type, and Delivery Place reference Master Data.

Users may update Birth Profile information after completion according to 
business rules.

5. Visibility Rules

Default visibility for approved relatives:

Profile Photo

Full Name

All remaining Birth Profile information remains private unless future privacy features are introduced.

Relationship status changes shall affect Birth Profile visibility according to Relationship Management rules.

6. Summary

The Birth Profile Data Dictionary establishes a normalized identity model by separating personal identity from authentication while integrating with shared Media, Location, Timeline, and Master Data services.

7. Next Document

11-05 Timeline & Events ERD