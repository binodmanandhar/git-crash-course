# GIT COMMANDS

```
git init
git add .
git commit -m "initial commit"
git remote add origin <repo-url>
git push -u origin main
```

#### to uncommit the commit but the revert is logs

```
git revert <id>

```

#### Quick cheat sheet

```
i → enter insert mode (start typing)

Esc → leave insert mode

:wq → save and quit

:q! → quit without saving
```

#### Git RESET

```
git reset --hard <id>
eg: git reset --hard 6b7c4d5
```

Be careful. If there are C1, C2, C3, C4, C5 commit.

if you reset to C2 log, then C3, C4, C5 will be deleted and cannot be recovered.

#### CREATE NEW BRANCH

```
git checkout -b <branch-name>
eg: git checkout -b FEAT/redirection
```

#### TO DELETE BRANCH

```
git checkout main
git branch -D FEAT/redirection
```

#### MERGE NEW BRANCH CHANGES TO MAIN BRANCH

```
git checkout main
git merge FEAT/animation
```

#### Suppose you are new branch and there is new commit in MAIN branch.

##### To pull changes into NEW BRANCH from MAIN BRANCH

```
git checkout new-branch
git merge main
```

---

#### After creating NEW BRANCH

```
git add .
git commit -m "message"
git push origin <branch-name>    //for first time then we can use git push
```

---

# GITHUB ACTIONS:

- Workflows
- Jobs
- Steps

#### FLOW

- Workflow 1 (Attached to a GitHub repository, contain one or more Jobs, Triggered upon Events)
  - Job 1 ( Define a Runner - execution environment )
    - Step 1 ( Execure a shell script or an Action, Can use customs or third-party actions)
    - step 2
  - Job 2
    - Step 1
