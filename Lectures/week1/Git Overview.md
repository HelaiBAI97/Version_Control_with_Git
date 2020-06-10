# Git Overview
https://www.coursera.org/learn/version-control-with-git/lecture/WFdJp/git-overview
---

## Version Control Overview

Version control 
- Content
  - Complete history tracked and avaliable
- Teams
  - Supports many workflows
  - Collaboration
  - Quality through team communication and reviews
- agility
  - Manages small changes
  - Easily test, fix or undo ideas and changes

#### Distribute Version Control System (DVCS)
remote repository + many local repositories

- Each user has a local project history (repository)
- Users can work offline
- Can easily synchronize repositories

## Git Overview

- Git is a distribute version control system
- Open source software
  - Has vibrant community and ecosystem
- Adapts to many types of projects and workflows
  - Works well for large or small projects

A **Git Repository**: A series of snapshots, or commits.

## Command Line vs. User Interface

### Commits
Git manages versions of products forming a project history. Each version of a project is called a commit. Each commit is a snapshot of the entire project at a given point in time. Each unique file is stored only once.

### Branchs

All commits belong to a branch.

A branch can be thought of as an independent line of development of the project. By default, there is a single branch and it's called master.

You can create a separate branch and work on it independently of the master branch to maintain a stable project at the same time that you are working on it.

### Pull Requests

Merging independent branches using pull requests.

When a branch is ready to become part of the master branch, it can be merged into the master branch.

A pull request is a request to merge your branch into another branch. This request is usually made by developer of the branch when the feature, bug fix or other change is complete. During a pull request team members can discuss, review, and approve your changes. You can also require that automated test pass before the merge is allowed to happen.

If the pull request is accepted, your version of the project is merged and becomes the latest commit on the master branch.

---
# Quiz:
1. Which one of the following statements about version control is true?
    - [ ] You must be online to use distributed version control.
    - [x] With distributed version control, each user has a local copy of the project history.
        - Correct. Each user has a local repository, containing the project history as a collection of commits.
    - [ ] Version control only manages source code.

2. Which one of the following statements about Git is true?
    - [ ] Git is owned by a single company.
    - [ ] A commit only holds the changes to a project since the previous commit.
    - [x] Git can be used while offline.
        - Correct. If you have a local repository, you can continue to work while offline.