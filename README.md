# EL_Task2_my-app

This is a simple Node.js app for demonstrating CI/CD using Jenkins and Docker.

## Task Objective

- Automate build and deployment using Jenkins pipeline.
- Trigger pipeline on every code commit using GitHub Webhooks.
- Build a Docker image of the app as part of the pipeline.

## Tools Used

- Jenkins
- GitHub
- Docker
- Node.js (sample app)

## Pipeline Stages

1. **Install Dependencies**: Runs `npm install`
2. **Test**: Runs `npm test`
3. **Docker Build**: Builds Docker image from the `Dockerfile`

## Outcome

Successfully set up a CI/CD pipeline that:
- Runs automatically on code push to GitHub
- Builds and packages the app using Docker
