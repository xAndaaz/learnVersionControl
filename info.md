# VCS - version control system 
## types of VSC
- Local/ Localized VCS
- Central/ Centralized VCS
- Distributed VCS (Combination of Locals & Centrals)

# GIT - Global Information Tracker (~ Linus Tornvalds)
## Working Stages of GIT
1. Working Directory
> place where we create/ modify files or perform any read/ write 
2. Staging Area/ Index/ Local Repository 
> ~add <br> place werher we keep the file for temp. period
3. Local Repository 
> ~commit <br> we are going to save the files permanent here

---
---
1. Initialize: 
```git
git init
```
2. Configuration:
```git
git config user.name = "user_name"
git config email = "email"
```
3. Add to copy the files from working directory to staging area
```git
git add file_name
git add file1 file2
git add .
```
> Check the file present in my staging area: ```git status```

4. Commit: 
```git
git commit -m "ANY MESSAGE"
```
```
// for individual commit with message for eg. if we have 
git add .
// and it has many files , then for commiting only one we can give its name after commit message 
git commit -m "this is only for a1.txt" a1.txt
```

### to check commit history
```
git log
// this will show full details
git log --oneline
// this will show 
```

### To limit the no of commits:
```
git log -n number_of_commits
```

### to show only commits made by specific author:
```
git log --author name_of_author
```

### To show the commits based on the commit message:
```
git log --grep = "bug fix"
```

### to show commit of file:
```
git log a.txt
```

### to show history of particular branch 
```
git log branch_name
```

### to update the commit message:
* root(first) commit can't be amended 
```
git commit --amend 
(applicable for recent commit)
```

5. Establish the connection: In order to upload the changes from local repo tp remote repo
```
git remote add alias_name remote_url
git remote add origin remote_url
```

-> to verify connection: git remote -v

6. Push:
```
git push origin master/main
```
7. Pull:
```
git pull origin master/main
```

## pull vs fetch 
* pull is fetch + merge 


# GIT branch
```
git branch --list 
OR
git branch
```

```
// To create a branch 
git branch branch_name

// To Switch branch 
git switch branch_name

```
