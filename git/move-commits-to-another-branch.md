# Move commits to another branch 

If you discover you’ve been working on the wrong branch and already committed your changes, don’t worry! 
Here’s an easy way to move those changes to a new branch:

1. Create a new branch from the right base (e.g., `main`):

```bash
git branch hotfix/fix-things
```

2. "Uncommit" your recent commits in the old branch, preserving changes in your working directory:

```bash
git reset --soft HEAD~1
```
(Replace `1` with the number of commits to move)

3. Stash the changes to move them to the new branch:

```bash
git stash
```

4. Switch to the new branch
   
```bash
git checkout hotfix/fix-things
```

5. Reapply your stashed changes:
   
```bash
git stash pop
```
Finally, commit the changes to the new branch.
