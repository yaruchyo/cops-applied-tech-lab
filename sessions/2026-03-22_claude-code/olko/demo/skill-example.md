---
name: fix-issue
description: Fix a GitHub issue by number
disable-model-invocation: true
---

Analyze and fix the GitHub issue: $ARGUMENTS.

1. Use `gh issue view $ARGUMENTS` to get the issue details
2. Understand the problem described in the issue
3. Search the codebase for relevant files
4. Implement the necessary changes
5. Write and run tests to verify the fix
6. Run lint and type checks
7. Create a descriptive commit message
8. Push and create a PR linking the issue
