---
name: frontend-ui
description: "Build or update browser-facing UI. Use for frontend components, pages, forms, dashboards, responsive layouts, accessibility, visual states, and client-side interactions."
user-invocable: true
argument-hint: "<UI task, page, component, route, design, or spec path>"
---

# Frontend UI

Build usable, accessible, responsive UI that matches the product context and existing design system.

## Workflow

### 1. Ground

- Read the request, existing routes/components, design tokens, state management, tests, and data APIs.
- Identify users, workflow, content hierarchy, interaction states, and responsive constraints.
- Reuse existing components and styling conventions before creating new ones.

### 2. Design the Interaction

- Define loading, empty, error, success, disabled, validation, and permission states.
- Pick controls that match the action: inputs for data, selects for choices, toggles for booleans, icons for common tools.
- Keep workflows efficient for repeated use.

### 3. Implement

- Make scoped component and route changes.
- Keep layout stable across viewport sizes.
- Preserve accessibility: labels, keyboard flow, focus, contrast, and semantic markup.
- Avoid decorative complexity that does not help the task.

### 4. Verify

- Run component, unit, integration, or E2E checks that cover changed behavior.
- Use `browser-verify` for rendered pages when available.
- Check desktop and mobile layouts for overlap, clipping, unreadable text, and console errors.

## Rules

- Do not build a marketing landing page when the user asked for an app or tool.
- Do not leave broken loading or empty states.
- Do not introduce a new UI library when the project already has one unless asked.
- User-visible text should be clear, short, and specific.
