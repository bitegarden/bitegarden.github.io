---
layout: post
title: Available OWASP Application Security Verification Standard for SonarQube&trade!
description: Security Plugin includes support for OWASP ASVS providing a full report assessment with all the requirements inside your SonarQube&trade; instance

permalink: support-for-owasp-asvs-standard-security-plugin-for-sonarqube
spanish: soporte-para-estandar-owasp-asvs-security-plugin-para-sonarqube
italian: supporto-owasp-asvs-security-plugin-per-sonarqube

cover: /img/posts/2022-05-31-new-release-security-plugin-owasp-asvs.png
---

We have released version 2.8 of the [Security Plugin for SonarQube](sonarqube-security) that allows to know the 
fulfillment of the security standards (OWASP, CWE/SANS) and now for the first time the ability to generate a security 
assessment for [OWASP Application Security Verification Standard](https://owasp.org/www-project-application-security-verification-standard/) (**ASVS**).

<br>

<img src="/img/sonarqube-security/owasp-asvs-header.png" alt="OWASP ASVS Security Assessment Summary with Rating" width="100%">

[Check this sample project in our demo instance>](http://sonarqube.bitegarden.com/project/extension/bitegardenSecurity/asvs_report_page?id=org.owasp%3Abenchmark&qualifier=TRK)

<br>

The OWASP Application Security Verification Standard (ASVS) Project provides a basis for testing web application technical 
security controls and also provides developers with a list of requirements for secure development.

The primary aim of the **OWASP Application Security Verification Standard (ASVS)** Project is to normalize the range in 
the coverage and level of rigor available in the market when it comes to performing Web application security verification 
using a commercially-workable open standard. The standard provides a basis for testing application technical security 
controls, as well as any technical security controls in the environment, that are relied on to protect against 
vulnerabilities such as Cross-Site Scripting (XSS) and SQL injection. This standard can be used to establish a level 
of confidence in the security of Web applications.

Get the latest stable version of the ASVS (4.0.3) from the [OWASP Downloads](https://github.com/OWASP/ASVS/tree/v4.0.3#latest-stable-version---403) page.

## How To Reference ASVS Requirements 

Each requirement has an identifier in the format `<chapter>.<section>.<requirement>` where each element is a number, for example: 1.11.3.

-- The `<chapter>` value corresponds to the chapter from which the requirement comes, for example: all 1.#.# requirements are from the Architecture chapter.

-- The `<section>` value corresponds to the section within that chapter where the requirement appears, for example: all 1.11.# requirements are in the Business Logic Architecture section of the Architecture chapter.

-- The `<requirement>` value identifies the specific requirement within the chapter and section, for example: 1.11.3 which as of version 4.0.3 of this standard is:

> Verify that all high-value business logic flows, including authentication, session management and access control are thread safe and resistant to time-of-check and time-of-use race conditions.

## Using SonarQube&trade; and Security Plugin to verify compliance with OWASP ASVS

New in OWASP ASVS 4.0 is a comprehensive mapping to the Common Weakness Enumeration (CWE). CWE mapping allows tool 
manufacturers and those using vulnerability management software to match up results.

Not every item in the ASVS has an associated CWE, and as CWE has a great deal of duplication. Verification controls are not always mappable to
equivalent weaknesses, but OWASP Foundation is working hard with the CWE community on closing this gap. 

This is why you will be able to see in Security Assessment ASVS page how many requirements from OWASP ASVS are covered in your SonarQube&trade; instance.
It will depend on your SonarQube&trade; edition, since commercial editions include additional security rules.

Once you access the new ASVS page for your project you will see the Chapter summary:

<br>

<img src="/img/sonarqube-security/owasp-asvs-chapter-summary.png" alt="OWASP ASVS Security Assessment Chapter Summary" width="100%">

<br>

Our [Security Plugin for SonarQube](sonarqube-security) will show you every OWASP ASVS Chapter with the requirements passing or failing. 

We have added a OWASP ASVS Chapter rating so that you can quickly find where are the vulnerabilities with the highest impact in security. 

This rating is computed the same way as the default SonarQube&trade; security rating (it will be E if at least one blocker vulnerability is found, ...).

## Check OWASP ASVS requirements compliance

Under the chapter summary, you will find a comprehensive list with all the requirements that are failing in each section.

You will find the requirement description with the related CWE ID, as long as the issues detected in SonarQube&trade; (both vulnerabilities or security hotspots).

<br>

<img src="/img/sonarqube-security/owasp-asvs-chapter-section-requirement.png" alt="OWASP ASVS Security Assessment Requirement Details" width="100%">

<br>

## Download the new version

The Security Plugin is now available for download through the [Universal Plugin Manager](/sonarqube-upm) or directly from 
the [product download page](/sonarqube-security-trial-form).

**Get your free trial and verify your OWASP ASVS compliance today!**

<a href = "/sonarqube-security#product-block-center" class = "btn btn-primary btn-call-to-action fancybox" style = "font-weight: bold; font-size: 16px; text-transform : mayúsculas; "> Start your free trial > </a>

<br/>

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_