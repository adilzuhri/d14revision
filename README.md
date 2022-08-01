# d14revision
#Reference

##Maven Command

mvnw

mvnw compile

mvnw clean package

mvnw spring-boot:run

mvnw clean package spring-boot:run

mvnw spring-boot:run -Dspring-boot.run.arguments="--port=3000"

mvnw spring-boot:run -Dspring-boot.run.arguments="--port=3000 --dataDir=c:\data"

mvnw clean test

##Git command

git init (initial a local repo, doesn't link to remote yet)

git remote add origin https://github.com//.git

git add * (add new/updated files to be commited into local repo)

git status (to check files that are going to commit into local repo)

git commit -m "" (commit new/updated files to local repo)

git push -u origin master (create a master branch in github and push the code to github master branch)

<don't develop in master branch - final/latest working baseline>

git checkout -b develop master (clone a copy from master to develop branch locally)

git push -u origin develop (push from local develop branch to github develop branch)

git checkout develop (to switch between branches)

git branch -a (show all local branches and remote branch refernces)

git branch (show all local branches)

git add *

git commit -m ""

git push -u origin develop (push code on local develop branch to github develop branch)

git checkout master

git merge develop (after changes in develop branch are complete without errors, in master branch, merge changes from develop branch)

git push -u origin master (in master branch to push merged changes from develop branch to github master branch)

##Deploy to heroku (must be on master branch locally and remote)

Create/use an existing heroku account

On your project root, you need a system.properties file.

put the following line in system.properties files. java.runtime.version=18

git add *

git commit -m "added/updated system.properties"

git push -u origin master

heroku login (in your terminal window/command prompt in the project root directory)

heroku apps:create

git remote -v (all remote branches. you should see refernce URL to heroku)

git push -u heroku master
