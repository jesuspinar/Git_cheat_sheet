# Git introduction
> Beginners guide that helps with git commands. 
## Global config
##### Add your name.
```bash 
git config --global user.name "Your name"
```

##### Add your email.
```bash 
git config --global user.mail "name@email.com"
```

##### Adds default text editor.
```bash 
git config --global core.editor "code --wait"
```

##### Opens config settings.
```bash 
git config --global -e
```

##### Specify the return type just one enter. *Linux|Mac*
```bash 
git config --global core.autocrlf input
``` 

##### Specify the return type just one enter. *Windows*
```bash 
git config --global core.autocrlf true
``` 

##### See other options.
```bash 
git config -h
```

## Usefull commands 
##### Initializes a git repo in local folder.
```bash 
git init
```

##### Adds all changes to stage (*deleted, modified and new files or dirs*).
```bash 
git add .
``` 

##### Make a commit and specify a message.
```bash 
git commit -m "Initial commit"
```

##### Delete file or dir from the working tree the file.
```bash 
git rm file
```

##### Renaming or moving files or dirs.
```bash 
git mv filename filename
``` 

##### Shows the changes at stage.
```bash 
git status
```

##### Shows the changes at stage, clean.
```bash 
git status -s
```

##### Compare the changes.
```bash 
git diff
``` 

##### Compares the changes on stage.
```bash 
git diff --staged
```

##### Review the commit history of the repository.
```bash 
git log
``` 

##### Review the commit history repo, clean.
```bash 
git log --oneline
```

##### Shows the actual brach.
```bash 
git branch
```
##### Shows local and remote branches and info.
```bash 
git branch -vva
```

##### Creates a new branch.
```bash 
git checkout -b name
```

##### Deletes a local branch.
```bash 
git branch -d branchName
git branch --delete branchName
```

##### Changes to branch .
```bash 
git switch branchName
```


##### Add changes of branchName to current branch.
```bash 
git merge branchName
```

##### Indicates remote server to push changes.
```bash 
git remote add origin www.github.com
```

##### Publishes the changes into branchName at repo on the server.
```bash  
git push origin branchName
```  
##### Publishes the changes into branch main if local and remote branch name are different.
```bash  
git push origin branchLocalName:branchRemoteName
```  

##### Creates a branch main and publishes changes into it at repo on the server.
```bash 
git push -u origin main
```
##### Show, remove , rename the remote repos
```bash 
git remote -v 
```
```bash 
git remote rm name 
```
```bash 
git remote remove name newname 
```

##### After pulling shows changes .
```bash 
git whatchanged
```
