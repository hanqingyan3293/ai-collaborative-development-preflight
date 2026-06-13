# AI Collaborative Development Preflight

> Make AI clarify, plan, and lock decisions before writing code.

AI Collaborative Development Preflight is an open workflow specification for AI-assisted development. It guides AI assistants to clarify requirements, ask questions, lock decisions, check risks, design architecture, and define acceptance criteria before implementation.

中文: [README.md](./README.md)

## Why this project exists

Many AI coding failures do not happen because the AI cannot write code. They happen because the project was not clarified before coding.

Common issues include:

- The user describes an idea but not the boundaries.
- The AI starts coding without asking questions.
- The technology stack changes randomly.
- Data structures and file formats are not defined.
- UI, errors, security, privacy, and acceptance criteria are ignored.
- The project requires repeated rework.

This repository turns the pre-development phase into a reusable workflow, skill, templates, checklists, and examples.

## Scope

This workflow applies to:

- Desktop apps
- Web apps
- Mobile apps
- Browser extensions
- AI tools
- Games
- Automation scripts
- Backend services
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

- [skill.md](./skill.md): Bilingual AI skill rules.
- [docs/](./docs/): Workflow documentation and question banks.
- [templates/](./templates/): Preflight templates.
- [checklists/](./checklists/): Checklists.
- [examples/](./examples/): Example projects.
- [.github/](./.github/): Issue and pull request templates.

## License

MIT License. See [LICENSE](./LICENSE).
