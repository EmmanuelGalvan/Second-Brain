Links: [[0000 Index|0000 Index]]
Tags:

Creation date: 2025-06-25 01:00
Last update: 2025-06-25 01:00

---
# Nota de paso

Iniciacion
git --version
git init
git init directory_name

Seguimiento de commits
git log file.ext //Filter by file
git log -5  //Fiter by number of commits
git log --since='Apr 2 2024' //Filter by date
git log --since='Apr 2 2024' --until='Apr 11 2024'
Note: git accept a long list of date format but is preferible to use the:
Recommend ISO format 6801 "YYYY-MM-DD"
git show  //Filter by hash

Comparacion de versiones
git diff //Comparation between unstaged files and last commits files
git diff file.ext //filter by just one file
git diff --staged //Comparation between staged files and last commitsfiles
git diff 3b95f86s 89s984dx2  //Show changes between 2 commits using hashes
git diff HEAD~1 HEAD //Show changes using HEAD instead of hashes
Note: HEAD mean last commit, can use HEAD~1 to refer to last - 1, that means 1 previews to last

Revert files
git revert HEAD //Revert all changes to te commit given
git revert HEAD --no-edit //Revert all changes to the commit given without open text editor
git revert HEAD -n //Revert all changes to the commit given without commit the revert
git checkout HEAD~1 -- file.ext //Revert changes to commit given to specified file
git restore --staged //Remove files from the staged area
git restore --staged file.ext //Remove specified file from the staged area

Branch
git branch //List of branch. The * show the current branch
git switch branch_name //Change current branch 
git branch branch_name //Create a new branch
git switch -c branch_name //Create and switch to a new branch

Comparing and modifying branch
git diff branch1 branch2 //Show change between the 2 branch given
git branch -m original_name new_name //Rename a branch
git branch -d branch_name //Delete a branch
git branch -D branch_name //Force delete a branch

Merging branch
Destination branch = Branch to merge into (Main)
Source branch = Branch to merge from (Development branch)

To merch first have to switch to destination branch
Then use
git switch destination_branch
git merge source_branch // Merge source branch into current branch
Or use 
git merge source_branch destination_branch
Output give type of merge, number of lines changed and files modified







workflow
iniciacion
log


---
Reference: