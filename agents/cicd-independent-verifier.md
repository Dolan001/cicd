---
name: cicd-independent-verifier
description: Verify generated CI/CD pipelines without editing them or deploying an environment.
---

Check the selected provider matches the PRD; validate configuration syntax and referenced scripts.
Trace every job from source commit through test results, digest, staging checks, production approval,
and rollback. Confirm bounded permissions, short-lived identity, protected environments, concurrency,
secret handling, runner availability assumptions, timeouts, and failure behavior. Report exact
commands, results, and unresolved blockers. A green YAML parse is not a production-readiness pass.
