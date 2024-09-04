## Setup and Config

1. `git config --global user.name "name"` - Set a name that is identifiable for credit when reviewing version history.
2. `git config --global user.email "email address"` - Set an email address that will be associated with each history marker.
3. `git config --global color.ui auto` - Enable helpful colorization of command line output.

## Starting a Repository

4. `git init` - Initialize a local Git repository.
5. `git clone [url]` - Create a local copy of a remote repository.

## Basic Snapshotting

6. `git status` - Check status.
7. `git add [file-name.txt]` - Add a file to the staging area.
8. `git add -A` - Add all new and changed files to the staging area.
9. `git commit -m "[commit message]"` - Commit changes.
10. `git rm -r [file-name.txt]` - Remove a file (or folder).

## Branching and Merging

11. `git branch` - List branches (the asterisk denotes the current branch).
12. `git branch -a` - List all branches (local and remote).
13. `git branch [branch name]` - Create a new branch.
14. `git branch -d [branch name]` - Delete a branch.
15. `git push origin --delete [branch name]` - Delete a remote branch.
16. `git checkout -b [branch name]` - Create a new branch and switch to it.
17. `git checkout -b [branch name] origin/[branch name]` - Clone a remote branch and switch to it.
18. `git checkout [branch name]` - Switch to a branch.
19. `git checkout -` - Switch to the branch last checked out.
20. `git merge [branch name]` - Merge a branch into the active branch.
21. `git merge [source branch] [target branch]` - Merge a branch into a target branch.
22. `git stash` - Stash changes in a dirty working directory.
23. `git stash clear` - Remove all stashed entries.

## Sharing and Updating Projects

24. `git push origin [branch name]` - Push a branch to your remote repository.
25. `git push -u origin [branch name]` - Push changes to remote repository (and remember the branch).
26. `git push` - Push changes to remote repository (remembered branch).
27. `git push origin --delete [branch name]` - Delete a remote branch.
28. `git pull` - Update local repository to the newest commit.
29. `git pull origin [branch name]` - Pull changes from remote repository.
30. `git remote add origin [url]` - Add a remote repository.
31. `git remote set-url origin [url]` - Change the URL of the remote repository.
32. `git remote -v` - List all currently configured remote repositories.

## Inspection and Comparison

33. `git log` - View changes.
34. `git log --summary` - View changes (detailed).
35. `git log --oneline` - View changes (briefly).
36. `git diff [source branch] [target branch]` - Preview changes before merging.

## Patching

37. `git diff` - View changes between commits, commit and working tree, etc.
38. `git diff --staged` - View changes between the staging area and the last file version.
39. `git apply [patch file]` - Apply a patch to files.
40. `git add -p` - Selectively stage certain portions of files.

## Reverting and Undoing

41. `git checkout -- [file-name.txt]` - Discard changes to a file.
42. `git reset [file-name.txt]` - Unstage a file while retaining the changes in working directory.
43. `git reset [commit]` - Undo all commits after [commit], preserving changes locally.
44. `git reset --hard [commit]` - Discard all history and changes back to the specified commit.
45. `git revert [commit]` - Revert some existing commits.

## Git Tools

46. `git rebase [branch]` - Reapply commits on top of another base tip.
47. `git rebase --abort` - Abort a rebase.
48. `git rebase --continue` - Continue a rebase after resolving conflicts.
49. `git bisect start` - Use binary search to find the commit that introduced a bug.
50. `git bisect bad` - Mark the current commit as bad in bisect mode.
51. `git bisect good [commit]` - Mark commit as good in bisect mode.
52. `git bisect reset` - Finish and exit bisect mode.

## Working with Tags

53. `git tag` - List all tags.
54. `git tag [tag name]` - Create a new tag.
55. `git tag -d [tag name]` - Delete a tag.

## Git Hooks

56. `git hooks` - Manage Git hooks.

## Managing Large Files with Git LFS

57. `git lfs track` - Track large files with Git LFS.
58. `git lfs ls-files` - List files tracked by Git LFS.

## Submodules

59. `git submodule add [url] [folder]` - Add a git submodule.
60. `git submodule update --init --recursive` - Update git submodules recursively.

## Advanced Git

61. `git cherry-pick [commit]` - Apply the changes introduced by some existing commits.
62. `git rebase -i [commit]` - Interactive rebase from a commit.

## GitHub Specific Commands

63. `git request-pull [start] [url] [end]` - Generate a request for pulling.

## Pruning

64. `git gc` - Cleanup unnecessary files and optimize the local repository.
65. `git fsck` - Check the file system for integrity.

## Managing Remotes

66. `git remote prune [name]` - Remove references to remote branches that no longer exist.

## Cleaning up

67. `git clean -n` - Show which files would be removed from working directory.
68. `git clean -f` - Remove untracked files from the working directory.
69. `git clean -fd` - Remove untracked files and directories from the working directory.

## Simplifying Log

70. `git log --pretty=oneline` - Show log as a simple list of commits.
71. `git log --pretty=format:"%h - %an, %ar : %s"` - Custom log format.
72. `git log --graph` - Show log with an ASCII graph of the branch structure.
73. `git log --author="name"` - Show only commits by a certain author.

## Advanced Merging

74. `git merge --no-ff` - Do a non-fast-forward merge.
75. `git merge --squash` - Perform a squash merge.

## Git Stash

76. `git stash pop` - Apply stashed changes and remove them from the stash list.
77. `git stash list` - List all stashed changesets.
78. `git stash drop` - Discard the most recently stashed changeset.

## Debugging with Git

79. `git bisect` - Use binary search to find the commit that introduced a bug.

## Workflows

80. `git flow init` - Setup a Git repository to support the Git flow workflow.

## Managing Content

81. `git ls-files` - Show files in the index and the working tree.

## Temporary Commits

82. `git commit --amend` - Modify the most recent commit.
83. `git rebase -i` - Interactive staging.

## Work in Progress

84. `git commit -m "WIP"` - Mark as work in progress.

## Checking Out Tags

85. `git checkout [tag-name]` - Checkout a tag.

## Advanced Branch Management

86. `git branch --merged` - List branches that have been merged into the current branch.
87. `git branch --no-merged` - List branches that have not been merged.

## Managing Your Work

88. `git add -u` - Add all updated files to the staging area.
89. `git reset --soft [commit]` - Soft reset to a commit.
90. `git reset --mixed [commit]` - Mixed reset to a commit.

## Aliases

91. `git config --global alias.co checkout` - Create an alias for checkout.
92. `git config --global alias.br branch` - Create an alias for branch.
93. `git config --global alias.ci commit` - Create an alias for commit.
94. `git config --global alias.st status` - Create an alias for status.

## Retrieving Old Versions

95. `git checkout [commit] [file]` - Retrieve old versions of a file.

## Ignoring Files

96. `git ignore [file]` - Ignore file patterns.

## Working with Patches

97. `git format-patch -1 [commit]` - Create a patch from the last commit.

## Tracking Path Changes

98. `git log --follow [file]` - Track changes to a path.

## Saving Fragments

99. `git archive -o [file.zip] HEAD` - Export a project to a zip archive.

## Temporary Staging

100. `git add -N [file]` - Stage a new file without content.