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
The current published release and the next release's checklist are kept in [`RELEASE_STATUS.md`](RELEASE_STATUS.md).
