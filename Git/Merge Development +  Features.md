## Create the Development Branch
- Switch to `main` branch and update:
  ```bash
  git checkout main
  git pull origin main
  ```
- Create and push the new branch:
  ```bash
  git checkout -b development
  git push -u origin development
  ```

## Merge Feature Branches
- Switch to `development` branch and start merging:
  ```bash
  git checkout development
  git merge --no-ff <feature-branch>  # Replace <feature-branch> with actual branch name
  # Resolve conflicts and commit
  ```
- Repeat for each feature branch.

## Test Features
- Deploy/test the `development` branch to ensure all integrated features work together.

## Final Merge to Main
- Once tested, merge `development` back to `main`:
  ```bash
  git checkout main
  git merge --no-ff development
  git push origin main
  ```

This workflow helps manage and test multiple features before integrating them into the main production branch.
