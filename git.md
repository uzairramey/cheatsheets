# Git Cheatsheet

## The Four Places
Your Folder -> `git add` -> Staging Area -> `git commit` -> Local Repository -> `git push` -> GitHub

- **Your Folder:** Files that I am editing right now
- **Staging Area:** Changes that I have decided to save
- **Local Repository:** Saved commits (snapshots) on my mac
- **GitHub:** Saved files stored online

## First Commands
- `git innit` | Turns the folder into a local repository, so Git starts tracking it | `git innit` | Once per project, it creates a hidden `.git` folder that holds the history
- `git status` | Shows what has changed and where the change exists | `git status` | Does not change anything only reports so run it often after and before `add`
- `git add` | Moves the changes from your folder to staging area | `git add .` `git add git.md` | `.` means every change made simple `add` does nothing
- `git commit -m "message"` | Save everything in the staging area as a snapshot into your history | `git commit -m "Add today's learnings to learning-log"` | `-m` means message - a note about what you saved.
- `git log --oneline` | Shows your history, one line per commit | `git log --oneline` | Each line consists of the commit id and your message. Press `q` if enters scrolling view