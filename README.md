## Create a Local Repository and Push  to GitHub

1. Create a new directory locally.   
    ```
    mkdir Trial
    ```
2. Enter the project directory.
   ```
   cd Trial
   ```

3. Initialize git
    ```
    git init
    ```
4. Create a README file
   
   ```
   touch README.md
   ```
5. Create a remote repository on GitHub.
6. Get the remote repo link  
    ``` 
    git@github.com:<username>/<repo_name>.git 
    ```
    Replace the username and repo name appropriately to match your repository.
    e.g
    ```
        git@github.com:Humphrey-nyaga/Trial.git 
    ```
7. Add the remote url of the project locally to link the local to remote: 
    
    ```
    git remote add origin git@github.com:<username>/<repo_name>.git
    ```
    Replace the repo details appropriately.
    E.g 

     ```
    git remote add origin git@github.com:Humphrey-nyaga/Trial.git
    ```
8.  Add and Commit the current file(s)  in the working directory.

    ```
    git add README.md
    ```
    or
    ```
    git add .
    ```
     then
     ```
     git commit "First Commit"
     ```
9.  Push the local files to the remote repository.  
   Use the -u flag to enable git to track the main branch of the local repo to the main of the remote repo.

    ```
     git push -u origin main 
    ```
    The same can be achieved by running the command:

    ```
    git push --set-upstream origin main
    ```