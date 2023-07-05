# aws-codepipeline-demo

this repo consits of workflow for setting up an aws code pipeline. The code pipeline pulls the source code here dockerfile and makes
a docker image of it and pushes it to aws private ecr, the build process is being carried out by aws code build and we create build project for it
which require a buildspec.yaml (a sample is being added in the repo), once the image is pushed into ecr we can deploy it using aws deploy or directly 
through aws ecs service where we can use the fargate or ec2 service, for deployment we need a imagedefinition.json file for updating the task definition
on every updation of the image.
