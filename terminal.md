# Termainal Cheatsheet (macOS)

## Navigation
- `pwd` | Show current folder | `pwd`
- `cd` | Change folder | `cd ~/Documents`
- `cd ..` | Go to one up folder | `cd ..`
- `ls` | List all files | `ls` `ls Documents` `ls -la` (for details)
- `mkdir` | Create folder(s) | `mkdir backup` `mkdir backup data`
- `touch` | Make a empty file | `touch head.txt` `touch hello.py title.txt`
- `cat` | Shows file's content | `cat head.txt`
- `rm` | Delete (No recycle bin) | `rm title.txt` `rm -r data` (-r for folders)
- `clear` | Clear the screen | `clear`
- `echo` | Overwrite(>) or Add(>>) to end of a file | `echo "print("Hello World")" > hello.py`
- `open .` | Open the current folder in Finder | `open .`
- `open` | Open the file with it's default app | `open title.txt` `open hello.py`

## Files
### cp (Copy)
- **Syntax:** `cp source destination`
- **Example:** `cp head.txt data/` `cp -iv title.txt backup/` (-iv provides a prompt before anything is overwritten and confirmation of what happened)
- **Gotcha:** needs `-r` for folders; overwrites silently without `-i` 

### mv (Move/Rename)
- **Syntax:** `mv source destination`
- **Example:** `mv title.txt data/` `mv title.txt data.txt`
- **Gotcha:** no trash, double check the destination

## Flags
### Looking Around
- `ls -la` | List all files, including hidden ones, with details
- `ls -lh` | Long list with human-readable sizes
- `ls -lt` | Long list, newest files first
- `cat -n file` | Show a file with line numbers

### Files & Folders
- `cp -iv head.txt title.txt` | Copy, ask before overwriting, show what happened
- `cp -r folder/ backup/` | Copy a folder and everything inside it
- `mv -iv title.txt head.txt` | Move or Rename, ask before overwriting
- `mkdir -p data/backup/phone` | Create nested folders in one go
- `rm -i file.txt` | Delete a file, ask first
- `rm -r backup/` | Delete a folder and its contents (permanently)

### Getting Help
- `man ls` | Full manual (`q` to quit)
- `python3 --version` | Check an installed version

### Git
- `git status -s` | Short summary of changes
- `git add .` | Stage all changes
- `git commit -m "message"` | Commit with a message
- `git commit -am "message"` | Stage tracked files and commit (skip new files)
- `git diff --staged` | See what you are about to commit
- `git clone <url>` | Copy a repo to your computer
- `git pull` | Download the latest changes from github

### Python & Pip
- `python3 -m venv venv` | Create a virtual enviroment named `venv`
- `source venv/bin/activate` | Activate virtual enviroment (`deactivate` to leave)
- `pip install package` | Install a package
- `pip install -U package` | Upgrade a package
- `pip install -r requirements.txt` | Install everything listed in a file
- `pip freeze > requirements.txt` | Save installed packages to a file
- `pip list` | Show installed packages

