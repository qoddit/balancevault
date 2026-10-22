# GitHub Workflow

The project is hosted at [qoddit/balance](https://github.com/qoddit/balance). The recent local commit mentioned was `f2150d8` (`fix: improve TUI`), and a push was rejected because the remote had commits not present locally.

Recommended safe recovery:
```bash
git pull --rebase origin main
git push origin main
```
If conflicts occur, inspect `git status`, resolve deliberately, then continue the rebase. Avoid force-pushing unless intentionally replacing remote history.

Related: [[CONTRIBUTING.md]], [[Testing and Release]], [[.gitignore]].
