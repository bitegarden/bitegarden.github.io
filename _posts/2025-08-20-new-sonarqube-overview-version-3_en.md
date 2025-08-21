---
layout: post
title:   New version of the Overview Report for SonarQube™ Server now available!
description: We have included support for reports in MQR Mode.

permalink: new-sonarqube-overview-version-3
spanish: nuevo-sonarqube-overview-version-3
cover: /img/posts/2025-08-20-new-sonarqube-overview-version-3_en.png
---

## Main highlights of the new version
At bitegarden we have released version 3.0 of the **Overview Report for SonarQube Server** plugin. This update includes support for reports in **MQR Mode (Multi-Quality Rule)**, opening the door to a much more complete view of project quality.

#### MQR Mode
If your instance is in MQR Mode, the plugin automatically detects it and displays the reports in that format.

<img width="100%" src="/img/sonarqube-overview/sonarqube-overview-modo-mqr.png" alt="Overview All projects MQR Mode">

*Screenshot of the Overview All Projects page with MQR Mode enabled*  
<br>

#### Standard Experience
If your instance is in Standard Experience, reports will be displayed in this mode by default.

<img width="100%" src="/img/sonarqube-overview/sonarqube-overview-modo-standar.png" alt="Overview All projects Standard Mode">

*Screenshot of the Overview All Projects page with Standard Mode enabled*  
<br>

### Option to force Standard Mode
One of the most useful new features is the ability to force Standard Mode even when your instance is configured in MQR. This option is available in the plugin settings, designed for users who prefer to keep the traditional view.

## Use cases: when to use each mode?

### When to use MQR
MQR Mode is ideal if your organization already works with advanced quality metrics and you want reports aligned with that configuration.

### When to use Standard Experience
Standard Experience is still the best option if you prefer simpler and more straightforward reports, or if your team is not yet using MQR as the default.

## How to update the Overview Report plugin
If you have the [Universal Plugin Manager for SonarQube Server™ (UPM)](//marketplace.bitegarden.com/product/bitegardenUniversalPluginManager) you just need to click the update button in your instance administration. 

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_