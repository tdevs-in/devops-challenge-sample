# Setting up Version Control Challenge

## Overview

In this exercise, you will learn the fundamentals of version control and set up a Git repository for your project. Version control is a crucial aspect of modern software development and DevOps practices, allowing teams to collaborate efficiently, track changes, and maintain code integrity. We will cover the process of creating a Git repository on a platform of your choice, initializing a local repository, adding sample files, pushing changes to the remote repository, and securing access using SSH keys.

## What topics we will cover

1. Creating a remote Git repository on a platform.
1. Initializing a local Git repository.
1. Adding and committing changes to the local repository.
1. Pushing the local repository to the remote repository.

# After this exercise, you will learn

-   How to create and manage Git repositories.
-   The basic workflow of version control using Git.
-   How to collaborate with others on the same codebase.
-   Best practices for using version control in a DevOps environment.
-   How to secure access to remote repositories using SSH keys.

# Exercise

1. Use the Gitlab server deployed on day 1 and create a new repository for your project. You can use Github or any other providers as well.
2. Open your terminal or command prompt and navigate to the location where you want to initialize the local Git repository.
3. Create a new directory named "DevOpsChallenge" and move into it.
4. Inside the "DevOpsChallenge" directory, create three sample files: "file1.txt", "file2.txt", and "file3.txt".
5. Add some content to each of the sample files using a text editor of your choice.
6. Initialize the local repository using the appropriate Git command.
7. Add the sample files to the staging area.
8. Commit the changes with an initial commit message.
9. Link your local repository to the remote repository you created in step 1.
10. Push the local repository to the remote repository on the chosen platform. In case your main branch is protected, you can either create a new branch to push changes and then merge them to main via a pull request or you can remove push restrictions on main branch.
11. Make sure you are using passwordless push.

In organizations, its a common practice that main branch is protected. It is to prevent any code going into QA without a code review. It's always a good practice to protect your main branch.

If you're using your own deployed server of GitLab, you might have noticed that the main branch is protected by default. In case of GitHub, your main branch won't be protected by default and you have to apply those rules separately. These rules won't work until you have GitHub Pro plan.
