---
layout: post
title: How to create a PDF report for SonarQube's Multi Quality Rule (MQR) Mode
description: Generate PDF reports in SonarQube with the Overview Report and the new MQR mode.

permalink: how-to-create-sonarqube-overview-mqr
spanish: como-exportar-informe-sonarqube-overview-mqr


cover: /img/posts/2025-12-09-how-to-create-sonarqube-overview-mqr_en.png
---

SonarQube is an essential tool for code quality analysis. With [version 3.0](/new-sonarqube-overview-version-3) of the **Overview Report Plugin for SonarQube&trade; Server**, you can now generate PDF reports compatible with the **Multi Quality Rule (MQR)** mode, providing a more comprehensive view of your projects’ quality.

<h2>What is the Overview Report for SonarQube Server?</h2>

The **Overview Report Plugin for SonarQube™ Server** helps provide an aggregated view of project metrics. With this plugin, you can group different projects, gaining a clearer perspective on the software quality status across your organization.

This plugin offers a **dedicated and navigable interface** for different project groupings: grouping the entire instance, by custom groups defined in the configuration, or using project tags.

<h2>What is the Multi Quality Rule (MQR) mode?</h2>

SonarQube’s MQR mode provides a more accurate way to **represent the impact of an issue** on all software qualities, assigning an independent severity to each rule according to each quality it affects. This allows you to:

- Clearly see the impact of each issue on all software qualities, not just the most affected one. <br>

- Evaluate quality issues in a more complete and objective way. <br>

<h2>What does each severity level mean?</h2>

- **Blocker**: Issue with a high probability of severe consequences for the application that must be fixed immediately (includes bugs causing production failures or critical security vulnerabilities). <br>

- **High**: Issue with high impact that should be resolved as soon as possible. <br>

- **Medium**: Issue with medium impact. <br>

- **Low**: Issue with low impact. <br>

- **Info**: Issue with no expected impact; for informational purposes only.

<h2>How to generate a PDF report from SonarQube</h2>

To download your report, follow these steps:

Check if MQR mode is enabled. <br>

1. [Install](/sonarqube-overview-trial-form.html) the Overview Report Plugin for SonarQube™ Server. <br>

2. Log in to your SonarQube instance. Go to the main menu and click on More. If the plugin is installed correctly, you will see different Overview tabs. <br>

3. Click, for example, on Overview All Projects and select Download PDF. <br>

Here’s an example of the PDF you can generate:

<img width="100%" src="/img/sonarqube-overview/sonarqube-overview-modo-mqr-pdf.png" alt="Example PDF in SonarQube MQR Mode with the Overview Report for SonarQube"> <br><br>

The **Overview Report Plugin for SonarQube™ Server**, combined with MQR mode, allows you to generate PDF reports that accurately reflect the **impact of issues across all software qualities**. This makes decision-making easier, improves **project status communication**, and supports continuous improvement in your software quality.

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_