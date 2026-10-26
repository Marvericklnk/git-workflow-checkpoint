# Git Workflow Checkpoint

## Status: terminal screenshots still required
The Git commands were executed by an assistant in a hosted Linux workspace at the user's request, not on the student's Windows laptop. These are real execution logs, not screenshots. This repository is not a complete screenshot submission yet.

## Evidence
- command-logs/01.txt through 17.txt: each exact command, output, exit code, and working directory.
- workflow.json: the same recorded results in structured form.
- learn_git.bundle: the original local Git repository history, preserved as a Git bundle.
- fourth.txt: final remaining practice file. third.txt was removed in the third practice commit.

The practice history contains, in order:
1. adding third.txt
2. adding fourth.txt
3. removing third.txt

The GitHub upload commits document uploading this evidence and are separate from the practice history. To inspect the original commits:

```bash
git clone learn_git.bundle learn_git
cd learn_git
git log
```

## Configuration
The command `git config --global core.pager cat` changed the hosted workspace's Git configuration. `git config --global --list` listed that workspace's global settings. Nothing on the student's Windows laptop was changed. The assistant used the user's GitHub no-reply address for the practice commit author identity through environment variables; the global configuration retained the workspace's default identity.

Step 17 (`git config --global` without an operation) prints "error: no action specified" and exits with status 129 on this installed Git version. No configuration operation was requested. Use git config -h for full help.

## Remaining work
Run the supplied steps on the student's laptop and add screenshots under a screenshots/ folder. Command logs do not replace the screenshots requested by GoMyCode. No terminal screenshots have been fabricated.
