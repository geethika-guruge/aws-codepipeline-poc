**End to End Deployment Pipeline**

This directory contains the cloudformation template to create a pipeline for an automated deployment build. Deploying this template will create a AWS CodePipeline and a AWS CodeCommit Repository, along with nececary IAM roles, S3 buckets and other infrasturcture. A prefix with the value of the input parameter `ServiceName` will be added to all these resources.

You must check in the `buildspec.yml` file, and any other supporting scripts to the CodeCommit repository created by this template.

A sample `buildspec.yml`, supporting scripts and a cloudformation template for the demo stack can be found in the [link to Demo-Project_repo ](Demo-Project_repo) directory