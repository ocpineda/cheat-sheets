## Shortcuts  

**Create bare remote repo**  
`ssh user@host git init --bare /path/to/repo.git`  

**List local branches**  
`git branch`  

**Checkout a local branch**  
`git checkout branch_name`  

**Create new branch**  
`git checkout -b myNewBranch branchingFrom`

**Push branch to remote**   
`git push -u origin branch_name`  

**Delete local branch**  
`git branch -d branch_name`  

**Delete remote branch**  
`git push origin --delete branch_name`  

**Diff two branches**  
`git diff master..test-dev`  

**Rebase from remote**  
```
git fetch origin            # Updates origin/master    
git rebase origin/master    # Rebases current branch onto origin/master`  
```

**Remove file from local file system, and repo**  
`git rm file1.txt`  
`git commit -m "remove file1.txt"`

**Remove from Git repo only**  
`git rm --cached file1.txt`

---

## Hotfix
If there has to be a hotfix in production, you should branch from a tag release of production from prior to the bug being introduced.

`git checkout tags/<tag_name> -b <branch_name>`

<!-- ***************************************************************** -->

## Other info

**Global git ignore file**    
located in `~/.gitignore_global`

<!-- ***************************************************************** -->

## Links

 - [Setting up a new remote git repository](https://gist.github.com/toolmantim/569530)

- [Add existing project from CLI](https://help.github.com/articles/adding-an-existing-project-to-github-using-the-command-line/)
