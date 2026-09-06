![alt text for screen readers](/01-Cloud-Computing-Fundamentals/cloud-computing-fundamentals.png "Cloud computing Basics").

# Cloud Computing Fundamentals

> A practical introduction to cloud computing concepts, deployment models, and cloud service models, with an Azure-oriented perspective.

## Table of Contents

- [What Is Cloud Computing?](#what-is-cloud-computing)
- [Why Cloud Computing?](#why-cloud-computing)
- [Cloud Deployment Models](#cloud-deployment-models)
  - [Public Cloud](#public-cloud)
  - [Private Cloud](#private-cloud)
  - [Hybrid Cloud](#hybrid-cloud)
- [Cloud Service Models](#cloud-service-models)
  - [IaaS](#iaas)
  - [PaaS](#paas)
  - [SaaS](#saas)
- [IaaS vs PaaS vs SaaS](#iaas-vs-paas-vs-saas)
- [Choosing the Right Model](#choosing-the-right-model)
- [Key Takeaways](#key-takeaways)

---

## What Is Cloud Computing?

Cloud computing is a way of consuming computing capabilities over a network instead of purchasing and maintaining all of the underlying infrastructure yourself.

Those capabilities can include:

- Compute
- Storage
- Networking
- Databases
- Application platforms
- Software
- Analytics and other managed services

A simple way to think about it is:

> **Instead of owning and operating every piece of infrastructure, you consume the resources you need from a cloud provider and pay according to the service and usage model.**

Examples of major cloud providers include **Microsoft Azure, Amazon Web Services (AWS), and Google Cloud**.

---

## Why Cloud Computing?

Traditional on-premises environments often require an organization to purchase hardware, provision capacity, install software, maintain infrastructure, and plan for future growth.

Cloud computing can reduce that operational burden by allowing organizations to consume infrastructure and managed services on demand.

Common benefits include:

- **Elasticity:** Increase or decrease resources as demand changes.
- **Consumption-based cost:** Many services can be paid for based on usage.
- **Faster provisioning:** New resources can often be created much faster than physical infrastructure.
- **Reduced infrastructure management:** The provider handles some or all of the underlying infrastructure depending on the service model.
- **Global reach:** Cloud providers offer infrastructure and services across multiple geographic regions.
- **Managed capabilities:** Services such as databases, messaging, monitoring, and application hosting can be consumed without managing every underlying component.

Cloud computing does not eliminate responsibility; it changes **which responsibilities belong to the cloud provider and which remain with the customer**.

---

# Cloud Deployment Models

A deployment model describes **where the infrastructure is hosted and who it is dedicated to**.

The three models covered here are:

1. Public Cloud
2. Private Cloud
3. Hybrid Cloud

## Public Cloud

In a public cloud, the cloud provider owns and operates the underlying physical infrastructure and makes computing services available to customers over a network.

For example, **Microsoft Azure** is a public cloud platform.

### Characteristics

- Infrastructure is operated by the cloud provider.
- Customers consume resources and services rather than owning the physical infrastructure.
- Resources can be provisioned, scaled, and removed as required.
- Customers typically manage their resources through portals, APIs, CLI tools, or other management interfaces.

### Advantages

- No need to purchase physical servers for every capacity increase.
- Resources can be scaled according to workload requirements.
- Consumption-based pricing can reduce the need for large upfront infrastructure investments.
- New resources can generally be provisioned quickly.
- The provider handles physical infrastructure maintenance.

### Considerations

- Applications depend on network connectivity to reach cloud services.
- The customer does not control the provider's physical infrastructure.
- Security responsibilities are shared between the provider and customer.
- Costs must be monitored carefully because usage can increase as resources scale.

---

## Private Cloud

A private cloud is an environment dedicated to a single organization.

It may be hosted within an organization's own datacenter or provided as a dedicated environment by another party.

Private cloud is often considered when an organization has strong requirements around:

- Data control
- Security
- Compliance
- Regulatory requirements
- Infrastructure customization

### Advantages

- Greater control over the environment.
- Infrastructure can be customized for organizational requirements.
- The organization can apply its own security and governance controls.
- Dedicated infrastructure can be appropriate for workloads with specific isolation requirements.

### Considerations

- Building and operating the infrastructure can require significant capital investment.
- Hardware, software, networking, maintenance, and operations may remain the organization's responsibility.
- Specialized IT skills may be required.
- Scaling can require additional infrastructure investment.

---

## Hybrid Cloud

A hybrid cloud combines **private/on-premises infrastructure with public cloud services**.

This model allows an organization to decide where individual workloads or data should run.

### Example

An organization could:

- Keep a sensitive database in an on-premises environment.
- Host a customer-facing application in Azure.
- Establish secure connectivity between the two environments.

Another scenario is a legacy application that cannot easily be moved to modern infrastructure. The organization may keep that application on-premises while using cloud services for selected capabilities such as storage, authentication, or other supporting functions.

### Advantages

- Provides flexibility in workload placement.
- Allows existing or legacy systems to continue operating.
- Can support gradual migration to the cloud.
- Makes it possible to keep selected workloads or data in a private environment.

### Considerations

- Architecture and operations can become more complex.
- Secure connectivity between environments must be designed and maintained.
- Monitoring and troubleshooting may span multiple environments.
- Costs can be higher because both on-premises and cloud infrastructure may need to be maintained.

---

# Cloud Service Models

A service model describes **how much of the technology stack the cloud provider manages for you**.

The three common models are:

| Model | Name |
|---|---|
| IaaS | Infrastructure as a Service |
| PaaS | Platform as a Service |
| SaaS | Software as a Service |

As you move from **IaaS → PaaS → SaaS**, the cloud provider generally takes responsibility for more of the underlying technology stack.

---

## IaaS

**Infrastructure as a Service (IaaS)** provides fundamental computing resources such as virtual machines, storage, and networking.

Instead of purchasing physical infrastructure, the customer consumes virtualized infrastructure from the cloud provider.

### Responsibility

The provider manages the physical infrastructure and virtualization layer.

The customer generally remains responsible for areas such as:

- Operating system
- Application
- Application configuration
- Data
- Network configuration within the service
- Security of the resources they configure

### When IaaS Makes Sense

IaaS can be useful when:

- You need substantial control over the operating system.
- An application requires a specific server configuration.
- You are migrating an existing workload that expects a traditional server environment.
- Storage or compute requirements are unpredictable.
- You want cloud infrastructure without purchasing physical hardware.

### Advantages

- High level of control.
- Flexible infrastructure configuration.
- Resources can be provisioned when required.
- Can support workloads that need operating-system-level access.

### Trade-off

The flexibility comes with additional management responsibility. You still have to maintain the operating system and the applications running on the infrastructure.

---

## PaaS

**Platform as a Service (PaaS)** provides a managed application platform so developers can focus primarily on building and operating applications rather than managing the underlying servers.

For example, a developer can deploy a web application using **Azure App Service** without having to manage the physical server or perform routine operating-system maintenance.

### Responsibility

The cloud provider manages more of the underlying stack, while the customer focuses on the application and its data.

Depending on the service, the provider may manage:

- Physical infrastructure
- Virtualization
- Operating system
- Runtime/platform components
- Platform maintenance

The customer generally manages:

- Application code
- Application configuration
- Data
- Application-level security

### When PaaS Makes Sense

PaaS is a strong choice when:

- Developers want to concentrate on application development.
- You don't need operating-system-level control.
- Faster deployment is important.
- The application can run on the capabilities supported by the platform.
- You want the provider to handle much of the infrastructure maintenance.

### Advantages

- Less infrastructure management.
- Faster development and deployment.
- Reduced operational overhead.
- Built-in platform capabilities can simplify application hosting.
- Developers can spend more time on application functionality.

### Trade-off

You give up some infrastructure-level control in exchange for easier management and faster development.

---

## SaaS

**Software as a Service (SaaS)** is a complete software application delivered by a provider.

The customer typically consumes the application through a web browser, desktop client, or other supported interface rather than managing the underlying servers and application platform.

Examples include cloud-hosted productivity, collaboration, file-sharing, and communication applications.

### Responsibility

The provider manages most of the technology stack, including:

- Infrastructure
- Operating systems
- Application platform
- Application software
- Maintenance and updates

The customer primarily manages:

- How the application is configured and used
- Users and access permissions
- Their organizational data
- Security settings exposed by the application

### When SaaS Makes Sense

SaaS is useful when:

- You need a ready-to-use application.
- You do not want to build and maintain the application yourself.
- Minimal infrastructure management is preferred.
- A subscription-based software model meets your requirements.

### Trade-off

SaaS provides the least infrastructure management but also gives the customer the least control over the underlying technology.

---

# IaaS vs PaaS vs SaaS

A useful way to remember the models is to compare **control versus management responsibility**.

| Area | IaaS | PaaS | SaaS |
|---|---|---|---|
| Physical infrastructure | Provider | Provider | Provider |
| Virtualization | Provider | Provider | Provider |
| Operating system | Customer | Provider | Provider |
| Runtime/platform | Customer | Provider | Provider |
| Application | Customer | Customer | Provider |
| Application data | Customer | Customer | Customer |
| Infrastructure control | High | Medium | Low |
| Customer management effort | High | Medium | Low |
| Typical focus | Infrastructure + application | Application development | Using the application |

> **Rule of thumb:** More control usually means more management responsibility.

---

# Choosing the Right Model

There is no universally best cloud service model. The choice depends on how much control and operational responsibility your application requires.

### Choose IaaS when:

- You need operating-system-level control.
- You are migrating traditional server-based applications.
- You need custom infrastructure configurations.

### Choose PaaS when:

- Your primary focus is application development.
- You don't need to manage the operating system.
- You want faster deployment with less infrastructure administration.

### Choose SaaS when:

- You need a complete application.
- You want minimal infrastructure responsibility.
- Building and maintaining the application yourself does not provide enough value.

---

# Key Takeaways

1. **Cloud computing** provides computing capabilities as services instead of requiring customers to own all physical infrastructure.
2. **Public cloud** uses provider-owned infrastructure shared across customers.
3. **Private cloud** provides an environment dedicated to one organization.
4. **Hybrid cloud** connects public cloud capabilities with private or on-premises environments.
5. **IaaS** provides infrastructure with a high degree of customer control.
6. **PaaS** provides a managed application platform and reduces infrastructure management.
7. **SaaS** provides a complete application with the provider managing most of the technology stack.
8. Moving from **IaaS → PaaS → SaaS** generally means **less customer management and less infrastructure control**.
9. The right choice depends on workload requirements, required control, operational capabilities, security, compliance, and cost.

---

## Azure Perspective

For an Azure-focused learning path, these concepts map naturally to services such as:

- **IaaS:** Azure Virtual Machines
- **PaaS:** Azure App Service, Azure Functions
- **Managed data services:** Azure SQL Database, Azure Cosmos DB
- **Storage:** Azure Storage
- **Messaging:** Azure Service Bus
- **SaaS:** Microsoft 365 and other cloud-hosted software products

Understanding the distinction between **deployment models** and **service models** is an important foundation for designing Azure solutions.
