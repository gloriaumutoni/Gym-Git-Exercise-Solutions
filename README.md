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

## Exercise 2
```bash
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

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (main|MERGING)  
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (ft/team-page)  
$ touch team.html

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (ft/team-page)  
$ git commit -a -m "adding new changes of team page"
On branch ft/team-page
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        team.html

nothing added to commit but untracked files present (use "git add" to track)

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (ft/team-page)
$ git add team.html

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (ft/team-page)
$ git commit -a -m "adding new changes of team page"
[ft/team-page 035691f] adding new changes of team page
 1 file changed, 11 insertions(+)
 create mode 100644 team.html

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (ft/team-page)  
$ git push
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (ft/team-page)  
$ git push --set-upstream origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 444 bytes | 444.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions/pull/new/ft/team-page
remote:
To https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (ft/team-page)  
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (main)
$ git chekout -b ft/contact-page
git: 'chekout' is not a git command. See 'git --help'.

The most similar command is
        checkout

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (main)
$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (ft/contact-page)
$ git branch
  dev
  ft/bundle-2
* ft/contact-page
  ft/service-redesign
  ft/team-page
  main

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (ft/contact-page)
$ git checkout  ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (ft/team-page)  
$ git log
commit 035691fec4ca57e0b60f874999574a7301064146 (HEAD -> ft/team-page, origin/ft/team-page)
Author: gloriaumutoni <gloriaumutoni54@gmail.com>
Date:   Mon Apr 22 17:20:18 2024 +0200

    adding new changes of team page

commit 5953e47c012f2907794af50c893a76b0deb719be (origin/main, main, ft/contact-page)      
Author: gloriaumutoni <gloriaumutoni54@gmail.com>
Date:   Mon Apr 22 16:37:45 2024 +0200

    new changes in service page

commit 10e370ceb372c5f43f09ace7c3f9f14614779c37
Author: Gloria Umutoni <124312203+gloriaumutoni@users.noreply.github.com>
Date:   Mon Apr 22 16:12:53 2024 +0200

    Update README.md

commit 66a516cc6abddc4e97d4013df5717490a6c5ae96
Merge: e3a7133 e32fbd9
Author: Christelle Gihozo <109101706+Gihozo23@users.noreply.github.com>
Date:   Mon Apr 22 16:09:17 2024 +0200

    Merge pull request #2 from gloriaumutoni/ft/bundle-2


Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (ft/team-page)  
$

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (ft/team-page)  
$ git checkout ft/contact-page
Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/contact-page)
$ git cherry pick ft/team-page                            Gym Git& GitHub (ft/contact-page
fatal: unknown commit pick

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/contact-page)
$ git cherry-pick ft/team-page^                           Gym Git& GitHub (ft/contact-page
The previous cherry-pick is now empty, possibly due to conflict resolution.
If you wish to commit it anyway, use:                     flict resolution.

    git commit --allow-empty

Otherwise, please use 'git cherry-pick --skip'
On branch ft/contact-page
You are currently cherry-picking commit 5953e47.
  (all conflicts fixed: run "git cherry-pick --continue") 
  (use "git cherry-pick --skip" to skip this patch)       
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)                                                operation)

nothing to commit, working tree clean

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (ft/contact-page
Gym Git& GitHub (ft/contact-page|CHERRY-PICKING)
$ touch contact.html

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/contact-page|CHERRY-PICKING)
$ git add .

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/contact-page|CHERRY-PICKING)
$ git commit -m "new changes on contact page"
[ft/contact-page 0cfb776] new changes on contact page
 Date: Mon Apr 22 16:37:45 2024 +0200
 1 file changed, 11 insertions(+)
 create mode 100644 contact.html

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/contact-page)
$ git --set-upstream origin ft/contact-page 
unknown option: --set-upstream
usage: git [-v | --version] [-h | --help] [-C <path>] [-c 
<name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           [--super-prefix=<path>] [--config-env=<name>=<envvar>]
           <command> [<args>]

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/contact-page)
$ git push --set-upstream origin ft/contact-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 444 bytes | 222.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0      
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page
remote:
To https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page   
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.
```

# Bandle 3

## Exercise 1

```bash
Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (ft/team-page)  
$ git checkout ft/contact-page
Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/contact-page)
$ git cherry pick ft/team-page                            Gym Git& GitHub (ft/contact-page
fatal: unknown commit pick

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/contact-page)
$ git cherry-pick ft/team-page^                           Gym Git& GitHub (ft/contact-page
The previous cherry-pick is now empty, possibly due to conflict resolution.
If you wish to commit it anyway, use:                     flict resolution.

    git commit --allow-empty

Otherwise, please use 'git cherry-pick --skip'
On branch ft/contact-page
You are currently cherry-picking commit 5953e47.
  (all conflicts fixed: run "git cherry-pick --continue") 
  (use "git cherry-pick --skip" to skip this patch)       
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)                                                operation)

nothing to commit, working tree clean

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (ft/contact-page
Gym Git& GitHub (ft/contact-page|CHERRY-PICKING)
$ touch contact.html

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/contact-page|CHERRY-PICKING)
$ git add .

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/contact-page|CHERRY-PICKING)
$ git commit -m "new changes on contact page"
[ft/contact-page 0cfb776] new changes on contact page
 Date: Mon Apr 22 16:37:45 2024 +0200
 1 file changed, 11 insertions(+)
 create mode 100644 contact.html

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/contact-page)
$ git --set-upstream origin ft/contact-page 
unknown option: --set-upstream
usage: git [-v | --version] [-h | --help] [-C <path>] [-c 
<name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           [--super-prefix=<path>] [--config-env=<name>=<envvar>]
           <command> [<args>]

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/contact-page)
$ git push --set-upstream origin ft/contact-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 444 bytes | 222.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0      
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page
remote:
To https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page   
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/contact-page)
$ git branch
  dev
  ft/bundle-2
* ft/contact-page
  ft/service-redesign
  ft/team-page
  main

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/contact-page)
$ git remote -r
error: unknown switch `r'
usage: git remote [-v | --verbose]
   or: git remote add [-t <branch>] [-m <master>] [-f] [--tags | --no-tags] [--mirror=<fetch|push>] <name> <url>    
   or: git remote rename [--[no-]progress] <old> <new>    
   or: git remote remove <name>
   or: git remote set-head <name> (-a | --auto | -d | --delete | <branch>)
   or: git remote [-v | --verbose] show [-n] <name>       
   or: git remote prune [-n | --dry-run] <name>
   or: git remote [-v | --verbose] update [-p | --prune] [(<group> | <remote>)...]
   or: git remote set-branches [--add] <name> <branch>... 
   or: git remote get-url [--push] [--all] <name>
   or: git remote set-url [--push] <name> <newurl> [<oldurl>]
   or: git remote set-url --add <name> <newurl>
   or: git remote set-url --delete <name> <url>

    -v, --verbose         be verbose; must be placed before a subcommand


Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/contact-page)
$ git pull
remote: Enumerating objects: 8, done.
remote: Counting objects: 100% (8/8), done.
remote: Compressing objects: 100% (6/6), done.
remote: Total 6 (delta 4), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (6/6), 3.06 KiB | 10.00 KiB/s, done.
From https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions
   4a73af5..5faea9c  ft/service-redesign -> origin/ft/service-redesign
Already up to date.

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/contact-page)
$ git branch
  dev
  ft/bundle-2
* ft/contact-page
  ft/service-redesign
  ft/team-page
  main

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/contact-page)
$ git add contact.html

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/contact-page)
$ git commit -m "pushing contact page"
[ft/contact-page c4a768d] pushing contact page
 1 file changed, 1 insertion(+), 1 deletion(-)

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/contact-page)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 301 bytes | 301.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0      
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions.git
   0cfb776..c4a768d  ft/contact-page -> ft/contact-page   

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/contact-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/faq-page)
$ touch faq.html

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/faq-page)
$ git add faq.html

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/faq-page)
$ git commit -m "faq pages"
[ft/faq-page d07aad4] faq pages
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/faq-page)
$ git push
fatal: The current branch ft/faq-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/faq-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/faq-page)
$  git push --set-upstream origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 421 bytes | 421.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0      
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub 
by visiting:
remote:      https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions/pull/new/ft/faq-page
Revert "adding new changes of team page"
remote:
To https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/faq-page)
$ git branch
  dev
  ft/bundle-2
  ft/contact-page
* ft/faq-page
  ft/service-redesign
  ft/team-page
  main

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/faq-page)
$ git checkout ft/team-page
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.     

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/team-page)
$ git revert 035691fec4ca57e0b60f874999574a7301064146     
[ft/team-page 91a0a59] Revert "adding new changes of team 
page"
 1 file changed, 11 deletions(-)
 delete mode 100644 team.html

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/team-page)
$ git push
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 262 bytes | 262.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0      
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions.git
   035691f..91a0a59  ft/team-page -> ft/team-page
```
## Exercises 2
```bash
Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/faq-page)
$ git chckout -b ft/home-page-redesign
git: 'chckout' is not a git command. See 'git --help'.

The most similar command is
        checkout

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/faq-page)
$ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/home-page-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (main)
$ git add .

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (main)
$ git commit -m "changes in main"
[main 00f3686] changes in main
 1 file changed, 1 insertion(+), 1 deletion(-)

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (main)
$ git push
To https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another 
repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.        
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (main)
$ git pull
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 5.06 KiB | 56.00 KiB/s, done.
From https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions
   5953e47..fbcf881  main       -> origin/main
Merge made by the 'ort' strategy.
 README.md | 546 ++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 1 file changed, 546 insertions(+)

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (main)
$ git push
Enumerating objects: 9, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 587 bytes | 293.00 KiB/s, done.
Total 5 (delta 3), reused 0 (delta 0), pack-reused 0      
remote: Resolving deltas: 100% (3/3), completed with 3 local objects.
To https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions.git
   fbcf881..5123b1d  main -> main

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (main)
$ git checkout  ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/home-page-redesign)
$ git rebase origin/main
Successfully rebased and updated refs/heads/ft/home-page-redesign.

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/home-page-redesign)
$ git add .

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/home-page-redesign)
$ git commit -m "new changes in homepage"
[ft/home-page-redesign 919b5ed] new changes in homepage
 1 file changed, 1 insertion(+), 1 deletion(-)

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/home-page-redesign)
$ git push
fatal: The current branch ft/home-page-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/home-page-redesign  

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/home-page-redesign)
$ git push --set-upstream origin ft/home-page-redesign 
Enumerating objects: 14, done.
Counting objects: 100% (14/14), done.
Delta compression using up to 4 threads
Compressing objects: 100% (12/12), done.
Writing objects: 100% (12/12), 1.30 KiB | 445.00 KiB/s, done.
Total 12 (delta 6), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (6/6), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions/pull/new/ft/home-page-redesign
remote:
To https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.
```
## Exercise 2
```bash
Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (ft/footer)     
$ git add .

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (ft/footer)     
$ git commit -m "second commit"
[ft/footer 1df5c32] second commit
 1 file changed, 1 insertion(+)

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (ft/footer)     
$ git add .

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (ft/footer)     
$ git commit -m "new changes"
[ft/footer 63e21f0] new changes
 1 file changed, 1 insertion(+), 1 deletion(-)

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (ft/footer)     
$ git push
fatal: The current branch ft/footer has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/footer

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (ft/footer)     
$ git push --set-upstream origin ft/footer
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 562 bytes | 281.00 KiB/s, done.
Total 6 (delta 4), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (4/4), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions/pull/new/ft/footer
remote:
To https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/footer -> ft/footer
branch 'ft/footer' set up to track 'origin/ft/footer'.

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (ft/footer)     
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (main)
$ git branch ft/squashing

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (main)
$ git merge --squash ft/footer 
Updating 621d18d..63e21f0
Fast-forward
Squash commit -- not updating HEAD
 home.html | 1 +
 1 file changed, 1 insertion(+)

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (main)
$ git commit -a -m "footer changes squashing"
[main b8cc13a] footer changes squashing
 1 file changed, 1 insertion(+)

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 336 bytes | 336.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions.git
   621d18d..b8cc13a  main -> main
```
# Bundle 5

## Exercise 2
``` bash
Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (main)
$ git clone https://github.com/gloriaumutoni/git-cafe-exercise.git
Cloning into 'git-cafe-exercise'...
remote: Enumerating objects: 107, done.
done.
remote: Total 107 (delta 5), reused 4 (delta 4), pack-reused 93Resolving deltas: 100% (5/5), done.), done.


Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (main)
$ git add .
warning: adding embedded git repository: git-cafe-exercise
hint: You've added another git repository inside your current repository.
hint: Clones of the outer repository will not contain the contents of
hint: the embedded repository and will not know how to obtain it.
hint: If you meant to add a submodule, use:
hint: 
hint:   git submodule add <url> git-cafe-exercise
hint: 
hint: If you added this path by mistake, you can remove it from the
hint: index with:
hint: 
hint:   git rm --cached git-cafe-exercise
hint: 
hint: See "git help submodule" for more information.

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (main)
$ git commit -a -m "new changes on forked repo"
[main efc5107] new changes on forked repo
 2 files changed, 2 insertions(+), 1 deletion(-)
 create mode 160000 git-cafe-exercise

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (main)
$ git push
To https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions.git
 ! [rejected]        main -> main (fetch first)
error: failed to push some refs to 'https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions.git'
hint: Updates were rejected because the remote contains work that you do
hint: not have locally. This is usually caused by another repository pushing
hint: to the same ref. You may want to first integrate the remote changes
hint: (e.g., 'git pull ...') before pushing again.
hint: See the 'Note about fast-forwards' in 'git push --help' for details.

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (main)
$ git pull
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 1.41 KiB | 5.00 KiB/s, done.
From https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions
   b8cc13a..d705e7e  main       -> origin/main
Merge made by the 'ort' strategy.
 README.md | 79 +++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 1 file changed, 79 insertions(+)

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (main)
$ git push
Enumerating objects: 9, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 752 bytes | 150.00 KiB/s, done.
Total 5 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
To https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions.git
   d705e7e..f3b31e3  main -> main

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (main)
$ git commit -a -m "new changes on forked repo"
[main aa2a5cf] new changes on forked repo
 1 file changed, 1 deletion(-)

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The Gym Git& GitHub (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 310 bytes | 310.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions.git
   f3b31e3..aa2a5cf  main -> main

```
# Bundle 6

## Exercises 1

```bash
Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (main)
$ git checkout -b ft/cafe                                 Gym Git& GitHub (main)
Switched to a new branch 'ft/cafe'

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/cafe)                                 Gym Git& GitHub (ft/cafe)       
$ touch Menu.html

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/cafe)
$ git commit -a -m "new branch ft/cafe"
On branch ft/cafe
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
  (commit or discard the untracked or modified content in 
submodules)
        modified:   git-cafe-exercise (modified content)

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        Menu.html

no changes added to commit (use "git add" and/or "git commit -a")

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/cafe)
$ git add .

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/cafe)
$ git add -A

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/cafe)
$ git commit -m "new branch ft/cafe"
[ft/cafe 757dd18] new branch ft/cafe
 1 file changed, 12 insertions(+)
 create mode 100644 Menu.html

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/cafe)
$ git push
fatal: The current branch ft/cafe has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/cafe

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.

Nicole@DESKTOP-NRC5VAI MINGW64 ~/Downloads/javascript/The 
Gym Git& GitHub (ft/cafe)
$   git push --set-upstream origin ft/cafe
Enumerating objects: 19, done.
Counting objects: 100% (19/19), done.
Delta compression using up to 4 threads
Compressing objects: 100% (16/16), done.
Writing objects: 100% (16/16), 2.99 KiB | 612.00 KiB/s, done.
Total 16 (delta 8), reused 0 (delta 0), pack-reused 0     
remote: Resolving deltas: 100% (8/8), completed with 3 local objects.
remote:
remote: Create a pull request for 'ft/cafe' on GitHub by visiting:
remote:      https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions/pull/new/ft/cafe
remote:
To https://github.com/gloriaumutoni/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/cafe -> ft/cafe
branch 'ft/cafe' set up to track 'origin/ft/cafe'.
```
