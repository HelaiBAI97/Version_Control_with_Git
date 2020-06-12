# Git Locations

https://www.coursera.org/learn/version-control-with-git/lecture/SMJIy/git-locations
---

**A PROJECT**

1. project directory
	1. working tree
	2. staging aera
	3. local repository
2. remote repository

## Working Tree

A single commit's directories and files.

A location in your computer that stores the directories and files, where you can view or edit the project.

## Staging Aera / Index

Store the files that are planned for the next commit.

## Local Repository

Contains the commits of the project.

## Project Directory

Including working tree, staging aera and local repository in your computer.

Myproject / working tree / .git    (The staging aera and local repository are stored in .git)

## Remote Repository

Contains the commits of the project.

---
# Quiz:
1. Which one of these statements is true?
    - [ ] The working tree is also called the index.
    - [ ] The working tree contains the history of the project.
    - [x] The staging area contains a list of files that will be in the next commit.
        - Correct.
2. Which one of these statements is true?
    - [ ] The project directory contains the local and remote repositories.
    - [ ] The project directory contains the remote repository.
    - [x] If you delete your project directory, you are also deleting your local repository.
        - Correct. Your project directory includes the working tree and a .git directory. The .git directory contains the local repository.