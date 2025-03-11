---
layout: post
title: What is a Quality Gate in SonarQube?
description: We teach you to use the Quality Gates to guarantee the security and quality of your code

permalink: what-is-quality-gate-sonarqube
spanish: que-es-un-quality-gate-sonarqube


cover: /img/posts/2025-03-02-what-is-quality-gate-sonarqube_en.png
---

SonarQube is a key tool for analyzing code. It consists of a series of **mechanisms that help developers to ensure the quality and security of code**. One of them, are the Quality Gates and in this article we will explain what they are and how you can configure them on an instance of SonarQube Server.

<h2>What is a Quality Gate? </h2>

A Quality Gate is a **mechanism** that measure whether a project meets certain quality standards. The user defines a set of conditions to be able to measure projects and answer the following question: **Is my project ready for launch?**. Examples of these conditions are: no issues and code coverage cannot exceed 40%. 

¡Atention! **Not all projects use the same Quality Gates**. Why? It is not practical for all projects. For example, a web project does not need the same code coverage as a Java project. 

For this, the user can define several Quality Gates. Below we show you how to create one. 

<h2>How to define a Quality Gate in SonarQube? </h2>

To set up a Quality Gate on SonarQube Server you must follow these steps: 

1 - **Access your SonarQube instance** . <br>
2 - In the **top menu** access Quality Gates. <br>
3 - Press the **Create** button and a screen will pop up for you to **add a name** to the Quality Gate. <br>
4 - By default, in the **Conditions** section there is already a listing for you to **edit values** (issues, security hotspots reviewed, coverage, % duplicate lines)
5 - If you want to **add more conditions**, you have to press the button **Unlock** and then the one of **Add conditions**. 

Once you have your Quality Gate created you can **set it as default**.

<h2>Benefits of using a Quality Gate</h2>

Here are some of the benefits of using Quality Gates to correct your projects: 

- Ensures the quality of code

- Gives visibility to the quality process

- Keeps the code safe

- Encourages the use of good practice

- Increases confidence on code development

SonarQube has specific information on the [Quality Gates in its documentation](https://docs.sonarsource.com/sonarqube-server/10.8/instance-administration/analysis-functions/quality-gates/){:target="_blank"}

<h3>Use the Quality Gates Board for SonarQube</h3>

At **bitegarden** we have developed a plugin so that you can validate your code against **more than one quality threshold**. We are talking about **Quality Gates Board for SonarQube**, which adds a page within the project so you can validate if your code meets more than one quality threshold.

On this new page you will be able to **customize the title of the quality thresholds** so that it is easier to read the analysis of the information. Below, we leave you an example of this page within a SonarQube Server project: 

<img width="100%" src="/img/sonarqube-quality-gates-board/quality-gates-board-2.png" alt="quality gates board with passed failed conditions">


If you want to test this plugin on your instance, you can download it via [this link](/sonarqube-quality-gates-board-trial-form). 

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_
