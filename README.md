# Titli HHT device logs

Diagnostic logs pushed automatically by the Titli Fashions HHT app.

Layout: `logs/<device>/<yyyy-MM-dd>/<HHmmss>.txt`

`<device>` is `MODEL-<8 hex of ANDROID_ID>` - stable per handheld, not tied to any person.
Each file holds only the log bytes written since that handheld's previous push, so the files
read in order as one continuous log. The first file of a run starts with a session banner
(app version, device, Android version, server URL, selected location).

This is an orphan branch: it shares no history with `main`, which carries `version.json` and
the release APKs. Nothing here is read by the app.