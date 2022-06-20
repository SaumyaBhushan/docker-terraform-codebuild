## This project will do the following task:
* Terraform project is build to create a Codebuild project.
* Terraform deploys the code to AWS and create the Codebuild project.
* When build is run, Codebuild builds the Docker image using the Github repository as source
* Finally, Codebuild pushes the Docker image to ECR.

### Firstly, you will need an ECR repository for our built Docker image. You can use the steps defined in AWS documentation to create a private ECR.
```terraform.tfvars file contains variables values as input. Make sure to update before deploying. ```
### Run the following commands to deploy and create the AWS Codebuild project
* terraform init
* terraform validate
* terraform apply

The project should now be visible in AWS console. Now it is time to build the project we created. Click on the project and then click Start build. As a result, our new Docker image pushed to our ECR repository.

