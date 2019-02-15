#### For more info, you may visit below link:
  * https://www.atlassian.com/git/tutorials/syncing/git-pull
#### Things you need to do to add files on github if you alredy have existing files in it
  * You clone {link}
  * go into the folder
  * git status
  * you may add username and email with below commands
  * git config --global user.name "robin"
  * git config --global user.email "xyz@gmail.com"
  * you can make change in files if you want
  * git commit -a -m "message" or follow below step
  * you may do git add {file.txt} or git add . ->to add anything and then commit with message
  * git log 
  * you will see the commit id
  * git reset {commit id} to return back to previous changes
  * git pull -> You want to pull from github when somebody makes changes on github(remote) and you want to have that change reflect on your local
  * Note: git pull {remote} -> is same as git fetch {remote} followed by git merge origin/{current branch}
  * git remote (will show origin)
  * git push origin master (where origin -> remote and branch -> master)
  
#### Things you need to do want to create a new folder and make a complete start using new repo
  * git init (do ls -lart) (you will see .git hidden directory)
  * git remote (you will not see anything since you are starting a complete new setup from local)
  * git remote -v (you may not see anything)
  * don't initialize with redme
  * git remote add origin {link}
  * git remote or git remote -v to see
  * git push origin master 
#### To work on different branches
  * git branch
  * git branch development
  * git checkout development
  * make changes
  * git push master
  * git checkout master
  * git merge development
#### Resolving confict
  * you neet to resolve git conflict if two developers made changes in the same line of code.
  * On github, you need to delete lines like >>>>>> and =======
  * Do commit merge.
  * Merge merge pull request and confirm merge
  
#### Create a repo mysource, add some files, clone it locally and then push it to  new repo called mytarget
  * Create a new repo at github (do not add any readme file or initialize git).
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
  * chmod 700 {filename}
  * chmod 600 {filename}
  * chmod 755 {filename} and so on
#### More, less, head, tail
  * more >> enter (more%) , b (less%)
  * less >> space (down) b (up)
  * head >> top 10 content within a file
  * tail >> buttom 10 content within a file 
