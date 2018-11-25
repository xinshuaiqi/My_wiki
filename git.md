use git log to visualize our chain of commits



use Git’s version of mv and rm: git mv
and git rm



Telling Git What to Ignore: .gitignore

```
If you're using Windows it will not let you create a file without a filename in Windows Explorer. It will give you the error "You must type a file name" if you try to rename a text file as .gitignore

enter image description here

To get around this I used the following steps

Create the text file gitignore.txt
Open it in a text editor and add your rules, then save and close
Hold SHIFT, right click the folder you're in, then select Open command window here
Then rename the file in the command line, with ren gitignore.txt .gitignore
```



Undoing a Stage: git reset

>  git reset HEAD README.md



# collaborative git

local => remote:	push

remote => local: 	pull



merge conflict





Getting Files from the Past: git checkout

> git checkout -- <file>

# 前三个版本

> git log --pretty=oneline --abbrev-commit -n 3
>
> git checkout 08ccd3b -- README.md
>
> git checkout 20041ab -- README.md



Saved working directory and index state WIP on master: 20041ab

> git stash

To reapply the changes we stashed

> git stash pop  





Undoing and Editing Commits: git commit --amend



Creating and Working with Branches: git branch and git checkout

> git branch readme-changes

switch to the readme-changes branch, use 

> git checkout readme-changes
>
> git commit -a -m "reformatted readme, added sample info"
>
> git log --abbrev-commit --pretty=oneline -n 3
>
> git checkout master
>
> git log --abbrev-commit --pretty=oneline -n 3

Merging Branches: git merge