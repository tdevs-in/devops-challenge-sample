# Static Code Analysis Challenge

## Overview

In this challenge, you will integrate a static code analysis tool, such as SonarQube, into your Jenkins pipeline. You will set up a SonarQube server or use a hosted service, configure the pipeline to execute code analysis after the build stage, and review/address any code quality issues reported by SonarQube.

## What topics we will cover

1. Integrating static code analysis tools into a CI/CD pipeline.
2. Setting up and configuring SonarQube.
3. Analyzing code quality and addressing issues.

## After this exercise, you will learn:

By completing this challenge, you will gain practical experience in integrating a static code analysis tool (such as SonarQube) into your Jenkins pipeline. You will learn how to set up and configure SonarQube, modify a Jenkins pipeline to include code analysis, and review/address code quality issues identified by SonarQube. This exercise will enhance your understanding of the importance of code quality in the DevOps process and equip you with skills to improve codebase health and maintainability. You will also become proficient in using SonarQube to analyze and enhance your projects' code quality.

## Exercise

For below exercise, use this java project for your pipeline: https://github.com/tdevs-in/d10c-w1d5

1. **Set Up SonarQube:**

    - Install and configure a SonarQube server locally or use a hosted SonarQube service (e.g., SonarCloud). You can also setup your own instance on cloud.
    - Obtain the necessary authentication tokens or credentials for SonarQube.

2. **Modify Jenkins Pipeline:**

    - Open the Jenkinsfile created in the previous challenge.
    - Add a new stage after the "Run Unit Tests" stage called "Static Code Analysis."
    - Inside the "Static Code Analysis" stage, configure the pipeline to execute the SonarQube analysis on your Java project.

3. **Configure SonarQube Analysis:**

    - Add the necessary SonarQube configuration to your project. In this step, you need to make changes in properties file in the cloned java project.
    - Configure SonarQube properties such as project key, project name, source directory, etc.

4. **Run the Pipeline:**

    - Trigger the Jenkins pipeline manually or automatically (based on your configuration in previous exercise).
    - Observe the pipeline execution as it builds, runs unit tests, and performs static code analysis.

5. **Review SonarQube Results:**

    - Access the SonarQube dashboard (web interface) to review the code analysis results for your project.
    - Explore the various code quality metrics, issues, and recommendations reported by SonarQube.

6. **Address Code Quality Issues:**
    - Identify specific code quality issues highlighted by SonarQube.
    - Analyze the issues and make improvements to the codebase to address the reported problems.
    - Commit the changes to your GitLab repository.

> **Bonus Exercise (Optional)**: The pipeline should fail if the code does not pass a defined quality score.
