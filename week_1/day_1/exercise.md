# Deploy Jenkins and GitLab Instances

## Overview

In this exercise, you will deploy Jenkins and GitLab instances on a cloud platform of your choice using Terraform templates. Alternatively, you can choose to deploy Jenkins and GitLab locally using a shell script, with the option to deploy on your local machine or within Docker containers.

## What topics we will cover

1. Deploying Jenkins on a cloud platform via Terraform templates.
2. Deploying Jenkins locally using a shell script (on your local machine or Docker).
3. Deploying GitLab on a cloud platform via Terraform templates.
4. Configuring GitLab post-deployment to disable password authentication and enable SSH-based authentication.

## After this exercise, you will learn

-   How to deploy Jenkins and GitLab instances using Terraform templates.
-   How to deploy Jenkins locally using a shell script and Docker.
-   How to configure GitLab to disable password cloning and enable SSH-based cloning.

## Exercise

1. Choose the cloud platform where you want to deploy Jenkins and GitLab (e.g., Azure, AWS, GCP) or set them up locally (on your local machine or within Docker).

2. **Deploy Jenkins on the Cloud (Terraform):**

    - Write a Terraform script (e.g., `jenkins.tf`) to define the infrastructure resources and configurations required to deploy Jenkins on the cloud platform of your choice.
    - Use Terraform commands to apply the script and deploy the Jenkins instance.
    - Ensure the Jenkins instance is accessible through a public IP or domain name and access should be restricted to your IP address only.

3. **Deploy Jenkins Locally (Shell Script):**

    - Write a shell script (e.g., `deploy_jenkins_local.sh`) to automate the installation and configuration of Jenkins either on your local machine or within a Docker container.
    - If deploying within Docker, ensure the necessary ports are exposed and accessible.
    - Execute the shell script to set up Jenkins locally.

4. **Deploy GitLab on the Cloud (Terraform):**
    - Write a Terraform script (e.g., `gitlab.tf`) to define the infrastructure resources and configurations required to deploy GitLab on the cloud platform of your choice.
    - Use Terraform commands to apply the script and deploy the GitLab instance.
    - Post-deployment, manually configure GitLab to disable password cloning and enable SSH-based cloning for repositories.
5. **Deploy GitLab Locally (Shell Script or Docker):**
    - Write a shell script (e.g., deploy_gitlab_local.sh) to automate the installation and configuration of GitLab on your local machine.
    - Alternatively, if you prefer Docker, write a shell script (e.g., deploy_gitlab_docker.sh) to set up GitLab within a Docker container.
    - If deploying within Docker, ensure the necessary ports are exposed and accessible.
    - Execute the shell script to set up GitLab locally.
6. Perform configuration on Jenkins by creating users and install plugins. Install plugins for building pipelines, access restrictions to users via matrix. Also, create a few users and setup roles for them and assign those roles to the created users.
7. Perform configuration on GitLab by creating admin account and user accounts. Also create service user and add these credentials to Jenkins for checking out of repositories. Setup RSA keypairs for passwordless authentication locally.
8. You can test the above by creating a sample pipeline and repository and checking out the repository in pipeline build. This step is optional.

There will be many exercises around pipeline development, CI/CD in future.
