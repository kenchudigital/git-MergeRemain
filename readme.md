branch: main

## Git Merge for Muti-stage Deployment

content: This is dev final update, which will merge to main branch, and I need the branch name in main is no change.

1. I created the `branch: main` in main branch
2. Create the new branch `dev` and change the name to `branch: dev`
3. After that, back to main branch and then `git merge dev`
4. It show the message:
```bash
Merge branch 'dev'
# Please enter a commit message to explain why this merge is necessary,
# especially if it merges an updated upstream into a topic branch.
#
# Lines starting with '#' will be ignored, and an empty message aborts
# the commit.
``` 
5. Of course, you can change the file like this:
```bash
Merge dev into main
- Updated branch name in README.md from dev to main
- Merged changes from dev into main branch
```
6. `:q` and then `git push`

<br>


## Why this is important?

By setting up path names that correspond to different stages (e.g., production, staging, development), you can ensure that files are automatically routed to the appropriate locations. This setup is crucial for automating deployments and managing files efficiently within a CI/CD pipeline.

## If only main branch update

Please remember to `git fetch main` and then, `git merge main` to update the dev branch.