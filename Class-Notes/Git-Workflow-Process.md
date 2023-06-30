Github workflow is:

1. create and name a branch `git checkout -b WMM001`
2. specify which remote repo we're working on: `git remote set-url origin <SSH_URL>`
  * Only one time per project
3. Perform work on the actual code files
4. Move files: Working Directory $\rightarrow$ Staging Area `git add .`
5. Move files: Staging Area $\rightarrow$ Local Repo  `git commit -m "did some stuff"`
6. Move files: Local Repo $\rightarrow$ Remote Repo  `git push -u origin WMM001`
  * This goes specifically to the branch you're working on
7. Change to the main branch `git checkout main`
8. Merge your work from the branch to main branch `git merge WMM001`
9. Push work to main `git push -u origin main`
