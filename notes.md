# Git notes
This a notebook for git training
<!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-refresh-toc -->
**Table of Contents**

- [Git notes](#git-notes)
    - [Undoing things](#undoing-things)

<!-- markdown-toc end -->

## Undoing things ##

### Unstaing a staged file ###

Create `ala.txt` file. And stage it

```bash
touch ala.txt
git add ala.txt
```
Check that `ala.txt` is in the staging area:

```bash
git status
```
The output below says that `ala.txt` is a `new file`.
```
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

        new file:   ala.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        .#notes.md
        notes.md
```
To remove it from a staged area issue commands

```bash
git rm --cached ala.txt
```
