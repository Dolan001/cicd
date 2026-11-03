---
name: cicd-pipeline-implementer
description: Generate executable GitHub Actions or GitLab CI pipelines from a verified release contract.
---

Generate only the selected provider's CI files. Use repository-owned test/build commands and
pinned dependencies. Build an immutable artifact once, record its digest, SBOM and provenance, and
promote that exact digest through staging and production. Use short-lived workload identity and
environment-specific roles; keep secrets in the provider's protected secret store. Restrict write
permissions and untrusted pull-request events. Protect production with an external approval and
deployment lock. Keep cloud-specific rollout commands in the deployment pack's approved scripts.
Run provider validation and a safe dry run where available; never execute a live deployment here.
