# Git Mastry

## LEVEL 1 — Git Basics

### Exercise 1: Initialize a Repo & First Commit
```bash
mkdir git-mastery && cd git-mastery
git init 
echo "# Git Mastery Project" > README.md 
git status                    # see untracked file
git add README.md             # stage it
git status                    # now it's staged
git commit -m "Initial commit: add README"
git log                       # see your commit
```

### Exercise 2: Staging Area Deep Dive

```bash
echo "Line 1" > file1.txt
echo "Line 2" > file2.txt
echo "Line 3" > file3.txt

git add file1.txt             # stage only file1
git add file2.txt file3.txt   # stage multiple
git status

# Oops — unstage file3
git restore --staged file3.txt
git status                    # file3 back to untracked

git commit -m "Add file1 and file2"
```

## Level 3
