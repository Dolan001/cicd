# Provider guidance

## GitHub Actions

Use pinned actions, minimal `permissions`, separate `staging` and `production` environments,
required reviewers/branch restrictions where available, and OIDC-scoped cloud roles. A workflow
file naming an environment is not proof that protection rules are configured; verify settings
before a production release. Use concurrency to prevent overlapping environment deployments.

## GitLab CI

Use an explicit stage graph, protected environments and branches, `resource_group` for serialized
deployments, protected/masked variables, and ID tokens for cloud federation. Verify project/group
settings rather than assuming the YAML alone enforces approvals.

Both providers must build once, record the image/package digest, verify staging, and promote that
digest to production without rebuilding. Keep provider configuration separate from AWS-specific
roles and infrastructure. If the selected provider lacks equivalent controls, block readiness.
