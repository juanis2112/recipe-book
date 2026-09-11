# Contributing to Community Recipe Book

Thank you for wanting to contribute! This guide will walk you through everything you need to get started.

---

## Table of Contents

1. [Finding an Issue](#1-finding-an-issue)
2. [Fork the Repository](#2-fork-the-repository)
3. [Clone Your Fork](#3-clone-your-fork)
4. [Set Up the Upstream Remote](#4-set-up-the-upstream-remote)
5. [Create a Branch](#5-create-a-branch)
6. [Make Your Changes](#6-make-your-changes)
7. [Commit Your Changes](#7-commit-your-changes)
8. [Push and Open a Pull Request](#8-push-and-open-a-pull-request)

---

## 1. Finding an Issue

Browse the [Issues tab](../../issues) to find something to work on.

- Issues tagged **`good first issue`** are ideal for first-time contributors.
- Issues tagged **`help wanted`** are tasks the maintainers would love community help with.
- Comment on the issue to let others know you're working on it!

---

## 2. Fork the Repository

Click the **Fork** button at the top-right of this page. This creates your own copy of the repo under your GitHub account.

---

## 3. Clone Your Fork

Clone your fork to your local machine. Replace `YOUR-USERNAME` with your GitHub username:

```bash
git clone https://github.com/YOUR-USERNAME/recipe-book.git
cd recipe-book
```

---

## 4. Set Up the Upstream Remote

Add the original repository as a remote called `upstream`. This lets you pull in future updates from the main project:

```bash
git remote add upstream https://github.com/ORIGINAL-OWNER/recipe-book.git
```

Verify your remotes look right:

```bash
git remote -v
```

You should see both `origin` (your fork) and `upstream` (the original).

---

## 5. Create a Branch

Never work directly on `main`. Create a new branch for your change:

```bash
git checkout -b your-branch-name
```

Use a descriptive branch name, for example:
- `fix/pancake-typo`
- `add/chocolate-cake-recipe`
- `update/smoothie-ingredients`

---

## 6. Make Your Changes

Edit the relevant file(s). For example, if you're fixing a typo in a recipe, open the file and make your edit.

Keep changes focused — one issue per branch/PR makes review much easier.

---

## 7. Commit Your Changes

First, check which files were modified:

```bash
git status
```

Then stage only the file(s) relevant to your change — avoid staging files you didn't intentionally edit:

```bash
git add path/to/your-file.md
git commit -m "fix: correct typo in pancakes recipe

The word 'buttermilk' was misspelled as 'buttermlik' in the
ingredients list of recipes/pancakes.md.

Closes #3"
```

### Commit Message Format

We follow this structure:

```
<type>: <short summary>

<optional longer description>

<optional issue reference>
```

**Types:**
| Type | When to use |
|------|-------------|
| `feat` | Adding a new recipe or feature |
| `fix` | Fixing a typo or bug |
| `docs` | Updating documentation |
| `chore` | Maintenance tasks |

---

## 8. Push and Open a Pull Request

Push your branch to your fork:

```bash
git push origin your-branch-name
```

Then go to your fork on GitHub. You'll see a prompt to **"Compare & pull request"** — click it!

### Writing a Good PR Description

- Describe **what** you changed and **why**
- Reference the issue it closes: `Closes #<issue number>`
- Keep it short and clear

---

## Questions?

If you get stuck, leave a comment on the issue or open a Discussion. We're happy to help!
