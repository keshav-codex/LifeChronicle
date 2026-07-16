00-05 Repository Structure
1. Introduction

This document defines the Git repository structure adopted for the LifeChronicle project. A consistent repository organization improves maintainability, simplifies collaboration, and enables scalable development throughout the project's lifecycle.

The repository is organized to clearly separate application source code, documentation, configuration, automation scripts, testing resources, and deployment assets.

2. Repository Objectives

The repository structure has been designed to:

Maintain a clean project organization.
Separate source code from documentation.
Simplify onboarding for new developers.
Support documentation-driven development.
Enable automated deployment.
Improve maintainability.
Support future project expansion.
3. Repository Layout
LifeChronicle/
│
├── apps/
├── config/
├── docs/
├── master_data/
├── tools/
├── static/
├── media/
├── templates/
├── tests/
├── requirements/
├── deployment/
├── logs/
├── backups/
├── .github/
├── manage.py
├── README.md
├── LICENSE
├── .gitignore
└── .env.example
4. Repository Directory Responsibilities
apps/

Contains all Django applications.

Each application is responsible for one business domain.

Example:

apps/
│
├── accounts/
├── administration/
├── birth_profile/
├── categories/
├── communication/
├── concerns/
├── events/
├── locations/
├── media/
└── ai/

No application should directly own another application's business logic.

config/

Contains Django project configuration.

Includes:

Settings
URLs
WSGI
ASGI
Environment Configuration

This folder represents the project configuration, not business functionality.

docs/

Contains the complete project documentation.

Documentation is divided into structured modules.

Examples:

Project Architecture
Functional Requirements
System Architecture
Module Documentation
Database Design
Business Rules
User Manual

Documentation is considered part of the source code.

master_data/

Contains version-controlled seed files.

Examples:

Languages
Categories
Subcategories
Departments
Designations
AI Prompts
Notification Templates
System Messages

These files are imported into the database using Django management commands.

tools/

Contains development utilities.

Examples:

Documentation Generator
Data Import Scripts
Migration Utilities
Developer Tools
Reporting Scripts

These utilities are not part of the production application.

static/

Contains global static assets.

Examples:

CSS
JavaScript
Fonts
Icons
Images
media/

Stores user-uploaded files.

Examples:

Event Images
Birth Profile Images

Media files are managed separately from application source code.

templates/

Contains reusable Django templates.

Templates shared across multiple applications are stored here.

Application-specific templates remain inside their respective applications where appropriate.

tests/

Contains automated test cases.

Examples:

Unit Tests
Integration Tests
API Tests
Business Rule Tests

Testing remains independent of application modules.

requirements/

Contains dependency files.

Examples:

base.txt
development.txt
production.txt

This allows different environments to manage dependencies independently.

deployment/

Contains deployment resources.

Examples:

Deployment Notes
Environment Configuration
Server Configuration
Production Setup
logs/

Stores application log files.

Examples:

Error Logs
AI Logs
Security Logs

Log files are excluded from version control unless required.

backups/

Stores backup-related resources.

Examples:

Database Backup Scripts
Recovery Procedures

Production backups are never stored in the repository.

.github/

Contains GitHub automation.

Examples:

GitHub Actions
CI/CD Workflows
Issue Templates
Pull Request Templates
5. Repository Design Principles

The repository follows these principles:

One responsibility per directory.
Business modules remain independent.
Documentation is version controlled.
Automation tools are isolated.
Configuration remains centralized.
User-generated content is separated from source code.
6. Naming Conventions

Repository naming standards:

Lowercase folder names.
Underscore-separated names where applicable.
Meaningful directory names.
No spaces in source code folders.
Consistent naming across modules.

Examples:

birth_profile
category_manager
master_data
deployment
7. Version Control Strategy

The repository is managed using Git.

All project assets except generated files should be version controlled.

Examples excluded from Git:

Python cache
Virtual environments
Database files
User uploads
Log files
Temporary files
8. Future Expansion

The repository structure is designed to support future additions such as:

Mobile applications
Microservices
Machine learning models
Background workers
Additional deployment environments
New documentation modules

without reorganizing the existing project.

9. Summary

The LifeChronicle repository is organized to provide a clean, scalable, and maintainable development environment. Every directory has a clearly defined responsibility, enabling developers to locate source code, documentation, configuration, and project resources quickly and consistently.

The structure supports documentation-driven development and long-term project growth while maintaining a clear separation between business logic, configuration, tooling, and generated data.

10. Next Document

00-06 Project Folder Structure

The next document explains the detailed internal folder organization of the Django project, including application directories, templates, static files, media organization, and development conventions.