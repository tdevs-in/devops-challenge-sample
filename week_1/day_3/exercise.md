# Branching and Merging Challenge

## Overview

In this exercise, you will explore branching and merging in Git, an essential aspect of version control. Branches allow teams to work on features or fixes independently without affecting the main codebase. We will define some common branching strategies organizations use, create a new branch in the Git repository, make changes to the sample files in the new branch, and then merge the changes back into the main branch. Additionally, you will intentionally generate a merge conflict during the merge process and ask the user to resolve it.

## What topics we will cover

1. Different branching strategies organizations commonly adopt.
1. Creating a new branch and switching between branches in Git.
1. Making changes to files in the new branch.
1. Merging changes from one branch into another.
1. Resolving merge conflicts in Git.

## After this exercise, you will learn

-   How to create and manage branches effectively.
-   The importance of using branching strategies in real-world projects.
-   How to collaborate on a project using separate branches.
-   How to handle merge conflicts that arise during code integration.

## Exercise

We will be creating a merge conflict intentionally in this exercise to understand on how to deal with conflicts.

1. Review and understand the branching strategies commonly used by organizations (e.g., GitFlow, GitHub Flow, Feature Branching).
1. Clone an existing git repository from your GitLab instance.
1. Create a new branch named "feature-xyz" in the cloned Git repository.
1. Make specific changes to the sample files (e.g., add or modify content) in the "feature-xyz" branch.
1. Commit the changes to the "feature-xyz" branch and push it to remote.
1. Switch back to the main branch.
1. Make different changes to the same lines of code in the sample files in the main branch.
1. Commit the changes to the main branch and push it to remote
1. Go to Gitlab server and raise a new pull request.
1. Merge the "feature-xyz" branch into the main branch, intentionally creating a merge conflict by modifying the same lines of code in both branches.
1. Pull the changes from remote and resolve the merge conflict by editing the conflicting files and preserving the desired changes.
1. Commit the resolved changes and merge the branch after pushing to remote.
