---
layout: post
title:  How to develop high-quality software with SonarQube
description: How to quantify the quality of a software and build a high quality product.

permalink: how-to-develop-high-quality-software-sonarqube
spanish: como-costruir-software-de-alta-calidad-sonarqube
cover: /img/posts/2021-05-14-how-to-develop-high-quality-software-with-sonarqube-thumb.png
---

Use a tool such as **SonarQube**, leads to higher quality and greater productivity for programmers and facilitates a sort of "standardization" of the code, a very important factor given that parts of software products are often shared between different people.

Through the static analysis of the source code, SonarQube measures the levels of reliability, maintainability, security, complexity, test coverage and duplication of code, assigning a score depending on the severity of the defects found.

When the quality of the software is kept high, it can **guarantee greater security** and makes it possible to **lower costs** during the entire life cycle of the product, **reduce maintenance time** and create value for producers, customers and financiers.

## How to quantify the quality of a software

The high quality of the software was related to:
- -- Reduction of testing and delivery times
- -- Reduction of more than 50% of repairs and modifications
- -- Increase in customer satisfaction
- -- Reduction, after release, of maintenance costs
- -- Reduction of disputes on project contracts
- -- Reduction of canceled projects
- -- Increase in reliability
- -- Reduction of security holes in released applications

## Categories of the SonarQube rules

SonarQube, to analyze the code, uses rules classified into four types: code smell, bug, vulnerability and security hotspot.

The **code smell** category includes the characteristics that indicate a programming defect but do not reveal errors and therefore do not affect the actual correctness of the software, but make the code less maintainable.

**Bugs** are errors on which unexpected or incorrect behavior of the program depends, reduce the reliability of the program.

**Vulnerabilities** are weaknesses that can be exploited to compromise the security level of the system.

**Security hotspots** are weaknesses that are not problematic, but could become vulnerabilities. Examples are bad cookie configuration, the use of non-standard cryptographic algorithms and the use of protocols that do not build secure connections.

*It is also possible to **create new rules** through the SonarQube platform, and it is possible to choose a set of rules to associate with each language.*

## Degrees of severity

During the analysis, issues are defined every time a code fragment breaks a rule. Each issue is linked to a different level of severity:
- **Blocker**: a bug that can change the behavior of the program. The code must be checked.
- **Critical**: A bug that is unlikely to change program behavior or a security flaw. The code is from to review.
- **Major**: code defects that lower developer productivity such as repeated code, unused parameters and variables
- **Minor**: Code defects that slightly reduce the productivity of developers like too long lines and switches with less than three cases.
- **Info**: This is not a real software defect, such as comments contending "TODO" or the use of deprecated constructs.

## Five status

An issue, once created, can assume five states: immediately after its creation it is **(1) open**, it becomes **(2) confirmed** when the user indicates that it is a valid problem, **(3) resolved** when the user indicates that in the next analysis should not be considered again because changes have been made, **(4) reopened** when the problem has been reported as resolved but has not really been corrected and **(5)closed** when SonarQube no longer recognizes it as a problem. A problem is closed when it has been **fixed** or because the related rule that recognizes it is no longer available, **removed**.

## Rating of the metrics

The metrics used to define code quality are complexity, duplication, maintainability, reliability, security, size and test coverage.

#### Reliability rating

- A = 0 bug
- B = at least one minor bug
- C = at least one major bug
- D = at least one critical bug
- E = at least one bug blocker

#### Safety Rating

- A = 0 vulnerability
- B = at least a minor vulnerability
- C = at least one major vulnerability
- D = at least one critical vulnerability
- E = at least one blocker vulnerability

#### Technical debt rating

It depends on the "technical debt ratio" (TD ratio) which is the ratio of the debt and the estimated development time, calculated as LOCx30min.

- A = TD ratio <= 5%
- B = TD ratio between 6 and 10%
- C = TD ratio between 10 and 20%
- D = TD ratio between 21 and 50%
- E = TD ratio> = 50%

## High quality software is cheaper to produce

If you believe in continuous integration, you cannot ignore the use of SonarQube, as it will allow you to check the code after each change, thus maintaining the quality of your software always high.

Happy coding!


---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_
