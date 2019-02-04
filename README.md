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
