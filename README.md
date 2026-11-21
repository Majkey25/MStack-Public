<p align="center">
  <img src="assets/mstack.svg" alt="" width="64" height="64">
</p>

<h1 align="center">MStack Public</h1>

<p align="center">Standalone agent skills for planning, coding, reviewing, research, and writing.</p>

<p align="center">
  <a href="SOURCES.md"><img src="https://img.shields.io/badge/licenses-per_skill-586574?style=flat-square" alt="Licenses by skill"></a>
  <a href="https://agentskills.io/specification"><img src="https://img.shields.io/badge/format-Agent_Skills-586574?style=flat-square" alt="Agent Skills format"></a>
  <a href="#install"><img src="https://img.shields.io/badge/install-with_npx-385d88?style=flat-square" alt="Install with npx"></a>
</p>

## Skills

### Frontend and browser

| Skill | Use it for |
| --- | --- |
| [`modern-web-guidance`](skills/modern-web-guidance/SKILL.md) | Choosing compatible web platform features from current guidance |
| [`design-taste-frontend`](skills/design-taste-frontend/SKILL.md) | Designing a clear, usable interface with an intentional layout |
| [`browser-testing-with-devtools`](skills/browser-testing-with-devtools/SKILL.md) | Diagnosing rendering, request, console, and performance problems |
| [`playwright`](skills/playwright/SKILL.md) | Automating a repeatable browser flow or regression test |
| [`animate`](skills/animate/SKILL.md) | Building UI motion with reduced motion support |
| [`review-animations`](skills/review-animations/SKILL.md) | Reviewing existing UI motion and interaction |

### Engineering and delivery

| Skill | Use it for |
| --- | --- |
| [`hillclimb`](skills/hillclimb/SKILL.md) | Improving a result against a baseline and regression checks |
| [`repo-onboarding`](skills/repo-onboarding/SKILL.md) | Getting a codebase running and finding the first place to make a change |
| [`grilling`](skills/grilling/SKILL.md) | Testing a plan before committing to it |
| [`domain-modeling`](skills/domain-modeling/SKILL.md) | Clarifying domain terms, boundaries, and decisions |
| [`api-and-interface-design`](skills/api-and-interface-design/SKILL.md) | Designing interface contracts, failures, and compatibility |
| [`ponytail`](skills/ponytail/SKILL.md) | Finding the smallest complete code change |
| [`incremental-implementation`](skills/incremental-implementation/SKILL.md) | Implementing a change in small slices with a check for each |
| [`debugging-and-error-recovery`](skills/debugging-and-error-recovery/SKILL.md) | Reproducing a failure and finding its root cause |
| [`code-review-and-quality`](skills/code-review-and-quality/SKILL.md) | Reviewing a change for correctness, security, and performance |
| [`documentation-and-adrs`](skills/documentation-and-adrs/SKILL.md) | Recording technical decisions and checking documentation for drift |
| [`ci-cd-and-automation`](skills/ci-cd-and-automation/SKILL.md) | Building and validating CI, build, and deployment workflows |
| [`file-pr`](skills/file-pr/SKILL.md) | Filing or updating a concise GitHub pull request |

### Research and communication

| Skill | Use it for |
| --- | --- |
| [`gold-standard-research`](skills/gold-standard-research/SKILL.md) | Checking claims against sources, calculations, and counterexamples |
| [`bro-what`](skills/bro-what/SKILL.md) | Explaining a confusing idea with the missing context restored |
| [`caveman`](skills/caveman/SKILL.md) | Shortening responses while keeping technical details |
| [`unslop`](skills/unslop/SKILL.md) | Cutting filler and generic phrasing from a draft |
| [`handoff`](skills/handoff/SKILL.md) | Giving another person or agent enough evidence to resume work |
| [`prompt-engineering`](skills/prompt-engineering/SKILL.md) | Revising and evaluating prompts and agent instructions |

## Install

Requires Node.js 22.20 or later for the [Skills CLI](https://github.com/vercel-labs/skills). Run this in your project to choose the skills and agents to install.

```sh
npx skills add Majkey25/MStack-Public
```

Install a single skill in a single agent.

```sh
npx skills add Majkey25/MStack-Public --skill hillclimb -a codex
```

> [!TIP]
> Add `-g` to install across projects. Each skill works on its own, so you can start with one.

<details>
<summary>Manual install</summary>

Copy the chosen directory from [`skills/`](skills/) into the skill directory your agent reads. For project installs, Codex reads `.agents/skills/` and Claude Code reads `.claude/skills/`.

</details>

## Credits

See [Sources and licenses](SOURCES.md) for upstream commits and adaptations. Each included upstream skill carries its license in its own directory.

The [full Prompt Engineering repository](https://github.com/Majkey25/prompt-engineering-skill) has additional examples and evaluation tools.
