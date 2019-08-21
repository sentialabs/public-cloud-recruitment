
<a href="https://sentia.com/">
    <img src="assets/logo.jpg" alt="Sentia - Lead the way" title="Sentia" align="right" height="60" />
</a>

# Sentia Recruitment

Welcome to Sentia Recruitment

The purpose of this repository is to provide an assignment that will highlight the strengths required by a cloud systems engineer in our public cloud consultancy workforce.

## Table of content

- [General Information](#general-information)
- [Assignment](#assignment)
    - [Part 1 - Transformation and Migration to the Public Cloud](#part-1---transformation-and-migration-to-the-public-cloud)
    - [Part 2 - CI/CD](#part-2---cicd)
- [Deliverables](#deliverables)
- [Links](#links)
- [License](#license)

## General Information

This assignment is meant to challenge the potential applicant in the complete spectrum of designing a solution and delivering an environment in the public cloud using Infrastructure as Code (IaC).

Please be aware of the fact that we are not only looking at the actual deliverables but also the process followed to achieve these results. *The presentation of the results is of equal importance to the actual results.*

You will need to make a choice of delivering your solution in either **Amazon Web Services** or **Microsoft Azure**. We prefer the usage of native tools for IaC. Please use *CloudFormation (CFN)* or *Azure Resource Manager (ARM)* templates for this purpose and **not Terraform**. Of course, third party tools are always necessary in some cases. Please find suggested tools and guides in the [Links](#links) section that may help you in this journey.

## Assignment

### Part 1 - Transformation and Migration to the Public Cloud

You have participated in a meeting with a client to assess their strategy to migrate to the public cloud. They are currently hosting 10 WordPress sites using WordPress Multisite in a private datacenter. They achieve High availability (HA) by using 2 servers and having two copies of their Multisite. For the database, they are using 2 MySQL servers behind and HAProxy to achieve HA.

The past few months, they have been having a lot of issues because their websites have increased in popularity, especially during certain timeframes. For the future state, they have agreed that they want to move away from Multisite, and have independent WordPress applications. They have also pointed out that they have 5 more sites in the making that will reach Production in the next 12 months.

The client is only interested in developing the WordPress sites from an application perspective. They work using GIT repositories, and they have agreed to provide access to the application source code in one or more repositories.

You have undertaken the task to design the future state of this environment in the public cloud. The solution needs to:
* be scalable and flexible.
* be futureproof and expandable with new WordPress sites with minimal effort.

We need to utilize to its full extend the ability of the cloud to scale, when necessary. We also need to version control our IaC templates and for this reason the environment should not be deployed manually within the console in terms of clicking around the different services.

Please provide a design for the designated architecture *in either AWS or Azure*. For the same design, please provide CloudFormation or ARM templates, and everything else that you need to accompany your solution.

### Part 2 - CI/CD

Please provide a design for the CI/CD pipeline that you will use to deliver the changes to the environment, every time the client updates any of their WordPress applications in GIT, where the GitFlow branching strategy is in place. For this purpose, please treat the target architecture from [Part 1](#part-1---transformation-and-migration-to-the-public-cloud) as a black box.

The customer has asked us to ideally use native pipelines (such as AWS CodePipeline or Azure DevOps) for this and that they will have only the Test and Production environments in the scope of this design.

## Deliverables

Please provide the following:
* For Part 1, an architectural design and IaC templates for deploying the components.
* For Part 2, a complete architectural design of the CI/CD process.
* Please include a simple time log of the activities you have performed.
* A presentation of the results within slides, ready to be presented to our client.

## Links

- [GitHub For Beginners: Don’t Get Scared, Get Started](https://readwrite.com/2013/09/30/understanding-github-a-journey-for-beginners-part-1/)
- [Draw.io](https://www.draw.io/)
- [AWS CloudFormation Documentation](https://docs.aws.amazon.com/cloudformation/index.html)
- [Resource Manager on Azure documentation](https://docs.microsoft.com/en-us/azure/azure-resource-manager/)
- [AWS Cloud Development Kit (AWS CDK)](https://github.com/aws/aws-cdk)
- [Amazon EC2 Auto Scaling](https://aws.amazon.com/ec2/autoscaling/?sc_channel=ba&sc_campaign=autoscaling-ec2-button&sc_medium=button&sc_country=global&sc_geo=global&sc_outcome=aware)
- [Microsoft Azure Virtual Machine Scale Sets](https://docs.microsoft.com/en-us/azure/virtual-machine-scale-sets/overview?toc=%2Fazure%2Fvirtual-machines%2Flinux%2Ftoc.json)
- [AWS Well-Architected](https://aws.amazon.com/architecture/well-architected/)
- [Microsoft Azure Cloud Design Patterns](https://docs.microsoft.com/en-us/azure/architecture/patterns/)
- [The Twelve Factors](https://12factor.net/)
- [GitFlow](https://nvie.com/posts/a-successful-git-branching-model/)
- [Containers](https://www.docker.com/resources/what-container)
- [Kubernetes (K8s)](https://kubernetes.io/)

## License

Copyright © 2019, [Sentia](https://sentia.com). All rights reserved.
