# push_project_with_git_to_any_repository

1. first open git command on project directory
2. git init - **initialize empty git repository**
3. git add .
4. git commit -m "Initial"
5. git remote add origin paste repo link + enter
6. to verify - git remote -v
7. git push origin master

* git status - display the branches
# find commited but unpushed

* git log origin/your-branch..HEAD

# important
  * when u use vs code commit the code and push through the cmd using this - git push origin branch_name
  * If You want to change the branch see below code

    
    PS C:\Users\molinduy\Desktop\mobitel_projec\TRAIN_TICKET\TRAIN> git fetch
    
    Switched to a new branch 'staging'
    
    branch 'staging' set up to track 'origin/staging'.
    PS C:\Users\molinduy\Desktop\mobitel_projec\TRAIN_TICKET\TRAIN> git pull origin staging
    
    From https://dev.azure.com/Mobitel-DevOps/Mobile%20Team%20Developments/_git/Railway%20Reservations%20Checker%20App
     * branch            staging    -> FETCH_HEAD
    Already up to date.

    PS C:\Users\molinduy\Desktop\mobitel_projec\TRAIN_TICKET\TRAIN> git checkout master
    Switched to branch 'master'
    
    PS C:\Users\molinduy\Desktop\mobitel_projec\TRAIN_TICKET\TRAIN>

############################################################################

# update codes to anther branch 
     git checkout your-another-branch
     git merge main
     # Add the resolved files
     git add .

     # Commit the changes
     git commit -m "Merged changes from main branch"

     git push origin your-another-branch


link- https://chat.openai.com/share/517098ee-a46c-4993-9a2e-ee114f92b80b

# 01. ERROR
# When error comes while pushing 
"Total 96 (delta 61), reused 0 (delta 0), pack-reused 0
error: RPC failed; curl 56 HTTP/2 stream 7 was reset
send-pack: unexpected disconnect while reading sideband packet
fatal: the remote end hung up unexpectedly"
#  to do 
* git config --global http.version HTTP/1.1, push, then git config --global http.version HTTP/2
# Follow this 
link - https://github.com/curl/curl/issues/11353#issuecomment-1687169241

# git pull origin master 
* update the code and commits from remote branch

# git fetch origin master
* update reference from remote branch
 * now use **git rebase origin/master**

# clone from github branch
* git clone -b branch-name --single-branch repository-url

# if it is main branch 
* git clone repository-url

# open .git

# echo hello > file1.txt
* create file1.txt with hello word

# git staging
git add file1.txt file2.txt
  or
git add *.txt - all files with .txt
  or
git add . - all large and all files staging

# modify
echo world >> file1.txt  - modify file1.txt

# git commit 
* shows recently commited files

# git commit -a -m "Fix the bug"
# git commit -am "Fix the bug"
 
* -a :- indicates all changed files.
* -m :- indicates commit message.

# rm file2.txt
* delete file2.txt

# git ls-files 
* shows all changes in staging area if deleted files exists.
* after **git add file2.txt** deletion saves completely

# git rm file2.txt *.txt 
* delete all text files

# mv file1.txt main.js
* file1.txt change as main.js
* **git add file1.txt** - to confirm file1.txt deletion
* **git add main.js** - changed file will be added
* in short form **git mv main.js file1.txt**

# mkdir logs
# echo hello > logs/dev.log

# echo logs/ > .gitignore
* create .gitignore file in the logs folder

# git rm -h
* quick help

# git rm --cached -r bin/
* internally remode directed are from stagning

# git diff --staged
* shows the differences between the index (staging area) and the last commit.
  
# DIFF TOOLS
* KDiff3
* P4Merge
* WinMerge(Windoes Only)
* vscode 

***watch video at 51 min to 55.41***

# git log 
* see history

# git log --oneline --reverse
* shows commits start to end

***watch video at 57.24min***






