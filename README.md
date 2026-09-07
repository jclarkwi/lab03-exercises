# Lab 03: Git and GitHub
This repository documents my practice with
local Git, GitHub, branches, and pull requests.
## README Responses

### 1.1 After initialization
```text
ls -la
total 12
drwxr-xr-x 3 johnc johnc 4096 Sep  3 10:04 .
drwxr-xr-x 5 johnc johnc 4096 Sep  3 10:04 ..
drwxr-xr-x 6 johnc johnc 4096 Sep  3 10:04 .git
```
### 1.2 First fit status
```text
git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)
```
### 1.3 After the first commit
```text
git status
On branch main
nothing to commit, working tree clean
```
### 1.4 git log
```text
git log --oneline
56f581c (HEAD -> main) Create lab README
```
### 1.5 git diff

Paste the `git status` and `git diff` commands and their output.
```text
git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

no changes added to commit (use "git add" and/or "git commit -a")
```
git diff
diff --git a/README.md b/README.md
index b0c0248..1e2f65c 100644
index b0c0248..1e2f65c 100644
index b0c0248..1e2f65c 100644
diff --git a/README.md b/README.md
index b0c0248..1e2f65c 100644
diff --git a/README.md b/README.md
index b0c0248..1e2f65c 100644
diff --git a/README.md b/README.md
index b0c0248..1e2f65c 100644
--- a/README.md
+++ b/README.md
@@ -1,5 +1,6 @@
 # Lab 03: Git and GitHub
-
+This repository documents my practice with
+local Git, GitHub, branches, and pull requests.
 ## README Responses

 ### 1.1 After initialization
@@ -24,9 +25,16 @@ Untracked files:
 nothing added to commit but untracked files present (use "git add" to track)
 ```
 ### 1.3 After the first commit
-
+```text
+git status
+On branch main
+nothing to commit, working tree clean
+```
 ### 1.4 git log
-
+```text
+git log --oneline
+56f581c (HEAD -> main) Create lab README
+```
 ### 1.5 git diff

How does this `git status` differ from the one in **1.2**?
```text
This git status shows uncommitted changes. 1.2 shows that there is nothing to commit.
```
### 1.6 Git command reflections

In one or two sentences each, what does each command do?

- `git init`: Reinitializes git repository.
- `git status`: Displays the files in the current directory that have not been committed, includes file edits.
- `git add`: Stages specified files to be committed.
- `git commit`: Saves a snapshot of all stages files when the commit is issued.
- `git log`: Shows commit history.
- `git diff`: Shows a lot of information including file contents.

### 1.7 Repository link
https://github.com/jclarkwi/lab03-exercises

### 1.8 Comparing approaches

In your own words:

- How does the nested-loop approach check for a duplicate?
	The nested-loop approach uses loops to compare values.
- How does the set-based approach check for a duplicate?
	The set-based approach uses a set to remember values. It compares the size of the set to the size of the
	input list.
- What is the runtime and memory trade-of of each?
	I don't know how to calculate runtime efficiency.

### 1.9 Pull request merge options

In your own words, what does each GitHub merge option do?

- Create a merge commit
- Squash and merge
- Rebase and merge
