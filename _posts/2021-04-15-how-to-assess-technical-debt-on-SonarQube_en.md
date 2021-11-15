---
layout: post
title:  How to evaluate the technical debt with Sonarqube
description: What is technical debt, how to measure and control with SonarQube.

permalink: how-to-evaluate-technical-debt-sonarqube
spanish: como-evaluar-deuda-tecnica-sonarqube
italian: come-valutare-debito-tecnico-sonarqube

cover: /img/posts/2021-04-15-how-to-evaluate-technical-debt-sonarqube-1.png
---

You may not know what we mean when we talk about **technical debt**, but surely, just by having the word “debt”, you can already imagine that it is not a good thing, and that it is something that if you don't work on it, it will affect your projects in some way.

Well, today we want to talk to you about the technical debt, how it affects your projects, and how you can avoid the problems that it would cause you.

## What is technical debt?

In the first place, we are going to see what technical debt consists of, and for this, nothing better than to compare it with a debt that you may know, economic debt.

On the occasions when you need a large amount of money (buying a home, setting up a business, etc ...) you need to ask for that amount to be loaned it to you, and later, return it in small payments over several years, as it would be difficult to have raised enough money in time to be able to face those purchases.

Well, the meaning of **technical debt** refers to when we need, in this case, an amount of time (that in our example was the money) to be able to deliver the agreed work on the agreed date.

And this happens, for example: when we **copy code** instead of creating a new class that performs the function we need, or when we **duplicate literals** instead of using constants.

In those cases, we are asking for time to deliver the code earlier, but as in the technical debt, we have to return that time. If we do not do so, we will have problems: maybe errors in the project, or in best-case scenario, investing after a great amount of hours for clean the code.

And also, another thing in which the technical debt is similar to the economic one, is that it has to be **paid with interest**. If in the financial debt, an additional amount is paid to pay for the loan, the context switch makes it take longer to solve a code smell (than if it had been done correctly from the beginning).

So, technical debt is not directly related to the reliability or security of our project, since these are errors that occurs in our code, mainly due to ignorance. It is related to **maintainability** with the ease for us to update or evolve our projects.

## How to measure technical debt

**Well, now that you know what technical debt is, how is it measured? How much technical debt do we have? Is it high or low?**

As we said at the beginning, in technical debt, what is borrowed is **time**, so what you have to give back is time. On the other hand, we have seen that it affects **maintainability**, and that is why you can see the measure in which SonarQube can help you with technical debt: when it detects a code smell, it tells you the **estimated time to solve it**.

<img src="img/posts/2021-04-15-how-to-evaluate-technical-debt-sonarqube-1.png" width="100%" alt="How to measure the technical debt with SonarQube">

## Level of the technical debt

It is important to be aware that this estimated time depends largely on the experience of the developer, and can also be affected by the particularities of the project, organization or even its infrastructure. So, although it is not exact information, it can serve as a first approximation.

But, on the other hand, knowing the time that we "owe" is not enough to know the level of technical debt of the project.

It is not the same that a person owes € 5,000 on a loan to buy a car that costs € 10,000, than an organization owes € 5,000 on a loan to buy offices that cost € 500,000.

In the first case, the debt is half of the asset (the car) and in some cases, if there is an unforeseen event (for example, that the indebted person is unemployed), the outstanding debt would be a problem. While in the second case, the debt is practically paid and should not cause any setbacks to the organization.

That is why the **technical debt must be related to the total development time of the project** (which would be equivalent to the total price of the good), and in this way it is also shown as a percentage.

Therefore, when we talk about a technical debt of 10%, it means that, if the project has been developed in about 1,000 hours, the time to correct the evidences related to maintainability (code smells) is approximately 100 hours.

## Control technical debt on SonarQube

SonarQube considers the monitoring of technical debt of great importance.

So much so that it uses it as one of its three main indicators which, as you may already know, are: reliability, security and maintainability.

## Technical debt in the global maintainability rating

<img src="img/posts/2021-04-15-how-to-evaluate-technical-debt-sonarqube-2.png" width="100%" alt="Global maintainability rating with SonarQube">

And in the case of the global maintainability rating, SonarQube will show the result based on the technical debt obtained.

Overall ratings range from A (best rating) to E (worst rating), and on maintainability, SonarQube can show the following results:

- A: Technical debt is less than 5%
- B: Technical debt is between 6% and 10%
 - C: Technical debt is between 11% and 20%
 - D: Technical debt is between 21% and 50%
 - E: Technical debt is greater than 50%

## Time required to resolve technical debt

On the other hand, SonarQube shows the total time of all code smells in the project.

Thus, in the previous image, you can see that in the new code (last 30 days) there is 1 code smell, whose approximate solution time is 30 minutes, so the technical debt of the new code will be that time: 30 minutes.

While in the complete project, there are more than 6,900 code smells, and the total time to solve them will be approximately 164 days.

Keep in mind that Sonarqube stores technical debt in minutes, but it can show it in hours or days (1 day = 8 hours of work).

## Technical debt monitoring

To track technical debt in SonarQube, we have different options.

In the **Measurements Section**, you can see the technical debt in overall code, or only in the new code.

<img src="img/posts/2021-04-15-how-to-evaluate-technical-debt-sonarqube-3.png" width="100%" alt="Technical debt monitoring with SonarQube">

While in the **Activity Section**, we can see the history of the result of the technical debt throughout the life of the project.

<img src="img/posts/2021-04-15-how-to-evaluate-technical-debt-sonarqube-4.png" width="100%" alt="Technical debt monitoring with SonarQube">

In this way, you can see the evolution of your technical debt although as we have said before, only in days.

If you really want to see what it means for the project, you should check the **technical debt ratio**, to see better the evolution, regardless of whether the project has grown in number of lines.

<img src="img/posts/2021-04-15-how-to-evaluate-technical-debt-sonarqube-5.png" width="100%" alt="Technical debt monitoringwith SonarQube">

And with this, you have been able to see what technical debt is, and how, thanks to SonarQube, you can keep it under control. 

So, try not to borrow too much, that in the future you will have to pay it ... and with interest! 😉


And if you need more, we have created some **Plugins for SonarQube** that improve your entire ecosystem of code quality.
<br>
<br>
<a href="/products" class="btn btn-primary btn-call-to-action fancybox" style="font-weight:bold;font-size:15px; text-transform: uppercase;">GIVE A LOOK TO THE PLUGINS FOR SONARQUBE> </a>
<br>
<br/>

Happy coding!

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_
