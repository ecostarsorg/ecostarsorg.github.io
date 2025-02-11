# Data security
* Version: v1.1
* Date of version: 2024-04
* Author: Information Security Officer
* Approver: CTO
* Confidentiality: Internal use. Shared upon request as part of a due diligence

## Data Centers 
Ecostars relies on world-class cloud providers, which have data centers located inside the European Union. Our current cloud provider is **[Microsoft Azure](https://azure.microsoft.com/)**.

All services are allocated in the **“West Europe” region**, located in several data centers in the outskirts of **Amsterdam (Netherlands)**.

As our data grows, we are planning to deploy in a second region for **geo-redundancy** reasons. We will probably do so as soon as the Madrid Data Center by Azure is ready. 

## Databases 
Databases are hosted by our cloud provider: [Microsoft Azure](https://azure.microsoft.com/) in its data centers in the “West Europe” region. In the future Google Cloud Platform or Amazon Web Services might be used too, always using EU datacenters compliant with our policies.

The following database managers handle Ecostars customers’ data. 

* Main database: PostgreSQL 14.12
* Search indexes: ElasticSearch 7.17 
* Real-time data: InfluxDB 2.7.6 
* Document database: MongoDB 7.0.14 


## Database replication
Databases are also replicated according to business and availability requirements (e.g. all non-transient data has at least a live replica and periodical off-site backups). 

## Backups
Data is backed-up in a fully automated way. Backups are kept in the Azure Blob Storage service, fully-encrypted at rest, and copied off-site periodically.

## Additional security measures 

At Ecostars we always try to follow security and scalability recommendations when we design, implement and deploy our services. These include, but are not limited to: 

* We follow [OWASP](https://owasp.org) recommendations for secure code development and service deployment

* Our applications are built using the [12 factor app methodology](https://12factor.net/) to ensure their portability and resilience

* Access to any service is filtered by a Web Application Firewall (WAF), which prevents brute force attacks, DDOS attempts and access from known compromised addresses. 

* All our databases follow a strict multi-tenant architecture. Users from one tenant are not permitted to access any other tenants’ information, even at the database level. Cross-tenant access is only ever used to query and aggregate data (e.g. to calculate benchmarks across the data from different tenants) and dropped immediately, following the principle of least privilege. 

* Our software follows the Command-Query Responsibility Segregation architecture, to allow, among other things, to more easily debug the code and prevent unintended side-effects. 

* Our development process includes code reviews on all software deployed, automated unit tests in business critical areas of the code, and Continuous Integration (CI) processes, which increases the code quality and speeds up the deployment times. 

* We have a strict QA process which includes a completely independent staging environment, populated with fake data. Critical features never go live until they have been thoroughly tested in the staging environment. 

* All secrets (API keys, etc.) are distributed using the Principle of Least Privilege. All queries and commands use accounts that follow this principle and have the least amount of permissions needed to execute said query or command. 

* Access to the production and staging environments is limited on a need-to-know basis. The production environment specifically cannot be accessed by most developers, but only those in a trusted-ring which only includes the most senior developers in the team. 

* Access to any environment is strictly done using secure protocols (e.g. SSH) and always with private keys. Password-based access is explicitly disabled in all services. 

* Our services run software from a read-only repository so even if one service is compromised, the intruder won't be able to affect other services. The software is also mounted from a read-only filesystem, so even an undesired access would prevent any changes in either the software or its configuration files. 

* Software at the OS-level and dependencies are updated automatically as part of the normal development flow. Our CI process allows us to deploy several times a week (often several times a day) and each of those deployments checks for published security fixes in all of our software. 

* Every 6 months, we undergo an internal information security assessment where we do end-to-end testing of security, upgrade software manually to the latest major versions and double-check security patches for known CVEs. Finally, we deploy a new environment to check the Disaster Recovery procedure hands-on. 


## Conditions of use 
Each acceptance (or termination) of our Terms & Conditions and Privacy Policy are kept according to the GDPR, being an opt-in process. Final users will be able to change this acceptance, allowing them to opt-in and opt-out from receiving commercial comms. The date for opt-ins and opt-outs are also saved in our systems.
