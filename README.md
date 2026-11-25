[![make.fun · u-deysumbrella-worst-fix-ever-funniest-commit-message-3f1d9722](https://make.fun/badge/u-deysumbrella-worst-fix-ever-funniest-commit-message-3f1d9722.svg)](https://make.fun/bounty/u-deysumbrella-worst-fix-ever-funniest-commit-message-3f1d9722?utm_source=github&utm_medium=readme&utm_campaign=worst-fix-commit)
[![rank](https://make.fun/badge/u-deysumbrella-worst-fix-ever-funniest-commit-message-3f1d9722/iqbalbeladaz/worst-fix-commit/rank.svg)](https://make.fun/bounty/u-deysumbrella-worst-fix-ever-funniest-commit-message-3f1d9722/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=worst-fix-commit)
[![reward](https://make.fun/badge/u-deysumbrella-worst-fix-ever-funniest-commit-message-3f1d9722/iqbalbeladaz/worst-fix-commit/reward.svg)](https://make.fun/bounty/u-deysumbrella-worst-fix-ever-funniest-commit-message-3f1d9722?utm_source=github&utm_medium=readme&utm_campaign=worst-fix-commit)

# Worst Fix Ever: Funniest Commit Message

My entry for the make.fun bounty `u-deysumbrella-worst-fix-ever-funniest-commit-message-3f1d9722`
("Worst Fix Ever: Funniest Commit Message", $2). One line: the commit
message for a bug fix that made everything worse.

## The line

> fix: fixed the crash by deleting the feature that kept crashing

Why this line: it reads like a real commit subject a tired engineer
would type at the end of a bad day, and the irony is specific — the
repair cured the crash by removing the very thing users were crashing
on. No revert, no "tested in production", just the fix eating its own
feature.

## How it works

- `main.py` — the program the harness runs (Python 3.13, standard
  library only, no network). It writes the line above, byte for byte,
  to `$MAKEFUN_OUTPUT_DIR/entry.txt`, defaulting to `/output/entry.txt`.
  Deterministic: two runs write identical bytes.

## Try it locally

```sh
MAKEFUN_OUTPUT_DIR=/tmp/out python3 main.py && cat /tmp/out/entry.txt
```
