05-03 Birth Profile Creation
1. Introduction

The Birth Profile Creation module defines the process of creating a user's Birth Profile in LifeChronicle Version 1.0.

After successful authentication, every registered user shall complete the Birth Profile before accessing the Timeline or any other application features.

The Birth Profile establishes the user's digital identity and becomes the foundation of the user's Life Timeline.

2. Purpose

The Birth Profile Creation module shall:

Create the user's Birth Profile.

Capture essential birth-related information.

Validate all required information.

Apply default privacy settings.

Initialize the user's Timeline.

Prevent access to the application until the Birth Profile is completed.
3. Prerequisites

Before creating a Birth Profile:

The user shall have a registered account.

The user shall be successfully authenticated.

The account shall be active.

No existing Birth Profile shall exist for the account.

Each account shall have only one Birth Profile.

4. Birth Profile Form Structure

The Birth Profile consists of the following sections.

Section A – Primary Information

Profile Photo *

The Profile Photo is mandatory.

The application shall encourage users to upload:

Birth Photo (Preferred)

or

Best Early Childhood Photo

The application shall display the following message:

"Don't have a birth photo? You can upload your best early childhood photo instead."

The user may upload the image using:

Camera

Gallery

Validation

Maximum 1 image.

Maximum file size: 2 MB.

Supported formats:

JPG

JPEG

PNG

Full Name *

Mandatory.

Childhood Nickname

Optional.

Section B – Birth Information

Birth Date *

Mandatory.

Birth Time

Optional.

If unknown, the field may be left blank.

Birth Day

Automatically calculated from the Birth Date.

Manual editing shall not be permitted.

Section C – Delivery Information

Delivery Type

The user may select:

Normal

Surgery

Delivery Place

The user may select:

Maternal Home

Paternal Home

Hospital

Birth Center

Other

Delivery Place Name

This field becomes mandatory only when:

Hospital

Birth Center

Other

is selected.

Section D – Birth Location

The application shall ask:

Do you want to add Birth Location?

The user may choose:

Yes

No

If Yes, the following fields shall be available:

Address Line 1

Address Line 2

State

Country

Google Map

Birth Location validation shall follow the Global Address Validation Rules defined by the application.

Section E – Privacy

Default Birth Profile visibility shall be:

Private

Users may modify privacy settings after the Birth Profile has been created.


5. Birth Profile Creation Workflow

Authentication Successful

          │

          ▼

Open Birth Profile Form

          │

          ▼

Complete Mandatory Information

          │

          ▼

Upload Profile Photo

          │

          ▼

System Validation

          │

          ▼

Birth Profile Created

          │

          ▼

Initialize Timeline

          │

          ▼

Open Timeline Dashboard
6. Completion Rules

A Birth Profile shall be considered complete only when:

All mandatory information has been provided.

Validation is successful.

The Profile Photo satisfies the configured validation rules.

Upon successful completion:

The Birth Profile shall be created.

The Timeline shall be initialized automatically.

The user shall be redirected to the Timeline Dashboard.

No draft mode shall be available in Version 1.0.

7. Business Rules

The Birth Profile Creation module follows these principles:

One Birth Profile per account.

Birth Profile is mandatory.

Birth Profile is not a Timeline Event.

Timeline access is not permitted until the Birth Profile is completed.

Birth Day is automatically calculated.

Birth Photo is preferred, but an Early Childhood Photo is accepted.

Default privacy is Private.

Timeline initialization occurs automatically after successful Birth Profile creation.
8. Summary

The Birth Profile Creation module establishes the user's permanent digital identity within LifeChronicle. By collecting essential birth information, validating user input, applying default privacy settings, and automatically initializing the Timeline, it ensures that every user's LifeChronicle journey begins with a complete, consistent, and meaningful foundation.

9. Next Document

05-04 Birth Profile Update