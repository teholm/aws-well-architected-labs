# Level 200: Testing for Resiliency of EC2
https://wellarchitectedlabs.com

## Introduction

The purpose if this lab is to teach you the fundamentals of using tests to ensure your implementation is resilient to failure by injecting failure modes into your application. This may be a familiar concept to companies that practice Failure Mode Engineering Analysis (FMEA). One primary capability that AWS provides is the ability to test your systems at a production scale, under load.

It is not sufficient to only design for failure, you must also test to ensure that you understand how the failure will cause your systems to behave. The act of conducting these tests will also give you the ability to create playbooks how to investigate failures. You will also be able to create playbooks for identifying root causes. If you conduct these tests regularly, then you will identify changes to your application that are not resilient to failure and also create the skills to react to unexpected failures in a calm and predictable manner.

In this lab, you will deploy a 2-tier resource, with a reverse proxy (Application Load Balancer), and Web Application on Amazon Elastic Compute Cloud (EC2).

The skills you learn will help you build resilient workloads in alignment with the [AWS Well-Architected Framework](https://aws.amazon.com/architecture/well-architected/)

## Goals:

* Reduce fear of implementing resiliency testing by providing examples in common development and scripting languages
* Resilience testing of EC2 instances
* Learn how to implement resiliency using those tests
* Learn how to think about what a failure will cause within your infrastructure
* Learn how common AWS services can reduce mean time to recovery (MTTR)

## Prequisites:

* An
[AWS Account](https://portal.aws.amazon.com/gp/aws/developer/registration/index.html) that you are able to use for testing, that is not used for production or other purposes.
* An Identity and Access Management (IAM) user or federated credentials into that account that has permissions to create Amazon Virtual Private Cloud(s) (VPCs), including subnets, security groups, internet gateways, NAT Gateways, Elastic IP Addresses, and route tables. The credentials must also be able to create the database subnet group needed for a Multi-AZ RDS instance. The credential will need permissions to create IAM Role, instance profiles, AWS Auto Scaling launch configurations, application load balancers, auto scaling group, and EC2 instances.
* An IAM user or federated credentials into that account that has permissions to deploy the deployment automation, which consists of IAM service linked roles, AWS Lambda functions, and an AWS Step Functions state machine to execute the deployment.

NOTE: You will be billed for any applicable AWS resources used if you complete this lab that are not covered in the
[AWS Free Tier](https://aws.amazon.com/free/).



<BR>

## [Start the Lab!](Lab_Guide.md)

<BR>
<BR>

***

## License

### Documentation License

Licensed under the [Creative Commons Share Alike 4.0](https://creativecommons.org/licenses/by-sa/4.0/) license.

### Code LicenseLicensed under the Apache 2.0 and MITnoAttr License.

Copyright 2019 Amazon.com, Inc. or its affiliates. All Rights Reserved.

Licensed under the Apache License, Version 2.0 (the "License"). You may not use this file except in compliance with the License. A copy of the License is located at

    https://aws.amazon.com/apache2.0/

or in the "license" file accompanying this file. This file is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the License for the specific language governing permissions and limitations under the License.
