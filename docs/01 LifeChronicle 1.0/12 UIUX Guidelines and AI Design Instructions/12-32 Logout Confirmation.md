12-32 Logout Confirmation

Page Information

Item	Value

Module	12 – UI/UX

Page Name	Logout Confirmation

Page ID	UI-032

Layout	LYT-19 Confirmation Dialog

Primary User	Registered User

Status	Version 1.0

Design Philosophy

Logging out is a security-related action that should prevent accidental sign-out while remaining quick and convenient.

The confirmation dialog should be simple, lightweight, and consistent with other confirmation dialogs used throughout the application.

1. Introduction

The Logout Confirmation dialog appears whenever a user chooses Logout from the User Menu.

It asks the user to confirm their intention before ending the current authenticated session.

2. Purpose

The Logout Confirmation dialog enables users to:

Confirm logout.

Cancel logout.

Securely end the current session.

3. User Access

User	Access

Registered User	✅

Guest	❌

Staff	✅

Super Administrator	✅

4. Layout

Uses

LYT-19 Confirmation Dialog

Displayed as:

Modal dialog (Desktop)

Bottom sheet dialog (Mobile)

Centered confirmation window (Tablet)

The current page remains visible behind the dialog.

5. Front View
────────────────────────────

🚪 Logout

Are you sure you want to logout?

You will need to sign in again to
access your LifeChronicle.

────────────────────────────

Cancel        Logout

────────────────────────────
6. User Actions

6.1 Cancel

Closes the dialog.

Returns to the current page.

No data is changed.

6.2 Logout

The system:

Ends the authenticated session.

Invalidates the active login token/session.

Clears temporary session data.

Redirects the user to the Landing Page.

7. Navigation Flow

Current Page

↓

👤 User Menu

↓

Logout

↓

Confirmation Dialog

↓

Logout

↓

Landing Page

8. Business Rules

Logout always requires confirmation.

Unsaved changes on the current page are handled according to the page's own 
save/unsaved-changes rules.

Only the current session is terminated.

Other active sessions on different devices remain active.

Logout is recorded in the audit log.

9. Global Validation Rules

No user input is required.

System validates:

Active authenticated session.

Successful session termination.

Secure token invalidation.

10. Master Data Dependencies

Code	Purpose

BTN_*	Button Labels

TXT_*	Labels

MSG_*	Messages

DLG_*	Confirmation Dialog Text

11. Shared Components Used

LC-DLG-001 Confirmation Dialog

LC-BTN-001 Primary Button

LC-BTN-002 Secondary Button

12. AI Usage

None.

Logout is a security operation and does not use AI.

13. Responsive Behaviour

Mobile

Bottom-sheet confirmation.

Large touch buttons.

Tablet

Centered dialog.

Responsive spacing.

Laptop/Desktop

Centered modal dialog.

Keyboard support (Enter/Esc).

14. Testing Checklist

Logout confirmation appears.

Cancel returns to current page.

Logout ends the current session.

Redirect to Landing Page.

Session token invalidated.

Responsive behaviour.

Keyboard accessibility.

15. Summary

The Logout Confirmation dialog provides a simple and secure way for users to end their authenticated session. By requiring explicit confirmation and using a consistent confirmation dialog design, it helps prevent accidental logout while maintaining a smooth user experience.