# App Review Notes — Holiday Expense Manager 2.0 — Build 31

Holiday Expense Manager 2.0 helps users plan trips, track travel expenses, store receipts, review OCR results, manage budgets, and share trip data with invited collaborators.

## iCloud / CloudKit usage

- The app uses iCloud / CloudKit.
- Private user data can synchronize through the user's private iCloud database.
- Trip sharing uses Apple's system CloudKit Sharing flow through `UICloudSharingController`.
- Accepting an iCloud sharing invitation requires the invited user to be signed in to iCloud.
- Full CloudKit Sharing verification is best performed with two Apple IDs and two physical devices.
- TestFlight may not always exercise the same system link/opening path for CloudKit Sharing as an App Store/App Review build. Build 31 is submitted to App Review partly to validate the full system CloudKit Sharing path.

## `.hemshare`

`.hemshare` files are only a trip preview / handoff artifact. They do not grant access to a shared trip. Real access is granted only through Apple's iCloud Sharing invitation.

## Suggested review test flow

1. Launch the app.
2. Create a trip.
3. Add an expense manually.
4. Optionally add a receipt image/PDF and run local OCR.
5. Open the trip's Sharing screen.
6. Use **Share with iCloud** / **Udostępnij przez iCloud**.
7. To fully test invitation acceptance, use a second iCloud account on a second device.

## Notes for reviewer

- The app does not require sign-in with a custom account.
- iCloud account availability is required for iCloud sync and CloudKit Sharing.
- Diagnostics logs are local. Users can copy/share them manually if support is needed.
- No advertising or third-party analytics SDK is intentionally included.

