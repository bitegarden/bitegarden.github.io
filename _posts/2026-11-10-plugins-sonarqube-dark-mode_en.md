---
layout: post
title: 5 SonarQube plugins with dark mode support
description: Discover five bitegarden plugins for SonarQube with dark mode support. See what changed in each release and download the plugins from the Marketplace.

permalink: plugins-sonarqube-dark-mode
spanish: plugins-sonarqube-modo-oscuro

cover: /img/posts/2026-11-10-plugins-sonarqube-dark-mode_en.png

---

The **bitegarden plugins for SonarQube Server** featured in this article now follow the light or dark theme selected in your account. You'll notice the change when you move from a project dashboard to a **Quality Gates board, review a security report, or open the plugin manager**. Depending on the plugin, selectors, notifications, and status icons also adapt to your theme.

Here's which release adds dark mode support for each plugin and what changes on screen. If you're **updating several plugins**, use this list to identify which views to check.

<h2>Plugins for reviewing code quality and security</h2>

<h3>Quality Gates Board version 1.1.5</h3>

Quality Gates Board brings multiple quality thresholds together on one board and shows which conditions your project meets. For example, you can check whether a branch meets both your basic requirements and the criteria for a stricter quality level. If you need to [configure multiple quality thresholds](https://www.bitegarden.com/new-product-quality-gates-board-sonarqube), the bitegarden guide shows you where to define them.

With **dark mode enabled, backgrounds, text, buttons, the branch selector, and status icons** follow the SonarQube theme.

<h3>Security Assessment version 2.36.2</h3>

Security Assessment organizes SonarQube findings into reports you can consult during a security review. If you're preparing for an audit, you can review findings grouped by standards such as OWASP ASVS or PCI DSS and generate a PDF to share with your team. The product page lists the [reports available in Security Assessment](https://www.bitegarden.com/sonarqube-security).

**Version 2.36.2 adds dark mode support to all on-screen reports**, including OWASP, CWE, CWE KEV, ASVS, CASA, PCI DSS, ISO 5055, and STIG. The theme applies to tables, charts, buttons, dropdown menus, and tooltips. The progress window shown when you download a PDF also follows the active theme.

To review the reports in dark mode, [download Security Assessment](https://marketplace.bitegarden.com/download/download-form/52) from the Marketplace.

<h3>Dependency Track version 1.1</h3>

Dependency Track lets you **view vulnerabilities in your project's dependencies directly in SonarQube**. Start with the summary of components and vulnerabilities, then review the breakdown by severity to decide which issues to investigate first. The documentation explains how to [configure the connection to Dependency Track](https://www.bitegarden.com/sonarqube-dependency-track-documentation).

Version 1.1 adapts tables, the version selector, notifications, and tooltips to dark mode. To try the updated view, [download Dependency Track 1.1](https://marketplace.bitegarden.com/download/download-form/61?selectedVersion=1.1).

<h2>Plugins for managing projects and extensions in SonarQube</h2>

<h3>Project Tag version 1.3.6 and later</h3>

Project Tag lets you **assign a tag during analysis** using a scanner property. If your pipeline already has project metadata, you can use it to tag projects by team or application and find them later in SonarQube.

Starting with version 1.3.6, **text, links, buttons, and other elements on the plugin page** follow the user's theme. Success and error messages shown when you update tags use the colors of the selected theme. Version 1.3.7 also supports both themes.

If you manage tags from this view, [download Project Tag 1.3.7](https://marketplace.bitegarden.com/download/download-form/58?selectedVersion=1.3.7).

<h3>Universal Plugin Manager (UPM) version 1.7.5</h3>

UPM lets you **install and update plugins** from the SonarQube Server administration interface. Browse the bitegarden catalog from your instance or upload a JAR file to install a custom extension.

Version 1.7.5 adapts backgrounds, buttons, notifications, links, and license icons to dark mode. To manage your extensions from SonarQube, [download Universal Plugin Manager](https://marketplace.bitegarden.com/download/download-form/59).

<h2>How to check dark mode after updating</h2>

1. Check the Marketplace listing to find the plugin version compatible with your SonarQube Server instance.
2. Install or update the plugin and select the dark theme in your SonarQube account.
3. Open the view you normally use. For example, switch branches in Quality Gates Board or open a report in Security Assessment to see how the controls adapt to the selected theme.

You can **switch back to the light theme from your account**. All five plugins follow that preference automatically.

If a screen still looks the same, first check the installed plugin version and the active theme in your account. Make sure you're viewing the plugin page within SonarQube. In Security Assessment, for example, you'll see the change when you open a report on screen or start a PDF download.

---

**<span style="color: green">bitegarden</span> team**

*Helping companies to develop better software*
