Git Learnings
mkdir directory_name 
mkdir gitlearn
HARI@HARI MINGW64 ~/Desktop
$ cd gitlearn/
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn
$ touch learn.txt
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn
$ ls
learn.txt
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn
$ git init
Initialized empty Git repository in C:/Users/HARI/Desktop/gitlearn/.git/
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (master)
$ ls
learn.txt
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (master)
$ ls -a
./  ../  .git/  learn.txt
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (master)
$ touch readme
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (master)

(base)
HARI@HARI MINGW64 ~/Desktop
$ ls
 Deep_interview.txt        'WPS Office.lnk'*                      gitlearn/
 Docs.lnk*                  apache-tomcat-7.0.99/                 interview.txt
'New Text Document.txt'     auto/                                 myfiles/
 Postman.lnk*               chrome-win64/                         pycode/
 Sheets.lnk*                desktop.ini                           sonarqube-6.6/
 Store.lnk*                 eclipse-jee-oxygen-3a-win32-x86_64/
'Visual Studio Code.lnk'*   edgedriver_win64/
(base)
HARI@HARI MINGW64 ~/Desktop
$ cd gitlearn/
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (master)
$ git branch -N main
error: unknown switch `N'
usage: git branch [<options>] [-r | -a] [--merged] [--no-merged]
   or: git branch [<options>] [-f] [--recurse-submodules] <branch-name> [<start-point>]
   or: git branch [<options>] [-l] [<pattern>...]
   or: git branch [<options>] [-r] (-d | -D) <branch-name>...
   or: git branch [<options>] (-m | -M) [<old-branch>] <new-branch>
   or: git branch [<options>] (-c | -C) [<old-branch>] <new-branch>
   or: git branch [<options>] [-r | -a] [--points-at]
   or: git branch [<options>] [-r | -a] [--format]

Generic options
    -v, --[no-]verbose    show hash and subject, give twice for upstream branch
    -q, --[no-]quiet      suppress informational messages
    -t, --[no-]track[=(direct|inherit)]
                          set branch tracking configuration
    -u, --[no-]set-upstream-to <upstream>
                          change the upstream info
    --[no-]unset-upstream unset the upstream info
    --[no-]color[=<when>] use colored output
    -r, --remotes         act on remote-tracking branches
    --contains <commit>   print only branches that contain the commit
    --no-contains <commit>
                          print only branches that don't contain the commit
    --[no-]abbrev[=<n>]   use <n> digits to display object names

Specific git-branch actions:
    -a, --all             list both remote-tracking and local branches
    -d, --[no-]delete     delete fully merged branch
    -D                    delete branch (even if not merged)
    -m, --[no-]move       move/rename a branch and its reflog
    -M                    move/rename a branch, even if target exists
    --[no-]omit-empty     do not output a newline after empty formatted refs
    -c, --[no-]copy       copy a branch and its reflog
    -C                    copy a branch, even if target exists
    -l, --[no-]list       list branch names
    --[no-]show-current   show current branch name
    --[no-]create-reflog  create the branch's reflog
    --[no-]edit-description
                          edit the description for the branch
    -f, --[no-]force      force creation, move/rename, deletion
    --merged <commit>     print only branches that are merged
    --no-merged <commit>  print only branches that are not merged
    --[no-]column[=<style>]
                          list branches in columns
    --[no-]sort <key>     field name to sort on
    --[no-]points-at <object>
                          print only branches of the object
    -i, --[no-]ignore-case
                          sorting and filtering are case insensitive
    --[no-]recurse-submodules
                          recurse through submodules
    --[no-]format <format>
                          format to use for the output

(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (master)
$ git branch -M main
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$ git branch reels
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$ git checkout reels
Switched to branch 'reels'
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (reels)
$ git status
On branch reels
nothing to commit, working tree clean
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (reels)
$ git status
On branch reels
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   learn.txt

no changes added to commit (use "git add" and/or "git commit -a")
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (reels)
$ git add .
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (reels)
$ git status
On branch reels
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   learn.txt

(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (reels)
$ git -m commit "reels added"
unknown option: -m
usage: git [-v | --version] [-h | --help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           [--config-env=<name>=<envvar>] <command> [<args>]
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (reels)
$ git commit -m "reels added"
[reels 19688eb] reels added
 1 file changed, 1 insertion(+)
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (reels)
$ git branch -m reelsfeature
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (reelsfeature)
$ git branch -m reels
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (reels)
$ git checkout main
Switched to branch 'main'
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$ git status
On branch main
nothing to commit, working tree clean
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$ ls
learn.txt  readme
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$ vi learn.txt
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$ git checkout reels
Switched to branch 'reels'
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (reels)
$ ls
learn.txt  readme
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (reels)
$ vi learn.txt
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (reels)
$ git checkout main
Switched to branch 'main'
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$ git status
On branch main
nothing to commit, working tree clean
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$ git branch -d reels
error: the branch 'reels' is not fully merged
hint: If you are sure you want to delete it, run 'git branch -D reels'
hint: Disable this message with "git config advice.forceDeleteBranch false"
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$ git branch -D reels
Deleted branch reels (was 19688eb).
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$ ls
learn.txt  readme
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$ cat learn.txt
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$ vi learn.txt

(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$ git branch chat
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$ git branch
  chat
* main
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$ git checkout chat
Switched to branch 'chat'
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (chat)
$ git branch
* chat
  main
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (chat)
$ cat learn.txt
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (chat)
$ vi learn.txt
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (chat)
$ cat learn.txt
this is chat feature
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (chat)
$ git add .
warning: in the working copy of 'learn.txt', LF will be replaced by CRLF the next time Git touches it
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (chat)
$ git commit -m "chat feature"
[chat dbc1d12] chat feature
 1 file changed, 1 insertion(+)
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (chat)
$ git status
On branch chat
nothing to commit, working tree clean
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (chat)
$ git checkout main
Switched to branch 'main'
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$ cat learn.txt
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$ git merge chat
Updating fc1e550..dbc1d12
Fast-forward
 learn.txt | 1 +
 1 file changed, 1 insertion(+)
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$ cat learn.txt
this is chat feature
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$ git branch new
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$ git branch
  chat
* main
  new
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$ git checkout new
Switched to branch 'new'
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ touch new.txt
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ vi new.txt
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ git add .
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ git commit -m "new file added"
[new 5e4fded] new file added
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 new.txt
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ vi new.txt
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ cat new.txt
hey there
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ git add .
warning: in the working copy of 'new.txt', LF will be replaced by CRLF the next time Git touches it
git (base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ git commit -m "data in new file"
[new 7437a37] data in new file
 1 file changed, 1 insertion(+)
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ vi new.txt
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ git log
commit 7437a37b0abf86fb1712336f3a7a36ced67fc1b9 (HEAD -> new)
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:54:09 2024 +0530

    data in new file

commit 5e4fded3c0bfca5e0d8e5130c162461dab6bb87b
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:52:53 2024 +0530

    new file added

commit dbc1d122dfd1ace2d66232814ece72504c468b7c (main, chat)
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:23:50 2024 +0530

    chat feature

commit fc1e5509c4b9e2b1d0af5839ea21710a13accc54
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:42:10 2024 +0530

    readme file added

commit 89c7065e9399b5b81b64fa2c7995c110baf27078
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:40:40 2024 +0530

    learn file added
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ git add .
warning: in the working copy of 'new.txt', LF will be replaced by CRLF the next time Git touches it
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ git commit -m "data 2"
[new b3a8ff5] data 2
 1 file changed, 2 insertions(+), 1 deletion(-)
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ git log
commit b3a8ff597ebfa31d1b639f9011e957fed05ea6ad (HEAD -> new)
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:55:38 2024 +0530

    data 2

commit 7437a37b0abf86fb1712336f3a7a36ced67fc1b9
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:54:09 2024 +0530

    data in new file

commit 5e4fded3c0bfca5e0d8e5130c162461dab6bb87b
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:52:53 2024 +0530

    new file added

commit dbc1d122dfd1ace2d66232814ece72504c468b7c (main, chat)
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:23:50 2024 +0530

    chat feature

commit fc1e5509c4b9e2b1d0af5839ea21710a13accc54
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:42:10 2024 +0530

    readme file added

commit 89c7065e9399b5b81b64fa2c7995c110baf27078
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:40:40 2024 +0530

    learn file added
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ git reset 7437a37b0abf86fb1712336f3a7a36ced67fc1b9
Unstaged changes after reset:
M       new.txt
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ git status
On branch new
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   new.txt

no changes added to commit (use "git add" and/or "git commit -a")
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ git log
commit 7437a37b0abf86fb1712336f3a7a36ced67fc1b9 (HEAD -> new)
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:54:09 2024 +0530

    data in new file

commit 5e4fded3c0bfca5e0d8e5130c162461dab6bb87b
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:52:53 2024 +0530

    new file added

commit dbc1d122dfd1ace2d66232814ece72504c468b7c (main, chat)
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:23:50 2024 +0530

    chat feature

commit fc1e5509c4b9e2b1d0af5839ea21710a13accc54
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:42:10 2024 +0530

    readme file added

commit 89c7065e9399b5b81b64fa2c7995c110baf27078
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:40:40 2024 +0530

    learn file added
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ cat new.txt
hey thereii
data 2
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ git add .
warning: in the working copy of 'new.txt', LF will be replaced by CRLF the next time Git touches it
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ git commit -m "2nd data"
[new f439b66] 2nd data
 1 file changed, 2 insertions(+), 1 deletion(-)
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ git log
commit f439b6659f2bc1e0d60be9650597ac4d5242263d (HEAD -> new)
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:58:08 2024 +0530

    2nd data

commit 7437a37b0abf86fb1712336f3a7a36ced67fc1b9
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:54:09 2024 +0530

    data in new file

commit 5e4fded3c0bfca5e0d8e5130c162461dab6bb87b
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:52:53 2024 +0530

    new file added

commit dbc1d122dfd1ace2d66232814ece72504c468b7c (main, chat)
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:23:50 2024 +0530

    chat feature

commit fc1e5509c4b9e2b1d0af5839ea21710a13accc54
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:42:10 2024 +0530

    readme file added

commit 89c7065e9399b5b81b64fa2c7995c110baf27078
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:40:40 2024 +0530

    learn file added
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ git reset dbc1d122dfd1ace2d66232814ece72504c468b7c --hard
HEAD is now at dbc1d12 chat feature
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ git log
commit dbc1d122dfd1ace2d66232814ece72504c468b7c (HEAD -> new, main, chat)
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:23:50 2024 +0530

    chat feature

commit fc1e5509c4b9e2b1d0af5839ea21710a13accc54
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:42:10 2024 +0530

    readme file added

commit 89c7065e9399b5b81b64fa2c7995c110baf27078
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:40:40 2024 +0530

    learn file added
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ git status
On branch new
nothing to commit, working tree clean
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ git reset 89c7065e9399b5b81b64fa2c7995c110baf27078
Unstaged changes after reset:
M       learn.txt
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ git restore .
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ git status
On branch new
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        readme

nothing added to commit but untracked files present (use "git add" to track)
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ git branch
  chat
  main
* new
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ git branch -D chat
Deleted branch chat (was dbc1d12).
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ git checkout main
error: The following untracked working tree files would be overwritten by checkout:
        readme
Please move or remove them before you switch branches.
Aborting
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ git branch -D new
error: cannot delete branch 'new' used by worktree at 'C:/Users/HARI/Desktop/gitlearn'
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ git checkout main
error: The following untracked working tree files would be overwritten by checkout:
        readme
Please move or remove them before you switch branches.
Aborting
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ rm readme.txt
rm: cannot remove 'readme.txt': No such file or directory
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ ls
learn.txt  readme
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ rm readme
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ ls
learn.txt
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (new)
$ git checkout main
Switched to branch 'main'
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$ git restore .
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$ git branch
* main
  new
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$ git branch -D new
Deleted branch new (was 89c7065).
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$ ls
learn.txt  readme
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$ git branch
* main
(base)
HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$ bash

HARI@HARI MINGW64 ~/Desktop/gitlearn (main)
$

(base)
HARI@HARI MINGW64 ~/Desktop
$ cd mylearning
bash: cd: mylearning: No such file or directory
(base)
HARI@HARI MINGW64 ~/Desktop
$ cd mylearnings
bash: cd: mylearnings: No such file or directory
(base)
HARI@HARI MINGW64 ~/Desktop
$ cd mylearnings
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings
$ ls
gitlearn/
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings
$ cd gitlearn
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git log
commit dbc1d122dfd1ace2d66232814ece72504c468b7c (HEAD -> main)
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:23:50 2024 +0530

    chat feature

commit fc1e5509c4b9e2b1d0af5839ea21710a13accc54
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:42:10 2024 +0530

    readme file added

commit 89c7065e9399b5b81b64fa2c7995c110baf27078
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:40:40 2024 +0530

    learn file added
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   readme

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        readme.txt

no changes added to commit (use "git add" and/or "git commit -a")
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ touch addhard
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ ls
addhard  learn.txt  readme  readme.txt
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ vi addhard
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ cat addhard
this is to add a file and hard reset
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git log
commit dbc1d122dfd1ace2d66232814ece72504c468b7c (HEAD -> main)
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:23:50 2024 +0530

    chat feature

commit fc1e5509c4b9e2b1d0af5839ea21710a13accc54
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:42:10 2024 +0530

    readme file added

commit 89c7065e9399b5b81b64fa2c7995c110baf27078
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:40:40 2024 +0530

    learn file added
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git add addhard
warning: in the working copy of 'addhard', LF will be replaced by CRLF the next time Git touches it
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git branch
* main
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git branch new
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git branch
* main
  new
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git checkout new
Switched to branch 'new'
A       addhard
M       readme
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git branch
  main
* new
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ touch newhard
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ vi newhard
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ cat newhard
this is new file
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ mv newhard addhard
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ ls
addhard  learn.txt  readme  readme.txt
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git log
commit dbc1d122dfd1ace2d66232814ece72504c468b7c (HEAD -> new, main)
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:23:50 2024 +0530

    chat feature

commit fc1e5509c4b9e2b1d0af5839ea21710a13accc54
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:42:10 2024 +0530

    readme file added

commit 89c7065e9399b5b81b64fa2c7995c110baf27078
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:40:40 2024 +0530

    learn file added
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git add .
warning: in the working copy of 'addhard', LF will be replaced by CRLF the next time Git touches it
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git log
commit dbc1d122dfd1ace2d66232814ece72504c468b7c (HEAD -> new, main)
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:23:50 2024 +0530

    chat feature

commit fc1e5509c4b9e2b1d0af5839ea21710a13accc54
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:42:10 2024 +0530

    readme file added

commit 89c7065e9399b5b81b64fa2c7995c110baf27078
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:40:40 2024 +0530

    learn file added
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git status
On branch new
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   addhard
        modified:   readme
        new file:   readme.txt

(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git commit -m "addhardfile
> "
[new ad6c894] addhardfile
 3 files changed, 1206 insertions(+)
 create mode 100644 addhard
 create mode 100644 readme.txt
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git status
On branch new
nothing to commit, working tree clean
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git log
commit ad6c894b9294dbecc53ed969ef5f69dd74cc5649 (HEAD -> new)
Author: Your Name <you@example.com>
Date:   Thu May 2 13:11:53 2024 +0530

    addhardfile

commit dbc1d122dfd1ace2d66232814ece72504c468b7c (main)
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:23:50 2024 +0530

    chat feature

commit fc1e5509c4b9e2b1d0af5839ea21710a13accc54
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:42:10 2024 +0530

    readme file added

commit 89c7065e9399b5b81b64fa2c7995c110baf27078
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:40:40 2024 +0530

    learn file added
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git reset ad6c894b9294dbecc53ed969ef5f69dd74cc5649 --hard
HEAD is now at ad6c894 addhardfile
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git reset dbc1d122dfd1ace2d66232814ece72504c468b7c --hard
HEAD is now at dbc1d12 chat feature
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git log
commit dbc1d122dfd1ace2d66232814ece72504c468b7c (HEAD -> new, main)
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:23:50 2024 +0530

    chat feature

commit fc1e5509c4b9e2b1d0af5839ea21710a13accc54
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:42:10 2024 +0530

    readme file added

commit 89c7065e9399b5b81b64fa2c7995c110baf27078
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:40:40 2024 +0530

    learn file added
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git status
On branch new
nothing to commit, working tree clean
(base)
HARI@HARI MINGW64 ~/Desktop
$ cd mylearning
bash: cd: mylearning: No such file or directory
(base)
HARI@HARI MINGW64 ~/Desktop
$ cd mylearnings
bash: cd: mylearnings: No such file or directory
(base)
HARI@HARI MINGW64 ~/Desktop
$ cd mylearnings
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings
$ ls
gitlearn/
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings
$ cd gitlearn
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git log
commit dbc1d122dfd1ace2d66232814ece72504c468b7c (HEAD -> main)
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:23:50 2024 +0530

    chat feature

commit fc1e5509c4b9e2b1d0af5839ea21710a13accc54
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:42:10 2024 +0530

    readme file added

commit 89c7065e9399b5b81b64fa2c7995c110baf27078
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:40:40 2024 +0530

    learn file added
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   readme

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        readme.txt

no changes added to commit (use "git add" and/or "git commit -a")
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ touch addhard
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ ls
addhard  learn.txt  readme  readme.txt
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ vi addhard
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ cat addhard
this is to add a file and hard reset
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git log
commit dbc1d122dfd1ace2d66232814ece72504c468b7c (HEAD -> main)
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:23:50 2024 +0530

    chat feature

commit fc1e5509c4b9e2b1d0af5839ea21710a13accc54
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:42:10 2024 +0530

    readme file added

commit 89c7065e9399b5b81b64fa2c7995c110baf27078
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:40:40 2024 +0530

    learn file added
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git add addhard
warning: in the working copy of 'addhard', LF will be replaced by CRLF the next tches it
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git branch
* main
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git branch new
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git branch
* main
  new
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git checkout new
Switched to branch 'new'
A       addhard
M       readme
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git branch
  main
* new
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ touch newhard
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ vi newhard
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ cat newhard
this is new file
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ mv newhard addhard
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ ls
addhard  learn.txt  readme  readme.txt
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git log
commit dbc1d122dfd1ace2d66232814ece72504c468b7c (HEAD -> new, main)
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:23:50 2024 +0530

    chat feature

commit fc1e5509c4b9e2b1d0af5839ea21710a13accc54
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:42:10 2024 +0530

    readme file added

commit 89c7065e9399b5b81b64fa2c7995c110baf27078
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:40:40 2024 +0530

    learn file added
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git add .
warning: in the working copy of 'addhard', LF will be replaced by CRLF the next tches it
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git log
commit dbc1d122dfd1ace2d66232814ece72504c468b7c (HEAD -> new, main)
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:23:50 2024 +0530

    chat feature

commit fc1e5509c4b9e2b1d0af5839ea21710a13accc54
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:42:10 2024 +0530

    readme file added

commit 89c7065e9399b5b81b64fa2c7995c110baf27078
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:40:40 2024 +0530

    learn file added
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git status
On branch new
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   addhard
        modified:   readme
        new file:   readme.txt

(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git commit -m "addhardfile
> "
[new ad6c894] addhardfile
 3 files changed, 1206 insertions(+)
 create mode 100644 addhard
 create mode 100644 readme.txt
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git status
On branch new
nothing to commit, working tree clean
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git log
commit ad6c894b9294dbecc53ed969ef5f69dd74cc5649 (HEAD -> new)
Author: Your Name <you@example.com>
Date:   Thu May 2 13:11:53 2024 +0530

    addhardfile

commit dbc1d122dfd1ace2d66232814ece72504c468b7c (main)
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:23:50 2024 +0530

    chat feature

commit fc1e5509c4b9e2b1d0af5839ea21710a13accc54
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:42:10 2024 +0530

    readme file added

commit 89c7065e9399b5b81b64fa2c7995c110baf27078
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:40:40 2024 +0530

    learn file added
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git reset ad6c894b9294dbecc53ed969ef5f69dd74cc5649 --hard
HEAD is now at ad6c894 addhardfile
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git reset dbc1d122dfd1ace2d66232814ece72504c468b7c --hard
HEAD is now at dbc1d12 chat feature
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git log
commit dbc1d122dfd1ace2d66232814ece72504c468b7c (HEAD -> new, main)
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:23:50 2024 +0530

    chat feature

commit fc1e5509c4b9e2b1d0af5839ea21710a13accc54
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:42:10 2024 +0530

    readme file added

commit 89c7065e9399b5b81b64fa2c7995c110baf27078
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:40:40 2024 +0530

    learn file added
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git status
On branch new
nothing to commit, working tree clean
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git reset (base)
HARI@HARI MINGW64 ~/Desktop
$ cd mylearning
bash: cd: mylearning: No such file or directory
(base)
HARI@HARI MINGW64 ~/Desktop
$ cd mylearnings
bash: cd: mylearnings: No such file or directory
(base)
HARI@HARI MINGW64 ~/Desktop
$ cd mylearnings
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings
$ ls
gitlearn/
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings
$ cd gitlearn
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git log
commit dbc1d122dfd1ace2d66232814ece72504c468b7c (HEAD -> main)
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:23:50 2024 +0530

    chat feature

commit fc1e5509c4b9e2b1d0af5839ea21710a13accc54
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:42:10 2024 +0530

    readme file added

commit 89c7065e9399b5b81b64fa2c7995c110baf27078
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:40:40 2024 +0530

    learn file added
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git status
On branch main
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   readme

Untracked files:
  (use "git add <file>..." to include in what will be committed)

bash: syntax error near unexpected token `('
bash: HARI@HARI: command not found
bash: $: command not found
bash: bash:: command not found
bash: base: command not found
bash: HARI@HARI: command not found
bash: $: command not found
bash: bash:: command not found
bash: base: command not found
bash: HARI@HARI: command not found
bash: $: command not found
bash: base: command not found
bash: HARI@HARI: command not found
bash: $: command not found
bash: gitlearn/: No such file or directory
bash: base: command not found
bash: HARI@HARI: command not found
bash: $: command not found
bash: base: command not found
bash: syntax error near unexpected token `('
bash: $: command not found
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `newline'
bash: Date:: command not found
bash: chat: command not found
bash: commit: command not found
bash: syntax error near unexpected token `newline'
bash: Date:: command not found
bash: readme: command not found
bash: commit: command not found
bash: syntax error near unexpected token `newline'
bash: Date:: command not found
bash: learn: command not found
bash: base: command not found
bash: syntax error near unexpected token `('
bash: $: command not found
bash: On: command not found
bash: Changes: command not found
bash: use: command not found
bash: use: command not found
bash: modified:: command not found
bash: Untracked: command not found
bash: use: command not found
bash: readme.txt: command not found
bash: syntax error near unexpected token `('
bash: base: command not found
bash: syntax error near unexpected token `('
bash: $: command not found
bash: base: command not found
bash: syntax error near unexpected token `('
bash: $: command not found
bash: addhard: command not found
bash: base: command not found
bash: syntax error near unexpected token `('
bash: $: command not found
bash: base: command not found
bash: syntax error near unexpected token `('
bash: $: command not found

bash: this: command not found
bash: base: command not found
bash: syntax error near unexpected token `('
bash: $: command not found
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `newline'
bash: Date:: command not found
bash: chat: command not found
bash: commit: command not found
bash: syntax error near unexpected token `newline'
bash: Date:: command not found
bash: readme: command not found
bash: commit: command not found
bash: syntax error near unexpected token `newline'
bash: Date:: command not found


bash: learn: command not found
bash: base: command not found
bash: syntax error near unexpected token `('
bash: $: command not found
bash: warning:: command not found
bash: base: command not found
bash: syntax error near unexpected token `('
bash: $: command not found
bash: learn.txt: command not found
bash: base: command not found
bash: syntax error near unexpected token `('
bash: $: command not found
bash: base: command not found
bash: syntax error near unexpected token `('
bash: $: command not found
bash: learn.txt: command not found
bash: new: command not found
bash: base: command not found
bash: syntax error near unexpected token `('
bash: $: command not found
bash: Switched: command not found
bash: A: command not found
bash: M: command not found
bash: base: command not found
bash: syntax error near unexpected token `('
bash: $: command not found
bash: main: command not found
bash: learn.txt: command not found
bash: base: command not found

bash: syntax error near unexpected token `('
bash: $: command not found
bash: base: command not found
bash: syntax error near unexpected token `('

bash: $: command not found


bash: base: command not found

bash: syntax error near unexpected token `('

bash: $: command not found

bash: this: command not found


bash: base: command not found

bash: syntax error near unexpected token `('

bash: $: command not found


bash: base: command not found

bash: syntax error near unexpected token `('

bash: $: command not found


bash: addhard: command not found

bash: base: command not found

bash: syntax error near unexpected token `('


bash: $: command not found

bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `newline'
bash: Date:: command not found










bash: chat: command not found













bash: commit: command not found





bash: syntax error near unexpected token `newline'





bash: Date:: command not found
bash: readme: command not found
bash: commit: command not found
bash: syntax error near unexpected token `newline'
bash: Date:: command not found
bash: learn: command not found
bash: base: command not found
bash: syntax error near unexpected token `('
bash: $: command not found
bash: warning:: command not found
bash: base: command not found
bash: syntax error near unexpected token `('
bash: $: command not found
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `newline'
bash: Date:: command not found
bash: chat: command not found
bash: commit: command not found
bash: syntax error near unexpected token `newline'
bash: Date:: command not found
bash: readme: command not found
bash: commit: command not found
bash: syntax error near unexpected token `newline'
bash: Date:: command not found
bash: learn: command not found
bash: base: command not found
bash: syntax error near unexpected token `('
bash: $: command not found
bash: On: command not found
bash: Changes: command not found
bash: use: command not found
bash: new: command not found
bash: modified:: command not found
bash: new: command not found
bash: base: command not found
bash: syntax error near unexpected token `('
bash: $: command not found
bash: [new: command not found
bash: syntax error near unexpected token `('
bash: create: command not found
bash: create: command not found
bash: base: command not found
bash: syntax error near unexpected token `('
bash: $: command not found
bash: On: command not found
bash: nothing: command not found
bash: base: command not found
bash: syntax error near unexpected token `('
bash: $: command not found
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `newline'
bash: Date:: command not found
bash: addhardfile: command not found
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `newline'
bash: Date:: command not found
bash: chat: command not found
bash: commit: command not found
bash: syntax error near unexpected token `newline'
bash: Date:: command not found
bash: readme: command not found
bash: commit: command not found
bash: syntax error near unexpected token `newline'
bash: Date:: command not found
bash: learn: command not found
bash: base: command not found
bash: syntax error near unexpected token `('
bash: $: command not found
HEAD: cannot open 'is' for reading: No such file or directory
HEAD: cannot open 'now' for reading: No such file or directory
HEAD: cannot open 'at' for reading: No such file or directory
HEAD: cannot open 'ad6c894' for reading: No such file or directory
HEAD: cannot open 'addhardfile' for reading: No such file or directory
bash: base: command not found
bash: syntax error near unexpected token `('
bash: $: command not found
HEAD: cannot open 'is' for reading: No such file or directory
HEAD: cannot open 'now' for reading: No such file or directory
HEAD: cannot open 'at' for reading: No such file or directory
HEAD: cannot open 'dbc1d12' for reading: No such file or directory
HEAD: cannot open 'chat' for reading: No such file or directory
HEAD: cannot open 'feature' for reading: No such file or directory
bash: base: command not found
bash: syntax error near unexpected token `('
bash: $: command not found
bash: syntax error near unexpected token `('
bash: syntax error near unexpected token `newline'
bash: Date:: command not found
bash: chat: command not found
bash: commit: command not found
bash: syntax error near unexpected token `newline'
bash: Date:: command not found
bash: readme: command not found
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ ^C
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git restore .
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git status
On branch new
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        readme.txt

nothing added to commit but untracked files present (use "git add" to track)
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git branch -D chat
error: branch 'chat' not found
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git branch -D new
error: cannot delete branch 'new' used by worktree at 'C:/Users/HARI/Desktop/mylelearn'
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git checkout main
Switched to branch 'main'
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git branch -D new
Deleted branch new (was dbc1d12).
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git reflog --no--abbrev
fatal: unrecognized argument: --no--abbrev
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git reflog --no-abbrev
dbc1d122dfd1ace2d66232814ece72504c468b7c (HEAD -> main) HEAD@{0}: checkout: movinto main
dbc1d122dfd1ace2d66232814ece72504c468b7c (HEAD -> main) HEAD@{1}: reset: moving tfd1ace2d66232814ece72504c468b7c
ad6c894b9294dbecc53ed969ef5f69dd74cc5649 HEAD@{2}: reset: moving to ad6c894b9294def5f69dd74cc5649
ad6c894b9294dbecc53ed969ef5f69dd74cc5649 HEAD@{3}: commit: addhardfile
dbc1d122dfd1ace2d66232814ece72504c468b7c (HEAD -> main) HEAD@{4}: checkout: movin to new
dbc1d122dfd1ace2d66232814ece72504c468b7c (HEAD -> main) HEAD@{5}: checkout: movinto main
89c7065e9399b5b81b64fa2c7995c110baf27078 HEAD@{6}: reset: moving to 89c7065e9399b7995c110baf27078
dbc1d122dfd1ace2d66232814ece72504c468b7c (HEAD -> main) HEAD@{7}: reset: moving tfd1ace2d66232814ece72504c468b7c
f439b6659f2bc1e0d60be9650597ac4d5242263d HEAD@{8}: commit: 2nd data
7437a37b0abf86fb1712336f3a7a36ced67fc1b9 HEAD@{9}: reset: moving to 7437a37b0abf83a7a36ced67fc1b9
b3a8ff597ebfa31d1b639f9011e957fed05ea6ad HEAD@{10}: commit: data 2
7437a37b0abf86fb1712336f3a7a36ced67fc1b9 HEAD@{11}: commit: data in new file
5e4fded3c0bfca5e0d8e5130c162461dab6bb87b HEAD@{12}: commit: new file added
dbc1d122dfd1ace2d66232814ece72504c468b7c (HEAD -> main) HEAD@{13}: checkout: movin to new
dbc1d122dfd1ace2d66232814ece72504c468b7c (HEAD -> main) HEAD@{14}: merge chat: Fa
fc1e5509c4b9e2b1d0af5839ea21710a13accc54 HEAD@{15}: checkout: moving from chat to
dbc1d122dfd1ace2d66232814ece72504c468b7c (HEAD -> main) HEAD@{16}: commit: chat f
fc1e5509c4b9e2b1d0af5839ea21710a13accc54 HEAD@{17}: checkout: moving from main to
fc1e5509c4b9e2b1d0af5839ea21710a13accc54 HEAD@{18}: checkout: moving from reels t
19688eb5c1f814504cd45b43515ba6e75d5b9a11 HEAD@{19}: checkout: moving from main to
fc1e5509c4b9e2b1d0af5839ea21710a13accc54 HEAD@{20}: checkout: moving from reels t
19688eb5c1f814504cd45b43515ba6e75d5b9a11 HEAD@{21}: Branch: renamed refs/heads/reto refs/heads/reels
19688eb5c1f814504cd45b43515ba6e75d5b9a11 HEAD@{23}: Branch: renamed refs/heads/re/heads/reelsfeature
19688eb5c1f814504cd45b43515ba6e75d5b9a11 HEAD@{25}: commit: reels added
fc1e5509c4b9e2b1d0af5839ea21710a13accc54 HEAD@{26}: checkout: moving from main to
fc1e5509c4b9e2b1d0af5839ea21710a13accc54 HEAD@{27}: Branch: renamed refs/heads/mas/heads/main
fc1e5509c4b9e2b1d0af5839ea21710a13accc54 HEAD@{29}: commit: readme file added
89c7065e9399b5b81b64fa2c7995c110baf27078 HEAD@{30}: commit (initial): learn file
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ ^C
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ ls
learn.txt  readme  readme.txt
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git stats
git: 'stats' is not a git command. See 'git --help'.

The most similar command is
        status
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git status
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        readme.txt

nothing added to commit but untracked files present (use "git add" to track)
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git branch
* main
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git checkout -b new dbc1d122dfd1ace2d66232814ece72504c468b7c
Switched to a new branch 'new'
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git branch
  main
* new
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git branch -D new
error: cannot delete branch 'new' used by worktree at 'C:/Users/HARI/Desktop/myle
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git status
On branch new
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        readme.txt

nothing added to commit but untracked files present (use "git add" to track)
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ ls
learn.txt  readme  readme.txt
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git branch -D new
error: cannot delete branch 'new' used by worktree at 'C:/Users/HARI/Desktop/myle
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git checkout new
Already on 'new'
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git checkout main
Switched to branch 'main'
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git branch -D new
Deleted branch new (was dbc1d12).
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git log
commit dbc1d122dfd1ace2d66232814ece72504c468b7c (HEAD -> main)
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:23:50 2024 +0530

    chat feature

commit fc1e5509c4b9e2b1d0af5839ea21710a13accc54
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:42:10 2024 +0530

    readme file added

commit 89c7065e9399b5b81b64fa2c7995c110baf27078
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:40:40 2024 +0530

    learn file added
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git reflog
dbc1d12 (HEAD -> main) HEAD@{0}: checkout: moving from new to main
dbc1d12 (HEAD -> main) HEAD@{1}: checkout: moving from new to new
dbc1d12 (HEAD -> main) HEAD@{2}: checkout: moving from main to new
dbc1d12 (HEAD -> main) HEAD@{3}: checkout: moving from new to main
dbc1d12 (HEAD -> main) HEAD@{4}: reset: moving to dbc1d122dfd1ace2d66232814ece725
ad6c894 HEAD@{5}: reset: moving to ad6c894b9294dbecc53ed969ef5f69dd74cc5649
ad6c894 HEAD@{6}: commit: addhardfile
dbc1d12 (HEAD -> main) HEAD@{7}: checkout: moving from main to new
dbc1d12 (HEAD -> main) HEAD@{8}: checkout: moving from new to main
89c7065 HEAD@{9}: reset: moving to 89c7065e9399b5b81b64fa2c7995c110baf27078
dbc1d12 (HEAD -> main) HEAD@{10}: reset: moving to dbc1d122dfd1ace2d66232814ece72
f439b66 HEAD@{11}: commit: 2nd data
7437a37 HEAD@{12}: reset: moving to 7437a37b0abf86fb1712336f3a7a36ced67fc1b9
b3a8ff5 HEAD@{13}: commit: data 2
7437a37 HEAD@{14}: commit: data in new file
5e4fded HEAD@{15}: commit: new file added
dbc1d12 (HEAD -> main) HEAD@{16}: checkout: moving from main to new
dbc1d12 (HEAD -> main) HEAD@{17}: merge chat: Fast-forward
fc1e550 HEAD@{18}: checkout: moving from chat to main
dbc1d12 (HEAD -> main) HEAD@{19}: commit: chat feature
fc1e550 HEAD@{20}: checkout: moving from main to chat
fc1e550 HEAD@{21}: checkout: moving from reels to main
19688eb HEAD@{22}: checkout: moving from main to reels
fc1e550 HEAD@{23}: checkout: moving from reels to main
19688eb HEAD@{24}: Branch: renamed refs/heads/reelsfeature to refs/heads/reels
19688eb HEAD@{26}: Branch: renamed refs/heads/reels to refs/heads/reelsfeature
19688eb HEAD@{28}: commit: reels added
fc1e550 HEAD@{29}: checkout: moving from main to reels
fc1e550 HEAD@{30}: Branch: renamed refs/heads/master to refs/heads/main
fc1e550 HEAD@{32}: commit: readme file added
89c7065 HEAD@{33}: commit (initial): learn file added
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ touch a b
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ ls
a  b  learn.txt  readme  readme.txt
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git status
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        a
        b
        readme.txt

nothing added to commit but untracked files present (use "git add" to track)
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ mkdir key
c(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ cd key
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn/key (main)
$ touch key1
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn/key (main)
$ cd .
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn/key (main)
$ cd //
(base)
HARI@HARI MINGW64 //
$ cd ~/Desktop/mylearnings/gitlearn/key
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn/key (main)
$ cd ..
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ touch install
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git status
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        a
        b
        install
        key/
        readme.txt

nothing added to commit but untracked files present (use "git add" to track)
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git add .
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git status
On branch main
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   a
        new file:   b
        new file:   install
        new file:   key/key1
        new file:   readme.txt

(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git reset
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git status
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        a
        b
        install
        key/
        readme.txt

nothing added to commit but untracked files present (use "git add" to track)
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ touch .gitignore
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ vim .gitignore
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ cat .gitignore
key/
install

(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git status
On branch main
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore
        a
        b
        readme.txt

nothing added to commit but untracked files present (use "git add" to track)
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git add .
warning: in the working copy of '.gitignore', LF will be replaced by CRLF the next time Git touches it
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git commit -m "ignore files"
[main 07533d9] ignore files
 4 files changed, 877 insertions(+)
 create mode 100644 .gitignore
 create mode 100644 a
 create mode 100644 b
 create mode 100644 readme.txt
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git status
On branch main
nothing to commit, working tree clean
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git log
commit 07533d9912579c2f7d0139e5cee93b16b409b9b9 (HEAD -> main)
Author: Your Name <you@example.com>
Date:   Thu May 2 17:49:46 2024 +0530

    ignore files

commit dbc1d122dfd1ace2d66232814ece72504c468b7c
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:23:50 2024 +0530

    chat feature

commit fc1e5509c4b9e2b1d0af5839ea21710a13accc54
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:42:10 2024 +0530

    readme file added

commit 89c7065e9399b5b81b64fa2c7995c110baf27078
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:40:40 2024 +0530

    learn file added
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ ls
a  b  install  key/  learn.txt  readme  readme.txt
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git branch new
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (main)
$ git checkout new
Switched to branch 'new'
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ ls
a  b  install  key/  learn.txt  readme  readme.txt
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git log
commit 07533d9912579c2f7d0139e5cee93b16b409b9b9 (HEAD -> new, main)
Author: Your Name <you@example.com>
Date:   Thu May 2 17:49:46 2024 +0530

    ignore files

commit dbc1d122dfd1ace2d66232814ece72504c468b7c
Author: Your Name <you@example.com>
Date:   Thu Apr 18 12:23:50 2024 +0530

    chat feature

commit fc1e5509c4b9e2b1d0af5839ea21710a13accc54
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:42:10 2024 +0530

    readme file added

commit 89c7065e9399b5b81b64fa2c7995c110baf27078
Author: Your Name <you@example.com>
Date:   Tue Apr 16 12:40:40 2024 +0530

    learn file added
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git reset dbc1d122dfd1ace2d66232814ece72504c468b7c
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git status
On branch new
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore
        a
        b
        readme.txt

nothing added to commit but untracked files present (use "git add" to track)
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git add .
warning: in the working copy of '.gitignore', LF will be replaced by CRLF the next time Git touches it
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git stash
Saved working directory and index state WIP on new: dbc1d12 chat feature
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git stash list
stash@{0}: WIP on new: dbc1d12 chat feature
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git stash callback
fatal: subcommand wasn't specified; 'push' can't be assumed due to unexpected token 'callback'
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git stash -pop
error: did you mean `--pop` (with two dashes)?
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git stash pop
On branch new
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .gitignore
        new file:   a
        new file:   b
        new file:   readme.txt

Dropped refs/stash@{0} (7cc2659e883ce25a9e6556b99317b86b41be86da)
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git stash pop stash@{0}
error: stash@{0} is not a valid reference
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git stash apply
No stash entries found.
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git stash
Saved working directory and index state WIP on new: dbc1d12 chat feature
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git stash list
stash@{0}: WIP on new: dbc1d12 chat feature
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git stash apply
On branch new
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   .gitignore
        new file:   a
        new file:   b
        new file:   readme.txt

(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git stash list
stash@{0}: WIP on new: dbc1d12 chat feature
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git stash clean
fatal: subcommand wasn't specified; 'push' can't be assumed due to unexpected token 'clean'
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git stash clear
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$ git stash list
(base)
HARI@HARI MINGW64 ~/Desktop/mylearnings/gitlearn (new)
$

