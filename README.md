# prysm-testing

Work-in-progress target app builds for Prysm, for every app. Never installed from by a release build of Prysm.

- Debug builds opt in per app via `DEBUG_TEST_APP_IDS` in Prysm's `gradle.properties`.
- One installable asset per release, named `<packageName>_<version>.apk` or `.apkm`.
- Tags: `<appId>-<version>[-note]`, e.g. `instagram-454.0.0.54.77`.
- The newest non-draft release holding an asset for an app is the one Prysm uses.

A build is published to the app's live repo (`issac-xt/prysm-<app>`) only after it passes on-device testing from here.
