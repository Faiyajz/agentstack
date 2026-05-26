---
name: backend-api
description: "Design and implement backend/API changes. Use for endpoints, services, database access, queues, authz, validation, contracts, migrations, and integration behavior."
user-invocable: true
argument-hint: "<API/backend task, endpoint, service, schema, or spec path>"
---

# Backend API

Build backend changes that are explicit about contracts, failure behavior, and data safety.

## Workflow

### 1. Understand

- Read the request, existing API patterns, schemas, services, tests, and clients.
- Identify contracts, authn/authz, validation, idempotency, pagination, rate limits, and failure modes.
- Ask before changing public shapes, persistence semantics, or compatibility guarantees.

### 2. Design

- Define request and response shapes, status codes, error bodies, side effects, and data ownership.
- Reuse existing framework conventions, middleware, serializers, repositories, and test helpers.
- Plan migrations and backfills when storage changes.

### 3. Implement

- Make the smallest backend change that satisfies the contract.
- Validate inputs at trust boundaries.
- Keep business rules out of controllers when the codebase already has service/domain layers.
- Handle concurrency, retries, and partial failure where relevant.

### 4. Verify

- Add contract, unit, integration, and migration tests in proportion to risk.
- Test authorization and important failure paths.
- Run focused tests and relevant lint/type checks.

## Rules

- Do not silently change existing API behavior.
- Prefer additive compatible changes when clients may already exist.
- Never log secrets, tokens, passwords, or sensitive payloads.
- Database writes should be transactionally safe where consistency matters.
