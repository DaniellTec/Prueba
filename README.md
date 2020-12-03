# Prueba Git

Exámen de **GitHub**

[title] (https://campus.ifp.es/)

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop
$ git config user.name DaniellTec
fatal: not in a git directory

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop
$ git config --global user.name DaniellTec

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop
$ git config --global user.email danieltecpuhawan@gmail.com

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop
$ git config --global user.password CyberCatNya25GH

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop
$ git clone https://github.com/DaniellTec/Prueba.git
Cloning into 'Prueba'...
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
Receiving objects: 100% (3/3), done.

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop
$ dir
desktop.ini  Desktop.rar  Prueba  TestGit

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop
$ cd Prueba

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop/Prueba (main)
$ git add *.txt

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop/Prueba (main)
$ git commit -m "First Commit"
[main bd782d0] First Commit
 3 files changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 1.txt
 create mode 100644 2.txt
 create mode 100644 3.txt

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop/Prueba (main)
$ git log --pretty=oneline
bd782d083c9edd03818f6a5dfc8a0e7594cfb8a2 (HEAD -> main) First Commit
bd3ef931634f5f691ec16a3a37e3bd681ed771ca (origin/main, origin/HEAD) Initial commit

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop/Prueba (main)
$ git status
On branch main
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop/Prueba (main)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 284 bytes | 284.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/DaniellTec/Prueba.git
   bd3ef93..bd782d0  main -> main

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop/Prueba (main)
$ git tag meh

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop/Prueba (main)
$ git tag -m
error: switch `m' requires a value

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop/Prueba (main)
$ git tag -l
meh

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop/Prueba (main)
$ git branch rama1

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop/Prueba (main)
$ git branch rama2

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop/Prueba (main)
$ git push
Everything up-to-date

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop/Prueba (main)
$ git checkout rama1
Switched to branch 'rama1'

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop/Prueba (rama1)
$ git add 4.txt

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop/Prueba (rama1)
$ git commit -m "First Commit"
[rama1 5206dc3] First Commit
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 4.txt

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop/Prueba (rama1)
$ git push
fatal: The current branch rama1 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin rama1


Daniell@DESKTOP-060HODV MINGW64 ~/Desktop/Prueba (rama1)
$ git push --set-upstream origin rama1
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 231 bytes | 231.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'rama1' on GitHub by visiting:
remote:      https://github.com/DaniellTec/Prueba/pull/new/rama1
remote:
To https://github.com/DaniellTec/Prueba.git
 * [new branch]      rama1 -> rama1
Branch 'rama1' set up to track remote branch 'rama1' from 'origin'.

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop/Prueba (rama1)
$ git branch
  main
* rama1
  rama2

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop/Prueba (rama1)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop/Prueba (main)
$ git merge rama1
Updating bd782d0..5206dc3
Fast-forward
 4.txt | 0
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 4.txt

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop/Prueba (main)
$ git branch -d rama2
Deleted branch rama2 (was bd782d0).

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop/Prueba (main)
$ git push
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0
To https://github.com/DaniellTec/Prueba.git
   bd782d0..5206dc3  main -> main

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop/Prueba (main)
$ git branch
* main
  rama1

Daniell@DESKTOP-060HODV MINGW64 ~/Desktop/Prueba (main)
$ git pull
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 3 (delta 1), reused 0 (delta 0), pack-reused 0
Unpacking objects: 100% (3/3), 702 bytes | 70.00 KiB/s, done.
From https://github.com/DaniellTec/Prueba
   5206dc3..15cd147  main       -> origin/main
Updating 5206dc3..15cd147
Fast-forward
 README.md | 6 +++++-
 1 file changed, 5 insertions(+), 1 deletion(-)

