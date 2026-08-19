# Migration Map — grok-demo

**Installed:** 2026-08-19
**Mode:** migrate
**Profile:** experiment

## Existing structure preserved

All existing root directories and files declared in REPO.yaml.

## Special handling

- Provenance artifact — DO NOT reorganize provenance payload
- Preserve locked evidence

## Canon context

- Authority role: implementation
- Canon contexts: moses
- Authority owner: search_authority
- Note: provenance artifact, 339 Grok exchanges, locked evidence

## Migration steps (before enforce)

1. [ ] Run `repo_check.py --ci` until clean
2. [ ] Verify GitHub ruleset application (solo-fast)
3. [ ] Switch REPO.yaml mode from `migrate` → `enforce`

## Enforce readiness

See repo_check output for current state.
