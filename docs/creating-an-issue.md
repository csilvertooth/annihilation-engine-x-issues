# How to Create an Issue

This tracker covers the **AEX Unit Editor** and **AEX Map Editor** only. The
core engine is private and is not tracked here.

## 1. Search first

Before filing, search existing issues to avoid duplicates:

- Open the [Issues tab](https://github.com/csilvertooth/annihilation-engine-x-issues/issues)
- Search by keyword. Include closed issues — your problem may already be fixed
  or planned.
- If you find a match, add a 👍 reaction or a comment with new details instead
  of opening a new issue.

## 2. Open the new-issue page

- Go to **Issues → New issue**, or
- Direct link: <https://github.com/csilvertooth/annihilation-engine-x-issues/issues/new/choose>

Blank issues are disabled — you must pick a form so reports stay consistent.

## 3. Pick the right form

| You want to… | Use this form |
|---|---|
| Report something broken in the Unit Editor | **Unit Editor Bug** |
| Suggest a Unit Editor capability | **Unit Editor Feature** |
| Report something broken in the Map Editor | **Map Editor Bug** |
| Suggest a Map Editor capability | **Map Editor Feature** |
| Share workflow / UX feedback or anything else | **General AEX Feedback** |

## 4. Fill in the form

The title prefix (e.g. `[Unit Editor Bug]:`) is added for you — just complete
the rest of the title with a short, specific summary.

**Good title:** `[Map Editor Bug]: Brush size resets to 1 after switching tabs`
**Weak title:** `[Map Editor Bug]: broken`

For **bug** reports, the form asks for:

- **Bug Description** — what went wrong, in one or two sentences.
- **Steps To Reproduce** — a numbered list someone else can follow exactly:
  1. Open the Map Editor
  2. Load map `Foo`
  3. Select the height brush, set size to 5
  4. Switch to the Features tab and back
  5. Brush size is now 1
- **Expected Behavior** — what you expected instead.
- **Screenshots or Logs** — drag images straight into the box. Paste log text
  inside triple backticks so it stays readable.

For **feature** requests, the form asks for:

- **Feature Description** — what you want, concretely.
- **Why Is This Useful?** — the problem it solves or the workflow it improves.

## 5. Submit

Click **Submit new issue**. The form automatically applies area/type labels and
`status: needs-triage`. A maintainer will triage it and update the labels
(`status: accepted`, `planned`, `blocked`, etc.) — you don't need to set
labels yourself.

## What not to post

Per the [README](../README.md) and [SECURITY](../SECURITY.md):

- ❌ Proprietary source code or engine internals
- ❌ Credentials, tokens, or secrets
- ❌ Security-sensitive implementation details (report those privately)
- ❌ Paid or private game assets

## After filing

- Watch for follow-up questions and respond — issues that can't be reproduced
  may be closed.
- Link related work or duplicates by referencing the issue number (`#12`).
- See the per-editor roadmap/tracking issues for what's already planned:
  [Unit Editor](https://github.com/csilvertooth/annihilation-engine-x-issues/issues/2)
  · [Map Editor](https://github.com/csilvertooth/annihilation-engine-x-issues/issues/3)
