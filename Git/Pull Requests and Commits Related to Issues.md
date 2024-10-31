
### 1. Linking Commits to Issues
When committing changes that address specific issues:
- Include a brief, clear commit message that describes the changes.
- Use keywords followed by the issue number to link the commit to the issue. Examples of keywords include:
  - `fixes #<issue_number>`
  - `resolves #<issue_number>`
  - `closes #<issue_number>`

#### Example Commit Message
```
git commit -m "Add user authentication, fixes #15"
```

### 2. Creating Pull Requests
When you are ready to merge changes from one branch to another (typically from `develop` to `main` or `master`):
- Navigate to the "Pull Requests" tab in your GitHub repository.
- Click on “New Pull Request.”
- Select the base branch (the one you want to merge into) and the compare branch (the one with your changes).
- Provide a descriptive title and a detailed description in the pull request body.
- Use keywords and issue numbers to reference and close related issues in the description.

#### Example Pull Request Description
```
This pull request improves the checkout process and enhances security.

- Enhances security protocols, closes #22
- Optimizes checkout flow, fixes #18
```

### 3. Reviewing Pull Requests
- Assign the pull request to a peer for review.
- Address any comments or required changes.
- Ensure all automated tests pass (if applicable).

### 4. Merging Pull Requests
Once the pull request is approved and all status checks pass:
- Click on “Merge Pull Request.”
- Confirm the merge and delete the branch if it is no longer needed.

### 5. Post-Merge Actions
After merging:
- Verify that all linked issues are automatically closed.
- Update project documentation as necessary.
- Communicate the changes to relevant stakeholders.
