# Claude Code: Features, Tools, Skills — How to Be More Productive

**Presenter:** Olko
**Date:** 2026-03-22

## Summary

A practical introduction to Claude Code — an agentic AI coding tool by Anthropic.
We cover installation, core features, productivity techniques (CLAUDE.md, skills, hooks, MCP),
and demonstrate real workflows in a live terminal session.

## Talk Outline (~20 min)

| # | Topic | Time |
|---|-------|------|
| 1 | What is Claude Code & how to install | 3 min |
| 2 | Core tools & capabilities | 4 min |
| 3 | CLAUDE.md — persistent memory | 3 min |
| 4 | Skills & custom commands | 3 min |
| 5 | Hooks, MCP, subagents | 3 min |
| 6 | Best practices & productivity tips | 2 min |
| 7 | Live demo | 2 min |

## How to Run

The notebook walks through setup and examples step by step:

```bash
pip install jupyter
jupyter notebook notebook.ipynb
```

For the live demo scripts:

```bash
# Install Claude Code (pick one)
curl -fsSL https://claude.ai/install.sh | bash   # native (recommended)
brew install --cask claude-code                    # Homebrew

# Start Claude Code in any project
cd your-project
claude
```

## Links

- [Claude Code Overview](https://docs.anthropic.com/en/docs/claude-code/overview)
- [Claude Code Best Practices](https://docs.anthropic.com/en/docs/claude-code/best-practices)
- [CLAUDE.md & Memory](https://docs.anthropic.com/en/docs/claude-code/memory)
- [Skills](https://docs.anthropic.com/en/docs/claude-code/skills)
- [Hooks](https://docs.anthropic.com/en/docs/claude-code/hooks)
- [CLI Reference](https://docs.anthropic.com/en/docs/claude-code/cli-reference)
- [Common Workflows](https://docs.anthropic.com/en/docs/claude-code/common-workflows)
- [code.claude.com](https://code.claude.com/)
