---
layout: post
title: Static Code Analysis with SonarQube
description: Investing in the quality control of projects means analyzing the code throughout the process and thereby including code reviews in workflows to maintain high quality.

permalink: static-code-analysis-with-sonarqube
spanish: analisis-estatico-del-codigo-con-sonarqube
italian: gestione-qualita-codice-con-sonarqube

cover: /img/thumbs/2020-07-13-static-code-analysis-using-sonarqube-thumb.png
---
Investing in the **quality control of projects** means analyzing the code throughout the process and thereby including code reviews in workflows to maintain high quality.

To obtain this result, it is necessary to include a static code analyzer, such as [**SonarQube&trade;**](https://www.sonarqube.org/).

![SonarQube](/img/posts/2020-07-13-static-code-analysis-using-sonarqube-logo-300x93.jpg){: .center-image}

---

## What is SonarQube&trade;?


**SonarQube&trade;** is an **open source** software that allows **static analysis** of the code and obtain metrics that 
allow you to improve the quality of the code and discover where you need to focus on.

**SonarQube&trade;** retrieves metrics from your source code and the metrics related to technical debt are based on 
[**SQALE**](https://www.bitegarden.com/sonarqube-sqale), which we could define as an algorithm that says if the quality 
expectations, that were set during the development life cycle, have been met and / or how long it will take to achieve them.

A good practice is to use **SonarQube&trade;** from the beginning of the projects precisely because it is **evolutionary** 
and analyze day by day what is happening. This tool will change the workflow - no more coding, coding, and coding, 
but coding, analyzing, and correcting. This new practice will prevent from a large technical debt and will allow you 
to improve the quality of the project.

Among the metrics you’ll find duplicate code, coverage, code smells, bugs, risk factor vulnerabilities, density of security breaches, and much more.

**SonarQube&trade;** is divided into two tools: the **server** where the compute engine that performs the analysis is located, 
stores the results and is where you can define the projects, quality parameters, analysis results, and will be in charge 
of each task. On the other side, we have **SonarQube Scanner**, the analyzer.

**SonarQube&trade;** is a multi-language tool, and is possible to analyze different codes and repositories.

Currently, the latest version is **8.4**, and it supports more than **27 programming languages**.

![Sonarqube - Lenguajes de programación](/img/posts/2020-07-13-static-code-analysis-using-sonarqube-programming-languages.jpg)

## Static or dynamic analysis of the source code

**Static analysis** of code means the process of evaluating the software without executing it, so you can get bugs, 
errors, and metrics as soon as possible.

On the other hand, **dynamic analysis** means that you have to run the software to see the behavior and the run-time. 
The issue with this approach is that you will need more tests to define if your code is working correctly or not.


## Most relevant features of SonarQube&trade;

- **Vulnerabilities**: SonarQube&trade; has a large DB of code smells and vulnerabilities giving you the details about 
the security level of the project.

- **Duplicate code**: the tool detects the duplicate code and allows you to choose to refactor or undock components.

- **Programming Standard**: lets you know if any standard has been violated and/or there are bad practices (code smells).

- **Coverage** : monitors whether test coverage is enough for quality standards and gives you a good base to define if 
is necessary to increase the investment in this area.

- **Quality profiles** : for each language, there is a default quality profile but you can also create a customized 
profile. This pack of rules will be applied during static code analysis.

As you have seen, [SonarQube&trade;](https://www.sonarqube.org/) is a very powerful tool - and also **free** and 
**open source** - that allows you to control the level quality with little efforts. And if you are in charge of many 
software projects, you’ll finally get everything under control.

The **Software Development Lifecycle** involves other roles too, not only developers, so we have created some 
[**plugins for SonarQube&trade;**](https://www.bitegarden.com/products/)  able to provide all the reporting features 
that are missing and are asked for by **Project Managers**, **Product Owners**. 

<a href="/products/" class="btn btn-primary btn-call-to-action fancybox">DISCOVER ALL PLUGINS ></a>

We are sure you will love it, so give it a try and let us know your experience.