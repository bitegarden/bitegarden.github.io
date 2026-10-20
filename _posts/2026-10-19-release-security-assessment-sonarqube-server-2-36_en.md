---
layout: post
title: Security Assessment for SonarQube 2.36, new PCI DSS PDF reports and MQR improvements
description: Discover downloadable PCI DSS PDF reports and new MQR reports for security standards.

permalink: release-security-assessment-sonarqube-server-2-36
spanish: version-security-assessment-sonarqube-server-2-36

cover: /img/posts/2026-10-19-release-security-assessment-sonarqube-server-2-36_en.png

---

At **bitegarden**, we continue to improve **Security Assessment for SonarQube&trade; Server** to make vulnerability analysis and code security assessment easier. That is why we are releasing version 2.36 of Security Assessment for SonarQube Server, an update that introduces **downloadable PCI DSS reports** in PDF format and expands MQR reporting support for various security standards.

<h2>What is Security Assessment for SonarQube?</h2>

Security Assessment for SonarQube is a bitegarden plugin for **SonarQube Server** that consolidates the vulnerabilities detected by SonarQube into a comprehensive security assessment. It provides a detailed, visual overview of each project's security compliance level, making it easier to interpret results and analyze vulnerabilities against different security standards.

This allows teams to **review their code security information** in a more structured and understandable way and **export their results as comprehensive PDF reports**.

<h2>What's new in Security Assessment for SonarQube 2.36</h2>

<h3>Download PCI DSS reports in PDF format</h3>

One of the main additions in version 2.36 is the ability to download **PCI DSS reports** in PDF format in the commercial editions of SonarQube Server.

<img width="100%" src="/img/sonarqube-security/security-assessment-sonarqube-server-pcid-download-PDF.png" alt="Ejemplo de PDF extraido de SonarQube">
<br><br>

This functionality is available for the following SonarQube Server elements:

**Projects**: get the PCI DSS report for a project.

**Applications**: download the report for an application.

**Portfolios**: generate a PDF document for a portfolio.

Reports can be downloaded in both Standard mode and MQR (Multi-Quality Rule) mode.


<h3>New MQR reports for security standards</h3>

Version 2.36 also expands security assessment capabilities by adding MQR reports for four standards:

- **CWE On the Cusp**: a new MQR report for analyzing results related to this selection of security weaknesses.

- **OWASP Top 10**: an MQR report for this widely recognized standard covering web application security risks.

- **OWASP ASVS**: a new MQR report for the OWASP Application Security Verification Standard.

- **ISO 5055**: an MQR report for this standard related to measuring the structural quality of software.


<h2>Improvements to the CASA page</h2>

In addition to the new reports, we have improved the CASA page interface. The **branch and pull request selectors** now include tooltips that provide contextual information about these elements.


<h2>How to update to the new version</h2>

If you already use the [Universal Plugin Manager](https://marketplace.bitegarden.com/product/bitegardenUniversalPluginManager), simply open the plugin's administration page and click the available update button. If you have not tried **bitegarden Security Assessment for SonarQube&trade; Server** yet, you can download it and install it on your instance using [this link](https://marketplace.bitegarden.com/product/bitegardenSecurity).


---

**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_