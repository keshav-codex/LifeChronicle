05-06 Birth Profile Validation Rules
1. Introduction

The Birth Profile Validation Rules define the validation requirements for all information collected during the creation and update of a Birth Profile.

The objective of these rules is to ensure data accuracy, consistency, and integrity while providing a user-friendly experience. All validations shall be configurable where applicable and shall be applied consistently throughout the application.

2. Purpose

The Birth Profile Validation Rules shall:

Ensure accurate profile information.

Maintain data consistency.

Prevent invalid or incomplete information.

Support configurable validation policies.

Improve overall data quality.

3. General Validation Rules

The system shall:

Validate all mandatory fields before saving.

Display meaningful validation messages.

Highlight invalid fields.

Prevent duplicate Birth Profiles for the same account.

Save the Birth Profile only after successful validation.

4. Section A – Primary Information Validation

Profile Photo

The Profile Photo is mandatory.

The application shall encourage users to upload:

Birth Photo (Preferred)

or

Best Early Childhood Photo

The application shall display an appropriate message encouraging users to upload the preferred image.

Validation

Exactly one image shall be uploaded.

Maximum file size: 2 MB

Supported formats:

JPG

JPEG

PNG

Corrupted or unsupported files shall be rejected.

Full Name

Validation Rules:

Mandatory.

Cannot be empty.

Leading and trailing spaces shall be removed automatically.

Shall follow the application's global text validation rules.

Childhood Nickname

Validation Rules:

Optional.

Shall follow the application's global text validation rules.

5. Section B – Birth Information Validation

Birth Date

Validation Rules:

Mandatory.

Shall be a valid calendar date.

Future dates shall not be permitted.

Birth Time

Validation Rules:

Optional.

If provided, shall be a valid time.

Birth Day

The Birth Day:

Shall be calculated automatically.

Shall not be editable by the user.

6. Section C – Delivery Information Validation

Delivery Type

Accepted values:

Normal

Surgery

Only configured values shall be accepted.

Delivery Place

Accepted values:

Maternal Home

Paternal Home

Hospital

Birth Center

Other

Delivery Place Name

Validation Rules:

Mandatory only when:

Hospital

Birth Center

Other

is selected.

7. Section D – Birth Location Validation

The Birth Location follows the application's Global Address Validation Rules.

Add Location = No

No location validation shall be performed.

Add Location = Yes

The user shall provide at least one location source.

Supported location sources:

Address

Google Map

Address Validation

The Address shall consist of:

Address Line 1

Address Line 2 (Optional)

State

Country

Google Map Validation

Case 1

Address empty.

Google Map selected.

Result

The application shall automatically populate the available address fields.

Case 2

Address entered.

Google Map not selected.

Result

The manually entered address shall be accepted.

Case 3

Address entered.

Google Map selected.

Result

The application shall compare both sources.

If inconsistencies are detected, a warning shall be displayed requesting the user to verify the information.

The application shall not automatically determine which information is correct.

Case 4

No Address.

No Google Map.

Result

Validation shall fail.

8. Privacy Validation

The system shall:

Apply the default privacy configuration during Birth Profile creation.
Validate any user-selected privacy configuration according to the application's business rules.

9. Validation Messages

Validation messages shall:

Be clear and user-friendly.

Support multilingual presentation.

Identify the affected field.

Explain the required corrective action.

10. Business Rules

The Birth Profile Validation module follows these principles:

Validation shall occur before saving.

Mandatory fields shall always be validated.

Birth Day shall always be system-generated.

Profile Photo validation shall follow configured media rules.

Birth Location shall follow the Global Address Validation Rules.

Validation policies shall be configuration-driven.

11. Summary

The Birth Profile Validation Rules ensure that all Birth Profile information is complete, accurate, and consistent before it becomes part of the user's permanent digital identity. By combining configurable validation, clear user feedback, and standardized business rules, the module maintains the integrity and reliability of LifeChronicle's foundational user data.

12. Next Document

05-07 Birth Profile Business Rules