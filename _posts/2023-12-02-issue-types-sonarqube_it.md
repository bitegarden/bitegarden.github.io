---
layout: post_it
title: 'Tipi di issues in SonarQube'
description: Ti spieghiamo cos'è un bug, una vulnerabilità e un code smell

permalink: tipo-di-issue-sonarqube
spanish: tipos-issue-sonarqube
english: issue-types-sonarqube

cover: /img/posts/2023-12-02-issue-types-sonarqube_en.png 
---

SonarQube è uno **strumento essenziale** per lo sviluppo di software perché offre una visione dettagliata della **qualità del codice**. Una delle caratteristiche più importanti di SonarQube è la sua capacità di identificare e classificare i problemi nel codice attraverso le issues. In questo articolo, spiegheremo i diversi tipi di issue che SonarQube può rilevare, sottolineando la loro importanza e come affrontarli per migliorare la **qualità del software**.

<h2>Quali tipi di issues sono disponibili su SonarQube?</h2>

<h3>Bugs</h3>

I bug sono un **errore di codice** che può causare un errore imprevisto durante l'esecuzione del codice. Nella seguente immagine possiamo vedere un esempio di bug. SonarQube lo classifica come tale, indica dove si trova e anche perché lo qualifica come una issue. 

<img src="/img/posts/bug-example.png" width="100%" alt="Bug example in SonarQube">

<h3>Vulnerability</h3>

Una vulnerabilità è un **punto nel codice scoperto**, vulnerabile agli attacchi esterni. Nell'immagine seguente possiamo vedere un esempio di vulnerabilità che SonarQube ha rilevato quando ritiene che una password possa essere esposta. 

<img src="/img/posts/vulnerability-example.png" width="100%" alt="Vulenrability example in SonarQube">


<h3>Code Smells</h3>

Un code smell è un **problema che rende il codice** difficile da capire. Nell'immagine seguente possiamo vedere un esempio di code smell in cui SonarQube suggerisce di eliminare un parametro che non viene utilizzato. 

<img src="/img/posts/code-smell-example.png" width="100%" alt="Code Smells example in SonarQube">

Va ricordato nell'ultima release di **SonarQube 10.3**, Sonar ha annunciato che questi tipi di issues **diventano obsoleti**. Quindi nei nuovi aggiornamenti i problemi saranno ora evidenziati con gli attributi di Clean Code e le qualità del software interessate. 

Ricorda che se hai bisogno di ulteriori informazioni, puoi contattarci tramite questo [modulo](https://www.bitegarden.com/it/contact/).

---
**<span style="color: green">bitegarden</span> team**

_Helping companies to develop better software_