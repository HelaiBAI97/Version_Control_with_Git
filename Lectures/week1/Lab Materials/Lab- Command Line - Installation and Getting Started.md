# Lab: (Command Line) Installation and Getting Started

Estimated time: 10 minutes

> Note: This lab assumes that you want to use a Command Line Interface (CLI) for this course. If you would prefer to use the Sourcetree graphical client, there are separate instructions.
> 
> Note: If you are a Windows user, the command line instructions assume you are using Git **bash**.

In this lab, you will:
1. Install the Git command line interface (if necessary).
2. Verify your Git version.
3. Explore Git help.
4. Configure your user name, email address and default Git editor.

## 1: Install the Git command line interface (if necessary).
1. If you have not installed Git, please use these instructions. 

		https://www.atlassian.com/git/tutorials/install-git.

> Congratulations, you have installed the Git CLI.

## 2: Verify your Git version.

1. Open a command line and verify that Git is installed.

```git --version```

2. If version information is not returned, install Git using task 1 of this lab.

> Congratulations, you have verified your Git version.

## 3: Explore Git help.

1. View overall Git help by typing `git` at the command line.
2. Choose any Git command that you see and view the help on it using `git help <command>`. For example, `git help init`.

3. View concise help on a command using the `-h` option. For example, `git init -h`.

> Congratulations, you have explored Git help.

## 4: Configure your user name, email address and default Git editor.

1. View your current setting for your user name with 

   `git config user.name`.

2. If you would like to change your user name, use 

   `git config --global user.name "Your Name"`.

3. View your current setting for your email address with 

   `git config user.email`.

4. If you would like to change your email address, use 

   `git config --global user.email "your@email"`.

5. View your current setting for default Git editor with 

   `git config core.editor`.

6. If you would like to change your default Git editor, use
   `git config --global core.editor your_preferred_editor`. nano seems to be a good

   editor for people who have not used vi or vim. Other options are Notepad++ (Windows) or Atom. Make sure that you install your editor before configuring it here.

   > Congratulations, you have configured your user name, email address and default editor.
> Congratulations. You have completed this lab.

Copyright © 2018 Atlassian