# Commit to a Local Repository

https://www.coursera.org/learn/version-control-with-git/lecture/zBlSu/command-line-commit-to-a-local-repository
---

## View file status using `git status`

Use `git status` to view the status of files in the working tree and staging aera.

<pre><code>myproj % <b>git status</b>
On branch master

No commits yet

nothing to commit (create/copy files and use &quot;git add&quot; to track)
myproj % <b>touch fileA.txt</b>
myproj % <b>git status</b>
On branch master

No commits yet

Untracked files:
  (use &quot;git add &lt;file&gt;...&quot; to include in what will be committed)

  <font color=red>fileA.txt</font>

nothing added to commit but untracked files present (use &quot;git add&quot; to track)
</code></pre>

## Stage content using `git add`

Use `git add <file-or-directory>` to add files into staging area.

<pre><code>
myproj % <b>git add fileA.txt</b>
myproj % <b>git status</b>
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	<font color=green>new file:   fileA.txt</font>


</code></pre>

Add directories with `git add <directory>`

<pre><code>
(create dirA and dirA/fileA.txt, dirA/fileB.txt)
myproj % <b>git status</b>
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

	<font color=red>dirA/</font>

nothing added to commit but untracked files present (use "git add" to track)
myproj % <b>git add dirA</b>
myproj % <b>git status</b>
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	<font color=green>new file:   dirA/fileA.txt</font>
	<font color=green>new file:   dirA/fileB.txt</font>

</code></pre>

Add all untracked or modified files using `git add .`

<pre><code>
myproj % <b>touch fileA.txt</b>
myproj % <b>touch fileB.txt</b>
myproj % <b>git add .</b>
myproj % <b>git status</b>
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

	<font color=green>new file:   fileA.txt</font>
	<font color=green>new file:   fileB.txt</font>

</code></pre>

Modified file

<pre><code>
myproj % <b>touch fileA.txt</b>               # create fileA.txt
myproj % <b>git status -s</b>                 # -s means short status
<font color=red>??</font> fileA.txt                           # <font color=red>??</font> means untracted
myproj % <b>git add fileA.txt</b>
myproj % <b>git status -s</b>
<font color=green>A</font>  fileA.txt                           # <font color=green>A</font> means added (staged)
myproj % <b>echo "feature 1" > fileA.txt</b>  # modify fileA.txt
myproj % <b>git status -s</b>     
<font color=green>A</font><font color=red>M</font> fileA.txt                           # <font color=green>A</font><font color=red>M</font> means added and modified
myproj % <b>git add fileA.txt</b> 
myproj % <b>git status -s</b>
<font color=green>A</font>  fileA.txt
</code></pre>

## Commit content using `git commit`

Add staged content to the local repository as a commit.
- Previously committed files are also included.
- Creates a snapshot of the entire project.

<pre><code>
myproj % <b>git commit -m "initial commit"</b>
[master (root-commit) a968663] initial commit
 1 file changed, 1 insertion(+)
 create mode 100644 fileA.txt
myproj % <b>git status</b>
On branch master
nothing to commit, working tree clean
</code></pre>

## View the commit history using `git log`

`--oneline` condensed version of the log
`-#` limit the log to the most recent # commits

<pre><code>
myproj % <b>git log</b>
commit <font color=CC9900>a9686631b123a61fec53005d4c273f36b329215f (</font><font color=00CCFF>HEAD -></font> <font color=green>master</font><font color=CC9900>)</font>
Author: Helai Bai <baiyihe@163.com>
Date:   Mon Jun 15 12:53:15 2020 +0800

    initial commit
myproj % <b>git log --oneline</b>
<font color=CC9900>f6b93b0 (</font><font color=00CCFF>HEAD -></font> <font color=green>master</font><font color=CC9900>)</font> Add feature 2
<font color=CC9900>b0c11b2</font> Update fileA.txt
<font color=CC9900>a968663</font> initial commit
myproj % <b>git log --oneline -2</b>
<font color=CC9900>f6b93b0 (</font><font color=00CCFF>HEAD -></font> <font color=green>master</font><font color=CC9900>)</font> Add feature 2
<font color=CC9900>b0c11b2</font> Update fileA.txt
</code></pre>

---
# Quiz:
1. Which one of the following statements is true?
    - [ ] A staged file will show as modified.
    - [ ] A staged file will show as untracked.
    - [x] A staged file will be part of the next commit.
        - Correct. The staging area contains a list of files that will be in the next commit.
2. Which one of the following statements is true?
    - [ ] A commit message is not part of the project history.
    - [x] The 'git log' command lists the commits of the project.
        - Correct.
    - [ ] A commit always contains only one file.