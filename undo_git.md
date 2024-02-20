# Uncommited local changes

## 1. Undo changes in one file
`git restore <filename>`

## 2. Restore a delete file
`git restore <filename>`

## 3. Discard chanks/lines of a update file
### This will dispaly all hunks/chunks and press `n` to keep or `y` to discard
`git restore -p <filename>` 

## 4. Undo all working changes since last commit  
`git restore .` or `git checkout`

# Commited local changes

## 5. Amend last commit
`git commit --amend -m "Updated last commit"`

## 6. Reverting a commit in the moddile
## Revert the commit 
`git revert <commit_hash>`

## 7. Resetting to a old revision
### Everything after commit 2 is bad. Forget commits 3-6
`git reset --hard <commit_hash_to_go_back_to>`

## 8. Resetting a file to an old revision (not all project like above)
`git restore --source <commit_hash> <filename>`

# Reflog- gits diary 

## 9. 
## When you wrongly reset to an old version. Brings up history of actions (commit, reset, merge ect)
`git reflog`
`git branch <new_branch_name> ` - includes lost commits

## 10. Recover a deleted branch 
`git reflog`
`git branch <new_branch> <commit_hash_from_feature>`

## 11. Moving a commit to a new branch
### When you should have created a new branch before commiting 
#### Create new branch 
`git checkout <new_branch_name>`
### Clean up master
`git checkout master`
`git reset HEAD~1 --hard`

## 12. Moving a commit to a different branch
`git checkout <correct_branch_name>`
`git cherry-pick <commit_has>`
`git checkout master`
`git reset --hard HEAD~1`

## 13. 

