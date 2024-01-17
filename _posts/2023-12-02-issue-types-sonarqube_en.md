---
layout: post
title: 'Types of issues in SonarQube'
description: We explain what is a bug, a vulnerability and a code smell

permalink: issue-types-sonarqube
spanish: tipos-issue-sonarqube
italian: tipo-di-issue-sonarqube

cover: /img/posts/2023-12-02-issue-types-sonarqube_en.png 
---

SonarQube is an **essential tool** for software development because it offers a detailed view of code quality. One of the most outstanding features of SonarQube is its ability to identify and classify problems in the code through issues. In this article, we will explain the different types of issues that SonarQube can detect, highlighting their importance and how to address them to improve software quality.

<h2>What types of issues are there in SonarQube?</h2>

<h3>Bugs</h3>

Bugs are a **code error** that can produce an unexpected failure during code execution. In the following image we can see an example of a bug. SonarQube classifies it as such, indicates where it is and also why it qualifies as an issue. 

<img src="/img/posts/bug-example.png" width="100%" alt="Bug example in SonarQube">

<h3>Vulnerability</h3>

A vulnerability is a **point in the code** that is exposed, vulnerable to external attacks. In the following image we can see an example of a vulnerability that SonarQube has detected when considering that a password may be exposed. 

<img src="/img/posts/vulnerability-example.png" width="100%" alt="Vulenrability example in SonarQube">


<h3>Code Smells</h3>

A code smell is a problem that makes the **code difficult to understand**. In the following image we can see an example of code smell in which SonarQube suggests removing a parameter that is not used. 

<img src="/img/posts/code-smell-example.png" width="100%" alt="Code Smells example in SonarQube">

Remember in the last release of **SonarQube 10.3**, Sonar announced that these types of issues **are obsolete**. So in new updates problems will now be enhanced with Clean Code attributes and affected software qualities. 

If you need  more information, you can contact with us via [this form](https://www.bitegarden.com/contact/)


---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_