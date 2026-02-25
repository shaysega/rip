---
description: "Grades A-F. What's broken and how to fix it."
---

## Step 1: Acknowledge immediately

Before reading anything, print: `let me look at this.`

## Step 2: Resolve Target

If `$ARGUMENTS` is provided:
- If it looks like a GitHub URL: `git clone --depth=1 $ARGUMENTS /tmp/rip-$(date +%s)`, analyze that dir, clean up after.
- Otherwise: local path.

If `$ARGUMENTS` is empty: current working directory.

## Step 3: Analyze

Read in order: README, package.json / pyproject.toml / Cargo.toml / go.mod, entry points (main.py, app.py, index.js, index.ts, server.py), largest source files, Dockerfile.

Skip: node_modules, .git, __pycache__, .venv, dist, build, .next, lock files, binary files, .env files.

Form two assessments:
- **Code quality**: architecture, engineering judgment, security, dependency choices. Specific — name files and patterns.
- **Product/concept**: is the problem real, does this solution make sense, will anyone use it.

## Step 4: Output

```
roast APP_NAME
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

Architecture        GRADE
Code Quality        GRADE
Security            GRADE
Product Concept     GRADE

Why it's broken:
SPECIFIC_PROBLEMS

What you should actually do:
- FIX_1
- FIX_2
- FIX_3

ONE_LINER
```

Tone: honest, direct, a little tired of seeing the same mistakes. Not mean for the sake of it — just not softening anything. Grade honestly. F is not rare. The fixes should be concrete enough to act on.
