
<a href="https://sentia.com/">
    <img src="assets/logo.jpg" alt="Sentia - Lead the way" title="Sentia" align="right" height="60" />
</a>

# Sentia Recruitment

Welcome to Sentia Recruitment

The purpose of this repository is to provide an assignment that will highlight the strengths required by a cloud systems consultant in our public cloud consultancy workforce.

## Table of content

- [General Information](#general-information)
- [Assignment](#assignment)
    - [Transformation and Migration to the Public Cloud](#transformation-and-migration-to-the-public-cloud)
- [Deliverables](#deliverables)
- [Links](#links)
- [License](#license)

## General Information

This assignment is meant to challenge the potential applicant in the complete spectrum of designing a solution and delivering an environment in the public cloud using Infrastructure as Code (IaC).

Please be aware of the fact that we are not only looking at the actual deliverables but also the process followed to achieve these results. *The presentation of the results is of equal importance to the actual results.*

You will need to make a choice of delivering your solution in either **Amazon Web Services** or **Microsoft Azure**.

## Assignment

### Transformation and Migration to the Public Cloud

You have participated in a meeting with a client to assess their strategy to migrate to the public cloud. They are currently hosting a customer facing web application on their on premise emnvironment based on a NodeJS application behind an NGINX reverse proxy. They are ustilizing a MongoDB cluster for storing data as well as an FTP server for document storage. They also maintain a cron server, mostly Bash and Python scripts, relevant to a small amount of jobs that need to be executed a few times per day (no more than once per hour). All the above services are hosted on several virtual machines.

Finally, the customer currently has 3 environements, namely Test, Acceptance and Production.

The customer is interested in migrating the complete envitonment to the Public Cloud. They are not in a rush, and they have given an indication that they want to go live on the Public Cloud 12 months after they have agreed on the vendor to support them in this journey. They want to make sure that they have enough time to adjust the application to any technology related changes originating from an infrastructure perspective.

There is a hard requirement for exporting all application and infrastructure logs to an ElasticSearch Cluster. The customer needs to have access to the Kibana dashboard within their headquarters but the cluster/dashboard *should not* be publically accessible.

You have undertaken the task to design the future state of this environment in the public cloud. The solution needs to:
* be scalable and flexible.
* utilize managed services as much as possible.

Cost optimization should be applied when necessarty, even if a few application related modifications are necessary. Environment isolation is important, but some shared services would be acceptable if they result in major cost reduction.

## Deliverables

Please provide the following:
1. An architectural design for all the components and all the environemnts.
2. An IaC project for deploying an MVP demo (excluding the CRON and the ElasticSearch requirements).
    * for AWS, write your IaC using: **AWS CDK**, or alternatively with AWS CloudFormation or Terraform.
    * for Azure, write your IaC using: **ARM Templates**, or alternatively with Terraform.
3. Include a simple time log of the activities you have performed.
4. Document any assumptions and decisions you have made.
5. A GIT repo with all the above.

## Links

- [The twelve-factor app](https://12factor.net/)
- [Draw.io](https://www.draw.io/)
- [AWS Well-Architected](https://aws.amazon.com/architecture/well-architected/)
- [Microsoft Azure Cloud Design Patterns](https://docs.microsoft.com/en-us/azure/architecture/patterns/)

## License

Copyright © 2019-2021, [Sentia](https://sentia.com). All rights reserved.