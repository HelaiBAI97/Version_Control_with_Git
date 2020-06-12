# Lab: (Command Line) Create a Local Repository

Estimated time: 5 minutes

> Note: This lab assumes that you are using a command line. If you would prefer to use
Sourcetree, there are separate instructions.
> 
> Note: If you are a Windows user, the command line instructions assume that you are
using **Git bash**.

In this lab, you will:
1. Initialize an empty local Git repository using git init .

## 1: Initialize an empty local Git repository using `git init`.
1. (If necessary) Create a repos directory for all your local repositories.
   You can create this in your user directory (~).

```
$ cd # this will change to your user directory
~$ mkdir repos
```

2. In your `repos` directory, create a project directory named `projecta`. This will be
your first local repository.

```
~$ cd repos
repos$ mkdir projecta
```

3. Change to your `projecta` directory and initialize a repository.

```
repos$ cd projecta
projecta $ git init
Initialized empty Git repository in projecta/.git/
```

Notice that Git informs you that an empty Git repository was initialized.

4. Verify that your `projecta` project directory contains a `.git` directory.

```
projecta $ ls -a
. .. .git
```

> Congratulations. You have created a local repository.

Copyright © 2018 Atlassian