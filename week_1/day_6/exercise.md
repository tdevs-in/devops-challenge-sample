# Security Scanning Challenge

## Overview

In this challenge, you will integrate a security scanning tool, such as OWASP ZAP (Zed Attack Proxy), into your Jenkins pipeline. You will set up an OWASP ZAP server or use the ZAP Docker container, run security scans against the sample application during the pipeline execution, analyze the security scan results, and address any vulnerabilities identified.

## What topics we will cover

1. Integrating security scanning tools into a CI/CD pipeline.
2. Setting up and configuring OWASP ZAP.
3. Performing security scans and analyzing results.

## After this exercise, you will learn

By completing this challenge, you will gain practical experience in integrating a security scanning tool (OWASP ZAP) into your Jenkins pipeline. You will learn how to set up and configure OWASP ZAP, modify a Jenkins pipeline to include security scans, analyze the scan results, and address security vulnerabilities. This exercise will enhance your understanding of the importance of security in the DevOps process and equip you with skills to proactively identify and mitigate potential security risks in your applications.

## Exercise

For below exercise, use this java project for your pipeline: https://github.com/tdevs-in/d10c-w1d5

1. **Set Up OWASP ZAP:**

    - Install and configure OWASP ZAP locally or use the OWASP ZAP Docker container.
    - Obtain the necessary authentication tokens or credentials for accessing your application.

2. **Modify Jenkins Pipeline:**

    - Open the Jenkinsfile created in previous challenges.
    - Add a new stage after the "Static Code Analysis" stage called "Security Scanning."
    - Inside the "Security Scanning" stage, configure the pipeline to execute security scans using OWASP ZAP against your sample application.

3. **Configure OWASP ZAP Scans:**

    - Define the necessary configurations for OWASP ZAP scans, such as target URLs, authentication settings, and scan policies.

4. **Run the Pipeline:**

    - Trigger the Jenkins pipeline manually or automatically (based on your configuration in previous exercises).
    - Observe the pipeline execution as it builds, runs unit tests, performs static code analysis, and conducts security scans.

5. **Analyze Security Scan Results:**

    - Access the OWASP ZAP interface or generated reports to review the security scan results for your sample application.
    - Identify and categorize security vulnerabilities based on severity levels.

6. **Address Security Vulnerabilities:**
    - Collaborate with your development team to address the identified security vulnerabilities.
    - Apply appropriate fixes, updates, or configurations to mitigate the vulnerabilities.

> **Bonus challenge (Optional):** Build a separate job for this exercise and run it regularly via cron schedule for predefined set of repositories. Send alerts to slack or other channels if any vulnerabilities are found. The notification setup will be the upcoming exercise.
