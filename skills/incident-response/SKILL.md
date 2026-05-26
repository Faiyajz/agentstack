---
name: incident-response
description: "Triage and manage production incidents. Use for outages, degraded services, alerts, customer-impacting bugs, security incidents, rollback decisions, and post-incident follow-up."
user-invocable: true
argument-hint: "<incident symptoms, alert, service, timeline, or severity>"
---

# Incident Response

Restore service first, preserve evidence, communicate clearly, and capture follow-up work.

## Workflow

### 1. Stabilize

- Identify service, impact, start time, affected users, severity, current mitigations, and owners.
- Avoid speculative root cause until evidence supports it.
- Ask before production-impacting actions when approval is required.

### 2. Triage

Inspect:

- recent deploys, config changes, migrations, and traffic shifts
- metrics, logs, traces, queues, databases, caches, and external dependencies
- error rates, latency, saturation, and user reports
- rollback, failover, feature flag, and scaling options

### 3. Mitigate

- Choose the fastest low-risk action to reduce impact.
- Prefer rollback, disablement, throttling, scaling, or traffic routing when they are safer than hot fixes.
- Keep a timestamped timeline of decisions and actions.

### 4. Verify and Communicate

- Confirm recovery with metrics and user-visible checks.
- Summarize current status, impact, mitigation, next update time, and known unknowns.

### 5. Follow Up

After stability, write root cause, contributing factors, prevention tasks, owners, and verification.

## Rules

- Do not hide uncertainty.
- Do not blame people.
- Do not destroy logs, traces, or other evidence.
- Security incidents require extra care with secrets, access, and disclosure.
