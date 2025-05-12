belarus@Roblox:~$ export GITHUB_USERNAME=HeinrichBelarus
belarus@Roblox:~$ export GITHUB_EMAIL=scpfapplicationsbot@gmail.com
belarus@Roblox:~$ export GITHUB_TOKEN=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
belarus@Roblox:~$ alias edit=nano
belarus@Roblox:~$ cd ${GITHUB_USERNAME}/workspace
belarus@Roblox:~/HeinrichBelarus/workspace$ source scripts/activate
belarus@Roblox:~/HeinrichBelarus/workspace$ mkdir ~/.config
mkdir: cannot create directory ‘/home/belarus/.config’: File exists
belarus@Roblox:~/HeinrichBelarus/workspace$ cat > ~/.config/hub <<EOF
github.com:
- user: ${GITHUB_USERNAME}
  oauth_token: ${GITHUB_TOKEN}
  protocol: https
EOF
belarus@Roblox:~/HeinrichBelarus/workspace$ git config --global hub.protocol https
belarus@Roblox:~/HeinrichBelarus/workspace$ mkdir projects/lab02 && cd projects/lab02
mkdir: cannot create directory ‘projects/lab02’: File exists
belarus@Roblox:~/HeinrichBelarus/workspace$ git init
Reinitialized existing Git repository in /home/belarus/HeinrichBelarus/workspace/.git/
belarus@Roblox:~/HeinrichBelarus/workspace$ git config --global user.name ${GITHUB_USERNAME}
belarus@Roblox:~/HeinrichBelarus/workspace$ git config --global user.email ${GITHUB_EMAIL}
belarus@Roblox:~/HeinrichBelarus/workspace$ git config -e --global
belarus@Roblox:~/HeinrichBelarus/workspace$ git remote add origin https://github.com/${GITHUB_USERNAME}/lab02.git
error: remote origin already exists.
belarus@Roblox:~/HeinrichBelarus/workspace$ git pull origin master
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (4/4), 1.51 KiB | 1.51 MiB/s, done.
From https://github.com/HeinrichBelarus/lab02
 * branch            master     -> FETCH_HEAD
 + 5ab4d6f...81799a6 master     -> origin/master  (forced update)
hint: You have divergent branches and need to specify how to reconcile them.
hint: You can do so by running one of the following commands sometime before
hint: your next pull:
hint: 
hint:   git config pull.rebase false  # merge
hint:   git config pull.rebase true   # rebase
hint:   git config pull.ff only       # fast-forward only
hint: 
hint: You can replace "git config" with "git config --global" to set a default
hint: preference for all repositories. You can also pass --rebase, --no-rebase,
hint: or --ff-only on the command line to override the configured default per
hint: invocation.
fatal: Need to specify how to reconcile divergent branches.
belarus@Roblox:~/HeinrichBelarus/workspace$ git config pull.rebase true
belarus@Roblox:~/HeinrichBelarus/workspace$ git pull origin master
From https://github.com/HeinrichBelarus/lab02
 * branch            master     -> FETCH_HEAD
warning: unable to rmdir 'projects/lab02': Directory not empty
warning: unable to rmdir 'tasks/lab01': Directory not empty
Successfully rebased and updated refs/heads/master.
belarus@Roblox:~/HeinrichBelarus/workspace$ touch README.md
belarus@Roblox:~/HeinrichBelarus/workspace$ git status
On branch master
nothing to commit, working tree clean
belarus@Roblox:~/HeinrichBelarus/workspace$ git add README.md
belarus@Roblox:~/HeinrichBelarus/workspace$ git commit -m"added README.md"
On branch master
nothing to commit, working tree clean
belarus@Roblox:~/HeinrichBelarus/workspace$ git push origin master
Enumerating objects: 2995, done.
Counting objects: 100% (2995/2995), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2815/2815), done.
Writing objects: 100% (2994/2994), 13.50 MiB | 6.71 MiB/s, done.
Total 2994 (delta 519), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (519/519), done.
remote: error: GH013: Repository rule violations found for refs/heads/master.
remote: 
remote: - GITHUB PUSH PROTECTION
remote:   —————————————————————————————————————————
remote:     Resolve the following violations before pushing again
remote: 
remote:     - Push cannot contain secrets
remote: 
remote:     
remote:      (?) Learn how to resolve a blocked push
remote:      https://docs.github.com/code-security/secret-scanning/working-with-secret-scanning-and-push-protection/working-with-push-protection-from-the-command-line#resolving-a-blocked-push
remote:     
remote:     
remote:       —— GitHub Personal Access Token ——————————————————————
remote:        locations:
remote:          - commit: 4a0053889bdc1aa4515087abcfba72199b9ed02c
remote:            path: reports/lab01/REPORT.md:6
remote:     
remote:        (?) To push, remove secret from commit(s) or follow this URL to allow the secret.
remote:        https://github.com/HeinrichBelarus/lab02/security/secret-scanning/unblock-secret/2wydHARWJzbfJ0J55s2lkWo6wIr
remote:     
remote: 
remote: 
To https://github.com/HeinrichBelarus/lab02.git
 ! [remote rejected] master -> master (push declined due to repository rule violations)
error: failed to push some refs to 'https://github.com/HeinrichBelarus/lab02.git'
belarus@Roblox:~/HeinrichBelarus/workspace$ git push origin master
Enumerating objects: 2995, done.
Counting objects: 100% (2995/2995), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2815/2815), done.
Writing objects: 100% (2994/2994), 13.50 MiB | 6.59 MiB/s, done.
Total 2994 (delta 520), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (520/520), done.
To https://github.com/HeinrichBelarus/lab02.git
   81799a6..e941ca2  master -> master
belarus@Roblox:~/HeinrichBelarus/workspace$ git pull origin master
remote: Enumerating objects: 4, done.
remote: Counting objects: 100% (4/4), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (3/3), 953 bytes | 953.00 KiB/s, done.
From https://github.com/HeinrichBelarus/lab02
 * branch            master     -> FETCH_HEAD
   e941ca2..4238e30  master     -> origin/master
Updating e941ca2..4238e30
Fast-forward
 .gitignore | 4 ++++
 1 file changed, 4 insertions(+)
 create mode 100644 .gitignore
belarus@Roblox:~/HeinrichBelarus/workspace$ git log
commit 4238e30e45a0efcf7a0db46b6763036d32b35078 (HEAD -> master, origin/master)
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 05:43:01 2025 +0300

    Create .gitignore

commit e941ca287c9ab264baf98cc5149c12816b78ec91
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 02:23:03 2025 +0000

    added README.md

commit 4a0053889bdc1aa4515087abcfba72199b9ed02c
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 01:52:43 2025 +0000

    added sources

commit 81799a60ab26750a55a4f21ec5f7942e412fee34
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 05:36:35 2025 +0300

    Initial commit
set mark: ...skipping...
commit 4238e30e45a0efcf7a0db46b6763036d32b35078 (HEAD -> master, origin/master)
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 05:43:01 2025 +0300

    Create .gitignore

commit e941ca287c9ab264baf98cc5149c12816b78ec91
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 02:23:03 2025 +0000

    added README.md

commit 4a0053889bdc1aa4515087abcfba72199b9ed02c
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 01:52:43 2025 +0000

    added sources

commit 81799a60ab26750a55a4f21ec5f7942e412fee34
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 05:36:35 2025 +0300

    Initial commit
...skipping...
commit 4238e30e45a0efcf7a0db46b6763036d32b35078 (HEAD -> master, origin/master)
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 05:43:01 2025 +0300

    Create .gitignore

commit e941ca287c9ab264baf98cc5149c12816b78ec91
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 02:23:03 2025 +0000

    added README.md

commit 4a0053889bdc1aa4515087abcfba72199b9ed02c
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 01:52:43 2025 +0000

    added sources

commit 81799a60ab26750a55a4f21ec5f7942e412fee34
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 05:36:35 2025 +0300

    Initial commit
log file: ource...skipping...
commit 4238e30e45a0efcf7a0db46b6763036d32b35078 (HEAD -> master, origin/master)
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 05:43:01 2025 +0300

    Create .gitignore

commit e941ca287c9ab264baf98cc5149c12816b78ec91
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 02:23:03 2025 +0000

    added README.md

commit 4a0053889bdc1aa4515087abcfba72199b9ed02c
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 01:52:43 2025 +0000

    added sources

commit 81799a60ab26750a55a4f21ec5f7942e412fee34
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 05:36:35 2025 +0300

    Initial commit
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
(END)
































commit 4238e30e45a0efcf7a0db46b6763036d32b35078 (HEAD -> master, origin/master)
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 05:43:01 2025 +0300

    Create .gitignore

commit e941ca287c9ab264baf98cc5149c12816b78ec91
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 02:23:03 2025 +0000

    added README.md

commit 4a0053889bdc1aa4515087abcfba72199b9ed02c
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 01:52:43 2025 +0000

    added sources

commit 81799a60ab26750a55a4f21ec5f7942e412fee34
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 05:36:35 2025 +0300

    Initial commit
~
~
~
~
~
~
~
~
 ESCOD
































commit 4238e30e45a0efcf7a0db46b6763036d32b35078 (HEAD -> master, origin/master)
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 05:43:01 2025 +0300

    Create .gitignore

commit e941ca287c9ab264baf98cc5149c12816b78ec91
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 02:23:03 2025 +0000

    added README.md

commit 4a0053889bdc1aa4515087abcfba72199b9ed02c
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 01:52:43 2025 +0000

    added sources

commit 81799a60ab26750a55a4f21ec5f7942e412fee34
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 05:36:35 2025 +0300

    Initial commit
~
~
~
~
~
~
~
~
 ESCOD
































commit 4238e30e45a0efcf7a0db46b6763036d32b35078 (HEAD -> master, origin/master)
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 05:43:01 2025 +0300

    Create .gitignore

commit e941ca287c9ab264baf98cc5149c12816b78ec91
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 02:23:03 2025 +0000

    added README.md

commit 4a0053889bdc1aa4515087abcfba72199b9ed02c
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 01:52:43 2025 +0000

    added sources

commit 81799a60ab26750a55a4f21ec5f7942e412fee34
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 05:36:35 2025 +0300

    Initial commit
~
~
~
~
~
~
~
~
 ESCOD
































commit 4238e30e45a0efcf7a0db46b6763036d32b35078 (HEAD -> master, origin/master)
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 05:43:01 2025 +0300

    Create .gitignore

commit e941ca287c9ab264baf98cc5149c12816b78ec91
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 02:23:03 2025 +0000

    added README.md

commit 4a0053889bdc1aa4515087abcfba72199b9ed02c
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 01:52:43 2025 +0000

    added sources

commit 81799a60ab26750a55a4f21ec5f7942e412fee34
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 05:36:35 2025 +0300

    Initial commit
~
~
~
~
~
~
~
~
 ESCOD
































commit 4238e30e45a0efcf7a0db46b6763036d32b35078 (HEAD -> master, origin/master)
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 05:43:01 2025 +0300

    Create .gitignore

commit e941ca287c9ab264baf98cc5149c12816b78ec91
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 02:23:03 2025 +0000

    added README.md

commit 4a0053889bdc1aa4515087abcfba72199b9ed02c
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 01:52:43 2025 +0000

    added sources

commit 81799a60ab26750a55a4f21ec5f7942e412fee34
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 05:36:35 2025 +0300

    Initial commit
~
~
~
~
~
~
~
~
 ESCOD
































commit 4238e30e45a0efcf7a0db46b6763036d32b35078 (HEAD -> master, origin/master)
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 05:43:01 2025 +0300

    Create .gitignore

commit e941ca287c9ab264baf98cc5149c12816b78ec91
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 02:23:03 2025 +0000

    added README.md

commit 4a0053889bdc1aa4515087abcfba72199b9ed02c
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 01:52:43 2025 +0000

    added sources

commit 81799a60ab26750a55a4f21ec5f7942e412fee34
Author: HeinrichBelarus <scpfapplicationsbot@gmail.com>
Date:   Mon May 12 05:36:35 2025 +0300

    Initial commit
~
~
~
~
~
~
~
~
 ESCOC
































ter, origin/master)






















~
~
~
~
~
~
~
~
 ESCOC
































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
~
~
~
~























~
(END)
























~
~
~
~
~
~
~













:



























~
~
~
~
~
~
~
















:
































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
(END)
































~
~
~
~
~
~
~























~
set mark: ...skipping...
~
~
~
~
~
~
~























~
...skipping...
~
~
~
~
~
~
~























~
set mark: ...skipping...
~
~
~
~
~
~
~























~
...skipping...
~
~
~
~
~
~
~























~

[1]+  Stopped                 git log
belarus@Roblox:~/HeinrichBelarus/workspace$ mkdir sources
mkdir: cannot create directory ‘sources’: File exists
belarus@Roblox:~/HeinrichBelarus/workspace$ mkdir include
mkdir: cannot create directory ‘include’: File exists
belarus@Roblox:~/HeinrichBelarus/workspace$ mkdir examples
mkdir: cannot create directory ‘examples’: File exists
belarus@Roblox:~/HeinrichBelarus/workspace$ cat > sources/print.cpp <<EOF
#include <print.hpp>

void print(const std::string& text, std::ostream& out)
{
  out << text;
}

void print(const std::string& text, std::ofstream& out)
{
  out << text;
}
EOF
belarus@Roblox:~/HeinrichBelarus/workspace$ cat > include/print.hpp <<EOF
#include <fstream>
#include <iostream>
#include <string>

void print(const std::string& text, std::ofstream& out);
void print(const std::string& text, std::ostream& out = std::cout);
EOF

$ cat > examples/example1.cpp <<EOF
#include <print.hpp>

int main(int argc, char** argv)
{
  print("hello");
}
EOF
$: command not found
belarus@Roblox:~/HeinrichBelarus/workspace$ cat > include/print.hpp <<EOF
#include <fstream>
#include <iostream>
#include <string>

void print(const std::string& text, std::ofstream& out);
void print(const std::string& text, std::ostream& out = std::cout);
EOF

$ cat > examples/example1.cpp <<EOF
#include <print.hpp>

int main(int argc, char** argv)
{
  print("hello");
}
EOF
$: command not found
belarus@Roblox:~/HeinrichBelarus/workspace$ cat > include/print.hpp <<EOF
#include <fstream>
#include <iostream>
#include <string>

void print(const std::string& text, std::ofstream& out);
void print(const std::string& text, std::ostream& out = std::cout);
EOF

$ cat > examples/example1.cpp <<EOF
#include <print.hpp>

int main(int argc, char** argv)
{
  print("hello");
}
EOF
$: command not found
belarus@Roblox:~/HeinrichBelarus/workspace$  cat > examples/example2.cpp <<EOF
#include <print.hpp>

#include <fstream>

int main(int argc, char** argv)
{
  std::ofstream file("log.txt");
  print(std::string("hello"), file);
}
EOF
belarus@Roblox:~/HeinrichBelarus/workspace$ $ edit README.md
$: command not found
belarus@Roblox:~/HeinrichBelarus/workspace$ edit README.md
belarus@Roblox:~/HeinrichBelarus/workspace$ $ git status
$: command not found
belarus@Roblox:~/HeinrichBelarus/workspace$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
	modified:   examples/example1.cpp

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	ources

no changes added to commit (use "git add" and/or "git commit -a")
belarus@Roblox:~/HeinrichBelarus/workspace$ git add .
belarus@Roblox:~/HeinrichBelarus/workspace$ git commit -m"added sources"
[master 2d9ea1f] added sources
 2 files changed, 23 insertions(+), 6 deletions(-)
 create mode 100644 ources
belarus@Roblox:~/HeinrichBelarus/workspace$ git push origin master
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 4 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (5/5), 741 bytes | 741.00 KiB/s, done.
Total 5 (delta 1), reused 0 (delta 0), pack-reused 0
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/HeinrichBelarus/lab02.git
   4238e30..2d9ea1f  master -> master
belarus@Roblox:~/HeinrichBelarus/workspace$ cd ~/workspace/
bash: cd: /home/belarus/workspace/: No such file or directory
belarus@Roblox:~/HeinrichBelarus/workspace$ ls -l ~
total 40
drwxr-xr-x 2 belarus belarus 4096 May 11 22:33 Desktop
drwxr-xr-x 2 belarus belarus 4096 May 11 22:33 Documents
drwxr-xr-x 2 belarus belarus 4096 May 11 22:33 Downloads
drwxrwxr-x 3 belarus belarus 4096 May 11 23:09 HeinrichBelarus
drwxr-xr-x 2 belarus belarus 4096 May 11 22:33 Music
drwxr-xr-x 3 belarus belarus 4096 May 11 22:38 Pictures
drwxr-xr-x 2 belarus belarus 4096 May 11 22:33 Public
drwx------ 5 belarus belarus 4096 May 12 00:00 snap
drwxr-xr-x 2 belarus belarus 4096 May 11 22:33 Templates
drwxr-xr-x 2 belarus belarus 4096 May 11 22:33 Videos
belarus@Roblox:~/HeinrichBelarus/workspace$ pwd
/home/belarus/HeinrichBelarus/workspace
belarus@Roblox:~/HeinrichBelarus/workspace$ mkdir ~/workspace
belarus@Roblox:~/HeinrichBelarus/workspace$ cd ~/workspace/
belarus@Roblox:~/workspace$ export LAB_NUMBER=02
belarus@Roblox:~/workspace$ git clone https://github.com/tp-labs/lab${LAB_NUMBER}.git tasks/lab${LAB_NUMBER}
Cloning into 'tasks/lab02'...
remote: Enumerating objects: 96, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 96 (delta 0), reused 1 (delta 0), pack-reused 93 (from 1)
Receiving objects: 100% (96/96), 1.29 MiB | 5.04 MiB/s, done.
Resolving deltas: 100% (28/28), done.
belarus@Roblox:~/workspace$ mkdir reports/lab${LAB_NUMBER}
mkdir: cannot create directory ‘reports/lab02’: No such file or directory
belarus@Roblox:~/workspace$ mkdir reports
belarus@Roblox:~/workspace$ mkdir reports/lab${LAB_NUMBER}
belarus@Roblox:~/workspace$ cp tasks/lab${LAB_NUMBER}/README.md reports/lab${LAB_NUMBER}/REPORT.md
belarus@Roblox:~/workspace$ cd reports/lab${LAB_NUMBER}
belarus@Roblox:~/workspace/reports/lab02$ edit REPORT.md
