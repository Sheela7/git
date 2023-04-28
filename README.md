1. Can we have a global .gitignore?
   -> Yes, we can have a global .gitignore file. To create it we can use touch .gitignore_global

2. How to find difference between two commits?
   -> We can use 'git diff' command followed by commit IDs in order to seee the differences between two commits.
   for eg. git diff 55e4c50 3585130 where, 55e4c50 3585130 are the commit ids of two different commits.

3. Write difference between git add and git commit commands.
   -> git add command takes the modified file of the working directory and places it in staging area to make a file ready to be commit whereas, git commit command will write the changes to the repository permanantly.

4. How to unstage files?
   -> To unstage files you can use the following commands:
   git reset fileName
   git restore --staged "fileName"

5. How to revert a commit?
   -> In order to revert a commit, you can use command : git revert < last commit id> or git revert HEAD (for reverting the most recent commit)

6. Difference between revert and reset.
   -> The difference between revert and rest is that git revert uncommits the file i.e. undo all the changes while still keeping the commit history whereas, git reset also undoes changes and even remove the commit history.
