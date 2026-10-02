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

## Requirements

The skills assume the `mattpocock-skills` plugin workflow in the host repo:
the issue tracker documented in `docs/agents/issue-tracker.md`, and the sibling skills `/grilling`, `/to-spec`,
`/to-tickets`, `/implement`, `/code-review`, `/simplify` and `/improve-codebase-architecture`.
