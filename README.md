Git Commands
===========

List of Useful Git commands

###Visualize commits
> gitk --all &

###List All Branches
> git branch &lt;branchName&gt;

###See hidden branches
> git branch -a 

###Create a branch without checking out to that branch
> git branch &lt;branchName&gt;

###Create and check out to a branch
> git checkout -b &lt;branchName&gt;

###Safely delete a branch
> git branch -d &lt;branchName&gt;

###Delete a branch even with unmerged changes
> git branch -D &lt;branchName&gt;

###Merging with another branch
*go to target branch*
> git merge &lt;source-branchName&gt;

###Base branch on another branch
git checkout -b &lt;branchName&gt; &lt;branchToBaseFrom&gt;

###Checkout a remote branch and setup local tracking
> git checkout -b &lt;branchName&gt; origin/&lt;branchName&gt;

*Alternative (shorter) way to checkout an existing remote branch*
> git checkout &lt;branchName&gt;

###Stash changes
> git stash

*do your stuff and then revert back*
> git stash pop

###Pull in remote branch
> git fetch &lt;remoteName&gt;

###Trace File history
> git blame &lt;fileName&gt;

###Deleting a branch from remote
> git push origin --delete &lt;branchName&gt;

###Push a local branch to remote
> git push -u origin &lt;branchName&gt;

### Git log
> git log --pretty=oneline

###Git tags
*to list tags*

> git tag

*to add tag*
> git tag &lt;tagName&gt;

> git push origin --tags

*delete tag*
> git tag -d &lt;tagName&gt;

*delete tag on remote*
> git push origin :refs/tags/&lt;tagName&gt

###Undo commits
*Undo one commit*
> git reset HEAD

*Undo a number of commits*
> git reset --hard HEAD~3

*Rename branch*
> git branch -m &lt;branch&gt;

*Delete a remote*
> git remote rm <remoteName>

*Add a new Remote*
git remote add origin-br git@github.com:blueraster/gfw-commodities-app.git

<!-- *Track the curent branch to a different remote branch*
git branch -u git@github.com:blueraster/gfw-commodities-app.git/master
 -->

*Track current branch to a different remote branch*
git branch -u origin-br &lt;branchName&gt;

git branch develop-br -u origin-br/master
git branch --set-upstream develop-br origin-br/master

*Pull from remote branch into current branch
git pull origin-br &lt;remoteBranchName&gt; 
git pull origin-br master; 

*Push current branch to remote branch
git push origin-br &lt;remoteBranchName&gt; 
git push origin-br develop-br; 

*Steps to Push to different Repo's Remote Branch*
git checkout -b develop-br
git remote add origin-br git@github.com:blueraster/gfw-commodities-app.git
git pull origin-br master
git push origin-br develop-br;
