elarus@Roblox:~$ $export GITHUB_USERNAME=HeinrichBelarus
GITHUB_USERNAME=HeinrichBelarus: command not found
belarus@Roblox:~$ $ export GITHUB_USERNAME=HeinrichBelarus
$: command not found
belarus@Roblox:~$ export GITHUB_USERNAME=HeinrichBelarus
belarus@Roblox:~$ export GIST_TOKEN=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
belarus@Roblox:~$ alias edit=vi
belarus@Roblox:~$ mkdir -p $HeinrichBelarus/workspace
mkdir: cannot create directory ‘/workspace’: Permission denied
belarus@Roblox:~$ sudo -p $HeinrichBelarus/workspace
usage: sudo -h | -K | -k | -V
usage: sudo -v [-ABkNnS] [-g group] [-h host] [-p prompt] [-u user]
usage: sudo -l [-ABkNnS] [-g group] [-h host] [-p prompt] [-U user]
            [-u user] [command [arg ...]]
usage: sudo [-ABbEHkNnPS] [-r role] [-t type] [-C num] [-D directory]
            [-g group] [-h host] [-p prompt] [-R directory] [-T timeout]
            [-u user] [VAR=value] [-i | -s] [command [arg ...]]
usage: sudo -e [-ABkNnS] [-r role] [-t type] [-C num] [-D directory]
            [-g group] [-h host] [-p prompt] [-R directory] [-T timeout]
            [-u user] file ...
belarus@Roblox:~$ mkdir -p ${HeinrichBelarus}/workspace
mkdir: cannot create directory ‘/workspace’: Permission denied
belarus@Roblox:~$ echo $GITHUB_USERNAME
HeinrichBelarus
belarus@Roblox:~$ mkdir -p HeinrichBelarus/workspace
belarus@Roblox:~$ cd $HeinrichBelarus/workspace
bash: cd: /workspace: No such file or directory
belarus@Roblox:~$ pwd
/home/belarus
belarus@Roblox:~$ cd $HeinrichBelarus/workspace
bash: cd: /workspace: No such file or directory
belarus@Roblox:~$ cd /home/HeinrichBelarus/workspace
bash: cd: /home/HeinrichBelarus/workspace: No such file or directory
belarus@Roblox:~$ echo $GITHUB_USERNAME
HeinrichBelarus
belarus@Roblox:~$ ls -l $GITHUB_USERNAME
total 4
drwxrwxr-x 2 belarus belarus 4096 May 11 23:09 workspace
belarus@Roblox:~$ pwd
/home/belarus
belarus@Roblox:~$ which nano
/usr/bin/nano
belarus@Roblox:~$ which vi
/usr/bin/vi
belarus@Roblox:~$ which vim
belarus@Roblox:~$ which subl
belarus@Roblox:~$ alias edit=nano
belarus@Roblox:~$ edit test_file.txt
belarus@Roblox:~$ mkdir -p $GITHUB_USERNAME/workspace
belarus@Roblox:~$ cd $GITHUB_USERNAME/workspace
belarus@Roblox:~/HeinrichBelarus/workspace$ pwd
/home/belarus/HeinrichBelarus/workspace
belarus@Roblox:~/HeinrichBelarus/workspace$ cd ..
belarus@Roblox:~/HeinrichBelarus$ pwd
/home/belarus/HeinrichBelarus
belarus@Roblox:~/HeinrichBelarus$ mkdir -p workspace/tasks/
belarus@Roblox:~/HeinrichBelarus$ kmdir -p workspace/projects/
Command 'kmdir' not found, did you mean:
  command 'mmdir' from deb simh (3.8.1-6.1)
  command 'mdir' from deb mtools (4.0.43-1)
  command 'rmdir' from deb coreutils (9.4-2ubuntu2)
  command 'mkdir' from deb coreutils (9.4-2ubuntu2)
Try: sudo apt install <deb name>
belarus@Roblox:~/HeinrichBelarus$ mkdir -p workspace/projects/
belarus@Roblox:~/HeinrichBelarus$ mkdir -p workspace/reports/
belarus@Roblox:~/HeinrichBelarus$ cd workspace
belarus@Roblox:~/HeinrichBelarus/workspace$ $wget https://nodejs.org/dist/v6.11.5/node-v6.11.5-linux-x64.tar.xz
bash: https://nodejs.org/dist/v6.11.5/node-v6.11.5-linux-x64.tar.xz: No such file or directory
belarus@Roblox:~/HeinrichBelarus/workspace$ wget https://nodejs.org/dist/v6.11.5/node-v6.11.5-linux-x64.tar.xz
--2025-05-11 23:27:22--  https://nodejs.org/dist/v6.11.5/node-v6.11.5-linux-x64.tar.xz
Resolving nodejs.org (nodejs.org)... 104.20.3.6, 172.66.128.116, 2606:4700:10::ac42:8074, ...
Connecting to nodejs.org (nodejs.org)|104.20.3.6|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 9356460 (8.9M) [application/x-xz]
Saving to: ‘node-v6.11.5-linux-x64.tar.xz’

node-v6.11.5-linux- 100%[===================>]   8.92M  8.71MB/s    in 1.0s    

2025-05-11 23:27:24 (8.71 MB/s) - ‘node-v6.11.5-linux-x64.tar.xz’ saved [9356460/9356460]

belarus@Roblox:~/HeinrichBelarus/workspace$ tar -xf node-v6.11.5-linux-x64.tar.xz
belarus@Roblox:~/HeinrichBelarus/workspace$ rm -rf node-v6.11.5-linux-x64.tar.xz
belarus@Roblox:~/HeinrichBelarus/workspace$ mv node-v6.11.5-linux-x64 node
belarus@Roblox:~/HeinrichBelarus/workspace$ ls node/bin
node  npm
belarus@Roblox:~/HeinrichBelarus/workspace$ echo ${PATH}
/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin:/snap/bin
belarus@Roblox:~/HeinrichBelarus/workspace$ export PATH=${PATH}:`pwd`/node/bin
belarus@Roblox:~/HeinrichBelarus/workspace$ echo ${PATH}
/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/snap/bin:/snap/bin:/home/belarus/HeinrichBelarus/workspace/node/bin
belarus@Roblox:~/HeinrichBelarus/workspace$ mkdir scripts
belarus@Roblox:~/HeinrichBelarus/workspace$ car > scripts/activate<<EOF
> export PATH=\${PATH}:`pwd`/node/bin
> EOF
Command 'car' not found, but can be installed with:
sudo apt install ucommon-utils
belarus@Roblox:~/HeinrichBelarus/workspace$ cat > scripts/activate<<EOF
export PATH=\${PATH}:`pwd`/node/bin
EOF
belarus@Roblox:~/HeinrichBelarus/workspace$ source scripts/activate
belarus@Roblox:~/HeinrichBelarus/workspace$ gem install gist
Command 'gem' not found, but can be installed with:
sudo snap install ruby           # version 3.4.3, or
sudo apt  install ruby-rubygems  # version 3.4.20-1
See 'snap info ruby' for additional versions.
belarus@Roblox:~/HeinrichBelarus/workspace$ sudo apt install ruby-gems
[sudo] password for belarus: 
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
E: Unable to locate package ruby-gems
belarus@Roblox:~/HeinrichBelarus/workspace$ gem install gist
Command 'gem' not found, but can be installed with:
sudo snap install ruby           # version 3.4.3, or
sudo apt  install ruby-rubygems  # version 3.4.20-1
See 'snap info ruby' for additional versions.
belarus@Roblox:~/HeinrichBelarus/workspace$ sudo apt install ruby-dev
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following additional packages will be installed:
  fonts-lato javascript-common libgmp-dev libgmpxx4ldbl libjs-jquery libruby
  libruby3.2 rake ruby ruby-net-telnet ruby-rubygems ruby-sdbm ruby-webrick
  ruby-xmlrpc ruby3.2 ruby3.2-dev ruby3.2-doc rubygems-integration
Suggested packages:
  apache2 | lighttpd | httpd gmp-doc libgmp10-doc libmpfr-dev ri bundler
The following NEW packages will be installed:
  fonts-lato javascript-common libgmp-dev libgmpxx4ldbl libjs-jquery libruby
  libruby3.2 rake ruby ruby-dev ruby-net-telnet ruby-rubygems ruby-sdbm
  ruby-webrick ruby-xmlrpc ruby3.2 ruby3.2-dev ruby3.2-doc
  rubygems-integration
0 upgraded, 19 newly installed, 0 to remove and 111 not upgraded.
Need to get 11.7 MB of archives.
After this operation, 64.5 MB of additional disk space will be used.
Do you want to continue? [Y/n] Y
Get:1 http://ru.archive.ubuntu.com/ubuntu noble/main amd64 fonts-lato all 2.015-1 [2,781 kB]
Get:2 http://ru.archive.ubuntu.com/ubuntu noble/main amd64 javascript-common all 11+nmu1 [5,936 B]
Get:3 http://ru.archive.ubuntu.com/ubuntu noble-updates/main amd64 libgmpxx4ldbl amd64 2:6.3.0+dfsg-2ubuntu6.1 [9,888 B]
Get:4 http://ru.archive.ubuntu.com/ubuntu noble-updates/main amd64 libgmp-dev amd64 2:6.3.0+dfsg-2ubuntu6.1 [340 kB]
Get:5 http://ru.archive.ubuntu.com/ubuntu noble/main amd64 libjs-jquery all 3.6.1+dfsg+~3.5.14-1 [328 kB]
Get:6 http://ru.archive.ubuntu.com/ubuntu noble/main amd64 rubygems-integration all 1.18 [5,336 B]
Get:7 http://ru.archive.ubuntu.com/ubuntu noble-updates/main amd64 ruby3.2 amd64 3.2.3-1ubuntu0.24.04.5 [50.7 kB]
Get:8 http://ru.archive.ubuntu.com/ubuntu noble/main amd64 ruby-rubygems all 3.4.20-1 [238 kB]
Get:9 http://ru.archive.ubuntu.com/ubuntu noble/main amd64 ruby amd64 1:3.2~ubuntu1 [3,466 B]
Get:10 http://ru.archive.ubuntu.com/ubuntu noble/main amd64 rake all 13.0.6-3 [61.6 kB]
Get:11 http://ru.archive.ubuntu.com/ubuntu noble/main amd64 ruby-net-telnet all 0.2.0-1 [13.3 kB]
Get:12 http://ru.archive.ubuntu.com/ubuntu noble-updates/main amd64 ruby-webrick all 1.8.1-1ubuntu0.1 [52.6 kB]
Get:13 http://ru.archive.ubuntu.com/ubuntu noble/main amd64 ruby-xmlrpc all 0.3.2-2 [24.8 kB]
Get:14 http://ru.archive.ubuntu.com/ubuntu noble/main amd64 ruby-sdbm amd64 1.0.0-5build4 [16.2 kB]
Get:15 http://ru.archive.ubuntu.com/ubuntu noble-updates/main amd64 libruby3.2 amd64 3.2.3-1ubuntu0.24.04.5 [5,341 kB]
Get:16 http://ru.archive.ubuntu.com/ubuntu noble/main amd64 libruby amd64 1:3.2~ubuntu1 [4,694 B]
Get:17 http://ru.archive.ubuntu.com/ubuntu noble-updates/main amd64 ruby3.2-dev amd64 3.2.3-1ubuntu0.24.04.5 [399 kB]
Get:18 http://ru.archive.ubuntu.com/ubuntu noble/main amd64 ruby-dev amd64 1:3.2~ubuntu1 [4,856 B]
Get:19 http://ru.archive.ubuntu.com/ubuntu noble-updates/main amd64 ruby3.2-doc all 3.2.3-1ubuntu0.24.04.5 [2,017 kB]
Fetched 11.7 MB in 1s (21.9 MB/s)       
Selecting previously unselected package fonts-lato.
(Reading database ... 151393 files and directories currently installed.)
Preparing to unpack .../00-fonts-lato_2.015-1_all.deb ...
Unpacking fonts-lato (2.015-1) ...
Selecting previously unselected package javascript-common.
Preparing to unpack .../01-javascript-common_11+nmu1_all.deb ...
Unpacking javascript-common (11+nmu1) ...
Selecting previously unselected package libgmpxx4ldbl:amd64.
Preparing to unpack .../02-libgmpxx4ldbl_2%3a6.3.0+dfsg-2ubuntu6.1_amd64.deb ...
Unpacking libgmpxx4ldbl:amd64 (2:6.3.0+dfsg-2ubuntu6.1) ...
Selecting previously unselected package libgmp-dev:amd64.
Preparing to unpack .../03-libgmp-dev_2%3a6.3.0+dfsg-2ubuntu6.1_amd64.deb ...
Unpacking libgmp-dev:amd64 (2:6.3.0+dfsg-2ubuntu6.1) ...
Selecting previously unselected package libjs-jquery.
Preparing to unpack .../04-libjs-jquery_3.6.1+dfsg+~3.5.14-1_all.deb ...
Unpacking libjs-jquery (3.6.1+dfsg+~3.5.14-1) ...
Selecting previously unselected package rubygems-integration.
Preparing to unpack .../05-rubygems-integration_1.18_all.deb ...
Unpacking rubygems-integration (1.18) ...
Selecting previously unselected package ruby3.2.
Preparing to unpack .../06-ruby3.2_3.2.3-1ubuntu0.24.04.5_amd64.deb ...
Unpacking ruby3.2 (3.2.3-1ubuntu0.24.04.5) ...
Selecting previously unselected package ruby-rubygems.
Preparing to unpack .../07-ruby-rubygems_3.4.20-1_all.deb ...
Unpacking ruby-rubygems (3.4.20-1) ...
Selecting previously unselected package ruby.
Preparing to unpack .../08-ruby_1%3a3.2~ubuntu1_amd64.deb ...
Unpacking ruby (1:3.2~ubuntu1) ...
Selecting previously unselected package rake.
Preparing to unpack .../09-rake_13.0.6-3_all.deb ...
Unpacking rake (13.0.6-3) ...
Selecting previously unselected package ruby-net-telnet.
Preparing to unpack .../10-ruby-net-telnet_0.2.0-1_all.deb ...
Unpacking ruby-net-telnet (0.2.0-1) ...
Selecting previously unselected package ruby-webrick.
Preparing to unpack .../11-ruby-webrick_1.8.1-1ubuntu0.1_all.deb ...
Unpacking ruby-webrick (1.8.1-1ubuntu0.1) ...
Selecting previously unselected package ruby-xmlrpc.
Preparing to unpack .../12-ruby-xmlrpc_0.3.2-2_all.deb ...
Unpacking ruby-xmlrpc (0.3.2-2) ...
Selecting previously unselected package ruby-sdbm:amd64.
Preparing to unpack .../13-ruby-sdbm_1.0.0-5build4_amd64.deb ...
Unpacking ruby-sdbm:amd64 (1.0.0-5build4) ...
Selecting previously unselected package libruby3.2:amd64.
Preparing to unpack .../14-libruby3.2_3.2.3-1ubuntu0.24.04.5_amd64.deb ...
Unpacking libruby3.2:amd64 (3.2.3-1ubuntu0.24.04.5) ...
Selecting previously unselected package libruby:amd64.
Preparing to unpack .../15-libruby_1%3a3.2~ubuntu1_amd64.deb ...
Unpacking libruby:amd64 (1:3.2~ubuntu1) ...
Selecting previously unselected package ruby3.2-dev:amd64.
Preparing to unpack .../16-ruby3.2-dev_3.2.3-1ubuntu0.24.04.5_amd64.deb ...
Unpacking ruby3.2-dev:amd64 (3.2.3-1ubuntu0.24.04.5) ...
Selecting previously unselected package ruby-dev:amd64.
Preparing to unpack .../17-ruby-dev_1%3a3.2~ubuntu1_amd64.deb ...
Unpacking ruby-dev:amd64 (1:3.2~ubuntu1) ...
Selecting previously unselected package ruby3.2-doc.
Preparing to unpack .../18-ruby3.2-doc_3.2.3-1ubuntu0.24.04.5_all.deb ...
Unpacking ruby3.2-doc (3.2.3-1ubuntu0.24.04.5) ...
Setting up javascript-common (11+nmu1) ...
Setting up fonts-lato (2.015-1) ...
Setting up ruby3.2-doc (3.2.3-1ubuntu0.24.04.5) ...
Setting up rubygems-integration (1.18) ...
Setting up libgmpxx4ldbl:amd64 (2:6.3.0+dfsg-2ubuntu6.1) ...
Setting up ruby-net-telnet (0.2.0-1) ...
Setting up ruby-webrick (1.8.1-1ubuntu0.1) ...
Setting up libjs-jquery (3.6.1+dfsg+~3.5.14-1) ...
Setting up ruby-xmlrpc (0.3.2-2) ...
Setting up libgmp-dev:amd64 (2:6.3.0+dfsg-2ubuntu6.1) ...
Setting up ruby3.2 (3.2.3-1ubuntu0.24.04.5) ...
Setting up libruby:amd64 (1:3.2~ubuntu1) ...
Setting up ruby (1:3.2~ubuntu1) ...
Setting up rake (13.0.6-3) ...
Setting up ruby-sdbm:amd64 (1.0.0-5build4) ...
Setting up libruby3.2:amd64 (3.2.3-1ubuntu0.24.04.5) ...
Setting up ruby-rubygems (3.4.20-1) ...
Setting up ruby3.2-dev:amd64 (3.2.3-1ubuntu0.24.04.5) ...
Setting up ruby-dev:amd64 (1:3.2~ubuntu1) ...
Processing triggers for man-db (2.12.0-4build2) ...
Processing triggers for fontconfig (2.15.0-1.1ubuntu2) ...
Processing triggers for libc-bin (2.39-0ubuntu8.4) ...
belarus@Roblox:~/HeinrichBelarus/workspace$ gem install gist
Fetching gist-6.0.0.gem
ERROR:  While executing gem ... (Gem::FilePermissionError)
    You don't have write permissions for the /var/lib/gems/3.2.0 directory.
	/usr/lib/ruby/vendor_ruby/rubygems/installer.rb:713:in `verify_gem_home'
	/usr/lib/ruby/vendor_ruby/rubygems/installer.rb:903:in `pre_install_checks'
	/usr/lib/ruby/vendor_ruby/rubygems/installer.rb:303:in `install'
	/usr/lib/ruby/vendor_ruby/rubygems/resolver/specification.rb:105:in `install'
	/usr/lib/ruby/vendor_ruby/rubygems/request_set.rb:195:in `block in install'
	/usr/lib/ruby/vendor_ruby/rubygems/request_set.rb:183:in `each'
	/usr/lib/ruby/vendor_ruby/rubygems/request_set.rb:183:in `install'
	/usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:215:in `install_gem'
	/usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:231:in `block in install_gems'
	/usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:224:in `each'
	/usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:224:in `install_gems'
	/usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:170:in `execute'
	/usr/lib/ruby/vendor_ruby/rubygems/command.rb:328:in `invoke_with_build_args'
	/usr/lib/ruby/vendor_ruby/rubygems/command_manager.rb:253:in `invoke_command'
	/usr/lib/ruby/vendor_ruby/rubygems/command_manager.rb:193:in `process_args'
	/usr/lib/ruby/vendor_ruby/rubygems/command_manager.rb:151:in `run'
	/usr/lib/ruby/vendor_ruby/rubygems/gem_runner.rb:52:in `run'
	/usr/bin/gem:12:in `<main>'
belarus@Roblox:~/HeinrichBelarus/workspace$ sudo apt install ruby-full
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following additional packages will be installed:
  ri
The following NEW packages will be installed:
  ri ruby-full
0 upgraded, 2 newly installed, 0 to remove and 111 not upgraded.
Need to get 7,294 B of archives.
After this operation, 24.6 kB of additional disk space will be used.
Do you want to continue? [Y/n] Y
Get:1 http://ru.archive.ubuntu.com/ubuntu noble/universe amd64 ri all 1:3.2~ubuntu1 [4,724 B]
Get:2 http://ru.archive.ubuntu.com/ubuntu noble/universe amd64 ruby-full all 1:3.2~ubuntu1 [2,570 B]
Fetched 7,294 B in 0s (114 kB/s)      
Selecting previously unselected package ri.
(Reading database ... 168365 files and directories currently installed.)
Preparing to unpack .../ri_1%3a3.2~ubuntu1_all.deb ...
Unpacking ri (1:3.2~ubuntu1) ...
Selecting previously unselected package ruby-full.
Preparing to unpack .../ruby-full_1%3a3.2~ubuntu1_all.deb ...
Unpacking ruby-full (1:3.2~ubuntu1) ...
Setting up ri (1:3.2~ubuntu1) ...
Setting up ruby-full (1:3.2~ubuntu1) ...
belarus@Roblox:~/HeinrichBelarus/workspace$ gem install gist
ERROR:  While executing gem ... (Gem::FilePermissionError)
    You don't have write permissions for the /var/lib/gems/3.2.0 directory.
	/usr/lib/ruby/vendor_ruby/rubygems/installer.rb:713:in `verify_gem_home'
	/usr/lib/ruby/vendor_ruby/rubygems/installer.rb:903:in `pre_install_checks'
	/usr/lib/ruby/vendor_ruby/rubygems/installer.rb:303:in `install'
	/usr/lib/ruby/vendor_ruby/rubygems/resolver/specification.rb:105:in `install'
	/usr/lib/ruby/vendor_ruby/rubygems/request_set.rb:195:in `block in install'
	/usr/lib/ruby/vendor_ruby/rubygems/request_set.rb:183:in `each'
	/usr/lib/ruby/vendor_ruby/rubygems/request_set.rb:183:in `install'
	/usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:215:in `install_gem'
	/usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:231:in `block in install_gems'
	/usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:224:in `each'
	/usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:224:in `install_gems'
	/usr/lib/ruby/vendor_ruby/rubygems/commands/install_command.rb:170:in `execute'
	/usr/lib/ruby/vendor_ruby/rubygems/command.rb:328:in `invoke_with_build_args'
	/usr/lib/ruby/vendor_ruby/rubygems/command_manager.rb:253:in `invoke_command'
	/usr/lib/ruby/vendor_ruby/rubygems/command_manager.rb:193:in `process_args'
	/usr/lib/ruby/vendor_ruby/rubygems/command_manager.rb:151:in `run'
	/usr/lib/ruby/vendor_ruby/rubygems/gem_runner.rb:52:in `run'
	/usr/bin/gem:12:in `<main>'
belarus@Roblox:~/HeinrichBelarus/workspace$ sudo gem install gist
Fetching gist-6.0.0.gem
Successfully installed gist-6.0.0
Parsing documentation for gist-6.0.0
Installing ri documentation for gist-6.0.0
Done installing documentation for gist after 0 seconds
1 gem installed
belarus@Roblox:~/HeinrichBelarus/workspace$ (unmask 0077 && echo ${GIST_TOKEN} >~/.gist)
Command 'unmask' not found, did you mean:
  command 'unmass' from deb unmass (0.9-7)
Try: sudo apt install <deb name>
belarus@Roblox:~/HeinrichBelarus/workspace$ (umask 0077 && echo ${GIST_TOKEN} >~/.gist)
belarus@Roblox:~/HeinrichBelarus/workspace$ export LAB_NUMBER=01
belarus@Roblox:~/HeinrichBelarus/workspace$ git clone https://github.com/tp-labs/lab${LAB_NUMBER} tasks/lab${LAB_NUMBER}
Command 'git' not found, but can be installed with:
sudo apt install git
belarus@Roblox:~/HeinrichBelarus/workspace$ sudo apt install git
Reading package lists... Done
Building dependency tree... Done
Reading state information... Done
The following additional packages will be installed:
  git-man liberror-perl
Suggested packages:
  git-daemon-run | git-daemon-sysvinit git-doc git-email git-gui gitk gitweb git-cvs git-mediawiki
  git-svn
The following NEW packages will be installed:
  git git-man liberror-perl
0 upgraded, 3 newly installed, 0 to remove and 111 not upgraded.
Need to get 4,804 kB of archives.
After this operation, 24.5 MB of additional disk space will be used.
Do you want to continue? [Y/n] Y
Get:1 http://ru.archive.ubuntu.com/ubuntu noble/main amd64 liberror-perl all 0.17029-2 [25.6 kB]
Get:2 http://ru.archive.ubuntu.com/ubuntu noble-updates/main amd64 git-man all 1:2.43.0-1ubuntu7.2 [1,100 kB]
Get:3 http://ru.archive.ubuntu.com/ubuntu noble-updates/main amd64 git amd64 1:2.43.0-1ubuntu7.2 [3,679 kB]
Fetched 4,804 kB in 0s (25.5 MB/s)
Selecting previously unselected package liberror-perl.
(Reading database ... 168371 files and directories currently installed.)
Preparing to unpack .../liberror-perl_0.17029-2_all.deb ...
Unpacking liberror-perl (0.17029-2) ...
Selecting previously unselected package git-man.
Preparing to unpack .../git-man_1%3a2.43.0-1ubuntu7.2_all.deb ...
Unpacking git-man (1:2.43.0-1ubuntu7.2) ...
Selecting previously unselected package git.
Preparing to unpack .../git_1%3a2.43.0-1ubuntu7.2_amd64.deb ...
Unpacking git (1:2.43.0-1ubuntu7.2) ...
Setting up liberror-perl (0.17029-2) ...
Setting up git-man (1:2.43.0-1ubuntu7.2) ...
Setting up git (1:2.43.0-1ubuntu7.2) ...
Processing triggers for man-db (2.12.0-4build2) ...
belarus@Roblox:~/HeinrichBelarus/workspace$ git clone https://github.com/tp-labs/lab${LAB_NUMBER} tasks/lab${LAB_NUMBER}
Cloning into 'tasks/lab01'...
remote: Enumerating objects: 74, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (3/3), done.
remote: Total 74 (delta 0), reused 1 (delta 0), pack-reused 71 (from 1)
Receiving objects: 100% (74/74), 945.07 KiB | 3.65 MiB/s, done.
Resolving deltas: 100% (20/20), done.
belarus@Roblox:~/HeinrichBelarus/workspace$ mkdir reports/lab${LAB_NUMBER}
belarus@Roblox:~/HeinrichBelarus/workspace$ cp tasks/lab${LAB_NUMBER}/README.md reports/lab${LAB_NUMBER}/REPORT.md
belarus@Roblox:~/HeinrichBelarus/workspace$ cd reports/lab${LAB_NUMBER}
belarus@Roblox:~/HeinrichBelarus/workspace/reports/lab01$ edit REPORT.md
belarus@Roblox:~/HeinrichBelarus/workspace/reports/lab01$ gist REPORT.md
https://gist.github.com/HeinrichBelarus/a1d4f5ad0c36348d692eefd613d66550
belarus@Roblox:~/HeinrichBelarus/workspace/reports/lab01$ edit REPORT.md
belarus@Roblox:~/HeinrichBelarus/workspace/reports/lab01$ 

