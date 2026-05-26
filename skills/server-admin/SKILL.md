---
name: server-admin
description: "Safely inspect and administer Linux servers. Use for SSH-based diagnostics, services, logs, disks, processes, networking, firewalls, packages, users, and system hardening."
user-invocable: true
argument-hint: "<server, symptom, service, log, or admin task>"
---

# Server Admin

Operate servers carefully. Inspect first, change second, and avoid destructive commands unless explicitly approved.

## Workflow

### 1. Scope

- Identify the host, access method, operating system, service, symptom, and risk.
- Ask before changing production systems, firewall rules, users, permissions, packages, or persistent config.
- Prefer read-only diagnostics until the cause is clear.

### 2. Diagnose

Use `references/linux-diagnostics.md` for read-only command patterns when helpful. Prefer distro-native tools and adapt commands to the host.

Check relevant areas:

- service status and recent logs
- disk, memory, CPU, and process pressure
- network listeners, DNS, routes, and firewall rules
- config files, environment, permissions, and recent changes
- package and kernel state when relevant

### 3. Change

- Make the smallest reversible change.
- Back up edited config files when practical.
- Use service reloads before restarts when safe and supported.
- Keep a command log for what changed.
- Prefer temporary mitigations only when they are clearly labeled and followed by a permanent fix.

### 4. Verify

- Confirm the service state, logs, health endpoint, open ports, and user-visible behavior.
- Report residual risk and recommended follow-up hardening.

## Rules

- Do not run destructive commands without explicit approval.
- Do not expose secrets from files, process lists, logs, or shell history.
- Do not disable security controls to make a symptom disappear.
- Prefer vendor docs and distro-native tooling for system changes.
- Treat production shell access as high risk: inspect, explain, then change.
