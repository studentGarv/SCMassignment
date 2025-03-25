<H3>Topic of File</H3>
"""
garvm@GMLOQ MINGW64 /d
$ git clone https://github.com/studentGarv/SCMassignment.git
Cloning into 'SCMassignment'...
remote: Enumerating objects: 5, done.
remote: Counting objects: 100% (5/5), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 5 (delta 1), reused 4 (delta 0), pack-reused 0 (from 0)
Receiving objects: 100% (5/5), done.
Resolving deltas: 100% (1/1), done.

garvm@GMLOQ MINGW64 /d
$ cd SCMassignment/

garvm@GMLOQ MINGW64 /d/SCMassignment (main)
$ ls
feature_details.txt  project_overview.txt

garvm@GMLOQ MINGW64 /d/SCMassignment (main)
$ git branch
* main

garvm@GMLOQ MINGW64 /d/SCMassignment (main)
$ git branch development

garvm@GMLOQ MINGW64 /d/SCMassignment (main)
$ git branch
  development
* main

garvm@GMLOQ MINGW64 /d/SCMassignment (main)
$ git checkout development
Switched to branch 'development'

garvm@GMLOQ MINGW64 /d/SCMassignment (development)
$ echo "create a new branch" > "todo.txt"

garvm@GMLOQ MINGW64 /d/SCMassignment (development)
$ ls
feature_details.txt  project_overview.txt  todo.txt

garvm@GMLOQ MINGW64 /d/SCMassignment (development)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

garvm@GMLOQ MINGW64 /d/SCMassignment (main)
$ git merge development
Already up to date.

garvm@GMLOQ MINGW64 /d/SCMassignment (main)
$ git add .
warning: in the working copy of 'todo.txt', LF will be replaced by CRLF the next time Git touches it

garvm@GMLOQ MINGW64 /d/SCMassignment (main)
$ git push orgin -u main
fatal: 'orgin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

garvm@GMLOQ MINGW64 /d/SCMassignment (main)
$ git push orgin main
fatal: 'orgin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

garvm@GMLOQ MINGW64 /d/SCMassignment (main)
$ git push  main
fatal: 'main' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

garvm@GMLOQ MINGW64 /d/SCMassignment (main)
$ git push main
fatal: 'main' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

garvm@GMLOQ MINGW64 /d/SCMassignment (main)
$ git push orgin -u main
fatal: 'orgin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

garvm@GMLOQ MINGW64 /d/SCMassignment (main)
$ git init
Reinitialized existing Git repository in D:/SCMassignment/.git/

garvm@GMLOQ MINGW64 /d/SCMassignment (main)
$ git branch
  development
* main

garvm@GMLOQ MINGW64 /d/SCMassignment (main)
$ git push orgin -u main
fatal: 'orgin' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

garvm@GMLOQ MINGW64 /d/SCMassignment (main)
$ git pull https://github.com/studentGarv/SCMassignment.git
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 996 bytes | 76.00 KiB/s, done.
From https://github.com/studentGarv/SCMassignment
 * branch            HEAD       -> FETCH_HEAD
Updating f22ab07..6356570
Fast-forward
 README.md | 1 +
 1 file changed, 1 insertion(+)
 create mode 100644 README.md

garvm@GMLOQ MINGW64 /d/SCMassignment (main)
$ echo "ignored by git" > "new.gitignore"

garvm@GMLOQ MINGW64 /d/SCMassignment (main)
$ ls
feature_details.txt  new.gitignore  project_overview.txt  README.md  todo.txt

garvm@GMLOQ MINGW64 /d/SCMassignment (main)
$ git branch development
fatal: a branch named 'development' already exists

garvm@GMLOQ MINGW64 /d/SCMassignment (main)
$ git checkout development
A       todo.txt
Switched to branch 'development'

garvm@GMLOQ MINGW64 /d/SCMassignment (development)
$ git add .
warning: in the working copy of 'new.gitignore', LF will be replaced by CRLF the next time Git touches it

garvm@GMLOQ MINGW64 /d/SCMassignment (development)
$ git checkout main
A       new.gitignore
A       todo.txt
Switched to branch 'main'
Your branch is ahead of 'origin/main' by 1 commit.
  (use "git push" to publish your local commits)

garvm@GMLOQ MINGW64 /d/SCMassignment (main)
$ echo "logs of new commit" > "new.log"

garvm@GMLOQ MINGW64 /d/SCMassignment (main)
$ ls
feature_details.txt  new.gitignore  new.log  project_overview.txt  README.md  todo.txt

garvm@GMLOQ MINGW64 /d/SCMassignment (main)
$ git commit -m "new"
[main 4a0f389] new
 2 files changed, 2 insertions(+)
 create mode 100644 new.gitignore
 create mode 100644 todo.txt

garvm@GMLOQ MINGW64 /d/SCMassignment (main)
$ git add .
warning: in the working copy of 'new.log', LF will be replaced by CRLF the next time Git touches it

garvm@GMLOQ MINGW64 /d/SCMassignment (main)
$ git commit -m "new"
[main 710d17a] new
 1 file changed, 1 insertion(+)
 create mode 100644 new.log

garvm@GMLOQ MINGW64 /d/SCMassignment (main)
$ git push origin -u main
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 8 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (7/7), 633 bytes | 90.00 KiB/s, done.
Total 7 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), done.
To https://github.com/studentGarv/SCMassignment.git
   6356570..710d17a  main -> main
branch 'main' set up to track 'origin/main'.

"""
This is to check if pull works in git 
Does Html code work in .md file
