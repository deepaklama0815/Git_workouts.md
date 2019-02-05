#### Create a repo mysource, add some files, clone it locally and then push it to  new repo called mytarget
  * Create a new repo at github.
  * Create second repo
  * Clone 1st repo (under 1st repo folder, create some files) git clone in local (copy source path and clone)
  * Git remote -v (will take origin by default)
  * git remote add target(secondrepo) (copy target path)
  * git remote -v
  * git push target master
  


#### Create a repo on github, create development branch, add some changes to development branch and then merge it with master
  * create branch called development
  * make some changes in files
  * Create base: master and compare with: development
  * create a pull request 
  * pull request merged by master

#### Create a repo, changes the default branch from master to development
  * git branch development
  * on settings, go to branches change the default branch and make update.
#### You can have Branch protection  rule 
#### Reset must be done within the same branch
  * git log
  * copy the commit id of unchanged version
  * git (commit id) --hard (throws back to earlier place)
#### Working with branches
  * git branch development -- will create a development branch
  * git checkout development -- you can now make some changes in development branch
  * git add .
  * git commit -m "made changes"
  * git push -u origin master -- will push changes made in development to master
  * git merge development -- will merge changes in development
#### .gitignore
  * you can keep files inside .gitignore and if you do git status, you will see only .gitignore 
  * lets say you make abc.log, bcd.log and .gitignore; you can vi .gitignore and .*log inside it. You can see the files by ls but you only see .gitignore in git status. 
#### setting password as user
  * cd 
  * sudo useradd robin
  * sudo passwd robin
#### create a shortcut of /tmp/abc.txt in home directory
  * cd /
  * vi /tmp/abc.txt
  * cd
  * ln -s /tmp/abc.txt shortcutabc.txt
#### giving permission to file name
  * chmod 700 <filename>
  * chmod 600 <filename>
  * chmod 755 <filename> and so on
#### More, less, head, tail
  * more >> enter (more%) , b (less%)
  * less >> space (down) b (up)
  * head >> top 10 content within a file
  * tail >> buttom 10 content within a file 
