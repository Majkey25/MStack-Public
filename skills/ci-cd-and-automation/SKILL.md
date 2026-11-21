---
name: ci-cd-and-automation
description: Design or repair CI checks, build automation, and deployment workflows. Use for pipeline failures, new quality gates, or unreliable releases.
license: MIT
---

# CI, CD, and automation

Read existing workflow definitions, manifests, lockfiles, and a failed or successful run for the relevant revision. Find the real runner, environment, event, and command. Reproduce the failing step with equivalent inputs when practical.

- Keep gates tied to a risk or contract. Use repository-owned commands, deterministic dependency versions, and clear failure output. Run equivalently scoped checks before changing caches or concurrency.
- Identify each workflow's triggers, required permissions, and artifacts. Keep secrets in the platform's secret store. Treat pull request text and code as untrusted inputs before adding privileged events or jobs.
- Trace deployments from the requested branch or artifact to the destination and confirmation signal. Preserve environment protections. Execute external writes or a production rollout only with authorization for that action.

Validate syntax and a focused run. Read back the revision, job outcome, and relevant artifacts. Clearly distinguish local evidence from platform execution.
