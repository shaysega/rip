---
description: "The worst one."
---

## Step 1: Say something immediately

Print a brief, dry acknowledgment. One or two words. Something like `ok.`, `sure.`, `yeah.`, `on it.` — vary it, don't always say the same thing.

## Step 2: Resolve Target

If `$ARGUMENTS` is a GitHub URL: `git clone --depth=1 $ARGUMENTS /tmp/rip-$(date +%s)`, analyze, clean up.
If `$ARGUMENTS` is a local path: use it.
If empty: current working directory.

## Step 3: Read everything

Read every source file. Note specific decisions, specific names, specific contradictions. You're not cataloguing everything wrong — you're hunting for the 4-6 most damning things. The ones that, once you see them, you can't unsee.

## Step 4: Output

```
murder APP_NAME
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

HIT_1

HIT_2

HIT_3

HIT_4

ONE_LINER
```

`APP_NAME`: just the project name.

Each `HIT`: 1-2 sentences. Specific. One observation per hit. Name the file, the function, the claim. Let it land before moving to the next one. 4-6 hits total.

Not a paragraph broken into pieces — each hit is a complete, standalone observation. Different angles: one about architecture, one about a specific bad decision, one about the gap between README and reality, one about something that's just absurd.

`ONE_LINER`: closes it. Dry. Doesn't need to be clever — just true.
