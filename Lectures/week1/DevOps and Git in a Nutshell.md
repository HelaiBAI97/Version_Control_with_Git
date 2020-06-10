# DevOps and Git in a Nutshell
https://www.coursera.org/learn/version-control-with-git/lecture/ySzMb/devops-and-git-in-a-nutshell
---

DevOps: modern software development practices

## Continues Improvement

DevOps has a few fundamental principles that most modern software projects follow. One of the key principles is to **continuously plan, build and release small improvements** to your product.

Waterfall approach, in which many features are planned, developed and released as one batch.

## Managing Project Versions

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
1. Which one of these statements about continuous improvement is true?
    - [ ] Continuous improvement applies to bugs, but not features.
    - [x] Small batch size leads to continuous improvement.
        - Correct. The integration of many small changes to the project leads to a continuously improving project.
    - [ ] Continuous improvement applies to features, but not bugs.

2. Which one of these statements about commits is true?
    - [ ] A commit contains only the changes to the project since the previous commit.
    - [x] The collection of commits contain the project's history.
        - Correct. A commit is a snapshot of the project in time, and the collection of commits contains the project's history.
    - [ ] A commit contains the project's history.
    
3. Which one of these statements about branches is true?
    - [x] Branches enable independent development of the project.
        - Correct. A branch can be created to work on a version of the project that other branches do not know about.
    - [ ] All commits must belong to the master branch.
    - [ ] Only one branch per project is allowed.

4. Which one of these statements about pull requests is true?
    - [ ] A pull request is a request to create a branch.
    - [ ] A pull request is a request to download the project.
    - [x] Pull requests can include team review and testing, improving product quality.
        - Correct. A pull request is a request for others to review and approve the changes made to the project on a branch.