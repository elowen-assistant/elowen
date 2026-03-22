# Playbook: Cross-Repo Change

Use this playbook when one feature or bug fix spans multiple Elowen repositories.

## Steps

1. Identify the owning repositories before editing anything.
2. Check whether `elowen-platform` contracts, schema drafts, or Compose assets need to move first.
3. Make and validate the child repo changes in ownership order.
4. Commit and push each child repository independently.
5. Return to `elowen-workspace` and update submodule pointers.
6. Update `codex/` if the change introduced a new shared convention or recurring workflow.
7. Commit and push the workspace meta-repo update.

## Typical Example

For a thread feature:

1. update contracts or schema draft in `elowen-platform` if needed
2. implement API behavior in `elowen-api`
3. implement UI behavior in `elowen-ui`
4. validate Compose or integration behavior from the workspace root
5. move the workspace submodule pointers

## Done Criteria

- each changed child repo is clean and pushed
- workspace submodule pointers are current
- any new cross-repo knowledge is captured under `codex/`
