# Changelog

## [3.1.0] - 2026-06-14

### 🔧 Major: Simulated Dialogue Hardening
After running a real preflight simulation (file encryption tool project):

- **STEPS → PHASES with loop gates**: replaced linear 12-step model with 11 phases. [QUESTION ⇄ LOCK] is now an explicit sub-loop with COMPLETENESS GATE exit condition
- **MANDATORY_COVERAGE per phase**: each phase now has a mandatory checklist (Direction: 6 items, Feature: 10 items, Engineering: 12 items)
- **QUESTION FORMAT V2**: every option MUST include pros/cons, technical term explanations, and "你也可以提出新方案" invite
- **【STATE】output**: every response begins with current state declaration
- **Completeness Gate**: 18-item checklist before exiting the question loop; any ⚠️/❌ triggers phase re-loop
- **New alternative handling**: user proposes new idea → PAUSE → verify phase completeness → re-loop if needed
- **LIGHT→FULL upgrade path**: small changes that require architecture → auto-upgrade to FULL MODE Phase 1
- **Detailed rollback spec**: 6-step change management with affected-decision table and module impact mapping
- **Compact 【ROUND OUTPUT】 format**: merged summary + decision table + risks into single format
- **README.md rewritten** in clean, structured reference style

## [3.0.0] - 2026-06-14

### 🚀 Major: Executable Runtime Engine
- SKILL.md rewritten as runtime execution engine, not documentation
- FULL MODE (12-step) and LIGHT MODE (6-step)
- State machine: INIT → UNDERSTAND → QUESTION → LOCK → SPEC → CONFIRM → READY
- Hard constraints on question format (A/B/C/D/E only in early phases)
- Mandatory decision lock table output after every user choice
- Block rules: absolutely no code before SPEC approval

### 📁 Repo Restructuring
- docs/legacy/ — archived v2.x documentation
- docs/templates/ — output templates
- docs/guides/ — Codex usage guides
- Root simplified to SKILL.md + plugin.json + core project files

### 🧩 Plugin Standardization
- .codex-plugin/plugin.json with full Codex interface
- plugin.json simplified root manifest
- agents/openai.yaml agent metadata

## [2.2.0] - 2026-06-13
- Converted to Codex Skill Plugin format
- Added .codex-plugin/plugin.json
- Added agents/openai.yaml

## [2.1.0] - 2026-06-13
- Streamlined skill to v2.1 with mandatory principles
- Option-based questioning system
- Anti-drift mechanism
- Dynamic question modules

## [2.0.0] - 2026-06-13
- Complete bilingual project scaffold
- 15-step preflight workflow
- Templates, checklists, examples, docs

## [1.0.0] - 2026-06-13
- Initial full project scaffold