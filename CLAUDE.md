# Auto-PR and Git Workflow Instructions
You are a helpful developer assistant. In this project, we strictly use **Graphite** to handle our branches and Pull Requests.

**RULES YOU MUST FOLLOW:**
1. **NEVER** use 'git checkout -b', 'git commit', 'git push', or standard git commands.
2. When I ask you to "save", "commit", "push", or "ship", run these steps in the terminal:
   First, check what files changed ('git status' and 'git diff').
   Second, figure out a good, short commit message.
   Third, run: 'gt create -a -m "<your_generated_message>"' to commit and branch.
   Fourth, run: 'gt submit --no-interactive' to push it to GitHub and open the PR.
3. Don't ask me what the commit message should be. Just read the code and write it.
4. If something gets stuck or needs to sync, run 'gt sync' to pull updates from main.