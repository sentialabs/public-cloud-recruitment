
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

## Assignment

### Transformation and Migration to the Public Cloud

You have participated in a meeting with a client to assess their strategy to migrate to the public cloud. They are currently hosting a customer facing web application in their on premise environment based on a NodeJS application behind an NGINX reverse proxy. OS level access is necessary in the solution they have developed and this needs to be taken into consideration. They are utilizing a MongoDB cluster for storing data relevant to the application. As a result of their processes, they are generating lot of PDF files for which they utilize local storage. They finance team needs to have access to these files via FTP. All the above services are hosted on several virtual machines.

Finally, the customer currently has 3 environments, namely Test, Acceptance and Production. They wish to keep the same environments in Azure, while following best practices in terms of workload isolation.

The customer is interested in migrating the complete environment to the Public Cloud. They want to leverage within Azure the maximum potential availability from a design perspective and they want the proposed solution to reflect this. The region of choice is West Europe. They have given an indication that they want to go live in Azure within 9 months. They are willing to make small modifications regards to how the application is deployed to the target infrastructure as long as the impact in terms of development technology is minimum and the benefits of the public cloud in terms of scalability substantial. They are not willing to change database technology as they have invested a lot of time in optimizing their MongoDB queries.

You have undertaken the task to design the future state of this environment in the public cloud. The solution needs to:
* be highly available, scalable and flexible.
* utilize only native Azure Services and Products.
* deployable completely using Infrastructure as Code (IaC) from a single codebase.

Any further assumptions that you need to make are welcome as long as they are documented accordingly.

## Deliverables

Please provide the following:
1. An architectural design of the solution. Please use only the latest [Azure Architecture Icons](https://docs.microsoft.com/en-us/azure/architecture/icons/) and export the solution in PDF.
2. A small presentation of no more than 10 slides, describing the solution and mapping the choices made to the various requirements, targeted towards the CTO of the customer.
3. An IaC project/codebase using ARM Templates for an MVP demo of the solution.
4. A link to a publicly accessible git repository containing all the above.

## Links

- [The twelve-factor app](https://12factor.net/)
- [Draw.io](https://www.draw.io/)
- [Microsoft Azure Cloud Design Patterns](https://docs.microsoft.com/en-us/azure/architecture/patterns/)
- [GitHub For Beginners: Don’t Get Scared, Get Started](https://readwrite.com/2013/09/30/understanding-github-a-journey-for-beginners-part-1/)

## License

Copyright © 2019-2021, [Sentia](https://sentia.com). All rights reserved.
