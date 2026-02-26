---
layout: post
title: How to Automate Project Tagging with Project Tag for SonarQube™
description: Automate project tagging in SonarQube with bitegarden’s Project Tag and maintain consistency in CI/CD without manual management.

permalink: automate-sonarqube-project-tags-project-tag-plugin
spanish: automatizar-etiquetas-proyectos-sonarqube-plugin-project-tag

cover: /img/posts/2026-02-10-automate-sonarqube-project-tags-project-tag-plugin_en.png
---

Have you ever tried to automate project **onboarding in SonarQube using tags**? If you work with multiple projects, you know how challenging it can be to keep everything organized manually. SonarQube allows you to manage tags within the project space, but until now, creating **new tags was only possible manually**. This is where Project Tag for SonarQube&trade; comes in, bitegarden’s plugin that simplifies this process in an automated and efficient way.

<h2>Why automate project tagging</h2>

Manual tag management becomes complex when:

- You have **hundreds of projects**.

- You want to maintain a consistent **tagging standard**.

- You need to use **project metadata during CI/CD analysis** (for example, in Jenkins).

With **Project Tag for SonarQube&trade;**, you only need to provide the tag as a command-line property, and the plugin will **automatically create and assign the tag**, preserving both system and custom tags.

<h2>Usage and configuration</h2>

**1 - Specify the tag in your analysis**

Add the following property to your SonarQube scanner:

```
-Dbitegarden.project.tag=yourtag
```

yourtag: replace it with the name of the tag you want to assign.

Make sure the characters comply with SonarQube™ rules: a-z, 0-9, '+', '-', '#', '.'.

The plugin will automatically capture this information and store it in SonarQube.
<br><br>

**2 - Run the tagging process in administration**

Once your projects have been analyzed using **the command-line property**:

Go to Administration → Configuration → Project Tag.

Run the process to **tag all projects**.

The plugin will assign the tag specified during analysis without removing existing tags. This means both system and custom tags will remain intact.
<br><br>

**3 - CI/CD integration**

If you already have project metadata available (for example, team name, project type, or client), you can use this data to automatically configure the tag **during analysis in your CI/CD tool** such as Jenkins, GitLab CI, or Azure DevOps. This ensures that each project has the correct tag as early as possible, without manual intervention.

<h3>Key benefits</h3>

Below are some of the key benefits of Project Tag for SonarQube&trade; Server:

- **Full automation**: no more manual tag creation.

- **Consistency**: all tags follow a standard defined by your analysis.

- **CI/CD metadata compatibility**: tags can be generated from dynamic pipeline properties.

- **Security and maintainability**: existing tags are not removed, only new ones are added.

With Project Tag for SonarQube&trade;, automating the tagging of your projects is straightforward. Configure your tags via the command line, integrate them with your CI/CD pipeline, and let the plugin keep your projects organized and consistent. [Here is the download link](https://marketplace.bitegarden.com/product/bitegardenProjectTag) to try it in your instance.

---

**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_