`git clone <addressoftherepo.git>` clones the repository to local.

`git add *` is a similar command that adds all the file

`git add filename.xyz` tracks a file

`git commit -m "message"` for commiting the changes

`git push` to send changes to git repository

### Branches

`git branch` to list all the local branches

`git checkout` for switching branches

`git checkout -b <branchnew>` creates a new branch called branchnew

`git checkout <branchab>` takes you to branchab

`git checkout <######>` where ###### are the first 6 characters from a commit log, takes to back to the time that commit was made

`git merge <branchxx>` merges content from branchxx to your current branch

`git log` branch specific, shows commit log

`git status` for status of the work in local

`git branch -d branchname` for deleting a branch
 
### Forking

Use the **Fork** button on GitHub to copy another user's repository to your GitHub. Clone the repository to local and go about usual business of `add`ing, `commit`ing and `push`ing to make changes to your copy of the repository.

For syncing with the original repository, [check](https://git-scm.com/docs/git-remote)

`git remote add upstream <linktooriginalrepo.git>`

`git pull` [check](https://git-scm.com/docs/git-pull) to make changes to local branch from a remote branch

### GitHub using ssh

If you are tired of typing your username and password each time you commit, check [this](https://help.github.com/en/github/authenticating-to-github/connecting-to-github-with-ssh)
