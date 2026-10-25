# Release status

Updated: 2026-10-25 (final verification run)

## Current published release (unchanged)

| Version | Code | File | SHA-256 | Checked |
|---|---|---|---|---|
| 2.1.0 | 7 | `apk/Pawse-2.1.0.apk` | `c8801d33730fabf0478ad2e4a63b5f142c81688bbe01814f466d0b17532cba53` | Re-verified 2026-10-25: SHA-256 of the repo file and of the served file match `latest.json`; `apksigner` v1+v2 OK, signer `8081688b…257b`; `aapt2` code 7 / 2.1.0, not debuggable |

`latest.json` still points at 2.1.0. Nothing in `apk/` was added, removed or changed.

## Next: PAWSE 3.0 (UNRELEASED)

There is **no 3.0 APK**. The app work is merged into `pawse-app/main`:

- [jithujsam/pawse-app#14](https://github.com/jithujsam/pawse-app/pull/14) (PAWSE 3.0) and the release-readiness work from [#13](https://github.com/jithujsam/pawse-app/pull/13) were merged into `main` through [#15](https://github.com/jithujsam/pawse-app/pull/15), with continuity (no death) as the default pet rules.
- The release procedure for this repo is [`docs/RELEASING.md`](https://github.com/jithujsam/pawse-app/blob/main/docs/RELEASING.md) in the app repo. Follow it for every release.

Why no release APK yet (2026-10-25): builds now run on GitHub Actions and work (see the test build below). A **release** build needs the release signing key added to the `pawse-app` repository secrets (see `apps/web/android/keystore/README.md` there), plus device tests and the owner's approval.

### Test build (separate from releases)

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

**`apk/` and `latest.json` are deliberately unchanged.** They're the public update channel, and they only take a release-signed `app.detoxcompanion` APK (certificate `8081688b…257b`). A test build there would be offered to every 2.1.0 user, and couldn't update their app anyway. Test builds live only in `test-builds/`.

New test builds come from every push to `pawse-app/main` (Actions → Android APK). Each run's artifact holds the APK and its build info.

### Checklist for 3.0

1. [x] #13 and #14 merged to `main` (via #15) with continuity as the default pet rules. Owner to confirm that default before release.
2. [x] `pnpm test` (166/166), `pnpm typecheck` and `pnpm build` pass on `main` at `c85fe89` (run 2026-10-25)
3. [x] Supabase migrations 0004 and 0005 are in effect in production (verified read-only 2026-10-25; applied 2026-10-24 by an unconfirmed actor, not by the 2026-10-25 session; migration history still lists only the first one, so never `db push`)
3a. [ ] **OpenRouter key rotated**: the new key is in Supabase Secrets (owner). Revoke the old key once a signed-in AI call is confirmed working
3b. [x] `ai` function deployed from `main` (version 14, 2026-10-25, owner-approved): live source matches the repo, no key in it, JWT verification on, cached answers carry the user id
3c. [ ] Leaked-password protection on (verified off today)
4. [x] `apps/web/version.json` is 3.0.0 / code 8 on `pawse-app/main`
5. [ ] Release APK built and signed with the existing key (same signature, so it installs over 2.1.0 and keeps data)
6. [ ] Device tests: install over 2.1.0 and confirm the data is kept; onboarding with a plan; urge flow; slip and reflection; weekly review; notifications per day; widget with app lock on
7. [ ] SHA-256 computed from the real signed file
8. [ ] `apk/Pawse-<version>.apk` added, older APKs kept, README version table and download link updated, `latest.json` updated last

### Draft release notes (edit after testing)

> **Pawse 3.0 (unreleased).** Set your own goal: stop, cut down, or understand it first. New urge support with several ways to get through it, a calm screen after a slip, and a weekly review with one small change to try. Days you don't record no longer count for or against you, and you can mark a day as "not tracking". Your companion can still get very frail, but by default it no longer dies, and everything can heal back (classic rules are optional). Because of this, some companions will look younger after updating. Milestones now count days of care and never reset.
