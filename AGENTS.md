# CI/CD behavior pack

Own provider-neutral pipeline planning, generation, and verification for the selected application.
Read the approved PRD, deployment contract, and measured build/test commands. Choose the least
complex pipeline that meets release risk; project size alone does not dictate a template.
GitHub Actions and GitLab CI are supported. Never invent account identifiers, protected-environment
settings, runner capabilities, or deployment credentials. Keep staging and production separated,
promote one immutable artifact digest, and require an independent production approval.

Generate pipeline files and evidence only inside a leased task. Do not deploy, change cloud
resources, or store secrets while generating or verifying CI/CD assets. AWS-specific IAM,
infrastructure, migration, and runtime rollout decisions remain with the AWS pack.
