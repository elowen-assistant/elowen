# Playbook: Release Flow

Use this playbook when promoting Elowen work to tagged releases.

## Child Repository Release

1. finish and validate the child repo change
2. merge or land it on the intended release branch
3. create a tag in the child repository
4. publish release notes in the child repository if desired

## Workspace Snapshot Release

1. update all needed child repositories first
2. update submodule pointers in `elowen-workspace`
3. validate the integrated stack from the workspace root
4. create a tag in `elowen-workspace` to mark the known-good system state

## Guidance

- Use child repo tags for service releases.
- Use workspace tags for integrated platform snapshots.
- Avoid tagging the workspace until submodule pointers match the intended release commits.
