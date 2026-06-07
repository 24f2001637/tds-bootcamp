---
---

--- Before Day-2 ---

I already knew some programming, machine learning, and data science concepts, and had basic familiarity with deploying apps on cloud platforms like Vercel, but I wanted a deeper understanding of Linux internals and shell environments.

---

## Day-2 Checklist

- [x] I understand what `PATH` is and why commands like `python` work without full paths
- [x] I can navigate the filesystem without clicking - using `cd`, `ls`, and `pwd` only
- [x] I can read, search, and inspect files using `cat`, `head`, `tail`, `grep`, and `wc`
- [x] I can edit a file using `nano` (open, edit, save, exit)
- [x] I understand pipes (`|`) and redirection (`>`, `>>`, `2>`) and can chain commands
- [x] I can set an environment variable in `.bashrc` and apply it with `source ~/.bashrc`
- [x] I know the difference between `export VAR=value` (available to child processes) and just `VAR=value` (shell-local)

--- After Day-2 ---

I learned these things as well, apart from the checklist:
- How the `.bashrc` file automatically executes every time a new terminal session starts, which is great for setting up environments or running a startup command like `fastfetch`.
- How to extract compressed archives (`.tar.gz`) natively in the terminal using `tar -xzf`.
- How `echo $?` helps in debugging by returning the exit status code of the last run command (e.g., 0 for success, 1 for permission denied). 
- Writing out these technical explanations is proving to be a highly effective way for me to practice becoming a fluent English speaker alongside my undergraduate coursework.
---

--- Feedback (Suggestions for the TDS Team) ---

This is my feedback:
The visual breakdown mapping out parent and child processes to explain the `export` command was incredibly helpful. Showing how a variable stays trapped in the parent shell unless specifically exported made an abstract concept much easier to grasp. The live troubleshooting of the GitHub caching issue was also a valuable debugging lesson.

---

---
---

You can write your personal notes here; they will not be parsed and are for your own reference.
- `PATH` searches linearly through directories. The first match it finds is the one it executes.
- Always use `source ~/.bashrc` to refresh configuration settings without needing to restart the shell.
- `grep` is going to be incredibly useful for filtering text and parsing logs when working with data science datasets.
- `nano` essentials: `Ctrl+O` saves (Write Out), `Ctrl+X` exits.
- When commands fail, check `echo $?` to see if it's a permission issue or a missing file.
