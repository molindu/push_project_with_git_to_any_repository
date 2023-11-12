# push_project_with_git_to_any_repository

1. first open git command on project directory
2. git init
3. git add .
4. git commit -m "Initial"
5. git remote add origin paste repo link + enter
6. to verify - git remote -v
7. git push origin master

important
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

update codes to anther branch 
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
