--- Before Day-5 ---

I already knew how to push basic code to GitHub to trigger cloud deployments on platforms like Vercel, but I mostly relied on GUI tools or rote memorization of terminal commands without a deep understanding of the staging area, SSH authentication, or reverting history.

--- 

## Day-5 Checklist

- [x] I have set up the basic Git configuration using `git config --global user.name "Your Name"`, `git config --global user.email "your.email@example.com"`, and set the default branch as main using `git config --global init.defaultBranch main`
- [x] I know GitHub allows only one user account per person, so I have merged my accounts (IITM and personal) into a single unified account
- [x] I understand the three states of a file in Git: working tree → staging → committed
- [x] I can run the daily workflow commands `git status`, `git diff`, and `git log` and know what each shows
- [x] I know how `.gitignore` works and how to use it to ignore files and folders that should not be pushed to the remote repository (e.g., `venv`, `__pycache__`, `.env`)
- [x] I can make a commit: `git add` → `git commit -m "message"` → `git push`
- [x] I know what `origin` and `main` are and can explain them in one sentence each
- [x] I can set up SSH key authentication and push to GitHub without entering a password
- [x] I can create an annotated tag (`git tag -a v0.1.0`) and push it to GitHub
- [x] I can write a meaningful commit message (not "fixed stuff" or "final.py")

--- After Day-5 ---

I learned these things as well, apart from the checklist:
* How external API schema changes (like a server suddenly swapping a JSON response from a dictionary to a list) can instantly break your analysis scripts, making `git revert` crucial for quickly rolling back to a previously working state.
* How to manage WSL disk space issues, specifically by using commands like `ollama rm <model_name>` to delete heavy local LLMs taking up gigabytes on the C drive.
* Writing these detailed daily reflections over the past week has been fantastic practice for structuring my technical thoughts and working toward my goal of becoming a more fluent English speaker.
---

--- Feedback (Suggestions for the TDS Team) ---

This is my feedback:
The storytelling approach used to explain Git—demonstrating a script breaking over several days due to server schema updates—made the "why" of version control much clearer than just memorizing the syntax. The live troubleshooting at the end regarding WSL partition space was also highly practical. 

---

---
---

Personal Notes:
* Remember to always copy the `.pub` (public) key when adding an SSH key to GitHub settings, never the private key.
* `git add .` stages all untracked and modified files in the current directory.
* Never commit `.env` files; API keys will be exposed and scraped. Use `.env.example` as a template instead.
