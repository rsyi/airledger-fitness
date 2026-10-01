# Privacy Policy — Ledger

_Last updated: September 30, 2026_

Ledger is a personal, single-user fitness tracking application operated
by Robert Yi. It is not a commercial product and has no other users.
This policy explains what data the app handles and how.

## What the app accesses

Ledger records the owner's own training data (strength, cardio, body
weight, climbing, nutrition, notes) and, with the owner's explicit
authorization, reads data from third-party services the owner already
uses:

- **WHOOP** — sleep, recovery, and cycle data, via the WHOOP API
  (read-only scopes: `read:sleep`, `read:recovery`, `read:cycles`).
- **Withings** — body-weight and body-composition measurements.
- **Google (Gmail / Photos Picker)** — read-only access used solely to
  import the owner's own climbing-log export and to attach the owner's
  own training videos.
- **Macrofactor / Android Health Connect** — the owner's nutrition data.

The app only ever accesses the account owner's own data, and only after
that owner grants access through each provider's standard OAuth consent.

## How data is stored and used

- Training data is stored in the owner's own private Google Spreadsheet
  and in local storage on the owner's own Android device.
- Access tokens for connected services are stored in the device's
  encrypted secure storage. They are never written to the spreadsheet
  or shared.
- Data is used only to display the owner's metrics, generate training
  guidance, and produce coaching summaries for the owner.
- Anonymized workout context may be sent to Anthropic's Claude API to
  generate coaching text and effort estimates, under Anthropic's terms;
  no data is used to train models.

## What the app does NOT do

- No data is sold, rented, or shared with any third party for
  advertising or any other purpose.
- There are no other users; no one else's data is collected.
- Data pulled from WHOOP, Withings, Google, or Macrofactor is used only
  for the owner's own tracking and is never redistributed.

## Data retention and deletion

The owner controls all stored data directly (the spreadsheet and the
device) and can delete it at any time. Disconnecting a service in the
app removes its stored access tokens. Access granted to Ledger can also
be revoked at any time from each provider's account settings (e.g. the
WHOOP app, Google Account permissions).

## Contact

Questions about this policy: rosiny@gmail.com
