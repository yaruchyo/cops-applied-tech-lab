# CoPS Applied Tech Lab

**Community of Practices** — a space to launch your own projects and level up your tech stack.

## Our Motivation

- Exchange ideas
- Technical support
- Share experience

## Meeting Agenda (~1 hour)

| Time | Activity |
|------|----------|
| 20 min | Practical talk / watch a 20-min video together |
| 10-15 min | Q&A |
| Remaining | Free format — Demo & Support. Share screens, show progress, get feedback |

## 4 Iron Rules

1. **Show, don't just tell.**
2. **No guilt.** Didn't have time this week because of your full-time job? Still come. We're here for support, not status reports.
3. **Respect the timebox.** Keep presentations within 20 minutes.
4. **Give feedback generously.** When someone shares — engage.

---

## Repository Structure

```
cops-applied-tech-lab/
├── README.md
├── sessions/
│   └── YYYY-MM-DD_session-topic/       # one folder per session
│       ├── README.md                    # session summary & links
│       ├── presenter-name/             # one subfolder per presenter
│       │   ├── notebook.ipynb
│       │   ├── slides.pdf
│       │   ├── demo/
│       │   │   └── ...
│       │   └── requirements.txt        # optional, for extra deps
│       └── another-presenter/
│           └── ...
```

## How to Add Your Presentation / Demo

### 1. Create a branch

```bash
git checkout -b session/YYYY-MM-DD-your-name
```

### 2. Create your session folder

```bash
mkdir -p sessions/YYYY-MM-DD_session-topic/your-name
```

Replace:
- `YYYY-MM-DD` with the session date (e.g. `2026-03-25`)
- `session-topic` with a short slug (e.g. `rag-pipelines`)
- `your-name` with your name or GitHub handle

### 3. Add your materials

Place any of the following inside your folder:

| Type | Examples |
|------|----------|
| Jupyter Notebooks | `*.ipynb` |
| Slides | `slides.pdf`, `slides.pptx` |
| Scripts | `*.py`, `*.sh` |
| Demo apps | `demo/` subfolder with its own README |
| Data files | Small datasets only (<10 MB). Use links for large files |
| Dependencies | Add to `pyproject.toml` or use a local `requirements.txt` |

### 4. Add a short README in your folder

Create `sessions/YYYY-MM-DD_session-topic/your-name/README.md`:

```markdown
# Talk Title

**Presenter:** Your Name
**Date:** YYYY-MM-DD

## Summary
Brief description of what you presented or demoed.

## How to Run
Instructions to reproduce the demo (if applicable).

## Links
- [Relevant article](https://example.com)
```

### 5. Open a Merge Request

```bash
git add .
git commit -m "Add session YYYY-MM-DD: your-topic by your-name"
git push origin session/YYYY-MM-DD-your-name
```

Then open a Merge Request to `main`.

---

## Naming Conventions

| What | Convention | Example |
|------|-----------|---------|
| Session folder | `YYYY-MM-DD_short-topic` | `2026-03-25_rag-pipelines` |
| Presenter folder | lowercase, hyphens | `oleksii-y` |
| Branch name | `session/YYYY-MM-DD-your-name` | `session/2026-03-25-oleksii-y` |
| Commit message | `Add session YYYY-MM-DD: topic by name` | `Add session 2026-03-25: rag-pipelines by oleksii-y` |

## Prerequisites

Install [uv](https://docs.astral.sh/uv/) (macOS):

```bash
brew install uv
```

Or via the official installer:

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

## Setup

```bash
uv sync
```

For Jupyter notebooks:

```bash
uv run jupyter notebook
```
