---
name: security-review
description: "Review code, configuration, architecture, or workflows for practical security risk. Use for auth, secrets, input handling, dependency risk, infrastructure exposure, and release gates."
user-invocable: true
argument-hint: "<diff, feature, repo path, service, config, or security concern>"
---

# Security Review

Find exploitable risk and practical fixes. Do not turn review into generic compliance advice.

## Workflow

### 1. Scope

- Identify assets, trust boundaries, actors, data sensitivity, environments, and changed files.
- Read relevant code, configs, dependencies, auth flows, and deployment paths.
- Ask only when missing context changes risk severity or recommended fixes.

### 2. Review

Check for:

- broken authentication or authorization
- injection, unsafe deserialization, XSS, SSRF, CSRF, path traversal, and command execution
- secret handling, logging, token storage, and credential exposure
- insecure defaults, CORS, cookies, headers, TLS, and network exposure
- dependency and supply-chain risk
- missing rate limits, abuse controls, audit logs, or monitoring

### 3. Report or Fix

- If asked to review, report findings ordered by severity and do not edit code.
- If asked to fix, make the smallest change that removes or reduces the risk and add verification.
- Distinguish confirmed vulnerabilities from plausible risks and hardening suggestions.

### 4. Verify

- Run targeted tests, scanners, lint rules, or manual checks when available.
- Do not claim security is complete; report what was and was not checked.

## Rules

- Do not provide offensive exploitation steps beyond what is needed to prove and fix a vulnerability.
- Never print secrets.
- Security fixes should preserve intended product behavior.
- Prefer simple, enforceable controls over policy-only recommendations.
