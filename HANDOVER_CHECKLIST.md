# Research Project Handover Checklist

A project is not ready for handover merely because its main author can run it.

## State recovery
- [ ] README identifies the project purpose.
- [ ] STATUS identifies the current gate/state.
- [ ] Canonical files are explicitly listed.
- [ ] Historical/superseded results are distinguishable.
- [ ] Open findings are visible.
- [ ] The next bounded action is stated.

## Scientific traceability
- [ ] Major assumptions are registered.
- [ ] Major source-derived values are registered.
- [ ] Consequential numbers have provenance.
- [ ] Consequential claims map to evidence/model outputs.
- [ ] Known contradictory evidence remains visible.
- [ ] Model closure and physical/deployment validation are distinguished.

## Reproducibility
- [ ] Environment/dependencies are documented.
- [ ] Core result can be regenerated with documented commands.
- [ ] Tests/verification can be run with documented commands.
- [ ] Figures/tables can be traced to generating data/code.
- [ ] Randomness and seeds are documented where relevant.
- [ ] External data/code dependencies are pinned or identified.

## Software quality
- [ ] Core scientific functions have appropriate tests.
- [ ] Known numerical limitations are documented.
- [ ] No required local secret/path is undocumented.
- [ ] CI status is visible if CI is used.

## Manuscript
- [ ] Manuscript points to canonical results.
- [ ] Citations/references resolve.
- [ ] Figures and tables match canonical data.
- [ ] Conclusions do not exceed evidence.
- [ ] Exact reviewed PDF/artifact is identifiable.

## External repositories
- [ ] External authoritative repository/commit is pinned.
- [ ] Write permissions/transfer rules are explicit.
- [ ] Proposed patches have verification evidence.

## Fresh-user test
A person or agent without the previous chat history should be able to:
1. identify the current state;
2. locate canonical evidence;
3. reproduce the core calculation;
4. identify unresolved limitations;
5. know the next action.

If not, handover is incomplete.
