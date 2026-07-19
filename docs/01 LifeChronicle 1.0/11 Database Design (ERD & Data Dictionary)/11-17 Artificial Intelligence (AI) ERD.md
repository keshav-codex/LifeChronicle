11-17 Artificial Intelligence (AI) ERD

1. Introduction

The Artificial Intelligence (AI) ERD defines the entities responsible for AI-assisted content improvement, content safety, administrative assistance, and intelligent recommendations within LifeChronicle.

The AI module provides suggestions only and never performs automatic business operations.

2. Entity Overview

The AI domain consists of the following entities:

AIProvider

AIPromptTemplate

AIRequest

AIFeedback

The domain integrates with:

Master Data

Shared Infrastructure

Birth Profile

Timeline & Events

Relationship Management

Concern Management

Administration

3. Entity Relationships

AIProvider

      │

      ▼

AIPromptTemplate

      │

      ▼

AIRequest

      │

      ▼

AIFeedback

AI services are shared across all supported application modules.

4. Entity Responsibilities

AIProvider

Represents the AI service provider used by the application.

Supports multiple providers while allowing Version 1.0 to use Gemini Free API.

AIPromptTemplate

Maintains configurable prompt templates used by AI features.

Prompt templates are managed without modifying application code.

AIRequest

Maintains the history of AI requests and responses.

Supports content improvement, categorization, administrative assistance, and safety analysis.

AIFeedback

Maintains user and staff feedback for AI-generated suggestions.

Supports future prompt improvement and AI quality evaluation.

5. Business Rules

The AI module shall ensure:

AI provides suggestions only.

AI never performs automatic business updates.

AI improves content quality.

AI assists administrative users.

AI suggests new Master Data entries.

AI detects incorrect category selections.

AI drafts concern responses.

AI detects harmful or inappropriate content.

AI detects abusive, illegal, sexually explicit, violent, hate, spam, or 
suspicious content.

AI generates Alerts through the shared Alert service.

AI configuration is maintained through Master Data.

AI requests are permanently logged.

AI never learns from user data in Version 1.0.

6. Summary

The AI ERD establishes a configurable and reusable artificial intelligence framework that improves application quality, assists users and administrators, and supports content safety while ensuring all business decisions remain under human control.

7. Next Document

11-18 Artificial Intelligence (AI) Data Dictionary