# Declarative Pipeline for Building and Running Unit Tests

## Overview

In this exercise, you will create a declarative Jenkins pipeline to build and run unit tests on a sample Java project. The pipeline will clone a sample Java repository, build the project, and run unit tests. The pipeline will simulate a failure or success of unit tests based on the value of a parameter called `TEST_SIMULATION_RESULT`.

## What topics we will cover

1. Creating a declarative Jenkins pipeline.
2. Checking out a Git repository.
3. Building a Java project.
4. Running unit tests with conditional behavior.

## Exercise

1. Clone the sample Java repository from GitHub:https://github.com/tdevs-in/d10c-w1d4 and create a new folder named "jenkins."

2. Inside the "jenkins" folder, create a Jenkinsfile.

3. Configure the Jenkinsfile to perform the following steps:

    - Checkout the sample Java repository from Git: https://github.com/tdevs-in/d10c-w1d4
    - Build the Java project.
    - Run unit tests.
    - The pipeline should fail if unit tests fail and pass if unit tests pass.
    - Create a parameter called `TEST_SIMULATION_RESULT` of type boolean with either `true` or `false`.
    - The unit tests will automatically read the value of this variable from the environment and act accordingly.

4. Push the changes after creating a new repository in your GitLab server and linking it to the checked-out repository.

5. On your Jenkins server, create a new Jenkins pipeline and link it to the new GitLab repository you created in step 4.

6. Configure Jenkins to fetch the pipeline from the linked GitLab repository.

7. Run the Jenkins pipeline and observe its behavior based on the value of the `TEST_SIMULATION_RESULT` parameter. If the parameter is set to `true`, the pipeline should fail (indicating a unit test failure). If the parameter is set to `false`, the pipeline should pass (indicating unit test success).

> **Bonus exercise (Optional)**: Configure GitLab deployed locally or on cloud to automatically run the pipeline as soon as any PR is raised. Configure Gitlab to make these pipelines success mandatory in order to merge changes to main branch.
