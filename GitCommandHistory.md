
SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (master)
$ git branch
$ ls
demo.html  Sample.java

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (master)
$ git branch release

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (master)
$ git branch
* master
  release

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (master)
$ git switch release
Switched to branch 'release'

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (release)
$ git branch
  master
* release

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (release)
$ ls
demo.html  Sample.java

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (release)
$ git log
commit 0242e78e9ba6b2fe71d30f9f6a5f570e55711e81 (HEAD -> release, origin/master, master)
Author: SiddhalinSP <siddhaling88@gmail.com>
Date:   Wed Jun 24 13:14:05 2026 +0530

    Succesfull added both file

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (release)
$ git status
On branch release
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   demo.html

no changes added to commit (use "git add" and/or "git commit -a")

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (release)
$ git add.
git: 'add.' is not a git command. See 'git --help'.

The most similar command is
        add

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (release)
$ git add .

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (release)
$ git status
On branch release
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   demo.html


SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (release)
$ git commit demo.html -m "modified index.html"
[release 4cf68df] modified index.html
 1 file changed, 3 insertions(+)

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (release)
$ git push release
fatal: 'release' does not appear to be a git repository
fatal: Could not read from remote repository.

Please make sure you have the correct access rights
and the repository exists.

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (release)
$ git push origin release
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 317 bytes | 317.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'release' on GitHub by visiting:
remote:      https://github.com/SiddhalingSP/Branching/pull/new/release
remote: 
To https://github.com/SiddhalingSP/Branching.git
 * [new branch]      release -> release

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (release)
$ git switch master
Switched to branch 'master'

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (master)
$ git status
On branch master
nothing to commit, working tree clean

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (master)
$ git branch
* master
  release

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (master)
$ git checkout -b feature
Switched to a new branch 'feature'

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (feature)
$ git branch
* feature
  master
  release

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (feature)
$ ls
demo.html  Sample.java

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (feature)
$ ls
demo.html  NewFeature.java  Sample.java

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (feature)
$ git add NewFeature.java

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (feature)
$ git commit -m "New Feature added"
[feature 9f39879] New Feature added
 1 file changed, 5 insertions(+)
 create mode 100644 NewFeature.java

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (feature)
$ git branch -r
  origin/master
  origin/release

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (feature)
$ git push origin feature
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 424 bytes | 424.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'feature' on GitHub by visiting:
remote:      https://github.com/SiddhalingSP/Branching/pull/new/feature
remote: 
To https://github.com/SiddhalingSP/Branching.git
 * [new branch]      feature -> feature

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (feature)
$ git branch -r
  origin/feature
  origin/master
  origin/release

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (feature)
$ git branch -m dev

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (dev)
$ git checkout master
Switched to branch 'master'

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (master)
$ git branch -r
  origin/feature
  origin/master
  origin/release

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (master)
$ git branch -m dev feature

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (master)
$ git branch -r
  origin/feature
  origin/master
  origin/release

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (master)
$ git branch -d feature
error: the branch 'feature' is not fully merged
hint: If you are sure you want to delete it, run 'git branch -D feature'
hint: Disable this message with "git config set advice.forceDeleteBranch false"

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (master)
$ git branch -d feature
error: the branch 'feature' is not fully merged
hint: If you are sure you want to delete it, run 'git branch -D feature'
hint: Disable this message with "git config set advice.forceDeleteBranch false"

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (master)
$ git branch -D feature
Deleted branch feature (was 9f39879).

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (master)
$ git branch -D feature
error: branch 'feature' not found

SIDDHALING@Siddha8055 MINGW64 /c/GitGithub_Class_DCL/Branching (master)
$ 
