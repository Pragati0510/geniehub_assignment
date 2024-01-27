Initialize: Create an empty Git repository or reinitialize an existing one.

bash
Copy code
git init
Add: Add files to the staging area.

bash
Copy code
git add <file1> <file2> ...
Commit: Record changes to the repository.

bash
Copy code
git commit -m "Commit message"
Push: Upload local repository contents to a remote repository.

bash
Copy code
git push origin <branch_name>
Pull: Fetch from and merge with another repository or a local branch.

bash
Copy code
git pull origin <branch_name>
Status: Display the status of the working directory.

bash
Copy code
git status
Branch: List, create, or delete branches.

bash
Copy code
git branch                            # List branches
git branch <branch_name>             # Create branch
git branch -d <branch_name>          # Delete branch
Checkout: Switch branches or restore working tree files.

bash
Copy code
git checkout <branch_name>             # Switch to branch
git checkout -b <new_branch_name>    # Create and switch to a new branch
Merge: Join two or more development histories together.

bash
Copy code
git merge <branch_name>
Remote: Manage set of tracked repositories.

bash
Copy code
git remote -v                        # List remote repositories
git remote add <name> <URL>         # Add remote repository
Fetch: Download objects and refs from another repository.

bash
Copy code
git fetch <remote>
Diff: Show changes between commits, commit and working tree, etc.

bash
Copy code
git diff
Log: Show commit logs.

bash
Copy code
git log
Reset: Reset current HEAD to the specified state.

bash
Copy code
git reset --hard <commit_hash>
Revert: Create a new commit that undoes the changes of the given commit.

bash
Copy code
git revert <commit_hash>
GitHub-Specific Commands:
Fork: Create a personal copy of someone else's project.

Click on the "Fork" button on GitHub UI.
Pull Request (PR): Propose changes to a repository.

After making changes in your forked repository, create a PR from GitHub UI.
Issues: Track ideas, enhancements, tasks, or bugs for work on GitHub.

Navigate to the "Issues" tab on a repository to create or view issues.
Wiki: Create documentation directly on GitHub.

Go to the "Wiki" tab on a repository to create or edit wiki pages.
Gists: Share single files, parts of files, or full applications.

Use the "Create a Gist" option on GitHub.
GitHub Pages: Host a website directly from a GitHub repository.

Configure in repository settings under the "Pages" section.

