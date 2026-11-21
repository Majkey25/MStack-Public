<p align="center">
  <img src="assets/mstack-public.webp" alt="MStack Public Skills. Four glass and metal modules in a stack." width="960">
</p>

<h1 align="center">MStack Public</h1>

<p align="center">Standalone agent skills for improving work, onboarding to a repository, researching a claim, and explaining it clearly.</p>

<p align="center">
  <a href="LICENSE"><img src="https://img.shields.io/badge/license-MIT-64B7DE?style=flat-square" alt="MIT license"></a>
  <a href="https://agentskills.io/specification"><img src="https://img.shields.io/badge/format-Agent_Skills-164869?style=flat-square" alt="Agent Skills format"></a>
  <a href="#install"><img src="https://img.shields.io/badge/install-with_npx-F5B85B?style=flat-square" alt="Install with npx"></a>
</p>

## Skills

| Skill | Use it when | Example request |
| --- | --- | --- |
| [`hillclimb`](skills/hillclimb/SKILL.md) | You have a baseline and a goal that takes several attempts to reach. | “Use hillclimb to reduce the import time below two seconds without dropping records.” |
| [`repo-onboarding`](skills/repo-onboarding/SKILL.md) | You need a trustworthy map of an unfamiliar codebase. | “Use repo-onboarding to show me how the API starts and where to add my first test.” |
| [`gold-standard-research`](skills/gold-standard-research/SKILL.md) | A factual answer needs sources you can inspect and conclusions you can check. | “Use gold-standard-research to compare SQLite and PostgreSQL for a desktop app with one writer.” |
| [`bro-what`](skills/bro-what/SKILL.md) | An explanation skipped the context you needed. | “Use bro-what to explain what the second database lock is waiting for.” |

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

The collection format takes cues from [TStack](https://github.com/t3dotgg/tstack), [PStack](https://github.com/cursor/plugins/tree/main/pstack), and [Matt Pocock’s skills](https://github.com/mattpocock/skills). The hillclimb skill credits its experiment workflow in the skill itself.

The more specialized [Prompt Engineering skill](https://github.com/Majkey25/prompt-engineering-skill) has its own repository.
