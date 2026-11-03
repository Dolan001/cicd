---
name: design-ci-cd-pipeline
description: Design a right-sized GitHub Actions or GitLab CI release pipeline from verified requirements and build evidence.
---

# Design CI/CD pipeline

Read the PRD, deployment contract, repository inventory, measured tests, and selected provider.
Use GitHub Actions only as the default; GitLab CI is supported when selected. If another provider
is required, report the missing provider implementation before generation. Define required checks,
build inputs, immutable artifact identity, staging verification, protected production approval,
rollback, permissions, OIDC/federation, runner needs, and cost/time limits. Scope jobs to the
project's risk and measured duration. Record decisions in `docs/deployment/ci-cd-contract.md`.
Do not create cloud resources or run a release.
