# Git Version Control Practice

A compact learning repository used to practice the core Git workflow.

## Topics

- Local and remote repositories
- Commits and history
- Push and pull
- Branching basics
- Working with files under version control

## Status

Completed learning exercise retained for reference.

## Why this repository matters

This small exercise is a starting point for **controlled changes**, not a production deployment. Git records how a script, report or test evolved and makes a working version recoverable.

### A real workflow, using fictional files

```bash
git status --short
git switch -c docs/synthetic-report
git add README.md
git diff --cached
git commit -m "docs: describe sample reporting workflow"
git log --oneline -5
```

Before pushing, inspect `git diff --cached` and confirm that data extracts, passwords and generated files were not staged. A new commit does not mean a test passed.

| Skill | When it helps | Evidence |
|---|---|---|
| Small commits | Change Python validation without modifying unrelated calculations | Reviewable diff |
| Branches | Compare documentation or SQL explanations safely | Clear baseline and candidate |
| Pull requests | Review a proposed automation or reporting change | Reviewer, test notes and diff |
| Tags/releases | Identify a reviewed learning checkpoint | Version reference, not deployment proof |
| Revert | Undo a problematic committed change | Recoverable history |

### Practical exercise

Create a fictional `docs/metric-definition.md`. Change one definition, review the diff, and describe in a PR why it changed. Keep the original historical `Markdown_instruction.md` intact.

**RU:** Git нужен для контроля версий Python, SQL-методологии, тестов и отчётности: правки в ветках, diff, code review и воспроизводимый baseline.

Learn next: [Git Collaboration Guide](https://github.com/KonstantinOreshnikov/git-instruction-workshop) · [Integrated learning map](https://github.com/KonstantinOreshnikov/git-markdown-practice). Official: [Git documentation](https://git-scm.com/docs).
