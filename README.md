# CI/CD behavior pack

Provider-neutral agents and skills for designing, generating, and verifying project CI/CD.
The current providers are GitHub Actions and GitLab CI. The pipeline is sized by workload,
repository layout, test duration, release frequency, and blast radius rather than an arbitrary
small/medium/large label.

The pack defines the common release contract: pull-request checks, reproducible build, immutable
artifact and provenance, staging deployment and live verification, protected production promotion,
rollback, and drift checks when infrastructure is managed as code. Cloud-specific commands and
identities come from the selected deployment pack. This repository contains no credentials,
cloud state, or reusable workflow that silently deploys a project.
