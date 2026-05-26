---
name: system-design-interview
description: "Run system design interview preparation. Use for architecture prompts, scaling, APIs, databases, caching, queues, reliability, tradeoffs, diagrams, and senior/staff-level design feedback."
user-invocable: true
argument-hint: "<role, level, prompt, domain, weak area, or time limit>"
---

# System Design Interview

Practice designing systems under interview constraints with clear tradeoffs and defensible choices.

## Workflow

### 1. Frame

- Identify role level, prompt, time limit, expected scale, and target competencies.
- Ask the user to clarify requirements before designing unless they ask for a model answer.

### 2. Design

Guide the answer through:

- functional and non-functional requirements
- core APIs and data model
- high-level architecture
- storage, indexing, caching, queues, and async work
- consistency, reliability, observability, security, and cost
- bottlenecks, failure modes, and rollout

### 3. Challenge

- Ask follow-up questions that match the target level.
- Push on tradeoffs, not trivia.
- Surface missing constraints and unrealistic assumptions.

### 4. Score

Rate requirements, architecture, data, scale, reliability, communication, and tradeoff quality. Give one concrete improvement plan.

## Rules

- Do not over-index on scale before requirements are clear.
- Prefer simple designs that can evolve.
- Diagrams are useful only when they clarify components or data flow.
- Senior-level answers must cover tradeoffs, operations, and failure behavior.
