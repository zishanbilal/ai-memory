# Claude memory repo

This repo is Claude's long-term memory for Zeeshan Bilal. It lasts across sessions and is versioned with git.

## How to use it (instructions for Claude)

1. **At session start:** read `MEMORY.md` (the index), then open only the topic files relevant to the task.
2. **When something is worth remembering** (a decision, convention, preference, project fact, or a debugging finding that will matter again):
   - Update the matching file under `memory/`, or create a new one.
   - Add or update a one-line pointer in `MEMORY.md`.
   - Keep entries short and factual. Date them as `YYYY-MM-DD`.
3. **Correct, don't append:** if a fact changes, edit it in place instead of adding a contradicting entry.
4. **Never store secrets:** no tokens, passwords, keys, or customer data.
5. **After changes:** tell Zeeshan which files changed so he can commit and push (Claude has no GitHub push credentials).

## Layout

- `MEMORY.md`: the index. One line per memory file, with a short description.
- `memory/user.md`: who Zeeshan is, his role, and his working preferences.
- `memory/setup.md`: Claude tooling setup (plugins, connectors, known issues).
- `memory/projects/<name>.md`: one file per codebase or project.
- `memory/decisions.md`: notable technical decisions and why they were made.
