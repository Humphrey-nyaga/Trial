## 1. Create a Local Repository and Push  to GitHub

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
    - Include an appropriate LICENSE and  .gitignore file

6. Get the remote repo ssh url  
    ``` 
    git@github.com:<username>/<repo_name>.git 
    ```
    For this repo it is:
    e.g
    ```
    git@github.com:Humphrey-nyaga/Trial.git 
    ```
7. Add the remote ssh url of the project locally to link the local to remote: 
    
     ```
    git remote add origin git@github.com:Humphrey-nyaga/Trial.git
    ```
8.  Pull from the remote main branch
    ```
    git pull origin main
    ```
9.  Add and Commit the current file(s)  in the working directory.

    ```
    git add README.md
    ```
    **OR**
    ```
    git add .
    ```
     **THEN**
     ```
     git commit "First Commit"
     ```
10. Push the local files to the remote repository.  
   Use the -u flag to enable git to track the main branch of the local repo to the main of the remote repo.

    ```
     git push -u origin main 
    ```
    **OR**

    ```
    git push --set-upstream origin main
    ```
