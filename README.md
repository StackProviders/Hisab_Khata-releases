# Hisab Khata — releases

Android release builds of **Hisab Khata** (হিসাব খাতা), a personal finance and project expense tracker.

This repository holds **only** the published APKs. The source code is private. The app reads the latest release here to offer in-app updates, without any login or token.

## Install or update

- **Inside the app:** go to Settings → Check for updates, or tap the "Update available" card. The app downloads the new version, checks its SHA-256, then opens Android's installer.
- **Manually:** download `hisab-khata-<version>.apk` from the latest [release](../../releases/latest) and open it on your phone.

The first time, Android asks you to allow installing apps from this source.

## Verify a download

Every release includes `hisab-khata-<version>.apk.sha256`. Check the APK against it:

```
sha256sum -c hisab-khata-<version>.apk.sha256
```

All releases are signed with the same key. Android refuses to install an update that is not signed with the key of the app already on your phone. The certificate's SHA-256 is:

`95:27:FD:F7:93:C0:E7:07:61:DB:C8:E0:6F:70:5E:98:7F:DB:07:49:4E:CC:31:2E:22:74:38:50:3E:00:D6:32`

Your records are stored in your Hisab Khata account, so installing an update never deletes them.
