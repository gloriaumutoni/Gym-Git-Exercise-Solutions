# Bundle 1

## Exercise 1
```bash
 git init
   28  git branch
   29  git branch -m master main
   30  vi README.md
   31  touch index.html
   32  git add -A
   33  git commit -m "created index file"
   34  git remote add origin  https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions.git
   35  git push
   36  git push --set-upstream origin main
   37  git fetch
   38  git log
   39  git merge
   40  git rm README.md
   41  ls
   42  git push
   43   git push --set-upstream origin main
   44  git pull
   45  git pull origin main
   46  git push
   47  git push --set-upstream origin main
   48  git pull origin main --allow-unrelated-histories
   49  git commit -m "first commit"
   50  git pull origin main --allow-unrelated-histories
   51  git status
   52  git push --set-upstream origin main
   53  git checkout -b  dev
   54  git branch test
   55  git branch
   56  git branch --delete test
```

## Execise 2
```bash
Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (dev)                                     Gym Git&
$ git add --all

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git&
Gym Git& GitHub (dev)
$ git stash
Saved working directory and index state WIP on dev: a2c378Gym Git&c Merge branch 'main' of https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions                                c Merge 

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (dev)                                     Gym Git&
$ ls
index.html  README.md

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git&
Gym Git& GitHub (dev)
$ touch about.html
                                                          Gym Git&
Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (dev)
$ git stash
No local changes to save                                  Gym Git&

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (dev)
$ git stash list
stash@{0}: WIP on dev: a2c378c Merge branch 'main' of https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions   

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (dev)
$ git add about.html

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (dev)
$ git stash
Saved working directory and index state WIP on dev: a2c378c Merge branch 'main' of https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (dev)
$ touch team.html

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (dev)
$ git add team.html

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (dev)
$ git stash
Saved working directory and index state WIP on dev: a2c378c Merge branch 'main' of https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (dev)
$ git stash pop restore about.html
Too many revisions specified: 'restore' 'about.html'

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (dev)
$ git stash list
stash@{0}: WIP on dev: a2c378c Merge branch 'main' of https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions
stash@{1}: WIP on dev: a2c378c Merge branch 'main' of https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions
stash@{2}: WIP on dev: a2c378c Merge branch 'main' of https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (dev)
$ git stash pop restore
error: restore is not a valid reference

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (dev)
$ git stash pop
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Dropped refs/stash@{0} (a89f5ae3c105b95939719d5fd5b08081a4f2ff17)

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (dev)
$ git stash apply
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   team.html


Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (dev)
$ git stash pop
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   team.html

Dropped refs/stash@{0} (18bdcf312350dc5ce9e4f8d2543578130a9366bc)

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (dev)
$ git stash pop
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html
        new file:   team.html

Dropped refs/stash@{0} (338315f7331d3adc42e7e27aac3bad80b37f6593)

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (dev)
$ git stash pop stashat '1'
Too many revisions specified: 'stashat' '1'

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (dev)
$ git stash pop stash@{1}
error: stash@{1} is not a valid reference

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (dev)
$ git stash list

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (dev)
$ git commit -a -m "stashing files"
[dev f09cf85] stashing files
 3 files changed, 11 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html
 create mode 100644 team.html

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (dev)
$ git reset

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (dev)
$ git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (dev)
$ git push --set-upstream origin dev
Enumerating objects: 13, done.
Counting objects: 100% (13/13), done.
Delta compression using up to 4 threads
Compressing objects: 100% (9/9), done.
Writing objects: 100% (13/13), 1.96 KiB | 501.00 KiB/s, done.
Total 13 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), done.
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions/pull/new/dev     
remote:
To https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (dev)
$ git reset
```
# Bundle 2
## Exercise 1
```bash
Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (dev)
$ git checkout -b ft/bundle-2
Switched to a new branch 'ft/bundle-2'

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (ft/bundle-2)   
$ touch services.html

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (ft/bundle-2)   
$ git commit -a -m "bundle 2 exercise 1"
[ft/bundle-2 e32fbd9] bundle 2 exercise 1
 1 file changed, 11 insertions(+)        

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (ft/bundle-2)
$ git push 
fatal: The current branch ft/bundle-2 has no upstream branch. 
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (ft/bundle-2)   
$  git push --set-upstream origin ft/bundle-2
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 405 bytes | 202.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
remote:
To https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.
```

##Exercise 2
```bash
Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git&
$ git checkout main
Switched to branch 'main'
Your branch is behind 'origin/main' by 5 commits, and can be fast-
  (use "git pull" to update your local branch)

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git&
$ git pull
remote: Enumerating objects: 12, done.
remote: Counting objects: 100% (11/11), done.
From https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions
   413014a..10e370c  main       -> origin/main
Updating a2c378c..10e370c
Fast-forward
 README.md  | 240 ++++++++++++++++++++++++++++++++++++++++++++++++
 about.html |   0
 home.html  |  11 +++
 index.html |  11 +++
 4 files changed, 261 insertions(+), 1 deletion(-)
 create mode 100644 about.html
 create mode 100644 home.html

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git&
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git&sign)
$ git commit -a -m "redesigning service page"
On branch ft/service-redesign
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        services.html

nothing added to commit but untracked files present (use "git add"

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git&sign)
$ git add services.html

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git&sign)
$ git commit -m "redesigning service page"
[ft/service-redesign 4a73af5] redesigning service page
 1 file changed, 11 insertions(+)
 create mode 100644 services.html

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git&sign)
$ git push
fatal: The current branch ft/service-redesign has no upstream bran
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git&sign)
$  git push --set-upstream origin ft/service-redesign
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 445 bytes | 148.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local objec
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub 
remote:      https://github.com/gloriaumutoni/Gym-Git-Exercise-Solce-redesign
remote:
To https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-re

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git&sign)
$ gti checkout main
bash: gti: command not found

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git&sign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git&
$ git add -A

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git&
$ git commit -m "new changes in service page"
[main 5953e47] new changes in service page
 1 file changed, 11 insertions(+)
 create mode 100644 services.html

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git&
$ git push --set-upstream origin main
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 460 bytes | 460.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local objec
To https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions.git
   10e370c..5953e47  main -> main
branch 'main' set up to track 'origin/main'.

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git&
$ git diff origin/main

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git&
$ git diff origin/ft/service-redesign
diff --git a/services.html b/services.html
index 957b318..addb25d 100644
--- a/services.html
+++ b/services.html
@@ -6,6 +6,6 @@
     <title>Document</title>
 </head>
 <body>
-    <h1>Adding new changes</h1>
+    <h1>Adding new changes to main branch</h1>
 </body>
 </html>
:...skipping...
diff --git a/services.html b/services.html     
index 957b318..addb25d 100644
--- a/services.html
+++ b/services.html
@@ -6,6 +6,6 @@
     <title>Document</title>
 </head>
 <body>
-    <h1>Adding new changes</h1>
+    <h1>Adding new changes to main branch</h1>
 </body>
 </html>
\ No newline at end of file
~
~
~
~
~
~
~
~
~
~
~
~

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git&
$ git checkout ft/service-redesign
Switched to branch 'ft/service-redesign'
Your branch is up to date with 'origin/ft/service-redesign'.

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git&sign)
$ git diff origin/ft/service-redesign

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git&sign)
$ git diff origin/main
diff --git a/services.html b/services.html
index addb25d..957b318 100644
--- a/services.html
+++ b/services.html
@@ -6,6 +6,6 @@
     <title>Document</title>
 </head>
 <body>
-    <h1>Adding new changes to main branch</h1>
+    <h1>Adding new changes</h1>
 </body>
 </html>
\ No newline at end of file

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git&sign)
$ git merge
Already up to date.

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git&sign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git&
$ git pull origin main
From https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions
 * branch            main       -> FETCH_HEAD
Already up to date.
$ git merge ft/service-redesign
Auto-merging services.html
CONFLICT (add/add): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.
```
