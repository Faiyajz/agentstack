---
name: fullstack-feature
description: "Build one vertical product slice across frontend, backend, data, tests, and rollout. Use for fullstack features that cross UI, API, database, services, and user-visible behavior."
user-invocable: true
argument-hint: "<feature, task, spec path, or issue reference>"
---

# Fullstack Feature

Ship one coherent product slice end to end. Prefer existing app patterns over new architecture.

## Workflow

### 1. Ground

- Read the request, product brief, spec, plan, and relevant code.
- Identify the user flow, data flow, API contracts, persistence, permissions, errors, and rollout needs.
- Ask only when missing information would change behavior, data shape, or user-visible scope.

### 2. Design the Slice

- Choose the smallest vertical path that proves the feature.
- Define UI states, backend endpoints or actions, schema changes, validation, and error behavior.
- Preserve existing contracts unless the task explicitly changes them.

### 3. Implement

- Build backend and frontend in small running steps.
- Add migrations, seeds, fixtures, or configuration only when needed.
- Handle loading, empty, success, error, and permission states where relevant.

### 4. Verify

- Add or update tests for backend behavior, frontend behavior, and integration boundaries.
- Run focused tests first, then wider checks when shared code changed.
- Use `browser-verify` for browser-facing work when available.

### 5. Report

Summarize the user flow delivered, files changed, checks run, and any rollout or follow-up risk.

## Rules

- One product slice at a time.
- Do not split by layer when a vertical slice is practical.
- Do not leave UI wired to fake behavior unless the task explicitly asks for a prototype.
- Data migrations must be reversible or have a clear rollback note.
