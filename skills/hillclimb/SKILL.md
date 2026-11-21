---
name: hillclimb
description: Improve a measurable result through experiments, regression checks, and fresh evidence. Use when asked to iterate toward a target, persist through a difficult task, or improve visual quality against an explicit rubric.
license: MIT
---

# Hillclimb

## Define success

- Record the target, baseline, comparison conditions, and behavior that must keep working. Use the user's threshold. If they leave it open, use a testable outcome grounded in the task.
- Reproduce the reported issue or measure the starting result. Check that the measurement distinguishes a meaningful improvement from noise. Keep workload, inputs, measurement method, and relevant resources comparable.
- When the user asks for a persistent goal and the agent supports one, use its documented goal mechanism. Preserve unrelated active goals. Otherwise keep a short checkpoint in the current run or an approved scratch location.

## Run experiments

1. Pick the hypothesis with the best evidence. Change one thing, or one set of changes that must work together.
2. Measure the new result and run the regression checks. For variable results, repeat enough to tell noise from improvement. If comparison conditions changed, take a new baseline and record why.
3. Keep a verified improvement. Discard only your own unsuccessful changes when safe. Record the hypothesis, measured result, regressions, and decision.
4. When progress stalls, use what failed to choose a different approach. Fix recoverable blockers and continue while a permitted experiment can materially advance the goal.

## Visual work

Use a real browser when visual success matters. Compare the baseline and latest revision with the same viewport, content, and interaction state. Cover relevant small and large widths, keyboard paths, and failure states. Recheck screenshots and behavior after changes that affect them.

When the user wants independent judging, give reviewers the same rubric and the current evidence they are authorized to see. Apply each threshold at the level the user specified. Every required criterion and reviewer gate must pass. A score with missing evidence, an outdated screenshot, or a timed out required review leaves that gate open. Substitute a reviewer only when the user's criteria allow it.

## Stop

Finish when the latest revision meets the target and its regression gates pass. Respect the user's stop, permissions, and runtime limits. When a required check is blocked, report the best verified result, the open gate, and what could unblock it. For an unsolved problem, label partial results and unproved steps.

The experiment loop draws on [PStack’s Hillclimb playbook](https://github.com/cursor/plugins/blob/2f87c854fe3e2fcda44ca86b46ede35aad3c46b7/pstack/skills/poteto-mode/playbooks/hillclimb.md).
