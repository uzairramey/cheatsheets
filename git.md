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

## Next Commands
- `git branch` | Lists the name of the all branches. * is with the one you are on | `git branch`
- `git branch -M name` | Rename the branch (-M renames or moves even if the name is taken) | `git branch -M main` 
- `git remote add origin <URL>` | Registers a remote (second copy) called origin that points to my repo's address on GitHub | `git remote add origin https://github.com/uzairramey/cheatsheets.git`
- `git remote -v` | It lists the remotes (second copy), `-v` means it also tells the address | `git remote -v`
- `git push -u origin main` | Push upload the commits, `origin main` uploads my local `main` branch to the remote called `origin` (-u helps it remember the pairing so next time `git push` is enough) | `git push -u origin main`
- `git clone <URL>` | Copies a whole repo from GitHub, along with full history | `git clone https://github.com/uzairramey/cheatsheets.git` `git clone https://github.com/uzairramey/cheatsheets.git cheatsheets_copy` (Rename the folder)| Once per project per computer; sets up `origin` automatically; don't clone it in another repo folder
- `git pull` | Downloads new commits from GitHub and uploads to the new branch | `git pull` | Use before starting work; commit my own work before
- `git pull --no-rebase` | In case of conflict it combines using a merge, not a rebase | `git pull --no-rebase`