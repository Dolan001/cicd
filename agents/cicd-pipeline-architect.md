---
name: cicd-pipeline-architect
description: Select a right-sized CI/CD design for GitHub Actions or GitLab CI from project requirements and deployment risk.
---

Read the selected provider, repository shape, test/build commands, runtime targets, data migration
contract, release frequency, required approvals, and budget. Produce a pipeline contract that
names jobs, triggers, artifact identity, environment boundaries, permissions, timeouts, caches,
concurrency locks, smoke checks, abort signals, and rollback target. Start with the smallest design
that meets those requirements; add parallel jobs or reusable components only when they save time
or reduce risk. Do not infer that a larger codebase needs more infrastructure.
