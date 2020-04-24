---
layout: post
title: How to detect vulnerabilities in your code
description: These last weeks have been challenging, we've all changed our habits as well as the companies. Remote work is here to stay and, probably even after the emergency. 

permalink: how-to-detect-vulnerabilities-in-your-code
spanish: como-detectar-vulnerabilidades-en-el-codigo
---

SonarQube™ has become the most powerful continuous inspection and static analysis tool.

For a couple of years, the development team has focused on improving all those analysis characteristics 
associated with vulnerability detection and security standards, including OWASP, SNAS, CWE, ... 
Now we can say that SonarQube™ is a SAST tool (Static Application Security Testing) .

In addition, if we extend the tool with other Open Source components such as [OWASP Dependency Check](https://owasp.org/www-project-dependency-check/), or 
with our [security plugin](/sonarqube-security), we will further increase its capacity through Software Composition Analysis (SCA) 
or by checking your code against Security Standards (OWASP Compliance). You can also extend the set of security rules 
available through third-party tools like [Find Security Bugs](https://find-sec-bugs.github.io) using the [sonar-findbugs](https://github.com/spotbugs/sonar-findbugs) plugin.

But beyond all this, how do we detect vulnerabilities in the code with SonarQube™?

## **Security issues:** Hotspots vs Vulnerabilities

The SonarQube™ Quality Model has two different types of rules for security.

**Security Hotspots** have been introduced for security protections that have no direct impact on the overall application's 
security. Most injection rules are vulnerabilities, for example, if a SQL injection is found, it is certain that a fix 
(input validation) is required, so this is a vulnerability. On the contrary, the httpOnly flag when creating a cookie 
is an additional protection desired (to reduce the impact when XSS vulnerabilities appear) but not always possible 
to implement or relevant depending on the context of the application, so it's a hotspot.

The main difference between a hotspot and a vulnerability is the need of a review before deciding whether to apply a fix:

![Hotspots vs vulnerabilities](/img/posts/hotspots-vulnerabilities.png){:width="100%" .center-image}

-- With a **Hotspot**, a security-sensitive piece of code is highlighted, but the overall application security may not be 
impacted. It's up to the developer to review the code to determine whether or not a fix is needed to secure the code.

-- With a **vulnerability**, a problem that impacts the application's security has been discovered that needs to be 
fixed immediately.

## **Step 1.** Activate security rules

If you want to do a first review of the security of your code, the first thing will be to setup your quality 
profile to detect as many problems as possible.

This is the default quality profile:

![Default rules](/img/posts/default-security-rules.png){:width="300px" .center-image}

There are 45 **vulnerability** rules and another 31 **security hotspots** rules.

But you can still activate almost 20 more rules associated with security. The default profile is usually sufficient but if
you want to try all activated, go ahead.


---
> **Tips and tricks:** some bug rules and code smells are also categorized into security standards. Find them and 
>activate them to improve the security analysis of your code.
>
>Here is an example of a bug rule that affects the OWASP standard (category A6):

![Bug que afecta a seguridad](/img/posts/bug-security-rule.png){:width="100%" .center-image}

> That is why it is so important that you check not only vulnerability and hotspot rules, but also go a little further, 
> since some bugs or code smells may also be related to future security problems.

---

## **Step 2.** Review your security rating

After analyzing your project, you can see your security rating on the main page:

![security rating](/img/posts/overall-security-rating.png){:width="100%" .center-image}

There is ratings for both vulnerabilities and hotspots.

-- In the case of vulnerabilities, it is calculated taking into account the severity of the detected vulnerabilities.

-- In the case of hotspots, it is calculated according to the number of hotspots that are pending review.

From here you can start to fix your code security  by browsing all the issues
detected. This is easy for a developer, but what about a security champion or manager who is not going to change the 
code? In that case the information that interests you is an executive summary.

## **Step 3.** Review your security standards compliance

In addition to the overall security rating, if you have installed [bitegarden Security](/sonarqube-security) you can also 
check compliance with standards in a dedicated section within the project. It includes some additional security metrics too.

This new section is more "friendly" than browsing all the issues and allows you to analyze the security of your code from 
a less technical point of view:

![compliance report](/img/posts/bitegarden-security-owasp-page.png){:width="60%" .center-image}

With this information you can review which security aspects are better or worse in your project.
Here you can decide which code vulnerabilities to resolve first based on categories and severity.

For example, you might be more interested in starting to solve security injection issues rather than configuration issues.

## **Step 4.** Export security information to PDF

Finally, if you need to publish the information or send it to other people outside your team, you can export all the 
information in PDF that everyone can see how secure is your code:

![owasp-report-page-1](/img/posts/owasp-report-page-1.png){:width="45%"} ![owasp-report-page-2](/img/posts/owasp-report-page-2.png){:width="45%"}

---

## Conclusion

SonarQube™ has improved its security engine and now the tool is playing in the Champions League the same way as
 other SAST tools. You can now tackle security issues with a sensible pattern led by the development team:

1. Activating the rules that detect vulnerabilities and hotspots
2. Reviewing the overall security rating of your project
3. Reviewing compliance with security standards
4. Sharing information with other teams through PDF reports

Try [bitegarden Security](/sonarqube-security) to improve the way you detect and fix vulnerabilities in your code:

<a href="/es/sonarqube-security-trial-form" class="btn btn-primary btn-call-to-action fancybox">DOWNLOAD NOW ></a>

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_