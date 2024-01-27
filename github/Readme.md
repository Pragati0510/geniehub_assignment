Git Basics

1.Initialize: Create an empty Git repository or reinitialize an existing one.
git init
2
.Add: Add files to the staging area.
git add <file1> <file2> ...

3.Commit: Record changes to the repository.
git commit -m "Commit message"

4.Push: Upload local repository contents to a remote repository.
git push origin <branch_name>

5.Pull: Fetch from and merge with another repository or a local branch.
git pull origin <branch_name>

6.Status: Display the status of the working directory.
git status

7.Branch: List, create, or delete branches.
git branch                            # List branches
git branch <branch_name>             # Create branch
git branch -d <branch_name>          # Delete branch

8.Checkout: Switch branches or restore working tree files.
git checkout <branch_name>             # Switch to branch
git checkout -b <new_branch_name>    # Create and switch to a new branch

9.Merge: Join two or more development histories together.
git merge <branch_name>

10.Remote: Manage set of tracked repositories.
git remote -v                        # List remote repositories
git remote add <name> <URL>         # Add remote repository

11.Fetch: Download objects and refs from another repository.
git fetch <remote>

12.Diff: Show changes between commits, commit and working tree, etc.
git diff

13.Log: Show commit logs.
git log

14.Reset: Reset current HEAD to the specified state.
git reset --hard <commit_hash>

15.Revert: Create a new commit that undoes the changes of the given commit.
git revert <commit_hash>

16.GitHub-Specific Commands:
I> Fork: Create a personal copy of someone else's project.
Click on the "Fork" button on GitHub UI.

II> Pull Request (PR): Propose changes to a repository.
After making changes in your forked repository, create a PR from GitHub UI.

III> Issues: Track ideas, enhancements, tasks, or bugs for work on GitHub.
Navigate to the "Issues" tab on a repository to create or view issues.

IV> Wiki: Create documentation directly on GitHub.
Go to the "Wiki" tab on a repository to create or edit wiki pages.

V> Gists: Share single files, parts of files, or full applications.
Use the "Create a Gist" option on GitHub.

VI> GitHub Pages: Host a website directly from a GitHub repository.
Configure in repository settings under the "Pages" section.

