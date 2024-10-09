# explain how to make repository and uploud it to GitHub

## first configuration with git

If you creat a repository in the first one, you must configure with git by using your name`user.name` and your email `user.email`.

>git config --global user.name "your name"
<!-- -->
>git config --global user.email "yourgmail.com"

To make sure your configuration :
> git config --list

## Second to create a local repository

1. create a new folder.
    - use this command: `mkdir NameOfFolder`
2. create a file in this folder.
    - use a command: `echo "content">>NameFile.txt`
3. converte a file to a new git repository.
    - use a command: `git init`
4. if you will puplish a local repo to GitHub, you must rename a repo.
    - use a command: `git branch -M main`
5. you can see the status of this file by using a command: `git status`

## third to track the history of a file

After creating a git repo, the file is now **untracked(U)** from a repo, so to convert it from **untracked** to **tracked(M)** using command:

>git add .

### Then convert the file from untracked to **modifier**

>git commit -m "initial commit"

## Forth uploud a local repo to GitHub

1. Creat a repository on GitHub from *New repository*, without **README.md** file,choose *public* or *private*, then creat repository.

2. Add a remote repo in a local repo by using a commant :
   `git remote add origin https://github.com/UserNameOnGitHub/NameRepo.git`

3. To make sure adding a remote repo, use a comment : `git remote` or `git remote -v`

4. To publish a local repo to a remote repo on Github, use a comment: `git push origin main`

    - make **authentication** on GitHub if you will publish a local repo on GitHub in the first:

       - `username for 'www.github.com' : "userName"`
       - `yourpassword for 'www.github.com' : "yourPassword"`
