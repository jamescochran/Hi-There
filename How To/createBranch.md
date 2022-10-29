# Create a Branch

To create a branch on the cli you will first need to pull your repo. After that you are able to begin:

`git checkout -b [new_branches_name]`

From there you should have created the new branch with whatever you named it and you can now add things and push it. To check you are in the new branch issue:

`git branch -a`

When you are ready to commit your changes you will need to set the upstream. In the following example my new branch name is "manage_branches"

`git push --set-upstream origin manage_branches`
