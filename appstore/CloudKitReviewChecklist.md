# CloudKit Review Checklist

## Container

- Container: `iCloud.com.hem.HolidayExpenseManager`

## Production readiness

- [ ] Production schema deployed.
- [ ] `cloudkit.share` exists in Production.
- [ ] HEM record types exist in Production.
- [ ] Root Trip records can be created in Production.
- [ ] `UICloudSharingController` is used for real iCloud Sharing.
- [ ] `.hemshare` is only a preview and does not grant access.
- [ ] Known TestFlight/App Store lookup limitation is described in App Review notes.

## Sharing verification

- [ ] Sender is signed in to iCloud.
- [ ] Receiver is signed in to a different iCloud account.
- [ ] Sender opens trip Sharing screen.
- [ ] Sender uses **Share with iCloud**.
- [ ] Receiver accepts the system iCloud Sharing invitation.
- [ ] Incoming share opens the app.
- [ ] Shared trip appears locally for receiver.
- [ ] Local logs show incoming CloudKit share acceptance.

