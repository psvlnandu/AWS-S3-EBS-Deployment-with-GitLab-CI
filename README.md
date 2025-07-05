# CI/CD Pipeline for a Static Website using GitLab CI
This project demonstrates a complete, automated CI/CD pipeline built on GitLab. The pipeline automatically builds, tests, and deploys a simple static website to GitLab Pages.
Live Demo: 
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

AWS Elastic Beanstalk: (Optional - add if you used it for this project) Deployed applications using a managed AWS service, understanding environment configuration and application versioning.


- **Check the** [**course notes**](docs/course-notes.md)

