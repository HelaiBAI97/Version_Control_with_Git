# Lab: (Command Line) Commit to a Local Repository

Estimated time: 10 minutes

> Note: This lab assumes that you are using a command line. If you would prefer to use
Sourcetree, there are separate instructions.
> 
> Note: If you are a Windows user, the command line instructions assume that you are
using **Git bash**.

In this lab, you will:
1. View file status using `git status`. 
2. Stage content using `git add`.
3. Commit content using `git commit`.
4. View the commit history using `git log`.

## 1: View file status using `git status`.
1. In a command line, navigate to your `projecta` directory and execute `git status`. You should see the message "Nothing to commit".
2. Create an empty file named `fileA.txt` in the `projecta` directory using `touch fileA.txt`. This is the first file in your working tree.
3. Execute `git status`. You should see that Git notices the `fileA.txt` file and identifies it as untracked.
> Congratulations, you have viewed an untracked file in your working tree.

## 2: Stage content using `git add`.
1. Add `fileA.txt` to the staging area using `git add fileA.txt`.
2. Execute `git status` again. You should see that Git adds `fileA.txt` under "Changes to be committed".
> Congratulations, you have staged a file.

## 3: Commit content using `git commit`.
1. Execute `git commit -m "add fileA.txt"` to create a commit. The -m option adds a commit message.
> Congratulations, you have created a commit.

## 4: View the commit history using `git log`.
1. Execute `git log`. You should see your commit details, including your commit message.
2. Execute `git log --oneline`. A concise version of the history is displayed.
3. You will not use the `projecta` repository in future labs. Feel free to delete it by simply
deleting the `projecta` directory.
> Congratulations. You have staged a file and created a commit.

Copyright © 2018 Atlassian