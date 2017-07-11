# Steam -> Firebase token generator

1) Enables users to log in via steam, then redirects passing a firebase auth token as query.
2) Users can link their Discord app to their steam account.

## Running

Dev: ``yarn dev``
Prod: ``yarn start``

In your firebase app redirect to /auth/steam?client_id=\<clientId\>. ``clientId`` needs to be configured in the CLIENTS environment variable (see below).

## Configuration

Copy .env.example to .env and fill in custom values.
FIREBASE_SERVICE_ACC is a firebase service account as json.
CLIENTS is json in the format { clientId: redirectUrl }



