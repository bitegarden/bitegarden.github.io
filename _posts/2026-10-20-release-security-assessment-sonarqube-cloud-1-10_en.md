---
layout: post
title: Security Assessment for SonarQube Cloud 1.10, new PCI DSS reports and security reporting improvements
description: Discover downloadable PCI DSS PDF reports and new MQR reports for security standards.

permalink: release-security-assessment-sonarqube-cloud-1-10
spanish: version-security-assessment-sonarqube-cloud-1-10

cover: /img/posts/2026-10-20-release-security-assessment-sonarqube-cloud-1-10_en.png

---

At bitegarden, we continue to improve Security Assessment for SonarQube&trade; Cloud to make **code security assessment** and reporting against different security standards easier.

Security Assessment for SonarQube&trade; Cloud version 1.10 is now available. This update introduces **PCI DSS support** and improves the generation of existing security reports.

Key additions include PCI DSS PDF reports, updated OWASP and CWE reports, and several configuration and presentation improvements.

<h2>What is Security Assessment for SonarQube&trade; Cloud?</h2>

**Security Assessment for SonarQube&trade; Cloud** is a bitegarden solution that allows teams to **generate security reports based on the vulnerabilities** detected by SonarQube Cloud. It provides a structured overview of project security results, mapping them to different software security standards and frameworks.

<h2>What's new in Security Assessment for SonarQube&trade; Cloud 1.10</h2>

<h3>New PCI DSS PDF report</h3>

The main addition in version 1.10 is **support for the PCI DSS standard** (Payment Card Industry Data Security Standard) in security reports. Starting with this version, the Security Assessment CLI can generate PCI DSS reports in PDF format for SonarQube Cloud projects.

This functionality includes:

Support for **PCI DSS 4.0 and 3.2**.

Report generation in MQR (Multi-Quality Rule) mode.

**Exporting** results in PDF format.

This addition expands the options for assessing and documenting code security, particularly for teams that need to analyze their projects against PCI DSS requirements.

<h2>Improvements to OWASP Top 10 and CWE reports</h2>

Version 1.10 also revises how existing security reports are generated. Updates include:

**OWASP Top 10**: introduction of the new security report based on this reference for web application security risks.

**CWE Top 25**: use of the project reports for this classification of software weaknesses.

**CWE On the Cusp**: introduction of the project reports associated with this selection of security weaknesses.

These improvements provide updated reports for analyzing the security results of SonarQube Cloud projects.

<h2>Shared configuration and report presentation improvements</h2>

In addition to the updates related to security standards, we have introduced several improvements to report generation and presentation:

**Visual identity**: the SonarQube Cloud logo has been restored to the report header.

**Default language**: reports use the system language by default.

**ISO 5055 reports**: unsupported CWEs are no longer displayed by default.

These changes aim to provide a more consistent experience and make results easier to review.

You can try this new version by [downloading it from the bitegarden marketplace](https://marketplace.bitegarden.com/product/bitegardenSonarCloudSecurity).

---

**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_