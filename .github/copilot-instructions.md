# Copilot / AI agent instructions for pp-ai-ml-2026

Purpose: short, actionable guidance so an AI coding agent can be productive immediately.

- **Big picture:** This is a tiny learning repo for Python/AI-ML exercises. The primary content lives under `python_refresher/` as notebooks (currently `python_refresher/day1.ipyb`) and a minimal `README.md` at the repo root.

- **Key files:**
  - `README.md` — project description and context.
  - `python_refresher/day1.ipyb` — main notebook file (currently empty/whitespace).

- **Architecture / intent:** Not a production app. Expect single-author learning artifacts (notebooks, small scripts). Do not introduce large infra, services, or CI without explicit user approval.

- **Files & naming patterns:**
  - Keep notebooks in `python_refresher/`. New notebooks should use the standard `.ipynb` extension unless the user requests otherwise; note current file uses the nonstandard `.ipyb` extension—ask before renaming.
  - If adding runnable scripts, place them in `python_refresher/` and prefer descriptive names like `day2_data_loading.py` rather than top-level scripts.

- **Run / dev workflow (discoverable):**
  - There are no build or test scripts. Open notebooks in VS Code or Jupyter to run interactively.
  - If you need to add dependencies, propose a `requirements.txt` at the repo root and ask the user before modifying environment files.

- **When changing repo shape:**
  - Ask before introducing virtualenvs, CI, or heavy dependencies. This repository is educational; the user likely prefers minimal changes.

- **Patterns & examples:**
  - Notebook-first edits: prefer incrementally updating notebooks with small, self-contained cells and short explanatory markdown blocks.
  - Example: add a new notebook `python_refresher/day2.ipynb` demonstrating a single ML concept and update `README.md` with a one-line pointer.

- **PR / commit guidance for agents:**
  - Keep changes focused and small (one learning task per PR). Describe intent in the PR body and include a short usage note (how to run the notebook or script).

- **What to avoid:**
  - Do not add large dependency sets, CI pipelines, or refactors across multiple notebooks without asking.
  - Do not automatically rename `day1.ipyb` to `day1.ipynb` without confirming—flag this as a suggested improvement.

- **If you need to add tests or automation:**
  - Propose them in a short PR and ask for approval before implementing. Prefer small, targeted tests (e.g., a script-level smoke test) over a broad test framework.

If any section is unclear or you want the instructions to enforce stricter conventions (naming, PR size, dependency rules), tell me which parts to expand or tighten.
