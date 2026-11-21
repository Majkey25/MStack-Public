---
name: playwright
description: Automate a browser flow with Playwright for reproduction, functional verification, or a regression test. Use when a task needs repeatable browser interactions or cross-browser checks.
license: Apache-2.0
---

# Playwright

Use the project's Playwright version, configuration, and supported runner. Identify the exact scenario and expected outcome. Use a clean browser context and test data the flow can safely create or change.

- Select by role, label, or other stable user-facing properties. Assert what the user observes, then check network or storage behavior only when relevant to the claim.
- Use Playwright's retrying assertions and wait for the condition the user cares about. Avoid fixed sleeps and test order dependencies. Register response or download waits before the action that triggers them.
- Capture a trace or screenshot when it clarifies a failure. Sanitize artifacts before sharing them. Keep production changes and account writes within the task's authority.

Run the focused scenario. Report the test command, browser or project, and the outcome. If the browser runner is unavailable, state which verification is still open.

See [Playwright documentation](https://playwright.dev/docs/intro) for current runner and locator APIs.

Adapted from [OpenAI's Playwright skill](https://github.com/openai/skills/tree/49f948faa9258a0c61caceaf225e179651397431/skills/.curated/playwright). MStack replaced the upstream wrapper and bundled usage guides with instructions for the project's Playwright runner.
