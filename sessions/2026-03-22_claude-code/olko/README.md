# Claude Code: Features, Tools, Skills — How to Be More Productive

**Presenter:** Olko
**Date:** 2026-03-22

## Summary

A practical introduction to Claude Code — an agentic AI coding tool by Anthropic.
We cover installation, core tools, and all the key productivity features:
CLAUDE.md, skills, agents, hooks, MCP. The session ends with a live demo
where we build a FastAPI app from an empty folder using only Claude Code.

## Talk Outline (~20 min)

| # | Topic | Time |
|---|-------|------|
| 1 | What is Claude Code & installation | 2 min |
| 2 | Core tools, CLI flags & interactive commands | 3 min |
| 3 | CLAUDE.md — persistent memory & rules | 3 min |
| 4 | Skills — reusable workflows & knowledge | 3 min |
| 5 | Agents (.claude/agents/) — custom subagents | 2 min |
| 6 | Hooks — deterministic automation | 2 min |
| 7 | MCP — connect external tools | 2 min |
| 8 | Best practices & productivity tips | 2 min |
| 9 | Live demo: empty folder -> tested API | 5 min |

## How to Run

The notebook walks through all topics as a presentation:

```bash
pip install jupyter
jupyter notebook notebook.ipynb
```

For the live demo:

```bash
# Install Claude Code
curl -fsSL https://claude.ai/install.sh | bash

# Create demo project
mkdir /tmp/demo-api && cd /tmp/demo-api
git init
claude
```

## Demo Files

| File | Description |
|------|-------------|
| `demo/CLAUDE.md.example` | Example project CLAUDE.md |
| `demo/skill-example.md` | Example `/fix-issue` skill (SKILL.md) |
| `demo/agent-example.md` | Example security-reviewer agent |
| `demo/hooks-example.json` | Example hooks configuration |

## Links

- [Claude Code Overview](https://docs.anthropic.com/en/docs/claude-code/overview)
- [Best Practices](https://docs.anthropic.com/en/docs/claude-code/best-practices)
- [CLAUDE.md & Memory](https://docs.anthropic.com/en/docs/claude-code/memory)
- [Skills](https://docs.anthropic.com/en/docs/claude-code/skills)
- [Agents (Subagents)](https://docs.anthropic.com/en/docs/claude-code/sub-agents)
- [Hooks](https://docs.anthropic.com/en/docs/claude-code/hooks)
- [MCP](https://docs.anthropic.com/en/docs/claude-code/mcp)
- [CLI Reference](https://docs.anthropic.com/en/docs/claude-code/cli-reference)
- [code.claude.com](https://code.claude.com/)
