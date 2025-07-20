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
## Bundle 1
### Exercise 2
```bash
Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)       
$ git status
On branch dev
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

nothing added to commit but untracked files present (use "git add" to track)

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)       
$ git stash list

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)       
$ git add home.html

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)       
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)    
        new file:   home.html


Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)       
$  git stash
Saved working directory and index state WIP on dev: c15274c Merge branch 'main' of https://github.com/Olivier-Masabo/Gym-Git-Exercise

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)       
$ git stash list
stash@{0}: WIP on dev: c15274c Merge branch 'main' of https://github.com/Olivier-Masabo/Gym-Git-Exercise      

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)       
$ git add about.html

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)       
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)    
        new file:   about.html


Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)
$ git stash
Saved working directory and index state WIP on dev: c15274c Merge branch 'main' of https://github.com/Olivier-Masabo/Gym-Git-Exercise

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)       
$ git stash list
stash@{0}: WIP on dev: c15274c Merge branch 'main' of https://github.com/Olivier-Masabo/Gym-Git-Exercise      
stash@{1}: WIP on dev: c15274c Merge branch 'main' of https://github.com/Olivier-Masabo/Gym-Git-Exercise      

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)       
$ git add team.html

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)       
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)    
        new file:   team.html


Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)       
$ git stash
Saved working directory and index state WIP on dev: c15274c Merge branch 'main' of https://github.com/Olivier-Masabo/Gym-Git-Exercise

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)       
$ git stash list
stash@{0}: WIP on dev: c15274c Merge branch 'main' of https://github.com/Olivier-Masabo/Gym-Git-Exercise      
stash@{1}: WIP on dev: c15274c Merge branch 'main' of https://github.com/Olivier-Masabo/Gym-Git-Exercise      
stash@{2}: WIP on dev: c15274c Merge branch 'main' of https://github.com/Olivier-Masabo/Gym-Git-Exercise      

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)       
$ ^C

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)       
$ git stash pop ^C

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (379ff6b678ee9ba817bacce4f51fb945500b3c0a)

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)       
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)    
        new file:   about.html
        new file:   home.html

Dropped stash@{1} (c853e7abef1863d757945f4f5f9c096e3a1006b6)

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)       
$ git add --all

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)       
$ git status
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)    
        new file:   about.html
        new file:   home.html


Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)       
$ git commit -m "setup the home and about page"
[dev 781762c] setup the home and about page
 2 files changed, 22 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)       
$ git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)       
$ git push --set-upstream origin dev
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 632 bytes | 25.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), done.
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/Olivier-Masabo/Gym-Git-Exercise/pull/new/dev
remote:
To https://github.com/Olivier-Masabo/Gym-Git-Exercise.git
branch 'dev' set up to track 'origin/dev'.

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)
$ git stash pop
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped refs/stash@{0} (9eb03ab0d5860fa31e12c7ece40db78f2bddd597)
        new file:   team.html

Dropped refs/stash@{0} (9eb03ab0d5860fa31e12c7ece40db78f2bddd597)
Dropped refs/stash@{0} (9eb03ab0d5860fa31e12c7ece40db78f2bddd597)

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)
$ git reset --hard
HEAD is now at 781762c setup the home and about page

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)
$ git status
On branch dev
Your branch is up to date with 'origin/dev'.

nothing to commit, working tree clean

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)
$ it checkout main
bash: it: command not found

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
```

## Bundle 2
### Exercise 1
```bash
Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (dev)
$ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (ft/bundle-2)
$ git status
On branch ft/bundle-2
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        service.html

nothing added to commit but untracked files present (use "git add" to track)

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (ft/bundle-2)
$ git add --all

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (ft/bundle-2)
$ git commit -m "add service page"
[ft/bundle-2 4edd0f9] add service page
 1 file changed, 11 insertions(+)
 create mode 100644 service.html

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (ft/bundle-2)
$ git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (ft/bundle-2)
$  git push --set-upstream origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 8 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 464 bytes | 232.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/Olivier-Masabo/Gym-Git-Exercise/pull/new/ft/bundle-2
remote:
To https://github.com/Olivier-Masabo/Gym-Git-Exercise.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.

Tech Heaven Shop@Mufasa MINGW64 ~/Myproj-2 (ft/bundle-2)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.
```