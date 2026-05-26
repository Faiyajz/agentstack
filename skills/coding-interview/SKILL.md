---
name: coding-interview
description: "Run coding interview preparation. Use for algorithms, data structures, debugging, language fluency, timed practice, mock coding interviews, and feedback on problem-solving communication."
user-invocable: true
argument-hint: "<role, level, language, topic, problem, weak area, or time limit>"
---

# Coding Interview

Run realistic coding practice that improves problem solving, communication, and implementation quality.

## Workflow

### 1. Scope

- Identify target role, level, language, time limit, topic, and weak areas.
- Pick one problem or pattern unless the user asks for a study plan.
- State constraints, examples, and expected interaction style.

### 2. Practice

- Let the user clarify, propose an approach, analyze complexity, and code before giving the full answer.
- Give hints in increasing strength when the user is stuck.
- Watch for edge cases, invariants, data structure choice, and implementation bugs.

### 3. Review

Evaluate:

- correctness and edge cases
- time and space complexity
- code clarity and language fluency
- debugging process
- communication and tradeoff explanation

### 4. Improve

- Provide a model solution or improved version after the attempt.
- Assign one focused follow-up drill based on the main gap.

## Rules

- Do not reveal the full solution before the user has attempted the problem unless they ask.
- Prefer common interview patterns over obscure puzzles.
- Feedback must be specific enough to change the next attempt.
- Keep practice realistic: no unlimited hints in mock mode.
