---
layout: post
title: 'Overview Report for SonarCloud 1.2'
description: This new version includes amazing new features to improve the information available in the report

permalink: new-release-overview-report-sonarcloud-1-2
spanish: nueva-version-overview-report-sonarcloud-1-2
italian: nuova-versione-overview-report-sonarcloud-1-2

cover: /img/posts/2022-07-27-new-release-overview-report-cloud.png
---

We have just released *[bitegarden Overview Report for SonarCloud&trade;](/sonarcloud-overview)* version 1.2.

This new version includes amazing new features to improve the information available in the report:

### Health Rating

A new ***health rating will be available in the overall section page*** (the first page), including the number of projects 
that are passing the quality gate and the projects that are failing. 

The health rating is the ratio of projects that have a Passed Quality Gate:

-- A: > 80%

-- B: > 60%

-- C: > 40%

-- D: > 20%
  
-- E: <= 20%

<br>
<img src="/img/posts/2022-07-27-overview-health-rating.png" alt="health rating" width="100%">
<br><br>

### Differential values

In the overall section now you will see a section with the **differential values for the main metrics since a given 
period**. 

There are three periods by default (since the first analysis, since six months ago, since last month), but if you prefer, 
you can set a specific date. Just add "-Dactivity.period=" to your command with the values:

-- 0 (since first analysis) Default value

-- 1 (since six months ago)

-- 2 (since last month)

-- YYYY-MM-DD (since specified date)

<br>
<img src="/img/posts/2022-07-27-overview-differential-values.png" alt="differential values" width="100%">
<br><br>

### Quality gates

Now in the project breakdown section you will be able to see for each project the quality gate status 
and a new section with the activity for the given period.

<br>
<img src="/img/posts/2022-07-27-overview-quality-gates.png" alt="quality gates" width="100%">
<br><br>

### Download the latest version

Hope that you like this new version and please, upgrade to the latest version to enjoy the new features!

You can download the new version from the [product download page](/sonarcloud-overview-trial-form).

Your feedback is really appreciated so feel free to open a ticket in 
our [customer support portal](http://support.bitegarden.com/) to help us continue adding new features 
and improve the product!

<a href = "/sonarcloud-overview-trial-form" class = "btn btn-primary btn-call-to-action fancybox" style = "font-weight: bold; font-size: 16px; text-transform : mayúsculas; "> Download > </a>

<br/>

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_