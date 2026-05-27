---
name: technical-article
description: "Write high-quality technical articles with research, runnable examples, citations, review, optional author voice matching, and optional translation. Use for tutorials, deep dives, how-to guides, comparisons, architecture articles, debugging guides, and developer education content."
user-invocable: true
argument-hint: "<topic, audience, author, language, target platform, constraints, or article brief>"
---

# Technical Article

Create a technical article that is accurate, useful, cited, and backed by a complete example when the topic benefits from one.

## Workflow

### 1. Initialize

- Identify topic, audience, primary language, author voice needs, target platform, deadline, and whether an example is expected.
- Create `content/articles/YYYY_MM_DD_<slug>/` unless the user gives another location.
- Use `references/folder-structure.md` for artifact layout.
- If author profile data exists, load it and use `references/author-voice.md`.

### 2. Plan

- Classify the article type using `references/article-types.md`.
- Write `01_planning/outline.md` with thesis, reader promise, section outline, example plan, research questions, and done criteria.
- Pause for approval when the article is high-effort, public, opinionated, or requires a runnable project.

### 3. Research

- Use current primary sources when facts, APIs, versions, pricing, laws, security, or behavior may have changed.
- Follow `references/research.md`.
- Save source metadata to `02_research/sources.json` and notes to `02_research/research_notes.md`.

### 4. Draft

- Write the first draft in `03_drafts/draft_v1.<lang>.md`.
- Mark where examples belong with `<!-- EXAMPLE: purpose -->`.
- Explain concepts before using them. Separate facts, tradeoffs, and opinions.

### 5. Build Example

- Use `references/runnable-examples.md` and `references/stack-examples.md`.
- Create a complete example in `code/` unless the article type clearly does not need one.
- Install dependencies, run the example, and run tests or equivalent verification.
- If verification fails, fix and rerun before integrating the example.

### 6. Integrate

- Replace example markers with concise snippets, file references, and run instructions.
- Ensure snippets match the verified files in `code/`.
- Save the integrated draft as `03_drafts/draft_v2.<lang>.md`.

### 7. Review

- Review with `references/review-checklist.md`.
- Fix flow, accuracy, source quality, voice, example integration, commands, and missing context.
- Do not finalize until the article and example pass review or limitations are explicitly documented.

### 8. Finalize

- Use `references/frontmatter.md` when the platform needs metadata.
- Write the final article as `<slug>.<lang>.md`.
- Translate only when requested, using `references/translation.md`.
- Report final files, sources used, example verification, and any known gaps.

## Rules

- Do not invent facts, sources, benchmark numbers, author history, or production claims.
- Prefer official docs, source repositories, standards, release notes, and primary vendor material.
- Runnable examples must be complete enough for a reader to execute, not loose snippets.
- Skip examples only when they would not help the reader; document why.
- Keep code snippets short in the article and point to full files in `code/`.
- Respect copyright: quote sparingly, cite sources, and paraphrase in your own words.
