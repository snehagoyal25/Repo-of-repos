1. Git and Github
What is Version Control system?
A system that keeps track of our files or projects.
It allows you to revert selected files to a previous state, revert the entire project to a previous state, compare changes over time, see who last modified something so that we can know what might be causing a problem, or what is the issue, who made it, and when with the details.

What is Git?
Free and open source version control system.

Why Git?
Free
Open source
Scalable
Super Fast
Cheap branching and merging

What is GitHub?
GitHub is a web-based hosting service for git repositories.
You can use git without Github, but you cannot use GitHub without Git.
Basic workflow of Git
Step 1 − You modify a file from the working directory.
Step 2 − You add these files to the staging area.
Step 3 − You perform commit operation that moves the files from the staging area. After push operation, it stores the changes permanently to the Git repository
GitHub workflow
Write code ------> Commit code changes ------> Pull request

Basic Git commands
git clone: Bring a repository hosted somewhere like Github into a folder or your local machine

git clone <github_url>
git init: Used to initialize a new Git repository.

git init
git add: The  git add command is used to add changes in your working directory to the staging area.

git add file_name

or,

git add .
git status: Displays the state of the working directory and the staging area.

git status
git commit: Save your files in git with messages

git commit -m "commit_message"
git remote: The git remote command lets you create, view, and delete connections to other repositories.

List the remote connections you have to other repositories.

git remote
Same as the above command, but include the URL of each connection.

git remote -v
Create a new connection to a remote repository. After adding a remote, you’ll be able to use ＜remote_name＞ as a convenient shortcut for ＜github_url＞ in other Git commands.

git remote add <remote_name> ＜github_url＞
Remove the connection to the remote repository called ＜remote_name＞.

git remote rm <remote_name>
Rename a remote connection from ＜old-name＞ to ＜new-name＞.

git remote rename <old-name> <new-name>
git push: Upload your commits to a git repo, like GitHub

git push <remote_name> <branch_name>
git pull: Download changes from a remote repository to your local repository.

git pull <remote_name> <branch_name>
git branch: The git branch command lets you create, list, rename, and delete branches. It doesn’t let you switch between branches or put a forked history back together again. For this reason, git branch is tightly integrated with the git checkout and git merge commands.

List all of the branches in your repository. This is synonymous with git branch --list.
git branch
Create a new branch. This does not check out the new branch.
git branch <branch_name>
Delete the specified branch. This is a 'safe' operation in that Git prevents you from deleting the branch if it has unmerged changes.
git branch -d <branch_name>
Force delete the specified branch, even if it has unmerged changes. This is the command to use if you want to permanently throw away all of the commits associated with a particular line of development.
git branch -D <branch_name>
Rename the current branch to ＜ branch_name ＞.
git branch -m <branch_name>
List all remote branches.
git branch -a
git checkout: The git checkout command lets you navigate between the branches created by git branch.

git checkout <branch_name>
git merge: Used to combine two branches.

git merge <new-feature>
Merge Conflicts
Occasionally, this process doesn’t go smoothly.
If you changed the same part of the same file differently in the two branches you’re merging, Git won’t be able to merge them cleanly. If your fix for feature branch modified the same part of a file as the hotfix branch, you’ll get a merge conflict.
Git commands to resolve conflicts
git log --merge: produce the list of commits that are causing the conflict.
git diff: Identify the differences between the states repositories or files.
git checkout: Used to undo the changes made to the file, or for changing branches.
git reset --mixed: Used to undo changes to the working directory and staging area.
git merge --abort: Helps in exiting the merge process and returning back to the state before the merging began.
git reset: Used at the time of merge conflict to reset the conflicted files to their original state.
 