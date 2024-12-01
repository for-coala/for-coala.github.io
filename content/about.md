+++
title = "About"
description = "Building formally verified IaC languages!"
date = "2024-10-05"
aliases = ["about-us", "about-hugo", "contact"]
author = "Hélène Coullon and Frédéric Loulergue"
+++

## Context 

Large distributed software systems (applications or infrastructures) are now ubiquitous, with component-based systems (e.g., service-oriented architectures or microservices) offering a convenient way to structure large systems, in particular distributed systems deployed in the Cloud, in the core, or at the edge of the network. Indeed, isolating functionalities in components and building systems through composition greatly enhances the adaptability and scalability of systems, two important requirements for many organizations.

However, the advantages of distributed architectures come at the price of increased complexity and technical challenges related to observability, coordination, maintenance, etc. A set of operations denoted as DevOps --- i.e. operations handled somewhere in between the developer and the machine administrator -- includes notably the system configurations and reconfigurations that are required to achieve adaptability. These operations include the initial and dynamic changes that may occur on a distributed service-oriented software architecture: adding or removing services, connecting or disconnecting services, and changing some parameters or the internal behavior of services. They may be required to handle various kinds of dynamic scenarios such as fault tolerance, scalability, software updates, various optimizations, etc.

![image](../for-coala-ex8.png)

Such changes may lead to faults. 

- [https://blog.cloudflare.com/cloudflare-outage-on-july-17-2020/](https://blog.cloudflare.com/cloudflare-outage-on-july-17-2020/)
- [https://engineering.fb.com/2021/10/05/networking-traffic/outage-details/](https://engineering.fb.com/2021/10/05/networking-traffic/outage-details/)

## Motivation

On the one hand, many configuration tools and languages exist in the DevOps community, some of them being specific to the provisioning of resources in Cloud providers, packaging problems, containerized deployments, configuration management of applications or infrastructures, etc. Such languages are often referred to as \emph{Infrastructure-as-Code} (IaC for short). IaC languages offer easier constructs than low-level scripts to facilitate software engineering properties such as composition and reuse. The main advantage of these tools is their full integration and adoption in the DevOps community. Their disadvantage is they lack both formal and textual specifications. Moreover, their contours are blurred. On the other hand, many initiatives have been studied in academia to contribute to the deployment, configuration, and reconfiguration of distributed software~\cite{CHL2023:CSUR}, bringing improvements such as expressivity, speed, safety, etc. Many come with precise and sometimes formal definitions. However, they lack the breadth of the mainstream DevOps tools. 

## Research problem and project objectives

The goal of For-CoaLa is twofold: (1) understand and bridge the gap between a popular tool from the DevOps community and a tool from academia; (2) improve the understanding of these languages based on mechanized formal semantics and develop verified semantic-preserving cross-language transformations. The outcomes of the project will be two open source formally certified configuration languages, their execution engine, and a verified translation tool.

- From academia we choose `Concerto`
- From the industry tool perspective, we chose [`Ansible`](https://www.ansible.com). 

`Ansible` is currently one of the most widely used tools, probably because of its very wide spectrum (from low-level scripting to high-level modular and compositional features) and low requirements for installation (it is agentless unlike \puppet, another popular tool). Second, an extensive set of `Ansible` playbooks (i.e. `Ansible` programs) and roles (i.e., a set of programs to configure a given application or system) are publicly available online and can be leveraged in \projectname. Third, `Concerto` and `Ansible` have already been compared and share common aspects that will facilitate a cross-language transformation. The research challenge is to identify and formalize the subset of `Ansible`, so that it is sufficiently powerful to answer the needs of companies while keeping the formalization tasks doable within the For-CoaLa project's timeframe. 

![image](../for-coala-full.png)