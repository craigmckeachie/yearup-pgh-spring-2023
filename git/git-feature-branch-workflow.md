# Git Collaboration: Feature Branch Workflow

1.  Pull the latest changes from the remote main branch on Github into your local main branch:

    ```bash
    git checkout main
    git pull origin main
    ```

1.  Create a new branch:

    ```bash
    git checkout -b feature/your-feature-name
    ```

1.  Make changes and commit:

    ```bash
    git add .
    git commit -m "Your commit message"
    ```

1.  Pull the latest changes from the remote main branch on Github into your local feature branch and resolve conflicts (if there are any):

    - Verify you are still in your feature branch

      ```bash
      # do not need to run this unless you changed branches
      git checkout feature/your-feature-name
      ```

    - Fetch the latest changes from the main branch into your feature branch and attempt to merge them:

      ```bash
      git pull origin main
      ```


      > Note: What git pull actually does is two commands: fetch and merge)
      > YOU WILL NOT NEED TO RUN THESE COMMANDS BUT AS AN EXAMPLE
      > ```bash
      > git checkout feature/your-feature-name #make sure you are in your feature branch
      > git fetch origin main 
      > git merge origin/main
      > ```

    - Resolve conflicts by editing the conflicting files manually.
    - Stage the resolved files for commit:
      ```bash
      git add .
      ```
    - Commit the changes with a merge conflict resolution message:

      ```bash
      git commit -m "Resolve merge conflicts"
      ```

1.  Push the feature branch to Github:

    ```bash
    git push origin feature/your-feature-name
    ```

1.  Repeat the last 3 steps until your feature is complete or you are at a point where you want to integrate it into the main branch.

1.  Open a pull request:

    Go to your GitHub repository on github.com.
    Create a new pull request, proposing your changes for review and merging.
    Specify the main branch and the branch containing your changes (feature).

1.  Review and address feedback:

    Team members review your code, provide feedback, and suggest changes on the pull request page.
    Make additional commits to address the feedback directly on the same feature branch.

1.  Merge the pull request:

    The pull request reviewer (designated person...often the owner of the repository) reviews the changes, ensuring they meet the requirements and have proper test coverage.

    If conflicts occur during the merge on GitHub.com, GitHub will notify you and prevent the merge from proceeding. Conflicts need to be resolved.

    a. Resolve conflicts locally:

    - Fetch the latest changes from the main branch:

      ```bash
      git checkout feature/your-feature-name
      git pull origin main
      ```

    - Resolve conflicts by editing the conflicting files manually.
    - Stage the resolved files for commit:
      ```bash
      git add .
      ```
    - Commit the changes with a merge conflict resolution message:

      ```bash
      git commit -m "Resolve merge conflicts"
      ```

    - Push the changes to the remote repository:

      ```bash
      git push origin feature/your-feature-name
      ```

    b. Update the pull request:

    - Return to the pull request page on GitHub.com.
    - GitHub will detect the new commits and indicate that the conflicts have been resolved.
    - The pull request reviewer can now proceed with merging the pull request on GitHub.com.

1.  Update the local repository:

    ```bash
    git checkout main
    git pull origin main
    ```

1.  Delete the feature branch (optional):

    - Once the changes are merged, you can choose to delete the feature branch, both locally and remotely, if it's no longer needed.

      ```bash
      # Locally delete the feature branch
      git branch -d feature/your-feature-name
      # Remotely delete the feature branch
      git push origin --delete feature/your-feature-name
      ```

1.  Repeat the process for new features.

By following these steps, you can effectively handle conflicts that arise during the pull request merge process on GitHub.com, ensuring the successful integration of changes into the main or master branch of your repository.
