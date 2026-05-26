# Working in AgentStack

AgentStack encodes practical software engineering and agentic engineering workflows: discover the product problem, design when architecture is ambiguous, spec when decisions matter, plan when work needs splitting, test before ship, refactor when code needs simplifying, review before merge, secure before release, operate production systems, and prepare engineers for interviews.

If you are an AI agent working in this repo, follow this guidance.

## The Flow

Use `product-brief -> design-doc -> spec -> plan -> implement -> review` for product or architecture work with ambiguity, tradeoffs, or cross-cutting concerns. Use `spec -> plan -> implement -> review` for changes that touch contracts, schemas, multiple files, user-visible behavior, or invariants. Skip stages only when explicitly told to or when the change is trivial and decision-complete.

Use `refactor` after implementation when changed code needs cleanup for reuse, quality, or efficiency. Use `security-review` for security-sensitive changes. Use `address-pr-feedback` after GitHub PR review comments exist.

Exploration is allowed without creating docs or issue tracker entries. Do not manufacture fake specs, plans, or issues for spikes.

## Skills

- `design-doc`: write a lightweight architecture design doc before implementation when the design is ambiguous.
- `product-brief`: clarify users, value, requirements, risks, and scope before technical work.
- `spec`: write the technical design before coding.
- `plan`: break a spec, brief, or request into agent-sized tasks.
- `implement`: execute one scoped change with tests and verification.
- `tdd`: test-first variant of implement.
- `fullstack-feature`: coordinate frontend, backend, data, tests, and rollout for one product slice.
- `backend-api`: design and implement robust API/backend changes.
- `frontend-ui`: build browser-facing UI with interaction, accessibility, and responsive verification.
- `devops-deploy`: prepare deployment, CI/CD, configuration, and rollback steps.
- `server-admin`: inspect and operate Linux servers safely.
- `security-review`: review code, configuration, and workflows for practical security risk.
- `incident-response`: triage, mitigate, communicate, and learn from production incidents.
- `interview-prep`: coordinate role-specific interview strategy and route focused practice.
- `coding-interview`: run algorithms, debugging, and live coding practice.
- `system-design-interview`: run architecture, scale, and tradeoff interview practice.
- `behavioral-interview`: prepare leadership, ownership, impact, and project stories.
- `refactor`: simplify changed code without changing behavior.
- `review`: pre-merge review for correctness, security, simplicity, robustness, and tests.
- `address-pr-feedback`: fetch GitHub PR feedback, judge each comment, fix valid issues, and verify.
- `browser-verify`: verify browser-rendered work in a real browser.
- `branch`: create a traceable Git branch with the ticket ID when available.
- `commit`: stage intended changes and write one clear Conventional Commit.

## Guidance

- Design docs default to `docs/<design-slug>/design.md`.
- One spec per feature, at `docs/<feature-slug>/spec.md`.
- Plans default to `docs/<feature-slug>/plan.md`. Push tasks to an issue tracker only when the user asks.
- If the task, spec, or plan is wrong, stop and update it. Do not push through.
- Tests are the verification mechanism; review checks they are real.
- Density over length.

## Out of Scope

AgentStack is not an issue tracker, architecture review board, or release process. It turns external context into high-quality instructions for coding agents. That's the entire job.
