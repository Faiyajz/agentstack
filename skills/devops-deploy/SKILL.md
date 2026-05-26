---
name: devops-deploy
description: "Prepare, review, or implement deployment and operations changes. Use for CI/CD, Docker, cloud deploys, environment configuration, release checks, rollback, and smoke tests."
user-invocable: true
argument-hint: "<deployment task, environment, pipeline, service, or release goal>"
---

# DevOps Deploy

Make deployment changes that are repeatable, observable, and reversible.

## Workflow

### 1. Inspect

- Read existing deployment docs, CI/CD files, Dockerfiles, infrastructure config, scripts, and environment examples.
- Identify environments, secrets, build artifacts, runtime dependencies, health checks, and rollback paths.
- Ask before touching production resources, credentials, DNS, destructive migrations, or cost-impacting infrastructure.

### 2. Plan the Release Path

- Define build, test, deploy, smoke check, monitor, and rollback steps.
- Keep configuration environment-specific and secrets out of source control.
- Prefer existing deployment tooling over new platforms.

### 3. Implement

- Make minimal config, script, pipeline, or documentation changes.
- Add health checks, readiness checks, or smoke commands when missing and useful.
- Keep local development and CI behavior compatible unless intentionally changed.

### 4. Verify

- Run syntax checks, local builds, CI-equivalent commands, or dry runs where possible.
- Report any steps that require credentials or external access.

## Rules

- Never print, commit, or request secrets in plain text.
- Do not run production-impacting commands without explicit approval.
- Prefer reversible deployment steps.
- Document manual operations that cannot be automated safely.
