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
   -> The difference between revert and reset is that git revert creates a new commit by undoing all the changes while still keeping the commit history whereas, git reset also undoes changes and also remove the commit history.

day:2
Add new answers to the README.MD file to the following questions:

a. Write the difference between fetch and pull command.
-> The differences between fetch and pull commands is that 'fetch' only downloads the changes and updates your remote tracking branches, while leaving your local working branch unchanged. On the otherhand,pull combines the fetch command with an automatic merge, which updates your local working branch with the changes from the remote repository.

b. How to handle merge conflicts?
-> In order to handel the merge conflits, we need to do the following steps:

1. First of all, run 'git status' command in order to identify the files with conflicts.
2. After that, you will see the conflicting code which will be marked as `<<<<<`,`=====`, and `>>>>>`.
3. Edit manually and delete or keep the code that you want to change and you want to keep.
4. After editing the file, save the changes and stage the file using `git add .` and after that commit the changes using `git commit`
5. If you further encounter any error while merging process, use `git merge --abort` to cancel merge and return to state before the merge.
6. Finally push the merge using `git push` command.
