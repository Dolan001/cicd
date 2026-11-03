---
name: verify-ci-cd-pipeline
description: Independently verify pipeline syntax, identity, artifact promotion, environment protection, and rollback.
---

# Verify CI/CD pipeline

Read the approved CI/CD contract and the generated files. Verify the provider and all referenced
scripts, job permissions, trust conditions, test coverage, build provenance, exact digest promotion,
staging health gate, production approval, concurrency, abort signals, and rollback. Validate the
configuration with provider tools when available. Do not treat a syntactically valid pipeline as
proof of a successful live deployment. Record truthful evidence and any blockers without editing
the pipeline or using live credentials.
