# Open Source Contributions

A curated record of my contributions to open-source projects — including bug fixes, compatibility improvements, build and packaging cleanup, tests, and community collaboration.

I'm a Computer Science student focused on backend development with .NET, and I enjoy learning from real-world codebases, investigating issues, and contributing fixes that make software more reliable.

## Contributions

| Project | Contribution | Status |
|---|---|---|
| [Beekeeper Studio](https://github.com/beekeeper-studio/beekeeper-studio) | [PR #4883 — Handle unavailable Redis MEMORY USAGE on older servers](https://github.com/beekeeper-studio/beekeeper-studio/pull/4883) | **Merged** |
| [SkiaSharp](https://github.com/mono/SkiaSharp) | [PR #5403 — Remove obsolete libmicrohttpd notice](https://github.com/mono/SkiaSharp/pull/5403) | **Open** |
| [sbox-public](https://github.com/Facepunch/sbox-public) | [Issue #12157 — discussion about project defaults and shader-related files](https://github.com/Facepunch/sbox-public/issues/12157#issuecomment-6291251506) | Discussion |

---

## Selected work

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

Participated in a discussion concerning default project `.gitignore` behavior and shader-related files. This is listed as issue/community participation, not as a pull request.

---

## Skills demonstrated

- Reading and navigating unfamiliar codebases
- Debugging compatibility issues
- Writing focused regression tests
- Type-safe handling of optional data
- Build and packaging verification
- Keeping changes scoped and documenting validation
- Communicating with maintainers and contributing to issue discussions

## Contribution log

I’ll add new entries as I make further contributions. Each entry should link to the original PR or issue and clearly identify its current status.

- **Merged** — accepted and merged into the upstream project.
- **Open** — submitted and awaiting review or a final decision.
- **Discussion** — issue comments or community participation; not a code merge.

## Links

- [GitHub profile](https://github.com/Saad-elnagar)
- [Inventory Management project](https://github.com/Saad-elnagar/InventoryManagement)
