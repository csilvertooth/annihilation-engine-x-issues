# Security Policy

Thank you for caring about the security of AEX Unit Editor and AEX Map
Editor. This repository is the public issue tracker; the engine and
editor source code are proprietary and live in a private repository.

## Reporting a vulnerability

**Please do not file public issues for security vulnerabilities.**
Issues filed in this repository are visible to everyone, which would
expose the problem to attackers before a fix is available.

Instead, use one of these private channels:

1. **GitHub Security Advisories** (preferred): open a private advisory
   at <https://github.com/csilvertooth/annihilation-engine-x-issues/security/advisories/new>.
   GitHub keeps the report private between you and the maintainers
   until a fix and CVE (if applicable) are coordinated.

2. **Email**: <chris@azimuthsystems.net>. Use the subject line
   `[AEX SECURITY]` so it routes correctly. PGP encryption is not
   required but is welcomed if you prefer; mention you have a key and
   I'll arrange an exchange.

I aim to acknowledge reports within **72 hours** and to ship a fix or
mitigation within **30 days** for verified high-severity issues.
Smaller or lower-impact findings are still welcome; their timeline is
case-by-case.

## Scope

In scope:

- The shipped AEX Unit Editor and AEX Map Editor binaries (macOS DMG /
  Windows EXE published to <https://aex-public-files.s3.us-west-2.amazonaws.com/aex-unit/>
  and <https://aex-public-files.s3.us-west-2.amazonaws.com/aex-mapedit/>).
- The auto-update infrastructure (the `latest-*.yml` manifests and
  `.blockmap` artifacts served from the same prefixes).
- The C++ headless backend (`aex_unitview_ipc` / `aex_mapedit_ipc`)
  packaged in those binaries, including its IPC protocol over stdio.

Out of scope:

- Bugs that only affect a self-built copy of the engine or editor.
- Issues that require physical or local-user-level access to a machine
  already running the application (e.g. the user can already write
  arbitrary files anywhere, or already has the user's session token).
- Third-party services we depend on (GitHub, AWS S3, Google Workspace);
  please report those to the relevant vendor.

## Safe-harbour intent

If you make a good-faith effort to comply with this policy when
researching and reporting an issue, I will not pursue legal action
against you for that research. This is an informal statement and not
legal contract language; the goal is simply: research responsibly,
report privately, and we'll work it through together.

## Acknowledgments

Reporters who help us fix verified security issues are welcome to be
credited in release notes or in this file's history (or to stay
anonymous — your choice).
