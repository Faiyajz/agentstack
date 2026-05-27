# Runnable Examples

Examples must be complete, runnable, and verified.

Minimum structure:

```text
code/
├── README.md
├── src/
└── tests/
```

For framework projects, use the framework's normal project structure rather than isolated fragments.

Verification requirements:

1. Install dependencies successfully.
2. Run setup commands successfully.
3. Start or execute the example successfully.
4. Run tests, checks, or equivalent verification successfully.
5. Document commands in `code/README.md`.

If any step fails:

- read the error
- fix the example
- rerun verification
- do not integrate the example as working until it passes

`code/README.md` should include:

- what the example demonstrates
- requirements
- setup commands
- run commands
- test/check commands
- key files
- article section references

Skip examples only for content where they add no value, such as pure opinion, news summaries, historical retrospectives, or philosophical essays. Document the skip reason in the planning notes.
