# Release status

Updated: 2026-10-25

## Current published release (unchanged)

| Version | Code | File | SHA-256 | Checked |
|---|---|---|---|---|
| 2.1.0 | 7 | `apk/Pawse-2.1.0.apk` | `c8801d33730fabf0478ad2e4a63b5f142c81688bbe01814f466d0b17532cba53` | Recomputed 2026-10-24; matches `latest.json` |

`latest.json` still points at 2.1.0. Nothing in `apk/` was added, removed or changed.

## Next: PAWSE 3.0 (UNRELEASED)

There is **no 3.0 APK**. The app work is merged into `pawse-app/main`:

- [jithujsam/pawse-app#14](https://github.com/jithujsam/pawse-app/pull/14) (PAWSE 3.0) and the release-readiness work from [#13](https://github.com/jithujsam/pawse-app/pull/13) were merged into `main` through [#15](https://github.com/jithujsam/pawse-app/pull/15), with continuity (no death) as the default pet rules.
- The release procedure for this repo is [`docs/RELEASING.md`](https://github.com/jithujsam/pawse-app/blob/main/docs/RELEASING.md) in the app repo. Follow it for every release.

Why no APK yet: the build environment couldn't download Android build dependencies (Maven Central returned HTTP 429), the release signing key isn't available there by design, and no device tests have run.

### Checklist for 3.0

1. [x] #13 and #14 merged to `main` (via #15) with continuity as the default pet rules. Owner to confirm that default before release.
2. [x] `pnpm test` (166/166), `pnpm typecheck` and `pnpm build` pass on `main` at `c85fe89` (run 2026-10-25)
3. [ ] Supabase: migrations 0004 and 0005 applied, `ai` function deployed (the app works without them, but urge strategies won't sync and the AI cache won't write)
4. [ ] `apps/web/version.json` bumped (name and a code above 7)
5. [ ] Release APK built and signed with the existing key (same signature, so it installs over 2.1.0 and keeps data)
6. [ ] Device tests: install over 2.1.0 and confirm the data is kept; onboarding with a plan; urge flow; slip and reflection; weekly review; notifications per day; widget with app lock on
7. [ ] SHA-256 computed from the real signed file
8. [ ] `apk/Pawse-<version>.apk` added, older APKs kept, README version table and download link updated, `latest.json` updated last

### Draft release notes (edit after testing)

> **Pawse 3.0 (unreleased).** Set your own goal: stop, cut down, or understand it first. New urge support with several ways to get through it, a calm screen after a slip, and a weekly review with one small change to try. Days you don't record no longer count for or against you, and you can mark a day as "not tracking". Your companion can still get very frail, but by default it no longer dies, and everything can heal back (classic rules are optional). Because of this, some companions will look younger after updating. Milestones now count days of care and never reset.
