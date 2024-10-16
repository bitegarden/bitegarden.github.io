---
layout: post
title: What is the difference between a hotspot and a vulnerability?
description: We teach you how to quickly differentiate a hotspot and a vulnerability

permalink: differences-hotspots-vulnerabilities
english: diferencias-hotspots-vulnerabilidades
italian: differencials-hotspots-vulnerabilities

cover: /img/posts/2024-10-01-differences-hotspots-vulnerabilities_en.png
---

In the field of software, security and code quality are critical aspects that must be considered at every stage of the development life cycle. 
To address these aspects, tools such as **SonarQube, SonarCloud and SonarLint** have become essential. These tools not only help identify 
problems in the code, but also classify these problems into different categories, among which stand out **hotspots and vulnerabilities**. 
Although both terms are related to software security, they represent different concepts that it is crucial to understand. In this article, we will explore the 
differences between a hotspot and a vulnerability in the context of these tools.

<h2>What is a vulnerability? </h2>

A vulnerability is a **defect** in a system that can be exploited by an attacker to **compromise the security of the software**. In simple terms, 
is a code flaw that can allow an attacker to perform unauthorized actions. For example, data theft, malicious code execution or access to 
sensitive information. In the context of SonarQube, SonarCloud and SonarLint, vulnerabilities are identified and classified based on predefined rules, many 
of which are aligned with **security standards such as OWASP**.

<br>

<img src="/img/sonarqube-report/hotspot-sonarqube.png" width="100%" alt="Ejemplo de hotspot">

<br>

<h2>What is a hotspot? </h2>

On the other hand, a hotspot is a **snippet of code** that is not necessarily vulnerable but **presents a potential risk due to its complexity**, its use of critical technologies 
or the way in which data entry is handled. Hotspots are areas of the code that require attention, as they could become vulnerable if not handled properly. 
In the Sonar ecosystem, hotspots are flagged for developers to carefully review the code and decide whether they need to be improved or not.

<br>

<img src="/img/sonarqube-report/vulnerability-sonarqube.png" width="100%" alt="Ejemplo de vulnerabilidad">

<br>


So, what are the differences between a vulnerability and a hotspot?

The clearest difference between a hotspot and a vulnerability is its nature. While a vulnerability is a **clear weakness** and present in the code, a hotspot is more of a **risk zone**. 
A hotspot could become a vulnerability if not addressed properly, but not all areas tagged as hotspots are vulnerable in themselves. 

The bitegarden plugins help you to read the list of hotspots and vulnerabilities in a fast way. Specifically, with the [Report Plugin for SonarQube](/sonarqube-report) you show this filter so that you can export a report of the analysis filtered by code smells, vulnerabilities and hotspots. 

<br>

<img src="/img/sonarqube-report/issue-type-report-plugin.png" width="100%" alt="Issue Type filtro">

<br>

So much for this article. Please feel free to contact us if you want more information. 

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_