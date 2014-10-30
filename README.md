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
> git checkout -d &lt;branchName&gt;

###Delete a branch even with unmerged changes
> git checkout -D &lt;branchName&gt;

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

###Undo commits
*Undo one commit*
> git reset HEAD

*Undo a number of commits*
> git reset --hard HEAD~3

*Rename branch*
> git branch -m &lt;branch&gt;