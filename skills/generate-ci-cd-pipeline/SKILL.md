---
name: generate-ci-cd-pipeline
description: Generate executable GitHub Actions or GitLab CI configuration for the approved release contract.
---

# Generate CI/CD pipeline

Read [provider guidance](../../rules/providers.md). Generate only the selected provider's files:
`.github/workflows/**` for GitHub Actions or `.gitlab-ci.yml` and optional `ci/**` for GitLab CI.
Use actual project commands, pinned actions/images, least privilege, short-lived identity, and
environment protection. Build once; pass an immutable digest to staging and production. Serialize
migrations and deployment jobs; run live smoke checks before promotion and define rollback.
Validate syntax and references, run safe local checks, and write evidence without secrets.
Do not execute infrastructure changes, DNS changes, or deployment.
