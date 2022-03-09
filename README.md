## Getting Started with Amazon WorkSpaces workshop template

This repository contains the AWS CloudFormation template to provision the prerequisites for the [Getting started with Amazon WorkSpaces workshop](https://workspaces.workshop.aws/).

### What is created
- VPC
- 2 private subnets
- 1 public subnet
- Internet gateway, NAT gateway and related routes
- Secret in Secrets Manager
- AWS Directory Service for Microsoft Active Directory

This template uses an AWS Lambda function to ensure the subnets are created in an Availability Zone supported by WorkSpaces. For supported Availability Zones, refer to the [Amazon WorkSpaces Administration Guide](https://docs.aws.amazon.com/workspaces/latest/adminguide/azs-workspaces.html).

## Instructions
1. Navigate to the AWS CloudFormation console.
    1. Verify a valid Region is selected in the upper right corner.
2. Choose **Create stack, with new resources (standard).**
3. Choose **Upload a template file**.
4. Select **cloudformation.yaml** from the repository.
5. For **Stack name**, enter *WorkSpaces-Workshop*.
7. Choose **Next**.
8. On the Configure stack options page, choose **Next**.
9.  Select **I acknowledge that AWS CloudFormation might create IAM resources with custom names**.
10. Choose **Create stack**.

Once your stack is created, you can start your workshop.

## Clean up
You can clean up the resources created by deleting the AWS CloudFormation template. For clean up of the workshop resources, refer to the [clean up section of the workshop](https://catalog.us-east-1.prod.workshops.aws/v2/workshops/ba8389fd-99a1-4010-a95e-d691a2c08311/en-US/cleanup).

1. Navigate to the AWS CloudFormation console.
2. Choose the *WorkSpaces-Workshop* stack.
3. Choose **Delete**.

## Security

See [CONTRIBUTING](CONTRIBUTING.md#security-issue-notifications) for more information.

## License

This library is licensed under the MIT-0 License. See the LICENSE file.

