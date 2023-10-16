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
