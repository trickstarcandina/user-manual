Deleting the .git folder may cause problems in your git repository. 
If you want to delete all your commit history but keep the code in its current state, it is very safe to do it as in the following:

1. Checkout

> - git checkout --orphan latest_branch

2. Add all the files

> - git add -A

3. Commit the changes

> - git commit -am "commit message"

4. Delete the branch

> - git branch -D main

5. Rename the current branch to main

> - git branch -m main

6. Finally, force update your repository

> - git push -f origin main

PS: this will not keep your old commit history around
