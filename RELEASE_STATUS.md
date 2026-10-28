# Release status

Updated: 2026-10-28 (3.9.16 release)

## 3.9.16 release (published to main by the publish workflow)

| Version | Code | File | SHA-256 | Signed with |
|---|---|---|---|---|
| 3.9.16 | 43 | `apk/Pawse-3.9.16.apk` (7150394 bytes) | `a1538ebc14d261af0b75b6755ff5f56e279f9160424c65aaa31599c30fd4c19a` | Release key, certificate SHA-256 `10ab3feb74724e2e38161c8027e679438a89d3521525980fbbd796ad62faa9f8` |

**Provenance.** Commit `cbb560074ead6a3c6152a5582d381cf95e202581`, built 2026-10-28T04:47:08Z by https://github.com/jithujsam/pawse-app/actions/runs/40633918198. Tests: 13 passed (13) 35 passed (35) 398 passed (398); Android unit tests passed.

## 3.9.15 release (published to main by the publish workflow)

| Version | Code | File | SHA-256 | Signed with |
|---|---|---|---|---|
| 3.9.15 | 42 | `apk/Pawse-3.9.15.apk` (6710400 bytes) | `a608dc37ac66b0ade36e3389c3c6657d0efb1fe034d627a65d65a2d312eff8fd` | Release key, certificate SHA-256 `10ab3feb74724e2e38161c8027e679438a89d3521525980fbbd796ad62faa9f8` |

**Provenance.** Commit `e1c2a3ce34ef3cbcb868823a04cad701b7035250`, built 2026-10-27T07:42:59Z by https://github.com/jithujsam/pawse-app/actions/runs/40468453830. Tests: 13 passed (13) 35 passed (35) 394 passed (394); Android unit tests passed.

## 3.9.14 release (published to main by the publish workflow)

| Version | Code | File | SHA-256 | Signed with |
|---|---|---|---|---|
| 3.9.14 | 41 | `apk/Pawse-3.9.14.apk` (6710400 bytes) | `4783f4333234af398fcc901a31e33b231d11bff979fe96c1e948327a052e2a9a` | Release key, certificate SHA-256 `10ab3feb74724e2e38161c8027e679438a89d3521525980fbbd796ad62faa9f8` |

**Provenance.** Commit `7f5cae49fbd278dd4a273fa4ad6908272f577a4b`, built 2026-10-27T07:23:48Z by https://github.com/jithujsam/pawse-app/actions/runs/40466713306. Tests: 13 passed (13) 35 passed (35) 394 passed (394); Android unit tests passed.

## 3.9.13 release (published to main by the publish workflow)

| Version | Code | File | SHA-256 | Signed with |
|---|---|---|---|---|
| 3.9.13 | 40 | `apk/Pawse-3.9.13.apk` (6710857 bytes) | `7045c1fb192cac43b467c2a94e7c8bbadfb2341bf7f2634c77a0feec5d0329b1` | Release key, certificate SHA-256 `10ab3feb74724e2e38161c8027e679438a89d3521525980fbbd796ad62faa9f8` |

**Provenance.** Commit `0836b429d7dbec39cb96092b5d7d37d38c8225e3`, built 2026-10-27T05:41:07Z by local build (claude session). Tests: 13 passed (schema), 29 passed (engine), 368 passed (web); Android unit tests passed.

## 3.9.12 release (published to main under the owner's standing approval)

| Version | Code | File | SHA-256 | Signed with |
|---|---|---|---|---|
| 3.9.12 | 39 | `apk/Pawse-3.9.12.apk` (6710837 bytes) | `9648ef63f7e09ffdbc1f1bb1607cd8b2717da6cc422339373ffa761a4fb89ef3` | Release key, certificate SHA-256 `10ab3feb74724e2e38161c8027e679438a89d3521525980fbbd796ad62faa9f8` |

**Provenance.** Built and signed from pawse-app `2584882` on `main`. That merge carries the widget work of 3.9.8 to 3.9.11 (from `ccr-8a2d4e37-nz8qm8`, merge `3c5f4a9`), which had not been on `main`, plus the launch-splash and update-notes scrollbar change (`5034e75`). Lint, typecheck, tests (368 web, 29 engine) and the web build passed; `./gradlew assembleRelease` passed.

**Verified on the signed file:** `apksigner` v2 signature, certificate `10ab3feb…a9f8`; `aapt2`: versionCode 39, versionName 3.9.12, not debuggable; the web bundle inside reports 3.9.12/39. Not checked on a device: the widget name labels and arrows, the launch-splash handoff and the update-notes scrollbar.

## 3.9.11 release (published to main under the owner's standing approval)

| Version | Code | File | SHA-256 | Signed with |
|---|---|---|---|---|
| 3.9.11 | 38 | `apk/Pawse-3.9.11.apk` (6710820 bytes) | `b4b7560a76d1fe219fb50c5e266de1df72ad4ee7a1d79fcc4bd1ee856cbf87c2` | Release key, certificate SHA-256 `10ab3feb74724e2e38161c8027e679438a89d3521525980fbbd796ad62faa9f8` |

**Provenance.** Built and signed from pawse-app `6359936` on the designated feature branch (`ccr-8a2d4e37-nz8qm8`), not `main`. The widgets show one pet per page: the pages slide every six seconds and the arrows step through them. Lint, typecheck and tests (368 web, 29 engine, 13 schema) and the web build passed; `./gradlew assembleRelease` passed.

**Verified on the signed file:** `apksigner` v2 signature, certificate `10ab3feb…a9f8`; `aapt2`: versionCode 38, versionName 3.9.11, not debuggable; the web bundle inside reports 3.9.11/38. Not checked on a device: the slideshow, the arrows and the widget with a PIN set.

## 3.9.10 release (published to main under the owner's standing approval)

| Version | Code | File | SHA-256 | Signed with |
|---|---|---|---|---|
| 3.9.10 | 37 | `apk/Pawse-3.9.10.apk` (6709454 bytes) | `80b9fd2ce44b0493d63251278dc9828b542493b7479d33617af7be74f8431bcf` | Release key, certificate SHA-256 `10ab3feb74724e2e38161c8027e679438a89d3521525980fbbd796ad62faa9f8` |

**Provenance.** Built and signed from pawse-app `1c467e5` on the designated feature branch (`ccr-8a2d4e37-nz8qm8`), not `main`. Adds the pet name under each pet, sent only when the app is unlocked. Lint, typecheck, tests (368 web, 29 engine, 13 schema) and the web build passed; `./gradlew assembleRelease` passed.

**Verified on the signed file:** `apksigner` v2 signature, certificate `10ab3feb…a9f8`; `aapt2`: versionCode 37, versionName 3.9.10, not debuggable; the web bundle inside reports 3.9.10/37. Not checked on a device: the name layout and colours, and the widget with a PIN set.

## 3.9.9 release (published to main under the owner's standing approval)

| Version | Code | File | SHA-256 | Signed with |
|---|---|---|---|---|
| 3.9.9 | 36 | `apk/Pawse-3.9.9.apk` (6708487 bytes) | `826017a491e1b43f9e26c474824d12e40216a2e49be6b8cb6bb70eb31064562e` | Release key, certificate SHA-256 `10ab3feb74724e2e38161c8027e679438a89d3521525980fbbd796ad62faa9f8` |

**Provenance.** Built and signed from pawse-app `a8ce9bd` on the designated feature branch (`ccr-8a2d4e37-nz8qm8`), not `main`. The widget change replaces the StackView with four fixed pet slots and removes `PetStackService`. `./gradlew assembleRelease` passed, and the web build passed. The Java widget change has no unit tests; `pnpm test` covers the web code only.

**Verified on the signed file:** `apksigner` v2 signature, certificate `10ab3feb…a9f8`; `aapt2`: versionCode 36, versionName 3.9.9, not debuggable; the web bundle inside reports 3.9.9/36; `PetStackService` is absent from the APK. Not checked on a device: the widget sizes.

## 3.9.8 release (published to main under the owner's standing approval)

| Version | Code | File | SHA-256 | Signed with |
|---|---|---|---|---|
| 3.9.8 | 35 | `apk/Pawse-3.9.8.apk` (6709342 bytes) | `34687b9bc2bc8c306bd12b6d4dcf6ce62420d7b8e8805835279ab265bc15cf88` | Release key, certificate SHA-256 `10ab3feb74724e2e38161c8027e679438a89d3521525980fbbd796ad62faa9f8` |

**Provenance.** Built and signed from pawse-app `4bdfbff`, which is `main` (`b8a3ff3`, the widget change from PR #32) plus the version bump to 3.9.8. Built on the designated feature branch, not on `main`, because the bump was not pushed to `main`. After lint, typecheck, test (368 passed) and build passed. `./gradlew assembleRelease`.

**Verified on the signed file:** `apksigner` v2 signature, certificate `10ab3feb…a9f8`; `aapt2`: versionCode 35, versionName 3.9.8, not debuggable; the web bundle inside reports 3.9.8/35. Not checked on a device: the widget sizes.

## 3.9.6 release (published to main under the owner's standing approval)

| Version | Code | File | SHA-256 | Signed with |
|---|---|---|---|---|
| 3.9.6 | 33 | `apk/Pawse-3.9.6.apk` (6,711,398 bytes) | `bdf73938be334b712d0238f785f12c70e59cb98b93c44c15f45de2d92d82f083` | Release key, certificate SHA-256 `10ab3feb74724e2e38161c8027e679438a89d3521525980fbbd796ad62faa9f8` |

**Provenance.** Built and signed from pawse-app `e338679` (main), after lint, typecheck, test (368 passed) and build passed. `./gradlew clean assembleRelease`.

**Verified on the signed file:** `apksigner` v2 signature, certificate `10ab3feb…a9f8`; `aapt2`: versionCode 33, versionName 3.9.6, not debuggable; the web bundle inside reports 3.9.6/33. The day sheet and the dropdown menus were checked in a browser. Not checked on a device: the reminders, the reused update download and the no-zoom setting.

## 3.9.5 release (published to main under the owner's standing approval)

| Version | Code | File | SHA-256 | Signed with |
|---|---|---|---|---|
| 3.9.5 | 32 | `apk/Pawse-3.9.5.apk` (6,710,094 bytes) | `8c0c6a71d69778bd8c2bbebf38c5b0ff040450eda8b73a51d6218b3548f2964d` | Release key, certificate SHA-256 `10ab3feb74724e2e38161c8027e679438a89d3521525980fbbd796ad62faa9f8` |

**Provenance.** Built and signed from pawse-app `8c90d4a` (main), after lint, typecheck, test (365 passed) and build passed. `./gradlew assembleRelease`.

**Verified on the signed file:** `apksigner` v2 signature, certificate `10ab3feb…a9f8`; `aapt2`: versionCode 32, versionName 3.9.5, not debuggable; the web bundle inside reports 3.9.5/32. The calendar sheet (editable, locked and future days), the slip form and the update pop-up were checked in a browser.

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
