# Git notes
This a notebook for git training
<!-- markdown-toc start - Don't edit this section. Run M-x markdown-toc-refresh-toc -->
**Table of Contents**

- [Git notes](#git-notes)
    - [Undoing things](#undoing-things)
        - [Unstage a file](#unstage-a-file)
        - [Remove a file from the staging area -- it will be **deleted**](#remove-a-file-from-the-staging-area----it-will-be-deleted)
        - [Reverting local changes](#reverting-local-changes)

<!-- markdown-toc end -->

## Undoing things ##

### Unstage a file ##
`bash
git reset HEAD ala.txt
git commit -m "the file 'ala.txt' is still in the repository"
`

### Remove a file from the staging area -- it will be **deleted** ##

`bash
git rm --cached ala.txt
git commit -m "the file 'ala.txt' is gone from the repository"
`

### Reverting local changes ##

` bash
git checkout -- ala.txt
`
## Remote repos ##

> You can have more than one remote repo.

### Add remote ###

`bash
git remote add github https://github.com/WitJakuczun/gittrain_remote.git
`

### List all remotes  ###

`bash
git remote -v
`
