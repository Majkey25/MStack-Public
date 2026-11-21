---
name: repo-onboarding
description: Build a day-one guide to an unfamiliar codebase. Use when asked how a repository works, how to run it, where to make a first change, or which checks contributors use.
license: MIT
---

# Repo onboarding

Start with what the newcomer needs to do. If they name a service, package, or contributor task, scope the guide to that path.

1. Read the repository instructions, README, manifests, lockfiles, task definitions, and CI. Identify the from-clone prerequisites and commands the repository currently uses.
2. Trace one representative workflow from its actual entrypoint through the main code it calls and the data it reads or writes. Identify external services and configuration boundaries along that path.
3. Find the focused tests for that workflow. Identify which checks are required by CI and which are optional. When accessible and relevant, use recent issues and pull requests to explain active pitfalls.
4. Cross-check commands against their definitions. Run harmless setup or test checks only when the environment is suitable and the task authorizes them. Mark commands read from source separately from commands actually run.

## Deliver the guide

- Open with what the app does and the quickest supported way to see it work.
- Give prerequisites and copyable commands in order. Link a sample config if one exists. Use placeholders for secrets. Name any missing access, seed data, or setup step.
- Map the main workflow using specific files and symbols. Show the first file to open and a nearby test.
- Give one bounded first change a newcomer can make and the check that would prove it works.
- Link repository-relative paths. Name uncertain setup steps and architecture claims as such.
