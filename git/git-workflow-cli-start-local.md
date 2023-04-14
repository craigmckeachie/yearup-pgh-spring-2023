# Git Workflow using Command-Line Interface (CLI) and starting with Code on your Computer

# Local Repository

## Objectives

- Start your project and write some code
- Save a snapshot (commit) of your initial code
- Write more code and save additional snapshots (commits) of the code frequently

## Steps

### Start your project and write some code

>

1. Create a directory on your machine to store your code for a project. We will call this the `project directory`.

   ```sh
   cd documents/learntocode
   mkddir pet-store
   ```

1. Change directory to the project directory.

   ```sh
   cd pet-store
   ```

1. Add an intial file to your project directory.

   ```sh
   touch index.html
   ```

### Save a snapshot of your initial code

1. Initialize a local git repository (database).

   ```sh
   pwd # .../pet-store
   git init
   ```

1. Verify your files are in the working directory (area) but have not yet been staged (untracked)

   ```sh
   git status
   ```

   > Untracked files are files that have been created within your repo's working directory but have not yet been added to the repository's tracking index using the git add command.

1. Stage your changes to the local git repository.

   ```sh
   git add .
   ```

   Note: There are variations on `add` see the table below.
   ![image](https://user-images.githubusercontent.com/1474579/231919014-51d16b04-cb64-482c-b457-a446140a830b.png)

1. Verify your files were staged

   ```sh
   git status
   ```

1. Add a message and commit your staged changes to the local git repository.

   ```sh
   git commit -m "initial commit"
   ```

1. View your commit.

   ```sh
   git status
   ```

### Write more code and save additional snapshots of the code frequently

1. Continue to develop and change files, delete files or add files.
1. Stage your change to the local git repository.

   ```sh
   git add .
   ```

1. Add another message and commit your changes to the local git repository.

   ```sh
   git commit -m "added heading"
   ```

   > Note: these last 3 steps can be repeated over and over after the project is setup to take additional snapshots (commits)

### &#10004; You have committed changes to a local Git repository

<br>

---

# Remote Repository

## Objectives

- Push/Publish code to a remote repository

## Steps

### Push/Publish Code to a remote repository

1.  "Push Publish" the `main` branch to the `origin` remote

    ```sh
      git push origin main
    ```

    > Note you won't have to specify the `remote` and `branch`. You can just do the following:

    ```
    git push
    ```

    *If you previously did this configuration:*

    ```sh
    git config --global push.default current
    ```

    [For more details see this stack overflow post](https://stackoverflow.com/questions/37770467/why-do-i-have-to-git-push-set-upstream-origin-branch).
