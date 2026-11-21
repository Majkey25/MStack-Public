---
name: modern-web-guidance
description: Find current web platform guidance and choose compatible HTML, CSS, or browser APIs. Use when building or modernizing UI, accessibility, forms, motion, or performance.
license: Apache-2.0
---

# Modern Web Guidance

Translate the request into one browser capability at a time. Search for “dismiss a modal with Escape” or “size a grid by container width”. Keep private product names, paths, and data out of external searches.

1. Read the target browser support policy, existing UI primitives, and acceptance criteria. Find the matching use case in the [Modern Web Guidance catalog](https://github.com/GoogleChrome/modern-web-guidance). When the official CLI is already installed, use `modern-web-guidance search "<query>"` and `modern-web-guidance retrieve "<id>"`. The catalog and public browser docs work without the CLI.
2. Check relevant compatibility data in [MDN](https://developer.mozilla.org/) or [Baseline](https://web.dev/baseline). Compare the feature with the actual support policy. Choose the native primitive when it covers the behavior and existing architecture. Add a fallback or use a broadly supported alternative when needed.
3. Verify the behavior in the affected browsers and states. For layout check content at representative widths. For interactions test keyboard, focus, and failure states. For performance compare the same workload and record any missing measurements.
4. Report the source, the specific decision it informed, and what the current test established. If a guide refers to a different environment or version, say how that affects the decision.

For a broad modernization request, first inventory candidate changes. Test each proposed replacement against the existing behavior and browser support before changing it.

Adapted from [GoogleChrome/modern-web-guidance](https://github.com/GoogleChrome/modern-web-guidance/tree/64a6d708f5a43f2cd3fde5d4d7db3905ba1bdf65). MStack makes CLI use optional and scopes the lookup to the requested work.
