# agent-policy-enforcement-engine

Runtime policy engine to validate prompts, tools, and data boundaries.

## Scope

Pre-execution policy checks with explicit allow/deny decisioning.

## Capabilities

- Pre-execution policy checks with explicit allow/deny decisioning.
- Declarative policy packs with versioned rollout controls.
- Violation reporting, quarantine actions, and review workflows.
- Extensible hook system for tenant, role, and context-based controls.

## Repository Layout

- `src/main.py` entrypoint and lightweight service bootstrap
- `src/project_profile.py` canonical project metadata
- `src/service_contract.py` baseline domain contract shape
- `tests/` smoke and contract tests
- `docs/` architecture and roadmap

## Quick Start

```bash
python3 -m venv .venv
source .venv/bin/activate
pip install -e .[dev]
pytest -q
python -m src.main
```
