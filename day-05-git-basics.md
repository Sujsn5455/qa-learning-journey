\# Day 5 — Git Basics



\## What is Git?

Git is a version control system that tracks changes to files over time.



\## Why Git Matters for QA

\- Store test scripts

\- Collaborate with team

\- Review changes

\- Enable CI/CD automation



\## Core Concepts



\### Repository

A folder tracked by Git.



\### Commit

A snapshot of files at a point in time.



\### Branch

A separate line of work.



\### Main Branch

The primary branch (main or master).



\### Remote

A copy on a server (GitHub).



\### Working Directory

Your actual files on disk.



\### Staging Area

Where files go after git add but before git commit.



\### HEAD

Pointer to current commit or branch.



\## Three States of a File

Working Directory → Staging Area → Repository

(edit)              (git add)        (git commit)



\## Essential Git Commands

| Command | What It Does |

|---------|--------------|

| git init | Creates new repo |

| git status | Shows current state |

| git add . | Stages all changes |

| git commit -m "msg" | Saves snapshot |

| git log --oneline | Shows commit history |

| git branch | Lists branches |

| git checkout -b name | Creates and switches branch |

| git merge name | Merges branch into current |

| git pull | Fetches from remote |

| git push | Sends to remote |

| git remote -v | Shows remote URLs |

| git branch -d name | Deletes branch |



\## Branching Workflow

1\. Create branch: git checkout -b feature-name

2\. Make changes

3\. Stage: git add .

4\. Commit: git commit -m "message"

5\. Switch back: git checkout main

6\. Merge: git merge feature-name

7\. Delete branch: git branch -d feature-name



\## Salon Project Application

\- main branch → stable code

\- feature/login-tests → login test cases

\- feature/booking-tests → booking test cases

\- bugfix/past-date-bug → fix for past date bug



\## Key Takeaway

Git tracks history. Branches let you work safely. Merge brings work together.

