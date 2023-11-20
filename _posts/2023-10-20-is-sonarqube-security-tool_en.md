---
layout: post
title: 'Is SonarQube a security tool?'
description: We explain why with SonarQube you will deliver secure code safely. 

permalink: is-sonarQube-security-tool
spanish: sonarqube-herramienta-segura 
italian: sonarqube-uno-strumento-sicuro

cover: /img/posts/2023-10-20-is-sonarqube-security-tool.png
---
 
In this article we give some reasons why we consider that **SonarQube is a good tool to deliver secure code safely**. This solution from Sonar not only teaches you how to deliver quality code, but also allows you to do so following safety standards. 

### Secure code delivery with SonarQube

SonarQube detects the following problems from standards-based rules and good coding practices: **bugs, vulnerabilities, code smells and hotsposts**. It is in this last problem that we will delve into. 

<h2>What are the hotspots?</h2>

Hotspots are code fragments that indicate a possible security risk. These fragments **should be checked to confirm or rule out the risk**.

> Let’s see an example of hotspot: SonarQube highlights the *'PASSWORD' detected rule in this expression, review this potentially hard-coded password*. In the code fragment we see a message that is explaining us that a string has been detected and that, by the context, SonarQube believes that it is a password. 

<img src="/img/posts/sonarqube-hotspots.png" width="90%" alt="Hotspots in SonarQube">


The detection and analysis of these hotspots is essential to improve and ensure the quality of the code. Reviewing the hotspots detected allows you to understand a possible risk, identify possible solutions and how to apply changes to protect the code.

On the other hand, it should be noted that the **bitegarden team** has developed a plugin that shows a list of vulnerabilities detected in SonarQube allowing to know the security compliance of the entire project **visual and detailed form**. This plugin is called Security Plugin for SonarQube and you can try it through [this link](https://www.bitegarden.com/sonarqube-security#product-block-center). 

Per quanto riguarda il punto di cui stavamo parlando degli hotsposts, con questo plugin potrai trovare tutte **le tue evidenze di OWASP** (sia vulnerabilità che hotspots di sicurezza) in una sola pagina ordinate per severità. Alleghiamo uno screenshot per te da vedere:

<img src="/img/sonarqube-security/security-owasp-vulnerabilities.png" width="90%" alt="Security Plugin for SonarQube">


### Consegna sicura del codice con SonarQube

Dalla versione di **SonarQube 8.9 LTS** lavorare con questa soluzione è ancora più sicuro, perché hanno aggiunto nuove funzionalità che rafforzano la sicurezza del tuo lavoro. Ne sono un esempio le seguenti caratteristiche: 

1 - L'azione di modifica delle credenziali dell'amministratore diventa obbligatoria. <br>
2 - L'accesso autenticato è determinato. <br>
3 - Accesso limitato ai plug-in in modo che i plugin di terze parti non influiscano sull'installazione. <br>
4 - Rinforzo da parte di Sonar al proprio processo di compilazione. <br>

Se desideri maggiori informazioni sulla sicurezza di Sonar o dei nostri plugin, non esitare a inviarci le tue domande. 

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_