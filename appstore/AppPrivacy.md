# App Privacy Proposal

This document is a proposed App Store Connect privacy questionnaire reference for Holiday Expense Manager 2.0. It should be reviewed manually before submission.

## Summary

Holiday Expense Manager 2.0 stores user-created travel data locally on the device and may synchronize it through the user's iCloud / CloudKit account. Shared trips may be shared with invited collaborators through Apple's CloudKit Sharing.

The app does not intentionally include advertising, tracking, or third-party analytics SDKs.

## Data Collected

To be confirmed in App Store Connect as appropriate:

- User Content:
  - trips,
  - expenses,
  - participants,
  - stays/accommodation,
  - budgets,
  - exchange rates,
  - receipt attachments,
  - OCR-recognized receipt text,
  - local user profile,
  - sharing/collaboration metadata.
- Diagnostics:
  - local diagnostic logs created by the app.

## Data Linked to User

Data may be linked to the user through the user's own device and iCloud account when iCloud / CloudKit sync is enabled or when sharing is used. The app does not create a separate HEM account.

## Data Not Used for Tracking

The data is not used for third-party tracking. There is no intentional advertising identifier use, ad network integration, or third-party analytics SDK.

## Purpose

- App Functionality:
  - trip planning,
  - expense tracking,
  - budgeting,
  - receipt OCR,
  - reports,
  - iCloud sync,
  - iCloud sharing.
- User Content:
  - user-entered trips, expenses, receipts and travel notes.
- iCloud Sync:
  - synchronization between the user's Apple devices,
  - shared trip access for invited collaborators.

## Diagnostics

Diagnostic logs are stored locally. They are not sent automatically. The user can copy/share logs manually for support.

## Manual confirmation before App Store Connect submission

- Confirm there are no third-party analytics SDKs.
- Confirm there are no advertising SDKs.
- Confirm whether OCR processing remains local only.
- Confirm whether any network calls besides iCloud/CloudKit and optional exchange-rate providers are active in the release build.
- Confirm exact App Store Connect categories selected under App Privacy.

