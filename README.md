# Open Source Contributions

A curated record of my contributions to open-source projects — including bug fixes, compatibility improvements, build and packaging cleanup, tests, and community collaboration.

I'm a Computer Science student focused on backend development with .NET. I enjoy learning from real-world codebases, investigating issues, and contributing focused fixes that make software more reliable.

## Contributions

| Project | Contribution | Status |
|---|---|---|
| [TUnit](https://github.com/thomhurst/TUnit) | [PR #7234 — Remove legacy JSON output implementation](https://github.com/thomhurst/TUnit/pull/7234) | **Merged** |
| [Beekeeper Studio](https://github.com/beekeeper-studio/beekeeper-studio) | [PR #4883 — Handle unavailable Redis MEMORY USAGE on older servers](https://github.com/beekeeper-studio/beekeeper-studio/pull/4883) | **Merged** |
| [SkiaSharp](https://github.com/mono/SkiaSharp) | [PR #5403 — Remove obsolete libmicrohttpd notice](https://github.com/mono/SkiaSharp/pull/5403) | **Open** |
| [sbox-public](https://github.com/Facepunch/sbox-public) | [Issue #12157 — Discussion about project defaults and shader-related files](https://github.com/Facepunch/sbox-public/issues/12157#issuecomment-6291251506) | Discussion |

---

## Selected work

### TUnit — Legacy JSON output removal

**[PR #7234](https://github.com/thomhurst/TUnit/pull/7234) · Merged**

Removed an unused legacy JSON output implementation after discussion with the project maintainer.

- Removed the unused JSON output command-line provider.
- Deleted obsolete JSON serialization models and extensions.
- Removed skipped JSON output tests and documentation for unsupported JSON flags.
- Removed 328 lines across 11 files.
- Validation reported in the PR: engine build passed; engine tests passed (**573 passed, 0 failed, 346 skipped**).

Related issue: [TUnit #7201](https://github.com/thomhurst/TUnit/issues/7201).

### Beekeeper Studio — Redis compatibility fix

**[PR #4883](https://github.com/beekeeper-studio/beekeeper-studio/pull/4883) · Merged**

Fixed key loading for older Redis servers where the `MEMORY USAGE` command is unavailable.

- Made memory usage optional so an unsupported command doesn't prevent the keys table from loading.
- Updated the TypeScript type to allow `number | null`.
- Added tests for both unsupported and supported `MEMORY USAGE` responses.
- Verified behavior with Redis 3 and Redis 7, and ran the relevant unit tests and lint checks.

Related issue: [#4882](https://github.com/beekeeper-studio/beekeeper-studio/issues/4882).

### SkiaSharp — Dependency notice cleanup

**[PR #5403](https://github.com/mono/SkiaSharp/pull/5403) · Open**

Removed an obsolete `libmicrohttpd` license-notice section after the dependency had already been removed.

- Kept the change focused on generated third-party notice accuracy; no source-code or public-API changes.
- Ran `git diff --check`.
- Packed the Linux native-assets project and checked that the generated notice no longer includes `libmicrohttpd` while retaining `libwebp`.
- This was a targeted content check, not a full native-assets packaging validation.

### Facepunch s&box — Community discussion

**[Issue #12157](https://github.com/Facepunch/sbox-public/issues/12157#issuecomment-6291251506)**

Participated in a discussion concerning default project `.gitignore` behavior and shader-related files. This is issue/community participation, not a pull request.

---

## Skills demonstrated

- Reading and navigating unfamiliar codebases
- Debugging compatibility issues and identifying unused code paths
- Writing focused regression tests
- Build and test validation
- Build and packaging verification
- Keeping changes scoped and documenting validation
- Communicating with maintainers and contributing to issue discussions

## Contribution log

I'll add new entries as I make further contributions. Each entry links to the original PR or issue and identifies its current status.

- **Merged** — accepted and merged into the upstream project.
- **Open** — submitted and awaiting review or a final decision.
- **Discussion** — issue comments or community participation; not a code merge.

## Links

- [GitHub profile](https://github.com/Saad-elnagar)
- [Inventory Management project](https://github.com/Saad-elnagar/InventoryManagement)
