---
layout: post
title: How to measure the code quality of a provider
description: Check goals and metrics when working with an external partner

permalink: how-to-measure-code-quality-suppliers
spanish: como-medir-calidad-de-codigo-proveedores
cover: /img/thumbs/2021-07-20-how-to-measure-the-code-quality-suppliers-thumb.png
---

To ensure achievement and verification of objectives when working with an external partner, it is necessary to pay attention to the quality and robustness of the source code that is delivered.

To identify metrics that provide reasonable assurance that the application is free of security issues and they have adopted the best practices, the use of analytics software is required.


## SonarQube the tool to measure code quality

[**SonarQube**](https://www.sonarqube.org/) is an open source software platform widely known in the developer community, robust and organized with add-ons to enrich its analysis capabilities.

Installation is very fast and can be based on docker containers, also hosted on cloud services such as Microsoft's Azure. If you need to respect the confidentiality of the source code, it is better to discard the SonarSource cloud service (SonarCloud).


## SonarQube features

It is a platform capable of verifying the quality of the source code, performing analysis of errors, suspicious code and security vulnerabilities in more than twenty programming languages.

All the analyzes used by Sonarqube are defined as [**static**](/static-code-analysis-with-sonarqube) (it doesn't require the execution of the program).

Its adoption, during the software development cycle, allows:

-- Improve component development and testing processes

-- Identify possible quality problems in development, before the software goes into production

-- Detect areas that require refactoring or simplification

-- Identify programming errors or defects

-- Increase development team communication and encourage developers to produce high-quality code


In addition, it integrates perfectly with the **Continuous Integration** practice (the creation of a source code baseline that contains all the work carried out by the team, several times a day), adding the information on the quality achieved.

## How it works

The [reports created by Sonarqube](/sonarqube-report) are collected on its platform and can be consulted by each member of the team. These are also automatically assigned to the developer who introduced the possible criticality (using the information from the commits extracted from the source code versioning system) and he is notified by email to notify him of the need for acknowledgment and resolution.
The adoption of continuous integration allows:

-- Confirm, several times a day, the robustness of the application by executing all the tests in an environment external to that of the developers.

-- Always have the latest version of the application ready, free of compilation errors and with all the tests passed (**Continuous Delivery**).

It is also possible to monitor the **[technical debt](/how-to-evaluate-technical-debt-sonarqube) accumulated**. The **[technical debt](/how-to-evaluate-technical-debt-sonarqube)** refers to the empirical time required to resolve the Sonarqube reports. Typically this does not require entering a specific task to resolve alerts.

Thanks to its simplicity, the team quickly learns how to navigate within the Sonarqube panel and limits the points to analyze or order them by different priorities.

## Benefits of SonarQube

- -Adoption is very fast and requires few operations and changes in equipment operations.

-- Have a single standard shared by the entire team through centralized rules

-- Detection of preventive errors (for example: parts of code never reached, test conditions always true, possible null pointers, ...) even before having written the UnitTests

-- Identification of possible security problems, thanks to the possibility of using public vulnerability databases (CWE, Sans, OWASP)

-- Reduction of code review time. The most experienced team members are consulted only on really complex problems and not on known and already documented best practices

-- Clear dashboard with progress measurement throughout the project development.

**SonarQube** is the perfect tool to measure the quality of the work done (both internally and by suppliers).


<hr>

### Plugins for SonarQube

If you want to manage or download the SonarQube reports, try our [**Plugins for SonarQube for free**](/products), they will give you the extra help you are looking for.

<a href="downloads" class="btn btn-primary btn-call-to-action fancybox" style="font-weight:bold;font-size:16px; text-transform: uppercase;"> Find out more </a>

<br>

<br>


---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_
