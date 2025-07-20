# Gym-Git-Exercise
## Bundle 1
### Exercise 1
```bash

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2
$ git init
Initialized empty Git repository in C:/Users/Tech Heaven Shop/Myproj-2/.git/

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        index.html

nothing added to commit but untracked files present (use "git add" to track)

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (master)
$ git branch -m master main

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (main)
$ git add index.html

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (main)
$ git commit -m "add index page to github"
[main (root-commit) 0f30f6f] add index page to github
 1 file changed, 11 insertions(+)
 create mode 100644 index.html

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (main)
$ git remote add origin https://github.com/Olivier-Masabo/Gym-Git-Exercise.git

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (main)
$ git push
fatal: The current branch main has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin main

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (main)
$  git push --set-upstream origin main
To https://github.com/Olivier-Masabo/Gym-Git-Exercise.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/Olivier-Masabo/Gym-Git-Exercise.git'
hint: Updates were rejected because the remote contains work that you do not
hint: have locally. This is usually caused by another repository pushing to
hint: the same ref. If you want to integrate the remote changes, use
hint: 'git pull' before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (main)
$ git pull origin main
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (4/4), 1.50 KiB | 32.00 KiB/s, done.
From https://github.com/Olivier-Masabo/Gym-Git-Exercise
 * branch            main       -> FETCH_HEAD
 * [new branch]      main       -> origin/main
fatal: refusing to merge unrelated histories

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (main)
$ git pull origin main --allow-unrelated-histories
From https://github.com/Olivier-Masabo/Gym-Git-Exercise
 * branch            main       -> FETCH_HEAD
Merge made by the 'ort' strategy.
 LICENSE   | 21 +++++++++++++++++++++
 README.md |  1 +
 2 files changed, 22 insertions(+)
 create mode 100644 LICENSE
 create mode 100644 README.md

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (main)
$  git push --set-upstream origin main
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 749 bytes | 93.00 KiB/s, done.
Total 5 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Olivier-Masabo/Gym-Git-Exercise.git
   478c4e5..c15274c  main -> main
branch 'main' set up to track 'origin/main'.

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (main)
$ git checkout -b dev
Switched to a new branch 'dev'

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)
$ git checkout -b test
Switched to a new branch 'test'

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (test)
$ git checkout dev
Switched to branch 'dev'

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)
$ git branch -d test
Deleted branch test (was c15274c).

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
```