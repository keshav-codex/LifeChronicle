11-16 Master Data Data Dictionary
1. Introduction

This document defines the data structure for the Master Data domain of LifeChronicle Version 1.0.

The Master Data domain provides centralized configuration, business values, localization, and validation rules used throughout the application.

2. MasterData
Purpose

Maintains configurable business values shared across all application modules.

Primary Key
Master Data ID
Main Information
Master Data Type
Parent Master Data
Code
Display Name
Description (Optional)
Display Order
System Defined
Active Status
Created On
Updated On
Relationships
Parent MasterData (Self Reference) (N:1)
MasterDataTranslation (1)
MasterDataValidation (1)
3. MasterDataTranslation
Purpose

Maintains multilingual values for Master Data records.

Primary Key
Translation ID
Main Information
Language
Display Name
Description (Optional)
Active Status
Relationships
MasterData (N:1)
4. MasterDataValidation
Purpose

Maintains configurable validation rules associated with Master Data.

Primary Key
Validation ID
Main Information
Validation Type
Validation Value
Validation Message
Active Status
Relationships
MasterData (N:1)
5. Business Rules

The system shall ensure:

A single MasterData entity is used throughout the application.
Parent-child hierarchy is supported.
Master Data supports multilingual translations.
Validation rules are configurable.
AI suggestions require administrator approval before implementation.
Used records support Soft Delete only.
Unused records may be Hard Deleted.
System-defined records cannot be deleted.
Excel Import and Export are supported.
All changes are recorded through the shared Audit service.
6. Usage Examples

The Master Data module supports configuration for:

The Master Data module supports configuration for:

Business Configuration

- Categories
- Subcategories
- Activity Types
- Relationship Categories
- Relationship Status
- Concern Categories
- Concern Priorities
- Staff Roles
- Departments
- Designations
- Permissions

Application Configuration

- Application Name
- Logo
- Favicon
- Login Background
- Banner Images
- Welcome Messages
- Footer Text
- Copyright
- Contact Information
- Social Media Links

Localization

- Languages
- Translation Labels
- Date Formats
- Time Formats
- Currency Formats

Validation Configuration

- File Types
- Upload Limits
- Password Policies
- Field Validation Rules

System Configuration

- Notification Types
- Alert Types
- Feature Flags
- AI Configuration
- Reference Number Formats
- Future application configurations

7. Summary

The Master Data Data Dictionary provides a centralized and extensible configuration framework that enables LifeChronicle to remain configurable, multilingual, maintainable, and scalable while minimizing application code changes.

8. Next Document

11-17 AI ERD