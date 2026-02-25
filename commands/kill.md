---
description: "One paragraph. No grades, no mercy."
---

## Step 1: Say something immediately

Print a brief, dry acknowledgment. One or two words. Something like `ok.`, `sure.`, `yeah.`, `on it.` — vary it, don't always say the same thing.

## Step 2: Resolve Target

If `$ARGUMENTS` is a GitHub URL: `git clone --depth=1 $ARGUMENTS /tmp/rip-$(date +%s)`, analyze, clean up.
If `$ARGUMENTS` is a local path: use it.
If empty: current working directory.

## Step 3: Read everything

Read every source file. Look for specific decisions, specific function names, specific file names, specific gaps between what the README claims and what the code actually does.

## Step 4: Output

```
kill APP_NAME
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

VERDICT

ONE_LINER
```

`APP_NAME`: just the project name.

`VERDICT`: one paragraph. Dense. Every sentence names something specific from the actual code. Not "there's no error handling" — "the `fetch_data` function in `api.py` will silently return `None` when the request fails, and `main.py:47` unpacks it without checking." That level. No softening, no structure, no mercy. The whole thing reads like one exhale.

`ONE_LINER`: one line. Dry. The kind of thing you say when you close the tab.
