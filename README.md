# GIT-TASK

## Level 1: Introduction to Git Commits

### Two commits

In this excercise, we need to make two commits in the main branch.

## Level 2: Branching in Git

### Create a branch

With **git checkout -b bugFix**, i created a new branch called bugFix.

## Level 3: Merging in Git

### Merge the bugFix branch to main

After create the bugFix branch, i went back to the main branch and merged the bugFix branch into it with **git merge**.

## Level 4: Rebase introduction

### Git rebase command

This command help us to merge the commits made in a branch to a top branch. For example, i can merge the commits in bugFix to main with **git rebase main**.

## Level 5: Detach yo' HEAD

### HEAD

HEAD label shows what are the current commit in the branch. Using **git checkout <any commit>** we can attach HEAD to any commit in the branch.

## Level 6: Relative refs (^) 

### Caret

With the caret (^), we can label the parent commit of the current commit. For example, if C3 is the parent of C4, when we use the **git checkout C4^**,
we are labeling HEAD to C3, who is the parent.

## Level 7: Relative refs #2 (~)

### Tilde

With the tilde (~), we can label the HEAD with an ancestor. For example, if we got the C4->C3->C2->C1 and the HEAD is on C4, we can use **git checkout HEAD~3**
and HEAD moves to C1. Also, with **git branch -f <branch> HEAD** we can force the branch to move to the current HEAD or the parent/ancestor with adding the tilde.

