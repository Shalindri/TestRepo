GIT Commands


### How to update a forked repo with git rebase

Step 1: Add the remote (original repo that you forked) and call it “upstream”
* git remote add upstream https://github.com/original-repo/goes-here.git
Step 2: Fetch all branches of remote upstream
* git fetch upstream
Step 3: Rewrite your master with upstream’s master using git rebase.
* git rebase upstream/master
Step 4: Push your updates to master. You may need to force the push with “--force”.
* git push origin master --force

[more info](https://medium.com/@topspinj/how-to-git-rebase-into-a-forked-repo-c9f05e821c8a)


