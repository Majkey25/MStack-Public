---
name: prompt-engineering
description: Write, revise, and evaluate prompts or agent instructions. Use when asked to make a prompt clearer, constrain an agent workflow, or diagnose a prompt failure.
license: MIT
---

# Prompt engineering

Start with the behavior the prompt should produce and the audience or model that will use it. Separate instructions from reference material. State the task, required inputs, output contract, and any approval or side effect boundaries.

1. Identify how the current prompt fails with real examples. Distinguish missing data, contradictory instructions, weak tool contracts, and behavior the model cannot guarantee.
2. Change the instruction that drives the failure. Use examples when the boundary or format is hard to convey. Preserve existing requirements that the user still needs.
3. Test ordinary work, the observed failure, and a realistic edge case under comparable settings. Check outputs against observable criteria. Label static inspection and live model results separately.
4. Deliver the revised prompt in the requested format, with evidence and material limitations. Keep private inputs out of examples and evaluation requests unless approved for the runtime.

The [full Prompt Engineering skill](https://github.com/Majkey25/prompt-engineering-skill) has additional prompt patterns and evaluation tooling.
