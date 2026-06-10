# GitHub Workflow

This repository should use GitHub as the project control center for KazTransCargo development.

## Recommended Features

### Issues

Use Issues for every product or engineering task.

Recommended issue types:

- `feature`
- `bug`
- `ui`
- `workflow`
- `security`
- `docs`
- `tech-debt`

Each issue should include:

- business goal;
- affected role;
- affected route or module;
- expected behavior;
- acceptance checks.

### Projects

Use GitHub Projects as the work board.

Recommended fields:

- Status: Backlog, Ready, In progress, Review, Done
- Area: Auth, Customer, Logistics, Admin, Accounting, UI, Docs
- Priority: P0, P1, P2, P3
- Transport mode: auto, air, rail, multimodal, all
- Risk: low, medium, high

Recommended views:

- Roadmap
- Current sprint
- Bugs
- UI polish
- Logistics workflow
- Security and data visibility

### Pull Requests

Every code change should go through a pull request once the repository contains source code.

Pull request checklist:

- The change is scoped to one task.
- Customer views do not expose supplier costs or margins.
- Server actions validate input.
- Business logic is not placed inside UI components.
- `npm run lint` passes.
- `npm run typecheck` passes.
- `npm run build` passes when the change is significant.

### Branch Protection or Rulesets

Protect `main` when source code is pushed.

Recommended rules:

- require pull request before merge;
- require status checks;
- block force pushes;
- block branch deletion;
- require linear history if the team prefers clean history.

### GitHub Actions

Add CI once source code is pushed.

Recommended checks:

- install dependencies;
- Prisma validation;
- lint;
- TypeScript check;
- build.

### GitHub Copilot / Agent Features

If enabled in the account, GitHub Copilot can help with:

- turning issues into implementation branches;
- opening pull requests;
- reviewing pull requests;
- running agent sessions from issues.

Use this only with clear task descriptions and the rules in `AGENTS.md`.

### Repository Documentation

Keep these files current:

- `README.md`
- `AGENTS.md`
- `docs/PRODUCT_OVERVIEW.md`
- `docs/ARCHITECTURE.md`
- `docs/LOCAL_SETUP.md`
- `docs/ROLES_AND_WORKFLOWS.md`
- `docs/SECURITY.md`
- `docs/DESIGN_SYSTEM.md`
- `docs/GITHUB_WORKFLOW.md`

## Suggested Working Order

1. Create or refine an Issue.
2. Link the Issue to the GitHub Project.
3. Move the Issue to Ready.
4. Create a branch for the task.
5. Implement the smallest safe change.
6. Run checks.
7. Open a pull request.
8. Review security and business rules.
9. Merge after checks pass.
