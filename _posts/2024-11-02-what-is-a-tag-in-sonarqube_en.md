---
layout: post
title: Tags in SonarQube, use and utilities in projects
description: Learn how to use tags in SonarQube and how our products can help you improve your management

permalink: what-is-a-tag-in-sonarqube
spanish: que-es-un-tag-en-sonarqube

cover: /img/posts/2024-11-02-what-is-a-tag-in-sonarqube_EN.png
---

SonarQube **tags** are a very useful tool to manage and find your organization’s projects. So in this article we will explain how you can use them and how you can extend their functionalities thanks to the products of bitegarden. 

<h2>What is a tag on SonarQube? </h2>

**Tags in SonarQube** are "labels" that are added to projects and allow them to be categorized for easy administration. Tags can be managed through the 'Project Information' tab in the left sidebar. The 'tags' section shows the tags configured for that project and the option to add more. 

In this image you can see an example of their location: 

<img src="/img/sonarqube-project-tag/tags-project-sonarqube.png" alt="Tags in SonarQube" width="100%" />
<br/>
<br/>


<h2>How to add tags to a SonarQube project? </h2>

In this same tab, by clicking on the '+' button you can **add more tags or create new ones** if they are not already created. It is a simple and intuitive way to classify projects and then find them according to the criteria you want. 

However, when the user wants to create tags when there are many projects, he is faced with a problem. The action of creating and assigning labels is completely manual, but at bitegarden we have **two products** that can help you during the management and configuration of labels. 

With **Project Tag for SonarQube**, you can configure and tag projects automatically. With the **Control Center for SonarQube** you can assign labels to projects in bulk. Let’s step by step learning how to perform these actions. 

<h2>How to automate the configuration of tags in SonarQube? </h2>

Here’s a step-by-step guide **how you can automate** the creation of labels in SonarQube: 

1 - Write the tag through the property "-Dbitegarden.project.tag=YOUR_TAG" in any of your scanners and the plugin will capture the information and save it to SonarQube.
<br>

2 - Once your projects have been parsed using the property, you can launch the process that will tag the projects. In particular, you have to go to Administration -> Configuration -> Project Tag and click on the button 'Update project tags'.
<br>

<img src="/img/sonarqube-project-tag/project-tag-administration.png" alt="Tags in SonarQube" width="90%"/>


If you want to test this plugin on your instance, you can download it through [this link](/sonarqube-project-tag#product-block-center)


<h2>How to tag projects in bulk on SonarQube? </h2>

If your goal is to tag projects in bulk you should follow the following steps on SonarQube: 

1 - Go to Administration -> Configuration -> Control Center - Project Management

2 - On the screen you will see all projects. This is when you select which projects you want to tag.

3 - Press the Bulk Actions -> Bulk Apply Tags button and select the tags you want to add to the selected projects.

<img src="/img/sonarqube-control-center\control-center-add-tags.png" alt="Tags in Control Center for SonarQube" width="90%"/>


If you want to test this plugin on your instance, you can download it through [this link](/sonarqube-control-center)

If you have any questions or want to learn more about our products, please contact our team. 

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_