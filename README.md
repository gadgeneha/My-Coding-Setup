# My Coding Setup
## Git Pull request Workflow

• git checkout -b <new-branch-name> this will create a new branch and switch local branch to new-branch-name. 
	Your changes will be made on this new branch.
	• Make changes to the code, verify that they are working. Now you are ready to check-in.
	• git add <updated-files>	 this will stage the files to be added on the git repo for the commit.
	• git commit -m "<add-a-commit message>"
	• git fetch origin
	• (option 1)git merge origin/master	 Resolve conflicts if any and commit again.
	(option 2)git rebase origin/master 	Resolve conflicts if any. Preferable as commit history remains linear.
	• git push origin new-branch-name 	This will push your code on new branch in remote.
	• Create a pull request to integrate changes from your branch to master. 
	Once PR is approved, your commit will be merged with the master branch via merge pull request.
	• Keep working in local repo until your push is merged with master. 
	You may create different local repo to work on different problems. 
	Try to keep them independant of each other to avoid conflicts due to dependancies.
	• git checkout master Switch local repo back to master branch (only after your changes are merged with the master).git
	• git pull 	Get all latest changes from the master.
	• git branch -d new-branch-name	 Delete local branch created after pushing and merging your changes. This is optional
