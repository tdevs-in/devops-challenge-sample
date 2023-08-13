# Weekend special - Build Notifications and Wrap-up Challenge

## Overview

In this final challenge, you will enhance your Jenkins pipeline by setting up build notifications to receive status updates on a platform of your choice, such as Slack or Email. Additionally, you will intentionally trigger a build that includes a failing test to verify that the build notifications are functioning correctly.

## What topics we will cover

1. Configuring build notifications in Jenkins.
2. Triggering and observing build notifications.
3. Reviewing the overall DevOps challenge experience.

## After this exercise, you will learn

By completing this challenge, you will gain practical experience in configuring build notifications and ensuring timely awareness of pipeline status. You will understand how to effectively receive notifications for both successful and failed builds, enabling you to maintain better control over your software delivery process.

## Exercise

For this exercise, use this project: https://github.com/tdevs-in/d10c-w1d4

1. **Configure Build Notifications:**

    - Decide on your preferred notification platform, such as Slack or Email.
    - For Slack: Create a new channel (e.g., #devops-notifications) or use an existing one.
    - For Email: Ensure you have a valid email address to receive notifications.
    - In your Jenkins server, navigate to the pipeline configuration (Jenkins job).
    - Look for the "Post-build Actions" section.
    - Add the appropriate plugin or action for your chosen notification platform (e.g., "Slack Notification" plugin for Slack or "Editable Email Notification" for Email).
    - Configure the plugin with the necessary details, such as channel name or email address.
    - Save the pipeline configuration.
    - You may need setup a sample mail server for receiving mails. (Sendgrid, mailchimp etc)

2. **Trigger a Build with Failing Test:**

    - Open the sample Java project that you've been working on.
    - Choose a unit test within the project and intentionally modify it to fail. For example, change an assertion to an incorrect value.
    - Commit the changes to your GitLab repository.

3. **Observe and Verify Notifications:**
    - In your Jenkins server, trigger a new build for your pipeline manually.
    - Monitor the build process and wait for it to complete.
    - Once the build is finished, check your preferred notification platform (Slack or Email) for the notification.
    - Verify that you receive a notification about the failed build, including relevant information such as build status, timestamp, and a link to the detailed build log.

> **Bonus Challenge(Optional)**: If you are using GitHub throughout the challenges, you may know about GitHub actions. You can build all pipelines via GitHub actions too. Try to implement this.

## Conclusion and Wrap-up

Congratulations! You have completed the first 7 days of DevOps challenge and gained valuable practical experience in working with Jenkins and Git. Through this final exercise, you've successfully set up build notifications and verified their functionality by intentionally triggering a build with a failing test. You've learned how to keep track of pipeline statuses and promptly respond to any build issues.

Your journey in this challenge showcases your dedication to enhancing your DevOps skills. Keep practicing, exploring, and applying what you've learned to real-world scenarios. As you continue your DevOps journey, remember that each step forward contributes to your growth as a DevOps practitioner.
