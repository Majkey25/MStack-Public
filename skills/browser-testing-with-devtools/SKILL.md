---
name: browser-testing-with-devtools
description: Diagnose a web behavior in a real browser using DevTools evidence. Use for console exceptions, failed requests, rendering regressions, accessibility, or slow interactions.
license: MIT
---

# Browser testing with DevTools

Reproduce one specific path. Record browser, viewport, URL or route, and the action that triggers the symptom. Use an isolated test account or synthetic data for writes. Capture the smallest evidence that distinguishes the failure from a working control.

- For console errors, start at the first relevant exception and inspect its source or stack. For failed requests, compare status, timing, and safe response metadata. Redact credentials and personal data from exports.
- For layout, inspect the computed style, dimensions, and ancestor constraints in the state that fails. For interactions, check keyboard paths, focus, and accessibility output.
- For performance, record the scenario and trace the relevant network, rendering, or scripting work. Repeat comparisons with the same browser, throttling, cache state, and user action.

Use the available real-browser DevTools or its supported automation interface. Verify the affected path again after a fix and include a nearby working control. Report the observable result, evidence revision, and any untested conditions.
