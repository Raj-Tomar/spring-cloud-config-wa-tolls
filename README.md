This is Configuration Server for Spring Cloud Config Project

============================================================
Git Basic Commands
	git init
	git add .
	git commit -m "my commit"
	git remote add origin <remote repository URL>
	
	git branch -M main
	git push -u origin main
		OR
	git push origin <remote branch name>
	
	 main is now named master 
	 If you have a local clone, you can update it by running:
		git branch -m main master
		git fetch origin
		git branch -u origin/master master
	
	Renaming local and remote
	
		# Rename the local branch to the new name
		git branch -m <old_name> <new_name>

		# Delete the old branch on remote - where <remote> is, for example, origin
		git push <remote> --delete <old_name>

		# Or shorter way to delete remote branch [:]
		git push <remote> :<old_name>

		# Prevent git from using the old name when pushing in the next step.
		# Otherwise, git will use the old upstream name instead of <new_name>.
		git branch --unset-upstream <old_name>

		# Push the new branch to remote
		git push <remote> <new_name>

		# Reset the upstream branch for the new_name local branch
		git push <remote> -u <new_name>

Undo a commit & redo
	$ git commit -m "Something terribly misguided" # (0: Your Accident)
	$ git reset HEAD~                              # (1)
	[ edit files as necessary ]                    # (2)
	$ git add .                                    # (3)
	$ git commit -c ORIG_HEAD                      # (4)
============================================================
