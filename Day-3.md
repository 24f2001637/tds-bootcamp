---
---

--- Before Day-3 ---

I already knew how to deploy projects using cloud platforms like Vercel and write standard Python code for my undergraduate machine learning and data science coursework, but my approach to dependency management was mostly limited to using standard global `pip` installs.

---

## Day-3 Checklist

- [x] I can run a Python script using `uv run script.py` without setting up a local virtual environment
- [x] I know where the temporary virtual environment is created when running the `uv add --script script.py pandas` command followed by `uv run script.py`
- [x] I can create a new Python project using `uv init` and understand what `pyproject.toml` is used for
- [x] I can add a dependency (e.g., `requests`) using `uv add` and see it reflected in the lockfile
- [x] I can create a traditional virtual environment using `uv venv` and know when to use it
- [x] I understand why installing packages globally with `pip install` is a bad habit
- [x] I can open a project in VS Code, select the correct Python interpreter, and run code from the integrated terminal
- [x] I know the difference between a `.py` script and a `.ipynb` notebook, and when to use each

--- After Day-3 ---
I learned these things as well, apart from the checklist:
- How Astral's `uv` acts as a lightning-fast replacement for traditional package managers, capable of automatically pulling down required Python versions (like swapping from 3.14 to 3.12 on the fly).
- The difference between Zsh and Bash, and how to use plugins like auto-suggestions to speed up terminal workflows.
- Important VS Code productivity shortcuts like `Ctrl+D` for multi-cursor editing, `Ctrl+B` to toggle the sidebar, and selecting the correct Python interpreter via the command palette.
- How `.gitignore` protects sensitive files (like `.env` API keys) from accidentally being pushed to public repositories.
---

--- Feedback (Suggestions for the TDS Team) ---

This is my feedback:
The introduction to `uv` was eye-opening. Transitioning from standard `python -m venv` to `uv init` and seeing how it handles `pyproject.toml` and lockfiles automatically makes project structuring feel much more professional. I also appreciate the communication practice these written summaries provide as I actively work toward becoming a more fluent English speaker.

---

---
---

You can write your personal notes here; they will not be parsed and are for your own reference.
- `uv init` scaffolds a project with a `README.md`, `.gitignore`, `pyproject.toml`, and `main.py`.
- `uv add requests` installs the dependency and strictly logs it in the `uv.lock` file.
- In VS Code, use `Ctrl+Shift+P` -> `Python: Select Interpreter` to ensure the terminal uses the project's `.venv` instead of the global bin.
- AI Pipe (the IIT Madras tool) provides a $1/week allowance for accessing premium LLM models for assignments.
- Markdown reminders: use `**` for bold, `*` for italic, and triple backticks for syntax-highlighted code blocks.
