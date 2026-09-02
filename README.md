# Kaya — update channel

This repository hosts the over-the-air update manifest for **Kaya**, an offline
Baduk (Go) app. The app reads `updater_metadata.json`, compares its `versionCode`
to the installed build, and if a newer one is listed, downloads and verifies the
release APK attached to this repo before installing it.

Kaya is otherwise fully offline — this check is its only network use, and it can
be turned off in the app's About screen.
