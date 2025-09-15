# Linux + Git Cheat Sheet

> Maintained by Your Name

---

## Linux Commands

### 1. `ls`
- List files and directories.  
- Useful flags:
  - `-l` long listing format
  - `-a` include hidden files
  - `-h` human-readable sizes  
- Examples:
  - `ls -la`
  - `ls -lh /usr/bin`

### 2. `cd`
- Change directory.  
- Examples:
  - `cd /usr/local` → move to /usr/local
  - `cd ..` → move up one level
  - `cd -` → switch back to previous directory

### 3. `pwd`
- Print working directory.  
- Shows the absolute path of your current location.  
- Example: `/Users/you/projects/git-cheatsheet`

### 4. `mkdir`
- Create new directories.  
- Examples:
  - `mkdir test` → create a folder named test
  - `mkdir -p a/b/c` → create nested directories

### 5. `rm`
- Remove files or directories.  
- Examples:
  - `rm file.txt` → delete a file
  - `rm -r folder/` → delete a directory recursively
  - `rm -i file.txt` → prompt before deleting

### 6. `cp`
- Copy files or directories.  
- Examples:
  - `cp a.txt b.txt` → copy file
  - `cp -r src/ backup/` → copy folder recursively

### 7. `mv`
- Move or rename files/directories.  
- Examples:
  - `mv old.txt new.txt` → rename
  - `mv file.txt ../` → move up a directory

### 8. `cat`
- Concatenate and print file contents.  
- Examples:
  - `cat file.txt`
  - `cat file1 file2 > combined.txt`

### 9. `less`
- View file contents one screen at a time.  
- Controls:
  - Space → next page
  - `b` → previous page
  - `/word` → search
  - `q` → quit  
- Example: `less bigfile.txt`

### 10. `grep`
- Search for patterns inside files.  
- Useful flags:
  - `-i` ignore case
  - `-n` show line numbers
  - `-R` search recursively  
- Examples:
  - `grep -i "error" logfile.txt`
  - `grep -R "TODO" .`

### 11. `find`
- Search for files and directories.  
- Examples:
  - `find . -name "*.py"` → all Python files
  - `find /tmp -type f -mtime -1` → files modified in last 24h

### 12. `chmod`
- Change file permissions.  
- Examples:
  - `chmod u+x script.sh` → make executable for user
  - `chmod 644 file.txt` → owner read/write, others read-only
  - `chmod -R 755 folder/` → set recursively

### 13. `chown`
- Change file owner/group.  
- Examples:
  - `sudo chown user file.txt`
  - `sudo chown user:staff file.txt`
  - `sudo chown -R user folder/`

### 14. `tar`
- Archive and extract files.  
- Useful flags:
  - `-c` create
  - `-x` extract
  - `-z` gzip
  - `-f` file name  
- Examples:
  - `tar -czf archive.tar.gz folder/` → create compressed archive
  - `tar -xzf archive.tar.gz` → extract archive

### 15. `ssh`
- Securely connect to remote machines.  
- Examples:
  - `ssh user@host`
  - `ssh -i ~/.ssh/id_ed25519 user@host`
  - `ssh -p 2222 user@host` → custom port

---

## Git Commands

### 1. `git init`
- Initialize a new Git repository.

### 2. `git status`
- Show working tree status (staged, unstaged, untracked).

### 3. `git add`
- Stage changes.  
- Examples:
  - `git add file.txt`
  - `git add .` → stage everything

### 4. `git commit`
- Record staged changes with a message.  
- Example: `git commit -m "Add feature"`

### 5. `git log`
- Show commit history.  
- Example: `git log --oneline --graph --decorate`

### 6. `git branch`
- List, create, or delete branches.  
- Examples:
  - `git branch` → list
  - `git branch feature` → create

### 7. `git checkout -b <name>`
- Create and switch to a new branch.  
- Example: `git checkout -b fix-bug`

### 8. `git merge <name>`
- Merge another branch into the current branch.  
- Example: `git merge feature`

### 9. `git remote add origin <url>`
- Add a remote repo.  
- Example: `git remote add origin git@github.com:user/repo.git`

### 10. `git push -u origin main`
- Push branch to remote and set upstream.

### 11. `git pull`
- Fetch and integrate changes from remote.  
- Example: `git pull origin main`

### 12. `git diff`
- Show changes between commits, branches, or working tree.  
- Example: `git diff HEAD`

### 13. `git clone <url>`
- Clone an existing repo.  
- Example: `git clone git@github.com:user/repo.git`

### 14. `git reset`
- Undo commits or unstage files.  
- Examples:
  - `git reset HEAD file.txt` → unstage
  - `git reset --hard <commit>` → reset everything

### 15. `git stash`
- Save changes temporarily without committing.  
- Example: `git stash save "work in progress"`




