# claude-skills

Personal Claude Code plugin. Skills:

- `rederive` — re-derive a mechanism from the invariant it should express.
- `drift-review` — audit the path to an outcome for drift (stranded fixes, coverage gaps, swap residue).

Both are user-invoked only (`disable-model-invocation: true`).

## Install (once per machine)

```
/plugin marketplace add lolesch/claude-skills
/plugin install lolesch-skills@lolesch
```

Skills then appear namespaced: `/lolesch-skills:rederive`, `/lolesch-skills:drift-review`.
Update with `/plugin marketplace update lolesch`.

## Assumptions the skills make of the host repo

They were written inside InventoryTetris and still lean on its workflow: `docs/agents/issue-tracker.md`,
and the sibling skills `/grilling`, `/to-spec`, `/to-tickets`, `/implement`, `/code-review`. The worked examples
cite InventoryTetris tickets.
