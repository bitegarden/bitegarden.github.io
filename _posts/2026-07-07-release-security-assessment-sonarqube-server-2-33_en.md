---
layout: post
title: Security Assessment for SonarQube Server 2.33
description: Added support for STIG ASD security standard analysis, along with the ability to export its assessment as a PDF report.

permalink: release-security-assessment-sonarqube-server-2-33
spanish: version-security-assessment-sonarqube-server-2-33

cover: /img/posts/2026-07-07-release-security-assessment-sonarqube-server-2-33_en.png

---

New release of **Security Assessment for SonarQube&trade; Server**! Version 2.33 introduces a **new security standard and performance improvements** that reduce the time required to generate selected reports.

The new standard is **STIG ASD** (Application Security and Development Security Technical Implementation Guide), developed by DISA (U.S. Department of Defense). This framework defines security requirements for **software development** to help protect data and reduce the risk of cyberattacks.

<img width="100%" src="/img/sonarqube-security/security-assessment-sonarqube-server-stig-asd.png" alt="Report STIG in SonarQube">
<br><br>

This addition also includes the option to download the report as a PDF:
<br>

<img width="80%" src="/img/sonarqube-security/security-assessment-sonarqube-server-stig-asd-pdf.png" alt="STIG PDF Report">
<br><br>

Starting with this release, you can assess your code against **STIG ASD**, which is now available alongside the **existing security standards**: OWASP Top 10, OWASP ASVS, CWE Top 25, CWE On the Cusp, CWE/KEV, and ISO 5055.


<h2>How do I update to the new version?</h2>

If you are using the [Universal Plugin Manager for SonarQube&trade; Server (UPM)](https://marketplace.bitegarden.com/product/bitegardenUniversalPluginManager) open the plugin manager and install the available update. If you haven't tried [bitegarden Security Assessment for SonarQube&trade; Server](https://marketplace.bitegarden.com/product/bitegardenSecurity) yet, you can download it and try it on your SonarQube instance for free.

---

**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_