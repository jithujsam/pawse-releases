# Release status

Updated: 2026-10-26 (3.9.4 release)

## 3.9.4 release (published to main under the owner's standing approval)

| Version | Code | File | SHA-256 | Signed with |
|---|---|---|---|---|
| 3.9.4 | 31 | `apk/Pawse-3.9.4.apk` (6,709,782 bytes) | `876f79309ee2c868a6df8b7c0fba8069c27858c0cc8379f99f166e9d76132635` | Release key, certificate SHA-256 `10ab3feb74724e2e38161c8027e679438a89d3521525980fbbd796ad62faa9f8` |

**Provenance.** Built and signed from pawse-app `6d52027` (main), after lint, typecheck, test (364 passed) and build passed. `./gradlew assembleRelease`.

**Verified on the signed file:** `apksigner` v2 signature, certificate `10ab3feb…a9f8`; `aapt2`: versionCode 31, versionName 3.9.4, not debuggable; the web bundle inside reports 3.9.4/31. The About page, update pop-up and day sheet were checked in a browser.

## 3.9.3 release (published to main under the owner's standing approval)

| Version | Code | File | SHA-256 | Signed with |
|---|---|---|---|---|
| 3.9.3 | 30 | `apk/Pawse-3.9.3.apk` (6,709,462 bytes) | `0adac978efaca7fffec0be6a65dcb6eddd19533ae376a7ba7b67dced2eb526e6` | Release key, certificate SHA-256 `10ab3feb74724e2e38161c8027e679438a89d3521525980fbbd796ad62faa9f8` |

**Provenance.** Built and signed from pawse-app `4ca0766`, after lint, typecheck, test (364 passed) and build passed. `./gradlew assembleRelease`.

**Verified on the signed file:** `apksigner` v2 signature, certificate `10ab3feb…a9f8`; `aapt2`: versionCode 30, versionName 3.9.3, not debuggable; the web bundle inside reports 3.9.3/30. The fix was also checked in a browser: tapping an editable calendar day opens the sheet with its content, and marking the day updates it.

## 3.9.2 release (published to main under the owner's standing approval)

| Version | Code | File | SHA-256 | Signed with |
|---|---|---|---|---|
| 3.9.2 | 29 | `apk/Pawse-3.9.2.apk` (6,709,412 bytes) | `971cbdc2dec69f6cfee5c28a04a407a9b71cb0fa89e486a9d7fd8c8c006674ca` | Release key, certificate SHA-256 `10ab3feb74724e2e38161c8027e679438a89d3521525980fbbd796ad62faa9f8` |

**Provenance.** Built and signed from pawse-app `ed9eb52` (main), after typecheck, test (364 passed) and build passed. `./gradlew assembleRelease`.

**Verified on the signed file:** `apksigner` v2 signature, certificate `10ab3feb…a9f8`; versionCode 29, versionName 3.9.2; the web bundle inside reports 3.9.2/29.

## 3.9.1 release (published to main under the owner's standing approval)

| Version | Code | File | SHA-256 | Signed with |
|---|---|---|---|---|
| 3.9.1 | 28 | `apk/Pawse-3.9.1.apk` (6,709,488 bytes) | `f2efbcb397367efb913bbe4b082a4210882f5e4aee11563ad702f8d551d4dc7c` | Release key, certificate SHA-256 `10ab3feb74724e2e38161c8027e679438a89d3521525980fbbd796ad62faa9f8` |

**Provenance.** Built and signed in a Claude cloud session from pawse-app `8d874f6` (main), after typecheck, test (364 passed) and build passed. `./gradlew assembleRelease`.

**Verified on the signed file:** `apksigner` v2 signature, certificate `10ab3feb…a9f8`; `aapt2`: versionCode 28, versionName 3.9.1; the web bundle inside reports 3.9.1/28.

**Supersedes 3.9.0 (code 27)**, which was published earlier the same day with the slide transitions still in place.

## 3.9.0 release (published to main under the owner's standing approval)

| Version | Code | File | SHA-256 | Signed with |
|---|---|---|---|---|
| 3.9.0 | 27 | `apk/Pawse-3.9.0.apk` (6,709,603 bytes) | `b6d8131342f2dc78e30876f16a150ccaed209698becea7b2f78582b858a15813` | Release key, certificate SHA-256 `10ab3feb74724e2e38161c8027e679438a89d3521525980fbbd796ad62faa9f8` |

**Provenance.** Built and signed in a Claude cloud session from pawse-app `faf2732` (main), after lint, typecheck, test (364 passed) and build passed. `./gradlew assembleRelease`.

**Verified on the signed file:** `apksigner` v2 signature, certificate `10ab3feb…a9f8`; `aapt2`: versionCode 27, versionName 3.9.0; the web bundle inside reports 3.9.0/27.

**Not yet done:** installing over 3.8.9 on a real phone, and checking the new update pop-up on the device.

## 3.8.9 release (published to main under the owner's standing approval)

| Version | Code | File | SHA-256 | Signed with |
|---|---|---|---|---|
| 3.8.9 | 26 | `apk/Pawse-3.8.9.apk` (6,709,716 bytes) | `374ce32d390be21791ff0616b6658d96e2e963e82cae76de31b1abb33ca21838` | Release key, certificate SHA-256 `10ab3feb74724e2e38161c8027e679438a89d3521525980fbbd796ad62faa9f8` |

**Provenance.** Built and signed in a Claude cloud session from pawse-app `7f0c84d` (main, merge of the calendar, loader and dropdown work), after `pnpm lint`, `typecheck`, `test` (364 passed) and `build` passed. Built with `./gradlew assembleRelease` (Gradle 8.11.1, Android SDK platform 35, build-tools 35.0.0).

**Verified on the signed file (2026-10-26):**
- `apksigner verify`: v1 and v2 signatures, one signer, certificate `10ab3feb…a9f8`;
- `aapt2`: `app.detoxcompanion`, versionCode 26, versionName 3.8.9, minSdk 23, target SDK 35;
- the web bundle inside reports `3.8.9`/26.

**Not yet done:** installing on a real phone over 3.8.8, and checking the new dropdown menus on the device.

## 3.8.6 release (published to main under the owner's standing approval)

| Version | Code | File | SHA-256 | Signed with |
|---|---|---|---|---|
| 3.8.6 | 23 | `apk/Pawse-3.8.6.apk` (6,696,639 bytes) | `e78166cdc525b2e305c48f9c965721da46577607d7fb6ecf2e7e54da451be6fd` | Release key, certificate SHA-256 `10ab3feb74724e2e38161c8027e679438a89d3521525980fbbd796ad62faa9f8` |

**Provenance.** Built and signed in a Claude cloud session from pawse-app `616e0a9` (main), after `pnpm lint`, `typecheck`, `test` (13 + 29 + 287) and `build` passed. Later main commits up to `6bb4bf5` change only the README and docs screenshots.

**Verified on the signed file (2026-10-26):**
- `apksigner verify`: v2 signature, one signer, certificate `10ab3feb…a9f8`;
- `aapt2`: `app.detoxcompanion`, versionCode 23, versionName 3.8.6, label `pawse`, not debuggable, target SDK 35;
- the web bundle inside reports `3.8.6`/23, and there's no API key in it;
- the zip passes an integrity check;
- the `docs/RELEASING.md` consistency check prints `OK 3.8.6 23`.

**Not yet done:** installing on a real phone over 3.8.5, and the widgets on a real launcher.

## 3.1.0 release (in this PR; published when it's merged)

| Version | Code | File | SHA-256 | Signed with |
|---|---|---|---|---|
| 3.1.0 | 9 | `apk/Pawse-3.1.0.apk` (4,836,249 bytes) | `33cc64ff62367a8d46fe7324589a99e00cc5925d811a1abdaa0d16effc1fdaf5` | Release key, certificate SHA-256 `10ab3feb74724e2e38161c8027e679438a89d3521525980fbbd796ad62faa9f8` (same as 3.0.0, so it installs over 3.0.0) |

**Provenance.** Built unsigned from pawse-app `f8ca50d` (main, merge of [#21](https://github.com/jithujsam/pawse-app/pull/21), the version bump) in [Actions run 40187542489](https://github.com/jithujsam/pawse-app/actions/runs/40187542489): lint, typecheck, tests (13 + 29 + 273) and the Android unit tests passed. The artifact zip matched GitHub's digest (`bb9da48c…2c41`), and the unsigned APK matched its BUILD-INFO SHA-256 (`469ffcce…f052`). It passed `zipalign -c -p 4` and was signed with the release key outside GitHub (build-tools 35.0.0). The key was deleted from the signing machine afterwards.

**Verified on the signed file (2026-10-25):**
- `apksigner verify`: v1, v2 and v3 signatures, one signer `CN=Pawse, O=Pawse`, certificate `10ab3feb…a9f8`;
- `aapt2`: `app.detoxcompanion`, versionCode 9, versionName 3.1.0, not debuggable, target SDK 35;
- the web bundle inside reports `3.1.0`/9, and there's no API key in it;
- the zip passes an integrity check;
- the `docs/RELEASING.md` consistency check prints `OK 3.1.0 9`.

**Not yet done:** installing on a real phone, in particular over 3.0.0. 3.1.0 moves local data to several recovery tracks per person, so check that the pet and history carry over.

## Previously published: 3.0.0

| Version | Code | File | SHA-256 | Signed with |
|---|---|---|---|---|
| 3.0.0 | 8 | `apk/Pawse-3.0.0.apk` (4,828,057 bytes) | `068d361827ef1ca61b98c022b5418b61adfe9bb555e7f3b93b038a794dd8c14c` | New release key, certificate SHA-256 `10ab3feb74724e2e38161c8027e679438a89d3521525980fbbd796ad62faa9f8` |

**Provenance.** Built unsigned by pawse-app `061424c` in [Actions run 40157196626](https://github.com/jithujsam/pawse-app/actions/runs/40157196626): lint, typecheck, 166 app tests and the Android unit tests passed. The zip matched GitHub's digest. The APK was then zip-align checked and signed with the release key outside GitHub.

**Verified on the signed file (2026-10-25):**
- `apksigner verify`: v1 and v2 signatures, signer `CN=Pawse, O=Pawse`, certificate `10ab3feb…a9f8`;
- `aapt2`: `app.detoxcompanion`, versionCode 8, versionName 3.0.0, not debuggable, min SDK 23, target SDK 35;
- the web bundle inside reports `3.0.0`/8, and there's no API key in it;
- the zip passes an integrity check;
- the `docs/RELEASING.md` consistency check prints `OK 3.0.0 8`.

**Not yet done:** installing on a real phone.

**New signing key.** The key that signed 2.1.0 (certificate `80:81:68:8B:…:25:7B`) existed only on a temporary build machine and was lost. The owner approved a new key on 2026-10-25, and keeps its backup. Because the signature changed, Android won't install 3.0.0 over 2.1.0. People on 2.1.0 uninstall it once and install 3.0.0; signing in restores their pet and history from their account. The README, and the update notes shown in the app, say this.

## Older release

| Version | Code | File | SHA-256 | Checked |
|---|---|---|---|---|
| 2.1.0 | 7 | `apk/Pawse-2.1.0.apk` | `c8801d33730fabf0478ad2e4a63b5f142c81688bbe01814f466d0b17532cba53` | Re-verified 2026-10-25: SHA-256 of the repo file and of the served file match `latest.json`; `apksigner` v1+v2 OK, signer `8081688b…257b`; `aapt2` code 7 / 2.1.0, not debuggable |

## Test builds (separate from releases)

The release procedure is [`docs/RELEASING.md`](https://github.com/jithujsam/pawse-app/blob/main/docs/RELEASING.md) in the app repo. Follow it for every release.

| File | App | Version | Signed with | SHA-256 | From |
|---|---|---|---|---|---|
| `test-builds/Pawse-Test-3.0.0-8.apk` | `app.detoxcompanion.test` ("Pawse Test") | 3.0.0, code 8 | Debug (test) key `fe72e8b1…d19a` | `3dd30940ff7d3a37d7495fecf3d46d2a34973a50ad032c408741d04c8ade3fa5` | pawse-app `90dda3e`, [Actions run 40156425870](https://github.com/jithujsam/pawse-app/actions/runs/40156425870) |

Verified 2026-10-25 after downloading the artifact:
- the zip matches GitHub's digest, and the APK passes an integrity check;
- `apksigner` verifies it;
- `aapt2` shows the package, code and version above;
- the web bundle inside reports `3.0.0`/8, and there's no API key in it;
- all 166 app tests and the Android unit tests passed in that run.

It hasn't been installed on a device yet.

**Test builds never go in `apk/` or `latest.json`.** Those are the public update channel, and they only take a release-signed `app.detoxcompanion` APK (certificate `10ab3feb…a9f8`). A test build there would be offered to every user, and couldn't update their app anyway. Test builds live only in `test-builds/`.

New test builds come from every push to `pawse-app/main` (Actions → Android APK). Each run's artifact holds the APK and its build info.
