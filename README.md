# Copilot Design Skill — by Tenten AI

**A Copilot-first creative skill for GitHub Copilot, ChatGPT, Codex, Claude, and Grok.**

[English](README.md) · [繁體中文](README.zh-TW.md) · [Changelog](CHANGELOG.md)

![Author: Tenten AI](https://img.shields.io/badge/Author-Tenten_AI-111111) ![License: MIT](https://img.shields.io/badge/License-MIT-2563eb) ![AI agents](https://img.shields.io/badge/Copilot%20%C2%B7%20ChatGPT%20%C2%B7%20Codex%20%C2%B7%20Claude%20%C2%B7%20Grok-ready-7c3aed)

Turn a plain-language brief into a polished, working visual artifact. Copilot Design Skill gives AI agents a complete design workflow—from direction and structure to interactive HTML, review, and export.

Built for **GitHub Copilot first**, with the same portable workflow available to **ChatGPT, Codex, Claude, and Grok** in file-capable agent environments.

## What you can create

- Product UI, landing pages, dashboards, and mobile screens
- Interactive prototypes, wireframes, and design systems
- Slide decks, documents, diagrams, and social creative
- Animations, data visualizations, and standalone HTML
- Editable PPTX, PDF, image, and video exports

## Why it feels different

- **One brief, full workflow.** The skill handles design direction, production, preview, and refinement.
- **Built from real context.** Give it screenshots, HTML/CSS, a codebase, GitHub repository, or Figma `.fig` file.
- **Designed to be edited.** Outputs are local, inspectable, and ready for another pass—not trapped in a black box.
- **Agent-flexible.** Use the same skill across Copilot, ChatGPT, Codex, Claude, and Grok.

> The agent needs permission to read and write files. Browser preview and terminal access are recommended for the complete workflow.

## Quick start

Install the skill:

```bash
npx skills add tentenco/Copilot-PTT-Design-Skill
```

Or point your AI agent directly to the skill entry file:

```text
Read skills/copilot-design/SKILL.md and follow it to create three high-fidelity
directions for a personal finance dashboard. Save the result as standalone HTML.
```

For a manual installation, copy [`skills/copilot-design/`](skills/copilot-design/) into the skills directory supported by your agent. The workflow starts from `SKILL.md`.

## How it works

```text
Your brief → design method → focused sub-skills → interactive HTML → review → export
```

The entry skill loads only the guidance needed for the job. Its built-in workflows cover high-fidelity UI, prototyping, decks, documents, motion, research, design systems, source imports, and production exports.

Everything is organized under one portable package:

```text
skills/copilot-design/
├── SKILL.md              # Start here
├── system-prompt.md      # Design method and quality bar
├── built-in-skills/      # Task-specific workflows
├── starter-components/   # Reusable visual building blocks
├── references/           # Agent-specific tool guidance
└── agents/               # Import, validation, and export utilities
```

## Prompt ideas

```text
Design a focused SaaS landing page using the visual language in this screenshot.
```

```text
Turn this product brief into an interactive mobile onboarding prototype.
```

```text
Create a 10-slide investor deck, add native build animations, and export it to PPTX.
```

```text
Import this Figma file as a design system, then build an analytics dashboard with it.
```

## Made for your AI stack

| Agent | Suggested use |
|---|---|
| **GitHub Copilot** | Primary, Copilot-first workflow |
| **ChatGPT** | Design and build in a file-capable coding workspace |
| **Codex** | Local implementation, preview, verification, and export |
| **Claude** | Design exploration and artifact production |
| **Grok** | Prompt-led creation in an environment with file tools |

## Author and license

Repurposed and maintained by **Tenten AI**.

This independent project adapts the Claude Design methodology for portable AI-agent workflows and is not affiliated with or endorsed by Anthropic, GitHub, OpenAI, xAI, or their products. Existing upstream copyright notices remain in effect. Released under the [MIT License](LICENSE).
