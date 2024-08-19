Blue-Green Deployment Project
In this project, I implemented a Blue-Green Deployment strategy using AWS services to minimize downtime during application updates. Here's a brief overview of the process:

IAM Roles:

Created IAM roles with permissions for S3, CodeDeploy, Pipeline, and Auto Scaling, ensuring secure and smooth operations across services.
Auto Scaling Group:

Set up an Auto Scaling Group with a custom launch template, security groups, and user data scripts. This group handled the dynamic scaling of instances, distributing traffic between the blue and green environments.
Load Balancer & Target Group:

Configured a new load balancer and target group to manage traffic routing between the two environments (blue and green), ensuring zero downtime during deployment.
CodeDeploy:

Created a CodeDeploy application and deployment group linked to the Auto Scaling Group. This facilitated automated deployments, allowing seamless transitions between the blue and green environments.
CodePipeline:

Set up a CodePipeline for continuous integration and continuous deployment (CI/CD). The pipeline fetched code from GitHub, built and tested it, and then deployed it using CodeDeploy.
Deployment Process:

After deploying the new version to the green environment, I monitored the deployment, rerouted traffic from the blue to the green environment using the load balancer, and terminated the old instances to finalize the switch.
S3 Bucket:

Used S3 to store artifacts and manage code files efficiently during the deployment process.
This project provided hands-on experience with AWS services and solidified my understanding of Blue-Green Deployment, CI/CD pipelines, and automated deployments.


