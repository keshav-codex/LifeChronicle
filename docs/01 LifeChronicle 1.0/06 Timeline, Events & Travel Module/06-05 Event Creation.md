06-05 Event Creation
1. Introduction

This document defines the functional requirements for creating events within LifeChronicle Version 1.0.

Events represent meaningful moments in a user's life and form the primary content of the Timeline. Every event created by a user becomes part of their personal Timeline and is displayed chronologically according to the event date.

The Event Creation process uses a single dynamic form that adapts based on the selected Parent Category and Child Category.

2. Purpose

The Event Creation module shall:

Create new Timeline events.

Support dynamic event forms.

Organize events using configurable categories.

Associate media and locations.

Support travel activities.

Support collaborative events.

Maintain chronological ordering.

Support AI-assisted event creation.

3. Actors

Primary Actor

Registered User

Secondary Actors

System

Artificial Intelligence

4. Preconditions

The following conditions shall be be satisfied:

User account is active.

User is authenticated.

Birth Profile exists.

Timeline has been initialized.

User has permission to create events.

Configuration-driven limits have not been exceeded.

5. Event Creation Philosophy

LifeChronicle Version 1.0 uses one universal Event Form.

The form dynamically changes according to the selected Parent Category and Child Category.

Benefits include:

Single Create Event page.

Single Edit Event page.

Consistent user experience.

Reduced maintenance.

Scalable architecture for future categories.

6. Event Information

Mandatory

Parent Category

Child Category

Event Title

Event Date

Optional

Event Time

Description

Cover Image

Contributors

Privacy

Additional fields may appear dynamically depending on the selected category.

7. Event Form Structure

The Event Creation form consists of the following sections.

Section A – Event Basics

Parent Category

Child Category

Event Title

Start Date *

End Date *

Same Day Event ☑ (Default: Checked)

Event Time (Optional)

Users who cannot find an appropriate Parent Category or Child Category may request AI assistance.

AI suggestions shall be selected only from existing configured categories and subcategories.

Section B – Description

Contains:

Event Description

Users may request AI assistance to improve or rewrite the description.

AI shall never modify the description automatically.

Section C – Media

Version 1.0 supports:

Camera
Gallery

One cover image may be uploaded.

Media validation follows the Media module.

Section D – Contributors

Users may optionally invite contributors to participate in the event.

Contributor invitations are managed through the Collaborative Event Management module.

The Birth Profile does not support contributors.

Section E – Privacy

Users may configure event privacy according to the application's hierarchical privacy model.

Event Privacy shall never exceed the permissions granted by higher privacy levels.

Section F – Dynamic Fields

Dynamic fields are loaded according to the selected Parent Category and Child Category.

For Travel categories, the standard location section is replaced by Travel Activities.

8. Travel Activities

If the selected Parent Category belongs to Travel, the form displays:

Add Activity

Add Another Activity

Each activity contains:

Activity Title

Activity Description

Optional Location

If a location is added, the application uses the Global Address Component consisting of:

Address Line 1

Address Line 2

State

Country

Google Map

Global address validation rules apply to every activity.

Users may create multiple travel activities subject to configuration-driven limits.

9. Artificial Intelligence

Version 1.0 provides AI assistance only for:

Category Selection

If users cannot identify an appropriate category or subcategory, AI analyzes:

Event Title

Event Description

AI recommends the most suitable existing categories.

AI shall never create new categories.

Description Assistance

Users may request AI to improve or rewrite the event description.

Acceptance of AI suggestions remains optional.

10. Validation

The Event Creation process performs validation in the following order:

Client-side Validation

Server-side Validation

Business Rule Validation

AI Validation (when requested)

AI processing shall occur only after normal validation succeeds.

11. Business Rules

The system shall ensure:

Events cannot occur before the user's Birth Date.

Future events are not permitted.

Parent and Child Categories must exist.

Event limits are configuration-driven.

Media limits are configuration-driven.

Contributor limits are configuration-driven.

Every event belongs to one Timeline.

Every event is displayed chronologically

Start Date is mandatory.

End Date is mandatory.

When Same Day Event is selected, End Date shall automatically equal Start Date.

End Date shall not be earlier than Start Date.

Event dates shall not precede the user's Birth Date.

Future dates are not permitted.

Timeline ordering shall use the Start Date.

The Event View shall display:

A single date for same-day events.

A date range for multi-day events.

12. Error Handling

Examples include:

Invalid event date.

Missing mandatory information.

Invalid category selection.

Upload limit exceeded.

Storage limit exceeded.

Configuration limit exceeded.

Errors shall be displayed using user-friendly validation messages.

13. Summary

The Event Creation module provides a unified, scalable, and AI-assisted mechanism for recording life events. Through a single dynamic event form, configuration-driven validation, travel activity support, collaborative event integration, and hierarchical privacy controls, the module ensures consistency while remaining flexible for future expansion.

14. Next Document

06-06 Event Update