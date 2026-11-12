# WMSHub Android downloads

Signed production APKs for external partners deploying WMSHub through their MDM.

## Download

- [Latest APK](https://github.com/kumbirai/wmshub-mobile-releases/releases/latest/download/wmshub-mobile.apk)
- [Release history and installation details](https://github.com/kumbirai/wmshub-mobile-releases/releases)
- [Latest SHA-256 checksum](https://github.com/kumbirai/wmshub-mobile-releases/releases/latest/download/SHA256SUMS)
- [Latest MDM package metadata](https://github.com/kumbirai/wmshub-mobile-releases/releases/latest/download/mdm-metadata.json)

For a controlled rollout, use the version-specific download link on the release page. The latest link changes when a new release is published.

## MDM installation

Download the APK and import it into your MDM as an Android enterprise/internal application. The package identifier is `biz.wmshub.wms`. The app connects to the WMSHub production service and requires a provisioned WMSHub account.

For an in-place update, the installed app must use the same package identifier and signing certificate, and the new version code must be higher. Check `mdm-metadata.json` for the minimum API level, version code, APK hash, and signing-certificate SHA-256 fingerprint.

Verify the download against `SHA256SUMS` before deployment. Device and MDM rollout testing remains the responsibility of the deploying organisation.

This repository contains distribution information and release binaries. Application source code is not included.
