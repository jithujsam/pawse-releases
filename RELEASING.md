# Maintaining this repository

This repository is how Pawse reaches phones. The app reads `latest.json` from `main` on every launch and offers whatever it points to. **Merging into `main` publishes a release.**

## Rules
- Only a **signed release APK** goes in `apk/`: built from reviewed `pawse-app/main`, with tests, typecheck and build passing and device tests done. Never a debug, unsigned or unverified build.
- `latest.json`, the APK filename, the README download link, the Versions table and the SHA-256 line all describe **the same file**. Checksums and sizes are measured from that file, never typed from memory.
- The new version `code` must be **higher** than the one published. Never replace an existing APK; older ones stay.
- Changes come as a PR from a branch. The owner reviews and merges, because merging is the release.

## How to release
Follow the full procedure in the app repo: [`docs/RELEASING.md`](https://github.com/jithujsam/pawse-app/blob/main/docs/RELEASING.md). It covers the gate, the build, artifact verification commands, the exact `latest.json` and README edits, a consistency check, and post-publish verification.

## Status
| | |
|---|---|
| Published | **2.1.0** (code 7), `apk/Pawse-2.1.0.apk`, SHA-256 `c8801d33730fabf0478ad2e4a63b5f142c81688bbe01814f466d0b17532cba53`. Checked 2026-10-24: the file hash matches `latest.json` and the README; it's signed with the release key (certificate SHA-256 `80:81:68:8B:…:25:7B`); its bundled version is 2.1.0/7. The source commit wasn't recorded. |
| Next | **Unreleased.** The changes in [pawse-app#13](https://github.com/jithujsam/pawse-app/pull/13) still need review and merge, production setup, a signed build and device tests. No new APK has been built. |
