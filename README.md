# Jefrey_ERICPSIL

Objective:EC2 Self-Hosted Runner Deployment

Overview:
This project aims to deploy an application to an AWS EC2 instance using GitHub Actions. The pipeline will pull the latest changes from our repository, build the application, and deploy it to the EC2 instance.

Running the Pipeline
To set up the pipeline to deploy the application to EC2 instance, follow these steps:

1. Created a self-hosted runner on your EC2 instance:
    step 1. navigate to setting
    step 2. navigate to Actions dropdown
    step 3. Now cilck on Runners
    step 4. click on "New self-hosted runner"
    step 5. setup using Runner image -Linux, Architecture -64 

2. Configured GitHub Actions workflow:
  Created a workflow file .github/workflows/main.yml (I have give in zip file)

3.Deployment

To deploy application, simply push your changes to the `main` branch. The GitHub Actions workflow will automatically trigger and deploy your application to the EC2 instance.

----------------------------------------------------------------------------------------------------------------------------------------

CI/CD Process:
The CI/CD process consists of the following stages:
1. Code Commit: Developers commit their code changes to a version control system of GIT.
2. Build: The CI server automatically pulls the latest code changes, builds the application, and runs automated tests.
3. Deploy: If the tests pass successfully, the CD server automatically deploys the application to the target machine.
4. Monitor and Feedback: The system continuously monitors the deployed application and provides feedback to the development team.
----------------------------------------------------------------------------------------------------------------------------------------
Tool Choices
For this project, I have chosen the following tools:

1. Version Control System: Git
Git is a distributed version control system that allows multiple developers to collaborate on a project efficiently.
2. CI/CD Platform: GitHub Actions
GitHub Actions is a CI/CD platform provided by GitHub.
It allows you to automate workflows directly from your GitHub repository.
3. Deployment Platform: Amazon EC2
Amazon Elastic Compute Cloud (Amazon EC2) is a web service that provides resizable compute capacity in the cloud.
It is suitable for hosting applications of various sizes and types.
4. Self-Hosted Runner
A self-hosted runner allows you to run GitHub Actions workflows on your own infrastructure, such as an EC2 instance.

Scaling for Larger Applications:
For larger applications, the CI/CD setup can be scaled by:

1. Using multiple self-hosted runners to parallelize workflows.
2. Implementing canary deployments or blue-green deployments for zero-downtime updates.
3. Implementing auto-scaling for the infrastructure to handle increased load.
----------------------------------------------------------------------------------------------------------------------------------------
Achieved :
Implementing a CI/CD process with GitHub Actions and Amazon EC2 allows for automated testing, rapid deployment, and efficient scaling of applications. By automating the development workflow, teams can reduce manual errors, deliver updates faster, and improve overall productivity
