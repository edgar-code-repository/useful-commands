GIT COMMANDS
-----------------------------------------------------------------------

Useful git commands.

-----------------------------------------------------------------------

**Global configuration:**
```
git config --global user.name "Your name"
git config --global user.email your-email@domain.com
```

**Local configuration:**
```
git config --local user.name "Your name"
git config --local user.email your-email@domain.com
```

**View all of your settings:**
```
git config --list
```

-----------------------------------------------------------------------

**Viewing commit history:**
```
git log
git log --oneline
git log --oneline --graph
```

-----------------------------------------------------------------------

**Cloning this repo:**
```
git clone https://github.com/edgar-code-repository/useful-commands
```

**Adding a remote:**
```
git remote add origin https://github.com/username/repo.git
```

**Listing remotes:**
```
git remote
git remote -v
```

-----------------------------------------------------------------------

**Staging and commiting a new file:**
```
git status

git add .                --> staging all files
git add file             --> staging one file
git commit -m "message"

```

-----------------------------------------------------------------------

**Soft and hard reset**

**Undoing the last commit (keeping the changes):**

```
git reset --soft HEAD~1
```

**Undoing the last commit (this also discard the changes in the working directory):**

```
git reset --hard HEAD~1

```

HEAD~1 -> is the commit previous to last commit

-----------------------------------------------------------------------

**Listing branches:**
```
git branch
```

**Creating a new branch:**
```
git branch branch-name
```

**Moving to new branch:**
```
git checkout branch-name
```

**Creating a new branch and moving to new branch in one step:**
```
git checkout -b branch-name
```

-----------------------------------------------------------------------

**Pulling changes from and pushing changes to remote:**
```
git pull remote-name branch-name
git push remote-name branch-name
```

-----------------------------------------------------------------------

**Pulling changes from one branch and take them to another branch:**

```
git checkout branch-A
git pull remote-name branch-A

git checkout branch-B
git merge branch-A
```

-----------------------------------------------------------------------


**Pulling changes from one branch and take them to another branch:**

```
git checkout branch-A
git pull remote-name branch-A

git checkout branch-B
git merge branch-A
```

-----------------------------------------------------------------------
