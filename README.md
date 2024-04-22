# Git exercise project

Bundle 1 
exercise 1:

REBECCA@DESKTOP-7D5E1TE MINGW64 ~/Git_Exercises
$ git init
Initialized empty Git repository in C:/Users/REBECCA/Git_Exercises/.git/

REBECCA@DESKTOP-7D5E1TE MINGW64 ~/Git_Exercises (master)
$ git branch -M main

REBECCA@DESKTOP-7D5E1TE MINGW64 ~/Git_Exercises (main)
$ touch README.md

REBECCA@DESKTOP-7D5E1TE MINGW64 ~/Git_Exercises (main)
$ git status
On branch main

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        README.md

nothing added to commit but untracked files present (use "git add" to track)

REBECCA@DESKTOP-7D5E1TE MINGW64 ~/Git_Exercises (main)
$ git add add 
fatal: pathspec 'add' did not match any files

REBECCA@DESKTOP-7D5E1TE MINGW64 ~/Git_Exercises (main)
$ git add add  .
fatal: pathspec 'add' did not match any files

REBECCA@DESKTOP-7D5E1TE MINGW64 ~/Git_Exercises (main)
$ git add .

REBECCA@DESKTOP-7D5E1TE MINGW64 ~/Git_Exercises (main)
$ git status
On branch main

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   README.md


REBECCA@DESKTOP-7D5E1TE MINGW64 ~/Git_Exercises (main)
$ git commit -m "project setup"                                                           
[main (root-commit) a3bdafb] project setup
 1 file changed, 2 insertions(+)
 create mode 100644 README.md

REBECCA@DESKTOP-7D5E1TE MINGW64 ~/Git_Exercises (main)
$ git remote add origin https://github.com/Beccatoni/Gym-git-exercise.git

REBECCA@DESKTOP-7D5E1TE MINGW64 ~/Git_Exercises (main)
$ git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


REBECCA@DESKTOP-7D5E1TE MINGW64 ~/Git_Exercises (main)
$ git push --set-upstream origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 264 bytes | 88.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/Beccatoni/Gym-git-exercise.git
 * [new branch]      main -> main
branch 'main' set up to track 'origin/main'.

REBECCA@DESKTOP-7D5E1TE MINGW64 ~/Git_Exercises (main)
$ git checkout -b dev
Switched to a new branch 'dev'

REBECCA@DESKTOP-7D5E1TE MINGW64 ~/Git_Exercises (dev)
$ git status
On branch dev
nothing to commit, working tree clean

REBECCA@DESKTOP-7D5E1TE MINGW64 ~/Git_Exercises (dev)
$ git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


REBECCA@DESKTOP-7D5E1TE MINGW64 ~/Git_Exercises (dev)
$ git push --set-upstream origin dev
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/Beccatoni/Gym-git-exercise/pull/new/dev
remote:
To https://github.com/Beccatoni/Gym-git-exercise.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.

REBECCA@DESKTOP-7D5E1TE MINGW64 ~/Git_Exercises (dev)
$ git checkout -b test
Switched to a new branch 'test'

REBECCA@DESKTOP-7D5E1TE MINGW64 ~/Git_Exercises (test)
$ git checkout dev
Switched to branch 'dev'
Your branch is up to date with 'origin/dev'.

REBECCA@DESKTOP-7D5E1TE MINGW64 ~/Git_Exercises (dev)
$ git branch -d test
Deleted branch test (was a3bdafb).

REBECCA@DESKTOP-7D5E1TE MINGW64 ~/Git_Exercises (dev)
$ git push origin --delete test
error: unable to delete 'test': remote ref does not exist
error: failed to push some refs to 'https://github.com/Beccatoni/Gym-git-exercise.git'

REBECCA@DESKTOP-7D5E1TE MINGW64 ~/Git_Exercises (dev)
$ git checkout -b test
Switched to a new branch 'test'

REBECCA@DESKTOP-7D5E1TE MINGW64 ~/Git_Exercises (test)
$ git push origin test
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
remote: 
remote: Create a pull request for 'test' on GitHub by visiting:
remote:      https://github.com/Beccatoni/Gym-git-exercise/pull/new/test
remote:
To https://github.com/Beccatoni/Gym-git-exercise.git
 * [new branch]      test -> test

REBECCA@DESKTOP-7D5E1TE MINGW64 ~/Git_Exercises (test)
$ git checkout dev
Switched to branch 'dev'
Your branch is up to date with 'origin/dev'.

REBECCA@DESKTOP-7D5E1TE MINGW64 ~/Git_Exercises (dev)
$ git push origin --delete test
To https://github.com/Beccatoni/Gym-git-exercise.git
 - [deleted]         test


 