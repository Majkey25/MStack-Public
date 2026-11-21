---
name: incremental-implementation
description: Implement a multi-part change in small runnable slices. Use when a feature crosses layers, needs migration or rollout, or can be verified progressively.
license: MIT
---

# Incremental implementation

Identify the smallest slice that delivers or proves behavior through a real entry point. State its acceptance check and the behavior existing callers rely on. Prefer a slice that exercises an important dependency or unknown early.

1. Capture the current behavior with an existing test, reproduction, or request.
2. Implement the slice across the layers it needs. Reuse stable contracts and preserve behavior for callers outside the slice. Separate migrations that must remain compatible during rollout.
3. Run the focused check through the entry point. Fix failures before layering on more changes. Keep partial work isolated when it would break users.
4. Pick the next slice from current evidence. Finish by checking the full requested path, error cases the change introduced, and the project's required checks.

Keep commits, feature flags, and rollout steps aligned with the repository and the task's authority.
