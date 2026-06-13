# AI Collaborative Development Preflight

> Make AI clarify, plan, and lock decisions before implementation.

AI Collaborative Development Preflight is an open workflow specification for AI-assisted development. It provides `skill.md`, templates, checklists, examples, and Codex instructions to help AI assistants clarify requirements, ask questions, lock decisions, design architecture, check risks, and define acceptance criteria before implementation.

中文: [README.md](./README.md)

## What this project is

This is a documentation-based and skill-based open-source project. It is designed for ChatGPT, Codex, Cursor, Claude, Copilot, and other AI coding assistants.

The goal is simple:

```text
Clarify first. Plan first. Lock decisions first. Implement later.
```

## Problems it solves

AI-assisted development often fails because the project enters implementation too early:

- The idea is vague.
- The AI does not ask enough questions.
- Scope is not locked.
- Technology choices change randomly.
- Architecture, data structures, UI, security, and tests are not designed.
- The project requires repeated rework.
- Acceptance criteria are unclear.

This repository turns the pre-development phase into a reusable workflow.

## Scope

It applies to:

- Desktop apps
- Web apps
- Mobile apps
- Browser extensions
- Backend services
- CLI tools
- AI tools
- Games
- Automation scripts
- Data tools
- Documentation systems
- Knowledge-base systems
- Plugin systems
- Open-source project planning

## Quick start

Send this prompt to an AI assistant:

```text
Please follow the AI Collaborative Development Preflight process. First restate your understanding of my project idea, then ask key clarification questions in rounds. Before requirements, technology choices, architecture, and acceptance criteria are locked, do not enter full implementation. After each round, summarize confirmed decisions, open questions, risks, and next questions.
```

See [QUICK_START.en.md](./QUICK_START.en.md).

## Core files

| File / Directory | Purpose |
|---|---|
| `skill.md` | Bilingual AI execution rules |
| `QUICK_START.md` | Quick startup prompt |
| `docs/` | Workflow docs, question banks, Codex guide |
| `templates/` | Requirement, decision, and development specification templates |
| `checklists/` | Preflight, coding, security, and release checklists |
| `examples/` | Example projects |
| `.github/` | Issue and pull request templates |

## License

MIT License. See [LICENSE](./LICENSE).
