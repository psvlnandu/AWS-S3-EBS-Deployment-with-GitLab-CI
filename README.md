# CI/CD Pipeline for a Static Website using GitLab CI
This project demonstrates a complete, automated CI/CD pipeline built on GitLab. The pipeline automatically builds, tests, and deploys a simple static website to GitLab Pages.
Live Demo: 
## Concepts Covered in This Repository
This project is a hands-on guide to building a complete CI/CD pipeline. Here’s a quick look at the key concepts and technologies you'll work with:
### CI/CD Fundamentals
What is CI/CD? We'll cover the basics of Continuous Integration (CI) and Continuous Deployment (CD).

CI: Automatically building and testing your code with every new commit.

CD: Automatically deploying every successful change to a live environment

Pipeline Structure: Learn how to design a multi-stage pipeline with jobs for build, test, and deploy. 
### Docker & GitLab Container Registry
Building Docker Images: We'll write a Dockerfile to package our application, starting with a lightweight base image like alpine.

GitLab Container Registry: Instead of Docker Hub, we'll use GitLab's own built-in registry to store and manage our Docker images.

Testing with Docker: Learn how to use a service in GitLab CI to run your Docker image in the background. GitLab automatically handles the networking, making it easy to test your running application.

###  GitLab CI/CD in Action
Commands & Keywords: Get familiar with the essential GitLab CI syntax and keywords used in the .gitlab-ci.yml file.

Controlling Deployments with rules: You don't want every commit on every branch to go live. We'll use rules to make sure the deployment job only runs when changes are merged into the main branch.

Using CI/CD Variables: See how to use GitLab's powerful built-in variables (like CI_COMMIT_REF_NAME and CI_DEFAULT_BRANCH) to make your pipeline scripts smarter and more flexible.

Integration Testing: We'll run simple but effective tests to confirm the application is working correctly after it's built. This involves using shell commands like curl and grep to check the content of the running website.
### Deploying to the AWS Cloud
Amazon S3 for Hosting: Learn how to deploy a static website to an AWS S3 bucket.

Configuring S3: We'll walk through all the necessary steps:

Uploading the build files to the bucket.

Setting the correct permissions and bucket policies to make the website public.


## Pipeline Stages
The .gitlab-ci.yml file defines the following stages that execute on every code commit:

build: This stage uses npm to install the necessary dependencies and build the static website files from the source code.

test: This stage runs automated tests against the code to ensure quality and prevent regressions. For this project, this includes linting checks.

deploy: Upon successful completion of the previous stages, this stage automatically publishes the built website to GitLab Pages, making it publicly accessible.
## Key Learnings & Skills Demonstrated

Cloud Deployment: Gained hands-on experience deploying web applications to the cloud using Amazon Web Services (AWS).

CI/CD Principles: Built a complete CI/CD pipeline to automate the workflow from code commit to a live cloud deployment.

GitLab CI: Became proficient in writing .gitlab-ci.yml files, defining stages, jobs, and securely managing AWS credentials.

AWS S3: Acquired skills in configuring S3 buckets for static website hosting, setting public access policies, and managing object permissions.

AWS Elastic Beanstalk:  Deployed applications using a managed AWS service, understanding environment configuration and application versioning.


- **Check the** [**course notes**](docs/course-notes.md)

