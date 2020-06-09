---
layout: post
title: What is a code smell and common mistakes
description: A code smell, also known as bad smell, in computer programming code, refers to any symptom in the source code of a program that possibly indicates a deeper problem 
cover: /img/posts/2020-05-08-what_is_code_smell_and_commons_mistakes.png

permalink: what-is-code-smell-and-common-mistakes
spanish: que-es-un-code-smell-y-errores-comunes
---


Jumping into the middle of an ongoing project is not always easy, could happen to find kind of annotations inside the code. If you're lucky, something like:  
  
`//TO DO` or `//FIX ME`  
  
These texts are not adding functionality but underline a potential bad implementation or something to check. The real problem, with this kind of code smell, is that you have to search for them and not always is an easy job because each developer has his “method” to mark it.  
  
![what is a code smell - bitegarden](/img/posts/2020-05-08-what_is_code_smell_and_commons_mistakes.png){:width="100%" .center-image}


## What’s a code smell?  
  
>“A code smell, also known as bad smell, in computer programming code, refers to any symptom in the source code of a program that possibly indicates a deeper problem. (...)  
>
>Code smells are usually not bugs — they are not technically incorrect and do not currently prevent the program from functioning.  
>  
>Instead, they indicate weaknesses in design that may be slowing down development or increasing the risk of bugs or failures in the future. Bad code smells can be an indicator of factors that contribute to technical debt."  
>  
>**Source**: [*Wikipedia*](https://en.wikipedia.org/wiki/Code_smell)  
  
## The most common code smells  
  
-- **Bloaters** are parts of code (classes, methods, ...) that have increased disproportionately and has become hard to work with and are doing too many things instead of having one clear responsibility. It can become a huge problem especially if nobody cares about its removal.  
  
-- **Duplicated code**. Could happen when a developer to meet deadlines (or just because is too lazy) copy and paste parts of code, instead of creating something ad hoc. Or when more programmers are working on the development of the same program. In the future, this will translate in a strong effort, because it means a change in more than one place or, worst, if one of them is forgotten will work differently.  
  
-- **Lazy classes**, as you know, maintain the classes cost money and time, so if a class was built only to anticipate futures features and is not doing much in the current situation should be deleted.  
  
Unfortunately, often these elements are not easy to fix and need a big effort or an important change of the code.  
  
## How to avoid code smells  
  
[SonarQube](https://www.sonarqube.org/) is an amazing tool to monitor the health of your code and to help to improve the review of these code smells.  
  
A good practice, for you and your team, is to start doing a continuous analysis of the code, in order to have continuous contributions to fix code smells and vulnerabilities instead of creating specific new processes to resolve it.  
  
And if you are already using SonarQube and are looking for a tool to put your technical debt under control, let’s try [SQALE Plugin](https://www.bitegarden.com/sonarqube-sqale) that is listed as an [official SQALE tool](http://www.sqale.org/tools) to manage the technical debt.
