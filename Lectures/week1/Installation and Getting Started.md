# (Command Line) Installation and Getting Started

https://www.coursera.org/learn/version-control-with-git/lecture/AiSks/command-line-installation-and-getting-started
---
## Installing Git

Verify that Git is installed:

`$ git --version`

## Git Synax

`git [command] [--flags] [arguments]`

## Getting Help

`git help [command]`

`git <command> -h`

##### Reading Help: https://github.com/git/git/blob/master/Documentation/CodingGuidelines

`git fakecommand (-p|--patch) [<id>] [--] [<paths>...]`

- `-f` or `--patch` Change the command's behaviour
- `|` Or
- `[optional]`
- `<placeholder>`
- `[<optional placeholder>]`
- `()` Grouping
- `--` Disambiguates the command
- `...` multiple occurance possible

## Configuring User Information and the Default Editor

`git config [-local|--global|--system] <key> [<value>]`

- The `--system` flag applies for every repository for all users on your computer
- The `--global` flag applies for every repository that you use on your computer
- No flag or `--global` applies only to the current repository (highest precedence)

Set user name and email

```
$ git config --global user.name "Pat"
$ git config --global user.email "pat@example.com"
```

Check the value

`git config <key>`

Specify an editor that you like:

`$ git config --global core.editor nano`

