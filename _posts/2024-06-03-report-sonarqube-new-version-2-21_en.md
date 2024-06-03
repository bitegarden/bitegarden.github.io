---
layout: post
title: 'New version! Report Plugin For SonarQube 2.21'
description: New report fields and new endpoint!

permalink: report-sonarqube-new-version-2-21
spanish: report-sonarqube-nueva-version-2-21
italian: report-sonarqube-nuova-versione-2-21

cover: /img/posts/2024-04-26-bitegarden-report-new-version-2-21_ENG.png
---

We have a new version of the [Report Plugin for SonarQube](/sonarqube-report). This is **version 2.21** which brings several new features!
This version adds some new fields to the reports, as you requested. From now on, you will be able to see:

- **Lines of Code**: You can now view the total number of lines of code analyzed.
- **Download Date**: The date the report was downloaded has been added.
- **SonarQube Version**: The reports now include the version of SonarQube used for the analysis.

<br/>

## Improvement in Email Notifications

Previously, the plugin allowed configuring a list of emails to be notified after each analysis. However, this was causing issues for some clients and affecting the analysis times by adding more work to the compute engine.

#### Implemented Solution

In this version, an endpoint has been included that allows notifying the desired users by sending the list of emails. In this way, email notifications are no longer executed in the compute engine, thus improving performance and reducing the reported issues.

<img src="/img/sonarqube-report/bitegarden-report-sonarqube-email-endpoint.png" width="100%" alt="endpoint">

## Applied Patch

A small patch has been implemented to resolve the issue of email crossovers between different projects when there were more than one worker configured in the compute engine. This improvement ensures that notifications are sent correctly without mixing recipients between different projects.

#### Advice

Therefore, as we have an endpoint for this, the previous functionality has been marked as ‘deprecated’ in order to keep only the new endpoint. It will be removed in future versions.
<br />

### Download the latest version
The Report for SonarQube Plugin is now available for download via the [Universal Plugin Manager](/sonarqube-upm) or from the [product download](/sonarqube-report-trial-form) page.

Remember, if you don’t already have this plugin you can **download it and try it for free**. 
<br>

<a href = "/sonarqube-report#product-block-center" class = "btn btn-primary btn-call-to-action fancybox" style = "font-weight: bold; font-size: 16px; text -transform : uppercase; "> Start your free trial > </a>


---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_