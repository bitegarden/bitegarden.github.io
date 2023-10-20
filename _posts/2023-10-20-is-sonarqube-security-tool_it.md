---
layout: post_it
title: 'SonarQube è uno strumento sicuro?'
description: Ti spieghiamo perché con SonarQube consegni codice sicuro in modo sicuro. 

permalink: sonarqube-uno-strumento-sicuro
english: is-sonarQube-security-tool
spanish: sonarqube-herramienta-segura

cover: /img/posts/2023-10-20-is-sonarqube-security-tool.png
---
 
In questo articolo diamo alcuni motivi per cui riteniamo che **SonarQube sia un buon strumento per consegnare codice sicuro in modo sicuro**. Questa soluzione Sonar non solo ti insegna come fornire codice di qualità, ma ti consente anche di farlo seguendo gli standard di sicurezza. 

### Consegna codice sicuro con SonarQube

SonarQube rileva i seguenti problemi da regole basate su standard e buone pratiche di codifica: **bug, vulnerabilità, code smells e hotsposts**. È su quest'ultimo problema che ci addentreremo. 

<h2>Cosa sono gli hotspot?</h2>

Gli hotspot sono frammenti di codice che indicano un possibile rischio per la sicurezza. Questi frammenti **devono essere controllati per confermare o escludere il rischio**.

> Vediamo un esempio di hotspot: SonarQube evidenzia la regola *'PASSWORD' detected in this expression, review this potentially hard-coded password*. Nel frammento di codice vediamo un messaggio che ci sta spiegando che una stringa è stata rilevata e che, dal contesto, SonarQube crede sia una password. 

<img src="/img/posts/sonarqube-hotspots.png" width="90%" alt="Hotspots en SonarQube">


Il rilevamento e l'analisi di questi hotspot è essenziale per migliorare e garantire la qualità del codice. La revisione degli hotspot rilevati consente di comprendere un potenziale rischio, identificare possibili soluzioni e applicare modifiche per proteggere il codice.
<br>

PD'altra parte, va notato che il **team di bitegarden** ha sviluppato un plugin che mostra un elenco di vulnerabilità rilevate in SonarQube consentendo di conoscere la conformità di sicurezza dell'intero progetto **in modo visivo e dettagliato**. Questo plugin si chiama Security Plugin for SonarQube e puoi provarlo tramite [questo link](https://www.bitegarden.com/it/sonarqube-security#product-block-center). 

Per quanto riguarda il punto di cui stavamo parlando degli hotsposts, con questo plugin potrai trovare tutte **le tue evidenze di OWASP** (sia vulnerabilità che hotspots di sicurezza) in una sola pagina ordinate per severità. Abbiamo allegato uno screenshot per te da vedere:

<img src="/img/sonarqube-security/security-owasp-vulnerabilities.png" width="90%" alt="Security Plugin per SonarQube">


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