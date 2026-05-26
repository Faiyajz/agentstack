---
name: product-brief
description: "Clarify a product idea before technical design. Use for product discovery, feature shaping, MVP scope, requirements, personas, success metrics, and launch risks."
user-invocable: true
argument-hint: "<product idea, feature request, market, users, or rough notes>"
---

# Product Brief

Turn a rough product idea into a decision-ready brief. Keep it concrete enough for `spec` and `plan` to use.

## Workflow

### 1. Understand

- Treat the full argument as the product input.
- Identify target users, problem, current workaround, business goal, constraints, and unknowns.
- Read referenced docs, issues, analytics, support notes, or code when available.
- Ask only when a missing answer would materially change scope or priority.

### 2. Shape

Use `references/template.md` for the output structure unless the user asks for a different format.

Define:

- User segments and primary jobs to be done
- Problem statement
- Goals and non-goals
- MVP scope
- User flows or workflows
- Functional requirements
- Quality requirements
- Success metrics
- Risks, dependencies, and open questions

### 3. Write

Write `docs/<product-slug>/brief.md` when there is a clear feature slug. Otherwise return the brief in chat.

### 4. Pause

Stop after the brief. Recommend `spec` or `design-doc` only when the next step is clear.

## Rules

- Do not invent market facts, user evidence, pricing, or legal claims.
- Separate known facts from assumptions.
- Prefer small MVPs that can be shipped and measured.
- Requirements must be testable or observable.
- Success metrics must name the behavior, event, or business outcome they measure.
- Keep product strategy distinct from implementation details.
