Git Commands
===========

List of Useful Git commands

###Visualize commits
> gitk --all &

###Checkout a branch
> git checkout -b &lt;branchName&gt;

###Merging with another branch
*go to target branch*
> git merge &lt;source-branchName&gt;

###See hidden branches
> git branch -a

###Checkout a remote branch and setup local tracking
> git checkout -b &lt;branchName&gt; origin&lt;branchName&gt;

###Stash changes
*stash temporaily*
> git stash

*do your stuff and them revert back*
> git stash pop

###Pull in remote branch
> git fetch &lt;remoteName&gt;

###Trace File history
> git blame &lt;fileName&gt;

###Deleting a branch from remote
> git push origin --delete &lt;branchName&gt;

###Push a local branch to remote
> git branch &lt;branchName&gt;
> git push -u origin &lt;branchName&gt;

### Git log
> git log --pretty=oneline

###Git tags
*to list tags*
> git tag

*to add tag*
> git tag &lt;tagName&gt;
> git push origin --tags

> delete tag
> git tag -d &lt;tagName&gt;

###Undo commits
*Undo one commit*
> git reset HEAD

*Undo a number of commits*
> git reset --hard HEAD~3

