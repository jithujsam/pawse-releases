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

Why no APK yet (2026-10-25): the release signing key isn't in the build environment (by design); Gradle couldn't reliably download dependencies there (intermittent Maven Central failures, 5 attempts); no device tests have run; and the security steps below aren't done. Full report: `docs/PAWSE_OVERNIGHT_REPORT.md` in the app repo (section "PAWSE 3.0 final verification").

### Checklist for 3.0

1. [x] #13 and #14 merged to `main` (via #15) with continuity as the default pet rules. Owner to confirm that default before release.
2. [x] `pnpm test` (166/166), `pnpm typecheck` and `pnpm build` pass on `main` at `c85fe89` (run 2026-10-25)
3. [x] Supabase migrations 0004 and 0005 are in effect in production (verified read-only 2026-10-25; applied 2026-10-24 by an unconfirmed actor, not by the 2026-10-25 session; migration history still lists only the first one, so never `db push`)
3a. [ ] **OpenRouter key rotated** (old key was in deployed source; not rotated yet)
3b. [ ] `ai` function deployed from `main` (the deployed version 12 predates the per-user cache and the no-in-source-key fix); JWT verification stays on (verified on today)
3c. [ ] Leaked-password protection on (verified off today)
4. [ ] `apps/web/version.json` bumped to 3.0.0 / code 8: in review (pawse-app branch `ccr-ea60e25f-6gxd74`), not on `main` yet
5. [ ] Release APK built and signed with the existing key (same signature, so it installs over 2.1.0 and keeps data)
6. [ ] Device tests: install over 2.1.0 and confirm the data is kept; onboarding with a plan; urge flow; slip and reflection; weekly review; notifications per day; widget with app lock on
7. [ ] SHA-256 computed from the real signed file
8. [ ] `apk/Pawse-<version>.apk` added, older APKs kept, README version table and download link updated, `latest.json` updated last

### Draft release notes (edit after testing)

> **Pawse 3.0 (unreleased).** Set your own goal: stop, cut down, or understand it first. New urge support with several ways to get through it, a calm screen after a slip, and a weekly review with one small change to try. Days you don't record no longer count for or against you, and you can mark a day as "not tracking". Your companion can still get very frail, but by default it no longer dies, and everything can heal back (classic rules are optional). Because of this, some companions will look younger after updating. Milestones now count days of care and never reset.
