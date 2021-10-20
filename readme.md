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



### How to revert the last commit
git checkout <hash of your good commit message>
git push -f origin last_known_good_commit:branch_name

### How to squash commits
* git rebase -i HEAD~<no of commits >

* These commands will bring up the below interface with options to perform the following: <br>
p, pick = use commit<br>
r, reword = use commit, but edit the commit message<br>
e, edit = use commit, but stop for amending<br>
s, squash = use commit, but meld into previous commit<br>
f, fixup = like “squash”, but discard this commit’s log message<br>
x, exec = run command (the rest of the line) using shell<br>
d, drop = remove commit<br>

[more info](https://medium.com/@slamflipstrom/a-beginners-guide-to-squashing-commits-with-git-rebase-8185cf6e62ec)


### How to change the last commit message after push

* git commit --amend -m "New message"
* git push --force repository-name branch-name
* 	Ex:- git push --force origin feature-revocation-api


