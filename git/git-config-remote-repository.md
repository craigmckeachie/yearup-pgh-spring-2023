## Git Collaboration: Locking the Main Branch and Adding Collaborators

To lock the main branch of your GitHub repository and allow collaborators to create their own branches, you can follow these steps:

1. Navigate to your repository on GitHub.
2. Click on the **Settings** tab located at the top-right corner of the repository page.
3. In the left sidebar of the Settings page, click on **Branches**.
4. Scroll down to the **Branch protection rules** section and click on the **Add rule** button.
5. Under the **Branch name pattern** field, type `main` to specify that you want to protect the main branch.
6. Enable the **Require pull request reviews before merging** option. This ensures that any changes to the main branch must go through a pull request and receive approval from collaborators.
7. Optionally, you can also enable other protections such as requiring status checks to pass before merging, requiring signed commits, or enforcing certain branch restrictions.
8. Click on the **Save changes** button to apply the branch protection rule.

Now that the main branch is locked, collaborators cannot directly push changes to it. Instead, they need to create branches, make changes, and submit pull requests for review. To add collaborators and give them write access to the repository so they can create branches, follow these additional steps:

1. On the repository page, click on the **Settings** tab.
2. In the left sidebar, click on **Collaborators**.
3. Click on the green **Add People** button.
4. Enter the GitHub username or email address of the collaborator you want to add.
5. Select the collaborator's name from the dropdown list that appears.
6. Choose the appropriate permission level for the collaborator (e.g., **Write** access).
7. Click on the **Add** button to invite the collaborator.

The collaborator will receive an email notification and can accept the invitation to become a collaborator on the repository. Once added, they can create their own branches, make changes, and submit pull requests for merging into the main branch.

