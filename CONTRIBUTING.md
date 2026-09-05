# Contributing to this repo

Thank you for contributing. These guidlines are written for someone making their very first pull request.

## The one rule

Open every pull request against `dev`. Never against `main`. `dev` is where work integrates, `main` is the protected production branch.

## Before you start

1. Create a GitHub account and install git.
2. Set your identity in git, once:

```bash
git config --global user.name "Your Name"
git config --global user.email "you@example.com"
```

3. Read the README so you know what this repo is.
4. Pick one open issue and claim it by commenting on it: "I will take this one." One issue, one owner.

## The contribution steps

Follow these eight steps and you will have a pull request open.

1. Fork the repository to your own account. The Fork button is at the top right of the repo page.
2. Clone your fork:

```bash
git clone https://github.com/YOUR-USERNAME/bte-build-sessions.git
cd bte-build-sessions
```

3. Branch from the latest `dev`:

```bash
git fetch upstream
git checkout -b docs/fix-readme-typo upstream/dev
```

If `upstream` is not set yet, add it first:

```bash
git remote add upstream https://github.com/E-Timileyin/bte-build-sessions.git
```

4. Make the change the issue describes. Keep it small. One issue, one branch.
5. Stage and commit with a clear message that starts with a type:

```bash
git add README.md
git commit -m "docs: fix the typo in the welcome paragraph"
```

6. Push your branch to your fork:

```bash
git push -u origin docs/fix-readme-typo
```

7. On GitHub, open the pull request. Base repository: `E-Timileyin/bte-build-sessions`, base branch: `dev`. Compare: your fork and your branch.
8. Fill in the pull request template and link the issue you claimed.

If you do not have git installed, everything above works from the GitHub website: open the file, click the pencil to edit, GitHub offers to fork, write a commit message in the same `docs: ...` style, propose the change, and set the base branch to `dev`.

## Commit message rules

- Start with a type: `feat`, `fix`, `docs`, `chore`, `refactor`, `test`, `ci`.
- Then a short sentence about why, not a list of files.
- `docs: fix the typo in the welcome paragraph` is good. `update` is not.

## What happens after you open the pull request

1. A human reads your diff and either approves or leaves comments.
2. If there are comments, push fixes to the same branch. The pull request updates in place.
3. Merge happens when the change is approved. You do not merge your own pull request.
4. After merge, delete the branch when GitHub offers.

## House style

- Full sentences. Sentence case for headings and buttons.
- No em dashes anywhere. Use a comma, a full stop, or a rewrite.
- Plain and direct. "Fix the spelling" beats "rectify orthographic discrepancies".

When you are comfortable here, the real platform repo, bte-campus-app, uses this same flow with automated checks and a stricter review on top.
