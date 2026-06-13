# How to Use with Codex

## Goal

Make Codex read this specification before coding, then clarify requirements and prepare a development specification.

## Recommended prompt

```text
Please read skill.md, docs/workflow.md, and templates/core/development-spec.md first. Then follow the AI Collaborative Development Preflight process: restate the project idea, ask clarification questions in rounds, output a decision lock table, risk list, and development specification. Do not enter full implementation until the specification is confirmed.
```

## Existing project

```text
Please inspect the current repository and this preflight specification. Do not modify code yet. First output:
1. Understanding of the project
2. Project type
3. Existing features
4. Suspected issues
5. Questions for the user
6. Proposed modification plan
```

## New project

```text
Please follow skill.md from requirement clarification to development specification, then implement.
```
