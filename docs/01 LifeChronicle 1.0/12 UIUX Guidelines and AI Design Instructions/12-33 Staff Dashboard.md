12-33 Staff Dashboard

Page Information

Item	Value

Module	12 – UI/UX

Page Name	Staff Dashboard

Page ID	UI-033

Layout	LYT-20 Staff Dashboard Layout

Primary User	Staff

Status	Version 1.0

Design Philosophy

The Staff Dashboard provides a centralized workspace for staff members to perform operational tasks assigned by the organization.

Unlike the Administration Portal, the Staff Dashboard focuses on day-to-day operations rather than application configuration.

The interface should prioritize efficiency, task visibility, and quick navigation.

1. Introduction

The Staff Dashboard is the home page for authenticated staff members.

It displays assigned work, operational statistics, recent activities, and quick access to staff functions based on the staff member's assigned role and permissions.

2. Purpose

The Staff Dashboard enables staff members to:

View assigned tasks.

Review pending verification requests.

Moderate reported content.

Manage support requests.

Review collaboration requests.

Access operational reports.

Monitor daily workload.

3. User Access

User	Access

Guest	❌

Registered User	❌

Staff	✅

Super Administrator	Full Access

4. Page Layout

Uses

LYT-20 Staff Dashboard Layout

The page consists of:

Staff Summary

Quick Statistics

Assigned Tasks

Quick Actions

Recent Activity

5. Front View
────────────────────────────────────────

Staff Dashboard

Welcome,

Krishna

────────────────────────────────────────

Pending Tasks

18

Verification Requests

6

Support Requests

12

Reported Content

4

────────────────────────────────────────

Quick Actions

✔ Verify Users

✔ Review Reports

✔ Support Requests

✔ Moderate Content

────────────────────────────────────────

Assigned Tasks

□□□□□□□□□□□□□□□□□□

────────────────────────────────────────

Recent Activity

□□□□□□□□□□□□□□□□□□
6. Page Sections

6.1 Staff Summary

Displays

Staff Name

Staff Role

Department (if applicable)

Current Status

6.2 Quick Statistics

Displays

Pending Tasks

Verification Requests

Support Requests

Reported Content

Assigned Cases

Statistics are updated in real time where practical.

6.3 Quick Actions

Displays shortcuts to commonly used functions.

Examples

Verify Users

Manage Support Requests

Review Reported Content

Moderate Media

Review Collaboration Requests

Available actions depend on staff permissions.

6.4 Assigned Tasks

Displays tasks assigned to the current staff member.

Each task card contains:

Task ID

Task Type

Priority

Assigned Date

Current Status

Selecting a task opens the corresponding management page.

6.5 Recent Activity

Displays recent actions performed by the current staff member.

Examples

User Verified

Support Request Closed

Report Reviewed

Collaboration Request Processed

This section provides a personal activity history only.

7. Navigation Flow

Staff Login

↓

Staff Dashboard

↓

Select Function

↓

Complete Task

↓

Return Dashboard

8. Business Rules

Dashboard content is permission-based.

Staff members only see assigned modules.

Quick Statistics update automatically.

Completed tasks move to history.

Administrative configuration options are not available.

Staff cannot access Master Data or System Configuration.

9. Global Validation Rules

System Managed

Staff Role

Assigned Permissions

Task Status

Dashboard Statistics

Activity History

No manual data entry is required.

10. Master Data Dependencies

Code	Purpose

STAFF_ROLE_*	Staff Roles

TASK_STATUS_*	Task Status

PRIORITY_*	Priority Levels

BTN_*	Buttons

TXT_*	Labels

11. Shared Components Used

LC-DASH-001 Dashboard Summary Card

LC-TASK-001 Task Card

LC-STAT-001 Statistics Card

LC-BTN-001 Primary Button

LC-TBL-001 Data Table

12. AI Usage

None.

Staff decisions remain manual in Version 1.0.

13. Responsive Behaviour

Mobile

Single-column dashboard.

Scrollable task list.

Large touch controls.

Tablet

Two-column dashboard.

Laptop/Desktop

Multi-column operational dashboard.

Persistent quick actions panel.

Responsive statistics cards.

14. Testing Checklist

Permission-based dashboard.

Statistics display.

Assigned task visibility.

Quick Actions.

Navigation.

Responsive behaviour.

Accessibility.

15. Summary

The Staff Dashboard provides operational staff with a focused workspace for completing assigned responsibilities efficiently. By separating operational tools from system administration and displaying only role-appropriate information, the dashboard supports secure, streamlined, and productive daily workflows.